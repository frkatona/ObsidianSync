Containerization (Docker, Kubernetes)
- Projects candidates 
	- Optical Profilometry
- Notes
	- Docker is different from naive VM implementations, which emulate hardware; Docker just emulates software environments.  This way, apps run on the machine (inside the container or otherwise) can share the kernel, mitigating otherwise massive overhead
	- Docker
		- Dockerfile - directions for how to build the image/environment
		- Image - snapshot of the host's software dependencies, down to the OS 
		- Container - actual software running in the real world (multiple containers can be spun up from the same image)
	- Kubernetes
		- orchestration - auto-scaling (distribution) and auto-healing of machines/infrastructure
		- cluster - system deployed on kubernetes
		- control plane - brain; exposes API server for management
		- ETCD - key-value database
		- nodes - worker machines (adding more nodes = scaling horizontally)
		- Kublets - application running on nodes, which contains 'pods' (like whales), i.e., units of containers
		- handles things like networking, persistent storage, secret management, etc.
		- replica set - set of running pods or containers ready to use
		- usually yaml objects define state of a cluster
	- Terminology
		- docker 
			- docker compose vs docker run
			- 'bind-mounting at runtime'
		- spin up
		- daemon - background process ("service" in windows)
		- cloud provider; cloud resources allocation; container provisioning; orchestration tools
		- auto-healing of containers
		- clusters; control planes
		- ETCD (key value data base)
		- node
		- kubelets and pods
		- replicate set



## Dockerize Optical Profilometry Pipeline as a Headless CLI

### Summary

- Package this repo as a thin Linux CLI image, optimized for docker run, not as a long-lived service.
- Keep code inside the image and keep raw .xyz inputs plus generated exports outside the image via bind mounts.
- Default to headless execution with Matplotlib’s non-GUI backend; do not support interactive plot windows in the first Docker pass.

### Implementation Changes

- Add requirements.txt and pin the currently working stack for reproducibility: numpy==2.1.2, scipy==1.14.1, matplotlib==3.9.2, tqdm==4.67.1.
- Add .dockerignore that excludes .git/, heightmaps/, exports/, literature/, _tmp_compare/, *.xyz, *.pdf, image artifacts, and __pycache__/. This matters because the current repo carries roughly 409 MB of heightmaps, 63 MB of exports, 36 MB of literature, and 389 MB of .git data that should not be part of the build context.
- Add a single-stage Dockerfile based on the Docker Official python:3.13-slim image. Set PYTHONDONTWRITEBYTECODE=1, PYTHONUNBUFFERED=1, and MPLBACKEND=Agg; install Python dependencies; copy the project source; create a non-root user; set WORKDIR /app; set ENTRYPOINT ["python", "analyze_heightmap.py"]; set CMD ["--help"].
- Keep analyze_heightmap.py as the primary container entrypoint. Do not make interpolation_study.py the default path; document it as an alternate command via --entrypoint python.
- Tighten headless behavior in analyze_heightmap.py: if --no-display is passed without --output-dir, exit with a clear error; never call plt.show() on the headless path.
- Update README.md with Docker build and run examples, using bind-mounted /data for inputs and /out for outputs, with PowerShell-friendly examples that quote paths correctly.

### Public Interface

- New runtime contract: docker run <image> /data/file.xyz -o /out --no-display [other flags].
- Inputs are provided by bind mount and should be treated as read-only.
- All generated outputs must go to a bind-mounted output directory.
- interpolation_study.py remains available as a secondary command, invoked explicitly rather than through the main entrypoint.

### Test Plan

- Build test: docker build -t optical-profilometer . succeeds from repo root.
- Help test: docker run --rm optical-profilometer prints the CLI help text from analyze_heightmap.py.
- Smoke test: bind-mount test.xyz and run --stats-only -r 32; expect exit code 0 and printed statistics.
- Export test: bind-mount an output directory and run -o /out --no-display -r 32; expect *_statistics.txt and *_analysis.png in /out.
- OBJ test: run with --export-obj roughness; expect *_roughness.obj in /out.
- Negative test: run --no-display without -o; expect a non-zero exit and a clear validation error.

### Assumptions And Defaults

- Chosen defaults: headless only and docker run workflow.
- Chosen scope: primary support for analyze_heightmap.py; secondary script is documented but not refactored into a first-class container UX.
- Chosen image shape: single-stage, not multi-stage, because this repo is a pure Python CLI with no compiled app artifact to copy between stages.
- Chosen data strategy: do not bake raw datasets or exports into the image.
- Windows note: if you use Docker Desktop, performance will be better when bind-mounted data lives in the WSL/Linux filesystem instead of a Windows or OneDrive path.

### References

- Docker Python Official Image: [![](https://hub.docker.com/favicon.ico)https://hub.docker.com/_/python](https://hub.docker.com/_/python)
- Docker build best practices: [![](https://docs.docker.com/favicon.ico)https://docs.docker.com/build/building/best-practices/](https://docs.docker.com/build/building/best-practices/)
- Docker bind mounts: [![](https://docs.docker.com/favicon.ico)https://docs.docker.com/engine/storage/bind-mounts/](https://docs.docker.com/engine/storage/bind-mounts/)
- Matplotlib backend environment variable: [https://matplotlib.org/stable/install/environment_variables_faq.html](https://matplotlib.org/stable/install/environment_variables_faq.html)
- Docker Desktop WSL file-performance guidance: [![](https://docs.docker.com/favicon.ico)https://docs.docker.com/desktop/features/wsl/best-practices/](https://docs.docker.com/desktop/features/wsl/best-practices/)

### brief
Implemented the Docker packaging and the headless CLI guard. The new container files are Dockerfile, .dockerignore, and requirements.txt. I also updated analyze_heightmap.py (line 996) so --no-display now fails fast without --output-dir, and the visualization path now only uses an output directory when one is explicitly provided (line 1096 (line 1096)). The help examples were corrected to use analyze_heightmap.py, and README.md (line 11) now documents the docker run workflow, bind mounts, PowerShell examples, and the interpolation_study.py alternate invocation.

Verified end to end: local py analyze_heightmap.py test.xyz --stats-only -r 32 succeeds, local py analyze_heightmap.py test.xyz --no-display returns the new validation error, docker build -t optical-profilometer . succeeds, docker run --rm optical-profilometer prints the CLI help, and container runs against a bind-mounted test.xyz produced stats, test_analysis.png, and test_roughness.obj in a mounted output directory