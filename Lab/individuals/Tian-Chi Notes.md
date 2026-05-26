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


---
# ChatGPT Question

# Question:
> I sandwiched some uncured PDMS impregnated with carbon black (as a photothermal agent) between two glass slides. Some larger bubbles were difficult to remove and so they remained inside. Then, I used a laser to write lines across the samples through the glass. what resulted was highly curved channels littered with what I assume are bubbles. 
> 
> I'll attach an image of this system which spans about 3 mm horizontally and another which spans about 10 mm horizontally. Evaluate them and tell me what you think happened. Why are the lines not straight like the laser pattern, are the lighter regions air channels, and why are there bubble-like objects inside of them? Further, what literature can you provide for roughly similar systems producing curved lines despite a linear power application?

# Response:
My best interpretation is that you did **not simply write straight cured PDMS lines**. You created a confined, laser-heated, two-phase flow problem: uncured CB/PDMS between glass slides, with trapped air, local photothermal heating, viscosity changes, gas expansion, partial curing, and probably local dewetting/void formation. The visible “lines” are therefore likely **the frozen aftermath of gas/liquid interface motion**, not a faithful map of the laser scan path.

## What the images suggest

In the ~10 mm image, the large bright ovals with dark rims look very much like **trapped air bubbles/voids**. The sinuous parallel bands are too coherent to be random individual bubbles; they look like **raster-written thermal tracks that became wavy through flow, dewetting, or thickness/interface instabilities**. In the ~3 mm image, the broader light-colored curved channels are filled or bordered by many small ring-like features, which strongly suggests **microbubble nucleation/expansion along the laser-heated path**.

The most likely sequence is:

1. **Carbon black absorbed the laser and generated localized heat.** Carbon-loaded PDMS is well-established as a photothermal composite; carbon nanoparticles in PDMS can produce localized heating, laser-assisted patterning, and optomechanical deformation.
2. **The heated region temporarily became a mobile, pressurized line.** Uncured PDMS near the beam would heat, decrease in viscosity, partially cure, thermally expand, and transfer heat to trapped gas pockets. Existing air bubbles would expand strongly, and small nuclei at carbon aggregates, dust, glass defects, or dissolved/entrained gas pockets could become visible bubbles.
3. **The air/vapor/low-viscosity region displaced viscous uncured PDMS between two glass plates.** That geometry is essentially a crude **Hele-Shaw cell**. In the classic Saffman–Taylor situation, a less viscous fluid such as air displacing a more viscous fluid between closely spaced glass plates develops round-ended fingers and interface instabilities rather than preserving a planar front. Your light channels look consistent with that kind of “gas finger through viscous liquid” behavior, except the driving pressure is locally generated by the laser rather than by an external syringe.
4. **The evolving interface was then frozen by curing/cooling.** Once part of the PDMS cured or gelled, the displaced/foamed morphology would stop relaxing, preserving curved channels and bubble chains.

## Why the lines are not straight

The key point is that the **laser path can be straight while the visible material response is not straight**. A straight line of heat in a confined liquid can create a moving meniscus, local pressure wave, gas finger, or thermocapillary flow. Those are nonlinear hydrodynamic objects, and they follow the path of least mechanical resistance, not necessarily the beam centerline.

Several factors would push the channels away from the intended linear scan:

**Pre-existing large bubbles:** The big air pockets are pressure reservoirs and optical lenses. They locally distort heat deposition, relieve pressure, block flow, and bend nearby fronts.

**Hele-Shaw/viscous fingering instability:** Air or vapor displacing uncured PDMS between slides is prone to curving, tip splitting, and rounded finger growth. This is one of the closest conceptual matches to “linear forcing, curved channel outcome.”

**Thermocapillary/Marangoni flow and dewetting:** Local heating creates surface-tension gradients. Literature on laser-heated thin liquid films shows that laser irradiation can deform, destabilize, rupture, and dewet thin films rather than simply making a local mark.

