---

---

 - one slide on background (how we think through this)
	 - difficult to think through the isolated heat sources since we don't know what they are, so maybe don't allude too much (is JP doing his reflectance thing?)
	 - mostly important that heating and cooling is fast, we can get to high temps
 - one slide on the lasing conditions (chamber, laser) and before and shot for the actual sample
 - then JP probably will be the one with all the characterization slides, but we can send the first XRD on a third slide and let Mike sort it out

7/1 thoughts
- work on scripting (ideally no labview, but maybe labview) 
	- visualize oscilloscope output in real time
	- sync with a secondary input
	- capture output a given time
	- fit a blackbody to 4 points
### To-do
 - lab
	 - [ ] Try lasing through acrylic in lab before buying full container
 - home
	 -  Search one last time for temperature determination in literature
		 - Onedrive folder
		 - wider lit search
	 - Purchasing
	 - Ask Ben S
		 - [ ] most recent video recordings
		 - [ ] If he'd prefer to wait until next week for new case/regulator

- Find out if we are retaining ligand from the polymer
	- [x] run the white sample (no Boron) see what happens
		- recall that TGA shows polymer without boron degrades around 450, but around 250 with Boron
	- [x] bring it back on Sapphire for Tainara to cut
- [ ] Buy stuff as soon as spending resumes on 6/30
	- Vacuum chamber
		- [ ] O2 meter ([RKI wireless](https://sensorpros.com/products/rki-instruments-gx3r-pro-gas-detector-with-wireless-communication?variant=39736879087690) $700, call about O2 sensitivity)
		- [ ] thermocouple (type k? cold junction?)
		- [ ] better regulator
		- [ ] forming gas (just get an H2 cylinder to run with Ar? Or is there Ar + H available?)
	- Thor etc. vendor purchases
		- [ ] optics
			- [ ] microscope objective for ~1 um OR simple lens for ~1 cm
			- [ ] apertures/fiber to define the collection area
		- [ ] detectors
			- [ ] photo-diodes and photo-multipliers with rise times of ~nanoseconds (e.g., InGaAs or Ge photodiodes for the near IR ~800-1700, e.g. Xu et al.)
		- [ ] split wavelengths (filtered mirrors? prism/grating?)
		- [ ] signal enhancement (PMT?)
		- [ ] ADC/Data Acquisition
	- Misc
		- Regulator (check inlet type) - [CGA580 inlet](https://www.amazon.com/ARCCAPTAIN-Regulators-Welding-Regulator-Connection/dp/B0D1KD5ZPT?sr=8-10) - $40
		- thermocouple
			- sensor
			- reader
		- oscilloscope (file:///C:/Users/antho/Downloads/071281002web.pdf)
			- probes ([tektronix passive](https://www.tek.com/en/products/oscilloscopes/oscilloscope-probes/passive-probe#) x2 = $168)
		- Vacuum container
			- google image 'positive pressure glass vacuum box'
			- able to mechanically seal, resistant to positive pressure (maybe bolts, but ideally something like a [toggle latch](https://www.amazon.com/Toggle-Latch-Pack-Adjustable-Industrial/dp/B0DKFPCRWG?dib=eyJ2IjoiMSJ9.n4y-4bK6e84yc7qxJion7bHdlDnSr3YWVcDGWarWVgOQO41DWCpuaXuUtMXyuSBrX70luV1KdsihFEV_aSipPKLUbER6pckyyDU6dvCkkHKZodt-IBVw8wIZ903QuhqToGwgTIAees8CkSHfSj525Pm4I8tg_BLfWfgJcY6EUn1ZuV3y4MacADrdSfs0SRlGn1IlpegANrXD2mAzCpuDKXnKYxpypZob-00ucG9HJYr2LaFl-9ghPYVEc1Gg-Wl5VD7AsidH3lUTUM3K5Ciw8Pd-lnxucNsUPvMNjI7LSF8.IfA3-UC-2EnzsI7GxKMGerrF6zxfPwCpp4ekDOYz74c&dib_tag=se&keywords=toggle+latch&qid=1750951998&sr=8-1) ~$17)
			- low absorption, strong, transparent enclosure
				- possibility 1: Pyrex top clamped onto steel enclosure
				- possibility 2: solvent-welded acrylic
					- easier to bolt to, but would need thick pieces to not break, along with nuts and o-rings
					- buy [solvent cement](https://www.amazon.com/Weld-Acrylic-Plastic-Cement-Applicator/dp/B0149IG548) $20
			- big enough to house O2, H2O, VOC sensors + pyrometer
			- port for wires
- [x] Get or take a desiccator downstairs (ask Kristen, see if it needs regenerated/bought again)
- [ ] Try forming gas
- [ ] Get FLIR images with or without wireless to report to Priya
- [ ] Email TJ about getting absorption for a given thickness at 532 and 1064 (what did Ben S say about it?)
---
### 7/02
- (little bit of a repeat) JP built a TGA MS similar to what the MSC has
- H2 basically fully peaks before the methane begins to come off, reinforcing notion that H2 removal is a part of the mechanism
- to-do
	- get good pics/vids of before/after samples and the lasing process
### 6/26 Notes
- Paper notes
	- (2024) Horcher - Ceramic coatings from PDC (silazane + Al2O3/ZrO2) lasing
		- motivated by need for ceramic coating formation mechanism where heat does not penetrate to the substrate, permitting application of materials which cannot be exposed to corrosive environments, but are thermally sensitive (here, high strength-to-weight magnesium alloys)
			- first establishes disadvantages with alternatives:
				- electroplating and chromating deal with toxic chemicals
				- anodizing with hard oxide ceramic-like surfaces leads to porous coatings which are permeable to corrosive environments
				- organic coatings are limited in application temperature and are susceptible to mechanical damage
				- vapor deposition (CVD or PVD) are costly and limited by their complexity
			- PCDs are good (commonly poly-siloxanes, -silanes, -carbosilanes, and -silazanes)
				- suspensions can be applied to surfaces through simple methods like dipping, spraying, spin-coating, and doctor blade
				- drawback is high shrinkage (~50% volume) leading to pores/cracks increasing with thickness due to gaseous pyrolysis products



### 6/25 Notes
- Rob opening notes
	- on-site is on (?) get to program manager 24th of July, so we need abstracts from everyone who is presenting for the posters everyone else is presenting
- Ben S.
	- MS signals show propane and butane ion currents raised around 200 C
	- Rob - Check out broader source of papers on hydrogen release to get ideas for how to measure it better (H2 release as novel mechanism to precede ceramic transformation, particularly with photothermal)
	- DCM cast samples appear different from the previous samples which might impact the ellipsometry that JP's group will do, and so Ben will have to think on whether JP's group is ok with that before he gets me sample
		- Rob - "I think the cloudiness is a surface roughness thing because it's a homopolymer and homopolymers don't phase separate...maybe do an SEM of the film and see if it's porous...try holding cloudy samples at 75C in vacuum to anneal out the voids...maybe some kind of evaporation induced phase separation...interesting to consider if voids/pores play a role in photothermal absorption"
	- Tainara XRD indexing shows BSi and no graphite
		- Rob - "your silica should convert to quartz at these temperatures...that amorphous peak is throwing me off because everything (except for some carbon) should be crystalline at those temperatures)...try SAX and WAX"
### 6/18 Notes
- Asma slides
	- above 1150K, B10H14 --> B10H12 + H2 is spontaneous
	- barrier is ~150 kcal/mol forward, ~90 backward
	- experimental H2 barrier calculations would be highly valuable
- Ben S slides
	- TGA-MS shows H2 and CH3 largely coming off first at ~300 C, both losses largely leveling (maybe H2 goes up a bit at 600 C and drops down).  Ben L raises point that it's really hard to compare the H2 and CH3 quantitatively b/c of unknown ionization efficiencies 
- note to self
	- Find a k-type to test for Priya
	- Find photosensor (look up what accessible tech is highest response time)
	- email TJ 

### 6/11 Notes
- Ben S. GCMS H2 (m = 2) peaks start alongside the small molecule (m = 15) (2500-4000 s)
- JP - those boron species are highly reactive, "basically just jet fuel"
	- JP concerned about the distance between the TGA and MS
	- Pick up some thermally conductive tape to apply to sapphire
- Ben - might be better with Ar carrier gas instead of N2
- What was called B-H peaks evolving in FTIR approaching 1200 C (in Molecules 2018 23 2461) is dubious, lending weight to our skepticism of their proposed mechanism
- JP will measure optical loss (k) on sapphire samples prepared as consistent as possible to explore why it is that absorption seems so low yet we're producing so much heat
- Check into literature to see what we're doing differently
	- is our mechanism different, "do we need this mechanism we're proposing"

### 6/4 Notes
- GCMS doesn't show much change and there's some doubt about the veracity of the data considering the strangeness of various peaks
- Could we borrow Ray's H2 meter to sample the gases that come off (if a lot of H2 comes off, it reinforces the "H-removal --> reactive boron" mechanism)
- 'think about how many times you're hitting one spot etc.' ask Ben what other than the notes would be helpful
- misc neutron scattering thoughts from Rob
	- maybe think a bit about the impact on the pyrolyze-->infiltrate cycling repetitions
---
### 5/28 notes
 - characterization may pivot to Raman-AFM
 - MS plotting update reveals some H2, CH2 (or BH3), and C2H4 (or B2H4) release at 250 C oven treatment, corresponding to some simulations
---
### 5/1 notes
1. ‘Necessary to initiate that first step, release of the hydrogen’
2. Do the thermocouple experiment to see if there’s any exotherm that arises after the laser pulse (in excess of the energy of a pulse)
3. “What if we made thin boron films on graphite” (or B  with a polymer layer on top) + BC4 and laser both and see what exotherms and products result
4. ‘We can start thinking about boron-carbon phases that form’ (phase diagram)
5. Tainara + JP show a boron-rich phase is forming in XRD
6. Ben Stovall follows up that he suspects boron oxide based on his XRD
	1. Rob warns that the literature mislabels XRD indices routinely, so be careful
	2. JP warns that a certain splitting feature suggests something highly crystalline (likely substrate) and so they warn to get long reference scans for the slide next time
7. Rob warns we need to spend more money - only $650k out of a bunch more after the first year
	1. Real problem is when we spend the money but we’re late with invoices - be sure we are spending and invoicing or we could lose money
8. Tainara SEM
	1. Keep note of the duty cycle (pulse width/rest period) for future samples
	2. 20 kHz vs 200 kHz look pretty different - 200 kHz looks like a honeycomb, but do 
	3. How far does what size beam move during a single pulse
		1. Try just lasing one a single spot (no movement) to see if it accounts for the weird scarring patterns on the SEM images
		2. Try making the beam as big as possible and change the duty cycle at a single spot
		3. ‘Anything we can establish as a constant, we have to march through that parameter space’
		4. How can we get it to not move at all? Try at minimum speed when the beam size is big from being defocused (or lens expanded) so that it doesn’t move off the same spot
			1. Or just try the YAG which is static and big already
		5. Is there a way to get a single pulse (or just set such a high scan rate that you get a single dot at each point (make dotted lines to create a parameter grid of pulses vs energy densities)
9. Ben Stovall will give me samples which aren’t super uniform this week, but next week they will be and then we’ll do the parameter space for JP
	1. This week, we’ll give the samples to Tainara to cut into pieces herself
---
