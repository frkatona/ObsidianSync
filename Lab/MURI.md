
### Experimental conditions to try once we have samples
- single line (how far out does it reach?  what resolution do we have?  does it correspond to the same line made on a piece of steel or something under the same conditions?)
- one-shot
- defocused beam
- scan rate/pulse rate such that there is no overlap
- laser -> XRD -> laser over the same space
	- iterate over same space
- thermocouple
- open to ambient atmosphere
- PCOD

### 9/17 Meeting Notes
- Asma presentation
	- simulated the PCD polymer change
	- MD at 1000, 1500, and 2000 K after 250 ps
		- 1000 K - (not very significant decomp) - 5 species (evolved? created?)
			- "system largely stable, only minor fragments observed"
		- 1500 K - 'significant' decomposition begins - 30 species
			- "significant fragmentation"..."medium clusters + boron hydrides form"
		- 2000 K - 'extensive' decomposition/degradation - 70 species
			- "many small molecules and clusters"
	- Ben S - we see the degradation begin earlier in the monomer than in the polymer
		- Adri responds with simulation to pursue this
- Kevindi - PCOD
	- Oven treated film looks nice
	- FIB and high-mag CTEM and SAED analyses
		- B4C, SiC, C observed, no (crystalline) SiO2 was observed (but tough to say about amorphous SiO2)
		- EELS map of cross section - Boron layer on the bottom ~1 micron, O2 on the top ~1 micron, Carbon distributed across, but with more in the top ~0.5 micron
			- Rob - Si might be missing because it's tough to see with EELS, but we can go back over with EDS
				- C tends to form at the top because of its low surface energy (Adri - carbon is a great surface former) 
### 9/10 Meeting Notes
- Ben S.: probably no laser stuff until the JP spin coating gets figured out...but no polymer until the glovebox problem gets figured out
- Tainara SEM images
	- inhomogeneity
- ***JP wants to know the power averaged over every pulse over the area of the sample surface (use pulse power, number of pulses, and scanned area)***
	- the distance between the lines is big compared to the spot size and so this number may not capture what I understand JP to be looking for, but he would like it anyway
	- bring value in "per hundred micron"...I guess to be safe, bring value also across the entire surface
- Ben S - new samples are ~100 to 150 um, but we'll spin coat going forward
- JP - we're getting much more conversion than the beam size, so let's test it with a single line
- Ben Lear - etch metal to make sure that the size/focus is actually what we think it is (at least that the stock values are accurate, i.e., 100 um) 
- JP - "the finest coating that would be considered functional is 5-10 microns"
- Rob - try PCOD (precursor without boron cage) again
### 9/4 Review summary notes
- PDCs are advantageous because they tend to yield ceramics under more mild conditions than traditional powder-sintering routes (~500-1000 C vs ?) and are chemically versatile in the elements they incorporate and how they control their 
- Ovens are still disadvantageous because they take a long time and ceramic systems are limited to heat-resistant substrates
- Laser-based ceramic formation opens otherwise-impossible precision (i.e., direct writing), speed, and applications (e.g., additive manufacturing)
	- Also, metastable states and defect structures are uniquely available through pulsed photothermal pathways due to rapid quenching
		- bear in mind that this rapid heating and quenching also induces intense thermal gradients, and thus high thermal stress, shrinkage, and cracking
			- strategies to mitigating cracking include scanning in overlapping passes, reducing pulse energy, and using multi-layer polymer coatings (which distribute shrinkage) 
	- Also, sensitive substrates that cannot withstand hot, long oven exposures (e.g., Mg at 1000 C) need not be exposed in photothermal procedures
- Absorption challenges
	- at 1064, Horcher et al (2024) added Al2O3/ZrO2 to their organosilazane to tune absorption 
	- Wilden and Fisher (2007) mention that only thin coatings/fibers at slow ramp rates and long dwell times are possible because of (1) degassing during pyrolysis and (2) residual stresses within the components 

### 9/3 PSU meeting notes
- Rob - working on setting up monthly meetings
- Ben S - made a spreadsheet to consolidate sample synthesis details, characterization, and results
- Rob - We gotta figure out what is absorbing, why we're able to thermalize
	- '2 pulse idea' kinda didn't work out by next test
	- explore 2PP more
	- Ben S - use more UV/Vis in-lab