**Gap-thickness variation between slides:** If the slides were not perfectly parallel, or if bubbles locally lifted the slide, the PDMS layer thickness would vary. That changes heat dissipation, pressure resistance, capillary pressure, and optical focus. The regular wave-like parallel bands in the 10 mm image could partly reflect a pre-existing thickness/meniscus field.

**Interaction between adjacent scan lines:** Once the first line creates a cured ridge, void, or displaced channel, later passes experience a different mechanical and thermal boundary condition. That can make neighboring lines curve in correlated ways.

## Are the lighter regions air channels?

Probably **partly**, but I would not call every light region “air” from the image alone.

The large bright ovals with sharp dark rims are very likely air voids. The broad light sinuous ribbons are likely one or more of the following:

- true air/vapor channels,
- PDMS-depleted regions where the film is much thinner,
- clearer or differently cured PDMS with lower carbon black optical density,
- meniscus-bounded channels containing both air pockets and residual PDMS,
- optical contrast from thickness/interference/topography rather than an empty hollow.

The dark outlines are consistent with refractive-index contrast at curved air/PDMS interfaces and/or carbon black being swept toward the channel edges. Also, photothermal PDMS/CB patterning can produce optical and topographic changes even without fully open voids. A 2025 RSC Applied Polymers paper reports micron-scale PDMS/CB surface features and optical-property changes from laser photothermal patterning.

## Why are there “bubbles inside” the channels?

If the light ribbons are fully open air channels, then the small ringed objects are not literally “air bubbles inside air.” More likely, the image is a projection through a 3D structure: small voids at different heights, residual PDMS droplets/islands inside a larger depleted corridor, or meniscus pockets along the channel floor/ceiling.

If the ribbons are not fully hollow, then the explanation is simpler: the laser-heated PDMS track nucleated or expanded many microbubbles. This is very close to the **microFLIB** literature, where nanosecond laser-induced bubbles in pre-curing PDMS are intentionally used to form hollow microchannels. Toba et al. report focusing and scanning a laser inside pre-curing liquid PDMS to generate a 3D line of bubbles; those bubbles persisted for more than 24 h and produced hollow microchannels after curing. Naruse and Hanada similarly describe focusing a laser at an uncured PDMS/metal target interface and scanning to generate a line of bubbles.

## Closest literature buckets

I do not know of an exact match to your geometry — **uncured PDMS + carbon black, sandwiched between glass slides, laser-written through glass, producing sinuous bubble-filled tracks** — but these are the closest analogs:

1. **Laser-induced bubbles in uncured PDMS / microFLIB.**  
    This is the most directly relevant family. It shows that laser scanning in pre-curing PDMS can create bubble lines that persist and become hollow microchannels.
2. **Carbon-black/PDMS photothermal curing and patterning.**  
    These papers establish that small amounts of carbon black can strongly photothermally heat PDMS and generate controlled patterning/topographic changes.
3. **Saffman–Taylor / viscous fingering in Hele-Shaw cells.**  
    Your sandwich is mechanically similar to two plates confining a viscous liquid, and gas/air displacement in such geometries naturally produces curved fingers.
4. **Laser-induced thermocapillary deformation/dewetting of thin liquid films.**  
    These systems show that local heating can rupture or redistribute thin films through Marangoni stresses, especially when a film is confined or partially wetting.
5. **Laser-induced cavitation and entrapped gas pockets near PDMS.**  
    Not identical, but useful: studies show that pressure gradients from laser-induced bubbles can expand and oscillate entrapped air pockets in PDMS microstructures.

## Experiments I would run next

The fastest way to identify the dominant mechanism is to repeat the pattern with a **fully degassed, spacer-controlled sandwich**. Use fixed-thickness spacers, degas the PDMS/CB thoroughly, assemble under gentle pressure, and compare against a deliberately bubble-seeded sample. If the curves and microbubbles largely disappear, the effect is mainly trapped-gas expansion/viscous fingering.

I would also do a simple **puncture-and-dye test**: after curing, nick one end of a light channel and place a low-viscosity dye or fluorescent oil at the opening. If it wicks through, the light region is an open or semi-open air channel. If it does not, it is more likely a cured/thinned/topographic optical feature with embedded bubbles.

