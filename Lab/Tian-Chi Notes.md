## Research Directions
### Photothermal Curing (general)
- academic motivations
	- polymer behavior with nano-scale physical/chemical property gradients
		- e.g., stiffness drops 10-fold from the laser center to 
	- polymer response to heat beyond normal degradation limits but for momentary exposure
- practical motivations
	- speed
		- "billion-fold" rate increases for, e.g., industrial
		- also: still works for sensitive substrates (e.g., paper, clothes, skin)
			- see: silicone + Perflurodecalin patch for laser tattoo removal ([wiki](https://en.wikipedia.org/wiki/Tattoo_removal))
	- precision
		- advantageous property gradients
		- remove need for wasteful bulk heating (e.g., car chassis coating ovens)
	- mold-less topology tuning
		- hydrophobicity & optics (i.e., Jackie's research)
		- adhesion (i.e., Sarah's research)
- lab work
	- buying non-Sylgard formulations OR synthesizing your own
		- then you can add your own filler basically re-do previous experiments to and see how it influences results
		- also it will interfere less with your analysis (e.g., IR)
	- use a different agent
		- CB is cheap and highly absorbing across many wavelengths, but...
			- would (e.g.) carbon nanotubes do a better job in some way?  Would different vastly different thermal conductivities influence the cure profile?
			- would 
### Underwater Curing
- academic motivations
	- extreme thermal sink at the point of absorption
		- can we generate both enough heat to generate change without prohibitive degradation
	- limitations from scattering
- practical motivations
	- repair ship coatings without costly and time-consuming dry docking
- lab work
	- first steps
		- laser conditions (power, PRF, scan speed) exploration
			- what conditions do anything meaningful?
			- can we get results like out-of-water?
			- can we get results that we can't get in air?  (if you get weird topologies or other results, is that (1) unique to your methods and (2) novel, or (3) useful in *any* conceivable way?)
	- is the cure profile more biased in the bulk of the material, like the weirdly bulbous cure shapes I saw in my "ultra-low loadings" paper?
	- spatial/temporal temperature measurements
		- esp32 + thermocouple

## Misc.
- Photo-elasticity
	- i.e., brightness and color distributions when looking at polarized light through photothermally-treated PDMS
	- can you write otherwise-undetectable patterns in PDMS, only revealed by polarizers?
- Nano-structure replication molding
	- e.g., diffractive molds
	- possibly a compelling demonstration that one of the most uniquely useful properties of silicone (high replication fidelity) is still available despite the massive temperature gradients
		- also perhaps demonstrates the utility of the surface-bias for temperature sensitive substrates since the diffractive material used as a mold here would also need to not melt/degrade until the features transferred to the cured PDMS


---

## Instruments & Skills
- PDMS
	- Concepts
		- thermoplastic vs thermoset
		- crosslinking + tracking kinetics
	- mixing, degassing, curing
- Lasers
	- Concepts
		- wavelength
		- beam character
			- distribution: Gaussian, top hat, etc.
			- quality
		- CW vs pulsed
			- Pulse Repetition Frequency (PRF, "repetition rate")
			- power vs energy vs flux ("radiant flux", "irradiance", "intensity") vs exposure ("radiant exposure", "fluence")
			- power meters
		- scanning
			- scan speed
			- rastering vs snaking
			- hatch distance
		- optics
			- mirrors, lenses, posts
			- beam stops
	- How to use
		- Fiber (1064 nm, pulsed, PRF 10s - 100s kHz)
			- Lightburn
				- shape drawing
				- parameter editing
				- parameter sweeps
		- Diode (808 nm, CW)
		- OPO/YAG (355 nm - 1064 nm, pulsed)
- Spectroscopy (IR, UV/Vis)
- Digital microscope
- Contact angle
## Software
- Scripting
	- Python
		- data analysis (e.g., pandas)
		- data vis (e.g., matplotlib, plotly)
	- code editors
		- VS Code (alternatively, Jupyter/Marimo)
- ImageJ/FIJI
- Adobe (Illustrator, Photoshop)

---
## Reading
- Basics
	- Polymers, Inorganic Polymers, PDMS

---
## Caution
- don't worry too much about the appearance of the things you make
	- ugly things are often interesting
	- I don't know that you "burn" your surface like you say sometimes, but even if you do, that does not qualify as an undesirable, useless, or uninteresting result
	- **unless** the motivation you choose for your story requires them to look a certain way
- don't worry about the *immediate* usefulness of the things you make
	- sometimes you make things which are simply chemically interesting or revealing
	- even when you are targeting an application, your research is usually only meant to inform the engineers who will be refining your ideas to build a product in like 10 years from now
- don't feel the need to get trained on every instrument you need to use
	- **unless** you genuinely think it's fun OR you're reasonably confident that you will need to collect lots of data with the instrument during your time here
- don't worry about faculty's feelings, especially with Ben
	- if they 