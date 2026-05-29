### home
- applications
- reschedule mtnittany for end of month
- email HR
	- email Pennie
	- find out what to get and when for applying
	- ask what the premiums and out-of-pockets would be
	- ask Energy if they are in-network with Pennie
- reply 
	- Tim
	- Zack 
- live transcription app really useful...try to dockerize so I don't have to hunt it down each time and can share it easily
### work

- Ben's project dockerization notes
	- just want an online fitting app?  does marimo not support these packages out of the box?  is there something that can't be pyodide'd?
		- otherwise, why not pyodide + github pages?
		- also, creating the dockerfile and using docker desktop + local web app is pretty straightforward as well
- meeting
	- lab jobs slide
	- read kristen's stats part to criticize
	- get a mockup of docker for Ben (static, offline docker desktop, and online container)

### subgroup
- Maybe new samples from Ben Stovall and AC this week
	- Rob on Ben about paper
	- next thin sample, do a million low power takes to deliver more total exposure, but at a rate that cannot increase temperature meaningfully
	- I should ask Tainara and AC if they can meet after Wednesday to get our expectations in order (when are the samples arriving, what is the time (and atmosphere) sensitivity, what tests need performed on them, how much sample needs allocated to which prep or analysis, when can I get them to Tainara and when can Tainara get to them, etc.)
- Ben Docker
	- blender
		- basic version success
		- profilometer progress
	- fitter
		- can do in a static site...what is it that you wanted?
		- libraries may expand image beyond ~500 MB limits for Google Cloud 'free tier'...are you will to pay a few bucks if something exceeds the guardrails?
- Tian-chi
	- scaring her over Marangoni flow
	- title of first paper something like "controlling topology in submerged PDMS coating cure through photothermal treatment"
		- my thought is that a baseline understand of all the most likely relevant chemical/physical phenomenon will be necessary or else the other ideas seem meaningless
		- also, 'marangoni flow' is strange to invoke as a rationale for defects and deformed/irregular textures since it is the reason for the regular textures
		- how to lean into the chemistry?
	- mechanism inventory
		- gel-front freezing
			- heating lowers viscosity initially, causing flow, then increases rapidly as crosslinking proceeds (freezing flow mid-motion)
			- test by allowing some amount of pre-cure
			- also applicable in-air (maybe future experiments should expand on in-air experiments to establish a better baseline)
		- other in-air: watching the bubbles for at slow-mo, changing up the de-gas parameter

Ben: "can you get the exact same with the parameters and expectations, then future work is what you could do to find what is actually different when you see it's different"

### Kaya/Bryan/Josh Docker explanation terminology
- https://docs.kernel.org/admin-guide/cgroup-v1/cgroups.html
- namespaces
- https://en.wikipedia.org/wiki/User_space_and_kernel_space
- https://blogs.oracle.com/linux/userspace-vs-kernelspace-understanding-the-divide