A third useful check is to image the sample **before lasing** and again after each pass. If the same waviness exists before lasing, you are seeing thickness/interference/topography imposed by slide spacing. If the waviness appears only after laser exposure, it is a processing instability.My best interpretation is that you did **not simply write straight cured PDMS lines**. You created a confined, laser-heated, two-phase flow problem: uncured CB/PDMS between glass slides, with trapped air, local photothermal heating, viscosity changes, gas expansion, partial curing, and probably local dewetting/void formation. The visible “lines” are therefore likely **the frozen aftermath of gas/liquid interface motion**, not a faithful map of the laser scan path.

## What the images suggest

In the ~10 mm image, the large bright ovals with dark rims look very much like **trapped air bubbles/voids**. The sinuous parallel bands are too coherent to be random individual bubbles; they look like **raster-written thermal tracks that became wavy through flow, dewetting, or thickness/interface instabilities**. In the ~3 mm image, the broader light-colored curved channels are filled or bordered by many small ring-like features, which strongly suggests **microbubble nucleation/expansion along the laser-heated path**.

The most likely sequence is:

1. **Carbon black absorbed the laser and generated localized heat.** Carbon-loaded PDMS is well-established as a photothermal composite; carbon nanoparticles in PDMS can produce localized heating, laser-assisted patterning, and optomechanical deformation.
2. **The heated region temporarily became a mobile, pressurized line.** Uncured PDMS near the beam would heat, decrease in viscosity, partially cure, thermally expand, and transfer heat to trapped gas pockets. Existing air bubbles would expand strongly, and small nuclei at carbon aggregates, dust, glass defects, or dissolved/entrained gas pockets could become visible bubbles.
3. **The air/vapor/low-viscosity region displaced viscous uncured PDMS between two glass plates.** That geometry is essentially a crude **Hele-Shaw cell**. In the classic Saffman–Taylor situation, a less viscous fluid such as air displacing a more viscous fluid between closely spaced glass plates develops round-ended fingers and interface instabilities rather than preserving a planar front. Your light channels look consistent with that kind of “gas finger through viscous liquid” behavior, except the driving pressure is locally generated by the laser rather than by an external syringe.
4. **The evolving interface was then frozen by curing/cooling.** Once part of the PDMS cured or gelled, the displaced/foamed morphology would stop relaxing, preserving curved channels and bubble chains.

## Why the lines are not straight

The key point is that the **laser path can be straight while the visible material response is not straight**. A straight line of heat in a confined liquid can create a moving meniscus, local pressure wave, gas finger, or thermocapillary flow. Those are nonlinear hydrodynamic objects, and they follow the path of least mechanical resistance, not necessarily the beam centerline.

Several factors would push the channels away from the intended linear scan:

**Pre-existing large bubbles:** The big air pockets are pressure reservoirs and optical lenses. They locally distort heat deposition, relieve pressure, block flow, and bend nearby fronts.

**Hele-Shaw/viscous fingering instability:** Air or vapor displacing uncured PDMS between slides is prone to curving, tip splitting, and rounded finger growth. This is one of the closest conceptual matches to “linear forcing, curved channel outcome.”

**Thermocapillary/Marangoni flow and dewetting:** Local heating creates surface-tension gradients. Literature on laser-heated thin liquid films shows that laser irradiation can deform, destabilize, rupture, and dewet thin films rather than simply making a local mark.

**Gap-thickness variation between slides:** If the slides were not perfectly parallel, or if bubbles locally lifted the slide, the PDMS layer thickness would vary. That changes heat dissipation, pressure resistance, capillary pressure, and optical focus. The regular wave-like parallel bands in the 10 mm image could partly reflect a pre-existing thickness/meniscus field.

**Interaction between adjacent scan lines:** Once the first line creates a cured ridge, void, or displaced channel, later passes experience a different mechanical and thermal boundary condition. That can make neighboring lines curve in correlated ways.

## Are the lighter regions air channels?