- JP - spin coating problem can be solved if Ben S 'tricks' the instrument to permit it
	- 'if i have 1 um of precursor, what is thickness of lased ceramic coating'
- Rob - other substrates - metal, etc.
	- what would we want for a paper?  properties or just that it happened
	- JP - if we can show it, that's good enough
- JP - take one sample, give it 100k pulses over square cm, XRD, put it back in the laser, repeat procedure on the same spot
	- Ben L - but does it matter that you're letting it cool between attempts, so try it a different way as well - separate pulses - follow up
	- **send "energy density per pulse" to JP**
- Rob - can we compare this to what other people made e.g. polycarbosilane...what are the differences
- Ben L - once we can reliably get the thing we want, try in ambient atmosphere

### 8/28 thoughts
- Sample conditions
	- repeat
		- 50% power, 100 mm/min scan speed (replicate 1)
		- 100% power, 30 mm/min scan speed (replicate 2)
	- new ideas
		- 25% power, 100 mm/min scan speed, repeat passes until black
		- 50% power, grid of increasing scan speeds, up to 1000 mm/min
		- rep rate
### On-site notes
- Alex brought up an interesting-sounding paper, something like "co2 laser rearrangement 33 sigmatropic shift multiphoton absorption ground state photochemistry"

### 8/26 thoughts
- should someone reach out to Rob for next meeting and the data labeling ideas
- Ask Ben S about the sapphire substrate to help avoid shattering
	- who sells it, is it ion-implanted, can we get a thicker version, or can I use some PVB on it with a glass secondary substrate to prevent shattering
### 7/1 thoughts
- work on scripting (ideally no labview, but maybe labview) 
	- visualize oscilloscope output in real time
	- sync with a secondary input
	- capture output a given time
	- fit a blackbody to 4 points
### To-do
 - home
	 -  Search one last time for temperature determination in literature
		 - Onedrive folder
		 - wider lit search
	 - Purchasing
		 - cga-350 regulator
		 - O2 sensor
		 - 
	- Lase
		- Alex R.'s sample
		- Paper or something to see if the chamber is insufficient

- Find out if we are retaining ligand from the polymer
	- [x] run the white sample (no Boron) see what happens
		- recall that TGA shows polymer without boron degrades around 450, but around 250 with Boron
	- [x] bring it back on Sapphire for Tainara to cut
