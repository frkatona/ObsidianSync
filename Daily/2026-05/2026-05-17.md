### home
- open mic to-do
	- test all the interface ports for bad connections and pre-amps
	- Edison for remix
	- custom FLR template + app layout features
		- EQ 
			- consider attaching sliders to the patcher template
		- limiter 
- applications/docker
- PSU parking

### work
- purchases (see yesterday)
- prepare for subgroup
	- tian-chi discussion points
		- 20-30 minute presentation seems like a lot for a few months of research, right?  Are they interrupting a lot?
		- slow motion video (and buying improved lighting)
		- determining the theoretical temperature increase from pulse energy and heat capacity
		- thermal conductivity
			- why were we talking about it last week?
			- what's the relationship we expect?
		- making a custom PDMS formulation (Si-O-vinyl + Si-O-silane + maybe catalyst, fillers, and solvent?)
		- best motivation to focus on (general surface vs underwater ship vs speed)
		- lingering on / emphasizing the chemistry for your committee (cross-linking reaction, physical explanation for siloxane utility)
		- Marangoni (thermocapillary) convection vs Rayleigh-Benard (natural) convection
			- about minimal gravity at mm scale
		- other possible mechanisms for surface texturing -> thermal expansion + buoyancy, cavitation (e.g., hitting the glass bottle on the top and breaking the bottom; propeller blades)
		- even the one 10% in-air surface appears slightly curved 
		- smoke vs vaporize and burned (combusted) vs pyrolyzed vs charred
		- incandescence / blackbody radiation, Kelvin color system (i.e., how hot is it if you can see it?  Like 800 K, maybe as high as like 2000 K;  maybe take a pic with a filter so it's not saturated)
		- thin plastic layer (~saran wrap) as possible replacement for glass slide sandwich (e.g., lighter under plastic water bottle not leaking)
		- varying heat capacity in coolant fluids rather than varying temperature
		- adhesion of PDMS to substrates (H-bonding?)
	- docker and other ideas for lab projects/resume building
- prepare for group
	- read Kristen's stats stuff to pepper questions

---
>For most laser-pulsed surface work, I would **not** start with exotic fluids. I would start with **flowing, degassed DI water**, then move to **water–glycerol** or **water–propylene glycol** if cavitation, splashing, oxidation, or bubble persistence becomes the limiting problem.

---
Thermocapillary vs. Buoyancy-Driven Convection on Earth There is **no universal Earth-surface fraction** such as “20% thermocapillary, 80% buoyant.” The better answer is that **thermocapillary flow can be negligible, comparable, or dominant on Earth**, and the controlling variable is often **liquid depth**, not gravity alone. A useful scaling comparison is the ratio of the Marangoni number to the Rayleigh number: $$ \frac{Ma}{Ra} = \frac{\Gamma}{\rho g \beta H^2} $$ where: - $\Gamma=-d\sigma/dT$ - $\rho$ is density - $\beta$ is thermal expansion coefficient - $H$ is liquid depth This follows from the fact that thermocapillary flow is driven by **surface-tension gradients at a free interface**, while Rayleigh/Bénard convection is driven by **buoyant density differences through the bulk**. See [MIT OCW, *18.357 Interfacial Phenomena, Lecture 9: Marangoni Flows*](https://ocw.mit.edu/courses/18-357-interfacial-phenomena-fall-2010/ebad47a511d146bd949f249eb5e4e046_MIT18_357F10_Lecture9.pdf). For water-like values near room temperature, using: - $\Gamma\approx1.6\times10^{-4}\ \mathrm{N\,m^{-1}\,K^{-1}}$ - $\rho\approx1000\ \mathrm{kg/m^3}$ - $\beta\approx2.1\times10^{-4}\ \mathrm{K^{-1}}$ the crude “driving-stress” split looks roughly like this: 

| Liquid depth \(H\) | \(Ma/Ra\) | Crude thermocapillary share \(Ma/(Ma+Ra)\) |
|---:|---:|---:|
| 0.1 mm | ~7800 | >99.9% |
| 1 mm | ~78 | ~99% |
| 3 mm | ~8.7 | ~90% |
| 1 cm | ~0.78 | ~44% | 
| 3 cm | ~0.087 | ~8% | 
| 10 cm | ~0.008 | <1% | 

So a clean, shallow, millimeter-scale free-surface film can be **mostly thermocapillary even on Earth.**  A several-centimeter-deep beaker or bath is usually **mostly buoyancy-driven**, with Marangoni effects strongest near the surface. NASA’s microgravity framing is consistent with this: in Earth gravity, surface-tension-driven convection is usually overshadowed by buoyancy, while in reduced gravity it becomes much easier to isolate. See [Ostrach and Kamotani, *Surface Tension Driven Convection Experiment*](https://ntrs.nasa.gov/citations/19890010943). 

The $H^{-2}$ dependence is the key intuition. Marangoni forcing is an **interfacial shear stress**; buoyancy is a **body force** acting through a volume. As the layer gets deeper, buoyancy grows in relative importance very quickly. Koschmieder and Switzer’s NASA-linked work states this qualitatively: onset is governed by the Marangoni number in thin layers and by the Rayleigh number in deep layers. They also note that $Ra\propto d^3$ while $Ma\propto d$, so buoyancy becomes more important with depth. See [Koschmieder final report / Koschmieder and Switzer manuscript](https://ntrs.nasa.gov/api/citations/19920008157/downloads/19920008157.pdf). 

### Caveats 

First, this “fraction” is only a **scaling estimate**, not a literal decomposition of measured velocity. In a real flow, buoyancy and thermocapillary stresses can reinforce each other, oppose each other, alter the same instability, or change the cell pattern. Some literature explicitly treats the net convective flow as a combination of surface-tension and density-gradient contributions rather than cleanly separable parts. See [Sequeira et al., *Revisiting the NASA Surface Tension Driven Convection Experiments*](https://pmc.ncbi.nlm.nih.gov/articles/PMC8857288/). 

Second, thermocapillary convection requires a **mobile free interface** with a **surface temperature gradient**. If the liquid is in a closed cell with no free surface, the thermocapillary contribution is essentially zero. If the surface is contaminated with surfactant, oxidized, skinned over, or mechanically constrained, Marangoni flow can be strongly suppressed. In molten metals, welding pools, laser melt pools, droplets, and thin films, however, the gradients and length scales can make Marangoni flow dominant despite normal gravity. 

## Practical Mental Model 
**On Earth, thermocapillary convection is not “microgravity-only.” It is shallow-free-surface convection.** In ~sub-mm to mm liquid layers, droplets, melt pools, or laser-heated surface films, it can dominate. In deep bulk liquids, ordinary buoyant convection usually dominates, and thermocapillary flow is more of a surface-bound correction unless temperature gradients are extreme. --- 

### Annotated Bibliography 

1. MIT OCW — *18.357 Interfacial Phenomena, Lecture 9: Marangoni Flows* Link: [https://ocw.mit.edu/courses/18-357-interfacial-phenomena-fall-2010/ebad47a511d146bd949f249eb5e4e046_MIT18_357F10_Lecture9.pdf](https://ocw.mit.edu/courses/18-357-interfacial-phenomena-fall-2010/ebad47a511d146bd949f249eb5e4e046_MIT18_357F10_Lecture9.pdf) **Use in response:** Basis for defining Marangoni stresses, thermocapillary flow, Rayleigh/Bénard convection, and the depth-scaling comparison between $Ma$ and $Ra$. 

2. Ostrach and Kamotani — *Surface Tension Driven Convection Experiment* Link: [https://ntrs.nasa.gov/citations/19890010943](https://ntrs.nasa.gov/citations/19890010943) **Use in response:** Supports the statement that Earth-gravity thermocapillary flows are often overshadowed by buoyancy-driven flows, motivating microgravity experiments. 

3. Koschmieder final report / Koschmieder and Switzer manuscript — *The Wave Numbers of Supercritical Surface Tension Driven Bénard Convection* Link: [https://ntrs.nasa.gov/api/citations/19920008157/downloads/19920008157.pdf](https://ntrs.nasa.gov/api/citations/19920008157/downloads/19920008157.pdf) **Use in response:** Supports the thin-layer versus deep-layer distinction and the idea that Marangoni onset dominates in shallow layers while Rayleigh onset dominates in deeper layers. 

4. Sequeira, Maitra, Pandey, and Jung — *Revisiting the NASA Surface Tension Driven Convection Experiments* Link: [https://pmc.ncbi.nlm.nih.gov/articles/PMC8857288/](https://pmc.ncbi.nlm.nih.gov/articles/PMC8857288/) **Use in response:** Supports the caveat that net thermocapillary flow can reflect combined surface-tension-gradient and density-gradient contributions rather than a cleanly separable percentage.