Probably **partly**, but I would not call every light region “air” from the image alone.

The large bright ovals with sharp dark rims are very likely air voids. The broad light sinuous ribbons are likely one or more of the following:

- true air/vapor channels,
- PDMS-depleted regions where the film is much thinner,
- clearer or differently cured PDMS with lower carbon black optical density,
- meniscus-bounded channels containing both air pockets and residual PDMS,
- optical contrast from thickness/interference/topography rather than an empty hollow.

The dark outlines are consistent with refractive-index contrast at curved air/PDMS interfaces and/or carbon black being swept toward the channel edges. Also, photothermal PDMS/CB patterning can produce optical and topographic changes even without fully open voids. A 2025 RSC Applied Polymers paper reports micron-scale PDMS/CB surface features and optical-property changes from laser photothermal patterning.

## Why are there “bubbles inside” the channels?

If the light ribbons are fully open air channels, then the small ringed objects are not literally “air bubbles inside air.” More likely, the image is a projection through a 3D structure: small voids at different heights, residual PDMS droplets/islands inside a larger depleted corridor, or meniscus pockets along the channel floor/ceiling.

If the ribbons are not fully hollow, then the explanation is simpler: the laser-heated PDMS track nucleated or expanded many microbubbles. This is very close to the **microFLIB** literature, where nanosecond laser-induced bubbles in pre-curing PDMS are intentionally used to form hollow microchannels. Toba et al. report focusing and scanning a laser inside pre-curing liquid PDMS to generate a 3D line of bubbles; those bubbles persisted for more than 24 h and produced hollow microchannels after curing. Naruse and Hanada similarly describe focusing a laser at an uncured PDMS/metal target interface and scanning to generate a line of bubbles.

## Closest literature buckets

I do not know of an exact match to your geometry — **uncured PDMS + carbon black, sandwiched between glass slides, laser-written through glass, producing sinuous bubble-filled tracks** — but these are the closest analogs:

1. **Laser-induced bubbles in uncured PDMS / microFLIB.**  
    This is the most directly relevant family. It shows that laser scanning in pre-curing PDMS can create bubble lines that persist and become hollow microchannels.
2. **Carbon-black/PDMS photothermal curing and patterning.**  
    These papers establish that small amounts of carbon black can strongly photothermally heat PDMS and generate controlled patterning/topographic changes.
3. **Saffman–Taylor / viscous fingering in Hele-Shaw cells.**  
    Your sandwich is mechanically similar to two plates confining a viscous liquid, and gas/air displacement in such geometries naturally produces curved fingers.
4. **Laser-induced thermocapillary deformation/dewetting of thin liquid films.**  
    These systems show that local heating can rupture or redistribute thin films through Marangoni stresses, especially when a film is confined or partially wetting.
5. **Laser-induced cavitation and entrapped gas pockets near PDMS.**  
    Not identical, but useful: studies show that pressure gradients from laser-induced bubbles can expand and oscillate entrapped air pockets in PDMS microstructures.

## Experiments I would run next

The fastest way to identify the dominant mechanism is to repeat the pattern with a **fully degassed, spacer-controlled sandwich**. Use fixed-thickness spacers, degas the PDMS/CB thoroughly, assemble under gentle pressure, and compare against a deliberately bubble-seeded sample. If the curves and microbubbles largely disappear, the effect is mainly trapped-gas expansion/viscous fingering.

I would also do a simple **puncture-and-dye test**: after curing, nick one end of a light channel and place a low-viscosity dye or fluorescent oil at the opening. If it wicks through, the light region is an open or semi-open air channel. If it does not, it is more likely a cured/thinned/topographic optical feature with embedded bubbles.

A third useful check is to image the sample **before lasing** and again after each pass. If the same waviness exists before lasing, you are seeing thickness/interference/topography imposed by slide spacing. If the waviness appears only after laser exposure, it is a processing instability.

---
### 2026-05-25 
- things tian chi might want to prioritize
	- profilometry pipeline
	- vacuum chamber
	- UV vis
- ChatGPT 