- [x] Buy stuff as soon as spending resumes on 6/30
	- Vacuum chamber
		- [x] Regulator (check inlet type) - [CGA580 inlet](https://www.amazon.com/ARCCAPTAIN-Regulators-Welding-Regulator-Connection/dp/B0D1KD5ZPT?sr=8-10) - $40
		- [x] bolts (6", full thread + nut/washer x4 [Amazon](https://www.amazon.com/Screws-Extra-large-Washers-Threaded-Stainless/dp/B08DCGY4X3?s=industrial&sr=1-4) $13)
		- [x] acrylic (12"x12", 1/4" thick [Amazon](https://www.amazon.com/CALPALMY-12-Plexiglass-Projects-Engraver/dp/B085L5V796?crid=1GQMAO77Q83&dib=eyJ2IjoiMSJ9.OcoZFCkOqjT5vO0DxOV-wO7CEYIzq74an48RTH2m1DEHDiIwvwJYu9-C2YMjiFj41Do-7GHHnamN6VtGDpCXweVX2ou_Ou1ZP35f1dxLoq27cFI9uMtdOLnuwHUTnNeMHVRTagun89lVSQ0fbsh1PynF6NN51iz65oVVhwdQRUzGvNz__b6R6c6iy12up6EtOMPUCsZv39F0zFnMcsGpBrIZq2X0T62RtHBAvGJqOKyRL11ZsuJGZNGiIQ4h39aF6SMJLMq5YlQybdUkSJGEgrUJvj3mxUYOXTPIrk9x7Uw.vtCB1BMvPnFqxZSJ1p7zmyWYxiMERycBsj4KOrYHL6U&dib_tag=se&keywords=acrylic&qid=1753195340&s=industrial&sprefix=acrylic%2Cindustrial%2C111&sr=1-9&th=1) x3 = $45)
		- [x] Weld-on Acrylic bonding agent ([Amazon](https://www.amazon.com/Weld-Acrylic-Plastic-Cement-Applicator/dp/B0149IG548?sbo=RZvfv%2F%2FHxDF%2BO5021pAnSA%3D%3D&sr=8-3) $17)
		- [x] gasket silicone [Amazon](https://www.amazon.com/Silicone-Rubber-Sheet-Durometer-Thick/dp/B08DDFQ9YM?crid=2SEL66BI1MQKS&dib=eyJ2IjoiMSJ9.G1-p0GLr7hKGThxt4fS5DB-Y8wjJNhxrgWHQsq3DhOQnB2cHlSIMi0q2KR3yii0SA0SmypuUDuo9dyWCnOofWdKyBhgLNbkcONmzaxuwgoFkSJ6dKsgCqiw-KcbX9-kC-Kgz9C1ZUEDhW6oLjwugJZgZppafumV8s5vd7kS0GltAolHXUKj-_-mN4mttr_FZiWwEWjZ4pP4zdg3bXCxAM7AuMjH1hQ_P6u12si42zZU.Cqc6Ol_9LzMXTuHHK6E3czbm4LFDSiTcEV7FZMSIA_8&dib_tag=se&keywords=food+grade+silicone+strip&qid=1753196984&sprefix=food+grade+silicone+strip%2Caps%2C129&sr=8-2#averageCustomerReviewsAnchor) $10
		- [x] bulkhead fitting sample port, 2" ([Amazon](https://www.amazon.com/Murtenze-Connector-Stainless-Thru-bulk-Aquariums/dp/B0F9K83TMH?sr=8-10) $21) - close with extra gasket or rubber stopper and add syringe
		- [x] bulkhead fitting gas connector ([Amazon](https://www.amazon.com/Joywayus-Connector-Theaded-Bulkhead-Stablizing/dp/B07GPP23K9?sr=8-15) x2 = $18)
		- [x] O2 trap [Analytics Shop](https://www.analytics-shop.com/us/re23805?utm_source=google_shopping&utm_medium=cpc&gQT=1) $256
		- [x] 1/4" hose connector [Swagelok](https://products.swagelok.com/en/c/connectors-plastic-tubing/p/SS-4-HC-1-4)  x2 = $??
		- [x] 10 ft vinyl tubing [Amazon](https://www.amazon.com/Flexible-Lightweight-Plastic-Chemical-Resistant/dp/B09Y5R8SSL?dib=eyJ2IjoiMSJ9.g6lpmgC4OwdfJr5JxOivXbCFu86BZrR1i_9NFP94kyriBVoup0Uouvy45WLNvyJK7OduydBUqrWVpZbnaUV4rHV5e0_E7LmziiRQfQpERdh5F1WHAiNdFk0YVNLdB1BLvds2NZYdHHmMzYZBubTK-xMZh60BpRxnKB-rJC7lCrODS0IFutDpC_Qp7LAJ9kDJVxYuCMqo14ndWUoYXW0-Hg0R2ndA0nfOpCG_eDdfZI3yifbOYUxoyUIkGFwpq90Bp6U5BruDpfJqjCaVs7u7Op7DisIrQ-YS13FXuEcQ9Ks.23IpNb2foQzpV5fC424uOByM35zUHR9OX09f_FQJFHM&dib_tag=se&keywords=gas%2Btubing%2B1%2F4%22&qid=1753203818&sr=8-2&th=1) = $9
		- [x] probes [Amazon](https://www.amazon.com/Universal-Oscilloscope-Accessories-100MHz-Minigrabber/dp/B0827JL1T2?dib=eyJ2IjoiMSJ9.bZDc7MWRCkthqLP5DJaRzdcr6JlDc8vZvjPJgrYsIHYwYWkk00pPTMLTbdri5CpH8gJLSaf-TYzBoizQTsDiRD_ZQY_hp0e7QGi01MFegNKD0CHWxtxD8RgvDAl8YNQrSnZryYO52ddxszK5M0_3qTUidKemcfH-K99z27IVan-NTtR8KiNHMPh8kq6SGPghCPJkdBhNyP1MZuyBmrVmS-dWHYSkqS8uov5LlgQwui8.Y4Et6cg30FpgT688ViJRaMKz2Qg0hL7JPIZIArDB85I&dib_tag=se&keywords=oscilloscope%2Bprobes&qid=1753201681&sr=8-3&th=1)$30
		- [ ] O2 meter $???
		- [ ] thermocouple (type k? cold junction?, get sensor and reader)
			- [x] acquire low-T wireless electronics with I2S compatibility
		- [x] forming gas (just get an H2 cylinder to run with Ar? Or is there Ar + H available?)
	- Thor etc. vendor purchases
		- [x] optics (OAP)
		- [x] detectors
			- [x] photo-diodes and photo-multipliers with rise times of ~nanoseconds (e.g., InGaAs or Ge photodiodes for the near IR ~800-1700, e.g. Xu et al.)
			- [x] split wavelengths (filtered mirrors? prism/grating?)
				- [x]  dichroic tree and bandpass filters
				- [x] signal enhancement (APD)
		- [x] ADC/Data Acquisition
			- [x] Tektronix oscilloscope (file:///C:/Users/antho/Downloads/071281002web.pdf)
	- Vacuum container
		- able to mechanically seal, resistant to positive pressure (maybe bolts, but ideally something like a [toggle latch](https://www.amazon.com/Toggle-Latch-Pack-Adjustable-Industrial/dp/B0DKFPCRWG?dib=eyJ2IjoiMSJ9.n4y-4bK6e84yc7qxJion7bHdlDnSr3YWVcDGWarWVgOQO41DWCpuaXuUtMXyuSBrX70luV1KdsihFEV_aSipPKLUbER6pckyyDU6dvCkkHKZodt-IBVw8wIZ903QuhqToGwgTIAees8CkSHfSj525Pm4I8tg_BLfWfgJcY6EUn1ZuV3y4MacADrdSfs0SRlGn1IlpegANrXD2mAzCpuDKXnKYxpypZob-00ucG9HJYr2LaFl-9ghPYVEc1Gg-Wl5VD7AsidH3lUTUM3K5Ciw8Pd-lnxucNsUPvMNjI7LSF8.IfA3-UC-2EnzsI7GxKMGerrF6zxfPwCpp4ekDOYz74c&dib_tag=se&keywords=toggle+latch&qid=1750951998&sr=8-1) ~$17)
		- low absorption, strong, transparent enclosure
		- big enough to house O2, H2O, VOC sensors + pyrometer
		- port for wires
	- Find literature for errors from emissivity which supposedly become overwhelming at high temperatures and with increasing surface oxidation  (also calibration drift)
- [x] Get or take a desiccator downstairs (ask Kristen, see if it needs regenerated/bought again)
- [x] Acquire forming gas (H2-balanced Ar)
- [ ] Get FLIR images with or without wireless to report to Priya
- [ ] Email TJ about getting absorption for a given thickness at 532 and 1064 (what did Ben S say about it?)
---
### 8/7 On-site Review
- Rob presentation - project overview
- Mike presentation - 3D printing, Raman characterizing, and infusing PDC precursors
	- PDC design - partial focus on amount of C and O desired in product
	- Evelyn's real time Raman monitoring of 
	- Si NP carbon scavenging ('reaction bonding') at 35 wt% and 1400 C
	- Q - Kenneth Lipkowitz - shrinkage is the 'kiss of death,' what are you thinking to minimize it
		- A - 'atom economy' is the name of the game...ideally you can just keep all atoms the same and rearrange the bonds...it'll come down to the hydrogen which is hard to get rid of in the design of the PDC precursor materials
- Adri presentation - ReaxFF force field development and simulations
	- Nomura et al Scientific Reports 2016 - absolutely sick looking 3D graphiticization web formation animation
- Alex presentation - designing ideal photothermal SiC precursors 
	- photodecomposition (solid, synthesize as designed) vs photocaging (molecules designed to release targets)
	- tetra alkyne Si-Si compound in our lab - shows UV Vis peaks around like 300ish nm (missed what the 3 curves were) and we should try to determine ideal absorption
- Aiichiro presentation - MD and ML of photochemical pyrolysis of Si polymers
- Rob presentation 2 - ROMP and PCD
- Ben
- JP
	- Indexing B4C is super hard --> lots of BC and BO look the same...but we still probably have B4C with really nice, big grains
	- building YAG into TGA-MS
	- idea: plasmonic field enhancement
	- future: Intense Pulsed Light (IPL) zaps a sheet of paper size at 1 Hz with like 96 J/cm2
- Adri
	- energetically, BC is really unstable, but B4C is only slightly more stable than B or C alone (both of which are considered quite stable)
	- alternative H2 release pathway through decaborane dimerization with modest activation energy
- Priya
	- mechanisms for evolution of methane, ethene, propane
- Pani - ONR review comments - good job with first year, try not to lose focus in the second year; we could have better clarified role of separate theorists and how specifically they contributed to the experiments (just a presentation note)
	- keep an eye on budge; - continue to spend the money and submit the invoices
- To-do
	- add images, other links to the QR code repo
### 8/6
- Ben S.
	- the original lased sample (nice pic) looks maybe like boric oxide or boric acid
- Rob
	- make sure we're doing like 100 C overnight with samples and lasing right away (water is hard to remove at RT)
	- looks like maybe it's boron oxide, but B metal may form, so try to be very thorough with sample prep
	- presentation
		- Kavindi's PCD-grafted silica lead to some B4C/SiC composites through carbothermal reduction
- Tainara
	- the ones we've indexed could be oxide or acid or something
- Notes from me
	- I don't have any XRDs, but we can lase an open-air PCD asap, either now or as soon as its out of the oven
	- sapphire sample I lased didn't look very pure in either chamber
		- lasing from the bottom resulted in some colored specks that look a little iridescent
- Ben S uses argon with 5% H2 for his oven pyrolysis
- REMEMBER
	- tomorrow morning set up posters at 8:30
	- dinner tomorrow evening, whenever we wrap up we'll walk down to Allen St

### 7/30

- Rob discussing a meeting he has to go to where he's making a quad chart that was DC but now isn't
- travel restrictions are hampering a few members, we'll discuss presenting tomorrow
- JP warns that budget is difficult to modify without the project getting scrutinized
- Get a CGA 350 from JP/Tainara
- JP's group will check out Raman and re-do XRD for the previously lased samples
- JP will also get Ea for the H2 release using calorimetry to report back to the computational people
- to discuss
    - [x]  CGA 350 regulator/adapter
        - will pick up from Tainara
### 7/23 In-person meeting notes
- Asma had questions for Ben S about the structure of the compound
- Ben S points out that the PCD structure can be drawn with the vinyl group at the edge of the repeat unit, but also not, and it's unclear how that influences the simulation -- and Asma's units may have been missing a carbon
- Ben S uses ~50 ccpm for his Ar flow, which I should try to use for my new flow chamber 

### 7/21 Ultrafast Blackbody Thermometer Notes
- (2011) Ni, P.A. et al ["Multi-channel optical pyrometer for sub-nanosecond..."](https://www.osti.gov/servlets/purl/1016573)
	- pyrometer is just an absolutely calibrated spectrometer operating at several discrete wavelengths in the visible and near-infrared regions which compares thermal radiation to temperature of the Planck formula
	- take into account all speed determining factors (modal dispersion of fibers, photodiode rise time, oscilloscope bandwidth)
		- but understand that all speed improvements will also lower sensitivity
	- Light Collection (LC) system
		- thermal emission collected by a relay system of lenses (pair of achromatic doubles, f=75 d=50.8 mm, coated for Vis/NIR) mounted on micro-positioning stage in a vacuum, oriented normal to the sample surface
		- produces a 1:1 image of the target on an optical fiber
		- lens focus/aperture chosen to match NA=0.2 = 24 degree acceptance angle; step-index, multimode, 400 um diameter silica fiber
		- asdf
	- Spectral resolution
		- asfd
	- Light detection (sensor)
		- Need broad frequency response current amplifier with a flat gain curve between the low cut (DC) and high cut (~GHz) frequencies
			- DC important since calibration is done with continuous radiation sources
		- PIN photo diode models 1591 and 1592 from Newfocus Inc ultimately chose
			- alternatives like (1) avalanche photodiodes (APD), (2) photomultiplier tubes (PMTs), and (3) micro-channel plates (MCPs) are considered to have a low-frequency cutoff from 10 kHz, making calibration difficult
			- also, avalanches and PMTs have high noise levels and saturate quickly; and PMTs and MCPs use phosphor which degrades over time and requires frequent recalibrations (and cost a lot per unit, which is untenable for a multi-channel detection system)

### 7/20 - Alex Presentation Notes
- Zoom presentation for updates on the design/synthesis of precursors for SiC photoceramization
- SiC is a good target for low-T photoceramization (well-represented both conventionally and with pre-ceramic precursors; also DOE considers it important)
- Two approaches to SiC photoceramization
	- "Decomposition Approach"
		- design precursor with defined Si:C stoichiometry and photodecompose (likely H2), leaving SiC behind
	- "Photocaging Approach"
		- design novel molecules bound to Si/C and photolyze to release SiC
	- Either way, long-term hope is for new synthetic chemistry and transferrable knowledge
- The "Decomposition Approach" is largely about getting the Si:C ratio right
	- Si is reluctant to form multiple bonds to other atoms, especially itself
	- Ideally, the designed material will be made entirely of Si and C, perhaps some H if necessary to terminate valency; Si:C will be 1:1 and/or tunable; must have a homolytic chromophore (Si-Si bond) 


### 7/18 Thor
- long/short ratio intermediate NIR solution for ultrafast blackbody thermometer
- Collect/transmit NIR light
	- hardware?  positioning?  ask Thor
		- OAP
		- Lens + fiber
- Split halfway into the detector range (~1250)
	- 1180nm longpass dichroic [DMLP1180](https://www.thorlabs.com/thorproduct.cfm?partnumber=DMLP1180)  ($250) (variations for size) (see [graph](https://www.thorlabs.com/newgrouppage9.cfm?objectgroup_id=3313))
- Detector
	- Avalanche free space [InGaAs 850-1650 nm](https://www.thorlabs.com/thorproduct.cfm?partnumber=APD310) (x2 = $6000)
	- Amplified free space [InGaAs 950-1650 nm](https://www.thorlabs.com/thorproduct.cfm?partnumber=FPD310-FS-NIR) (x2 = $4500)
	- Ordinary free space [InGaAs 800-1700 nm](https://www.thorlabs.com/thorproduct.cfm?partnumber=DET08C/M#ad-image-0) (x2 = $700) (detector [main page](https://www.thorlabs.com/newgrouppage9.cfm?objectgroup_id=7537))
- Filter below and above the sensors?
- Misc.
	- posts, mounts, rails, signal cable adapter to BNC
---
### 7/16
- Pre-meeting notes
	- PCD sample
		- Results from last one?
		- Any new sample?
	- Ask for Alex's presentation recording on the OneDrive
	- On-site
		- We're giving poster abstracts to the program manager before July 24th?  Give to Rob or email directly?
- Meeting Notes
	- Rob is still gone, so it's just me, Ben S, and Kavindi (later found out Tainara misunderstood Rob's email and thought the meeting was cancelled)
	- XRD was down, so no new results about anything
	- Ben S is emailing Rob asking about the poster abstract stuff (when? to whom? any special instructions?).  He'll let me know what he finds out.
	- Ben S giving me some more sample on sapphire to lase
		- He wants the same procedure as normal
		- Remember to document the process well, both in notes and in taking good photos/videos)
		- He scored it and cut the sample above it with a razor in an attempt to get a clean cross section, but the sapphire cracked into two slivers off the main body (pics taken on phone)
			- I'll try to put a little tape on them to prevent shattering if they crack from thermal shock, same as the last samples, which seemed to work well.
	- Ben S put the Alex talk link, so I should check to see if there are clues to what Alex wants specifically from me for his sample that I got in the mail (or what it is/if it's hazardous/needs stored in special conditions)

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
	- on-site is on August 7th, get to program manager 24th of July, so we need abstracts from everyone who is presenting for the posters everyone else is presenting
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
