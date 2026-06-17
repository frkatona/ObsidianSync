## General Interview

## timeline
- 9:30 - voice STAR

### examples/responses with the 'STAR' method
- Situation (20%)
	- what is some brief context for the story?
- Task (10%)
	- what was the problem/task/challenge you took responsibility for?
- Action (60%)
	- what did you do?  Highlight skills and character traits
- Result (10%)
	- what positive outcomes followed from those efforts?

### STAR stories
- situation which involved fast pacing or multitasking
	- **Situation/Task** 
		- post-doc MURI collaboration + safety officer + group meeting coordinator + instrumentation + mentoring
	- **Action**
		- using calendars and when2meet polls, creating reminders for me to send gentle reminders to participants
		- documenting readable status and procedures in a shared location, along with comprehensive photo/video record
			- also, making everyone aware of it by showing them my screen accessing it and explaining where to find everything at least twice
	- **Result**
		- managed to never be caught off-guard and was the lab's central resource for ground truth
- troubleshooting
	- **Situation**
		- samples meant for pyrolysis were combusting in air, and the commercial air-free chamber was inflexible for the targeted improvements
	- **Task**
		- find a better way to protect the sample from oxygen atmosphere
	- **Action**
		- custom-built flow/purge chamber.  Researched materials which were compatible with our laser systems, purchased sheets, machined to size specifications,  tapped/melted gas ports, added downline bubbler
	- **Result**
		- first consistently successful conversions
- surface

### on-the-job problem solving example
- customer problem
	- high rolling force / dirty strip, instability, corrosion, foam, poor cleanliness
- likely variables
	- concentration, droplet size, surfactant balance, pH, water hardness, temperature, contamination, iron fines, microbial growth, base oil-additive depletion
- tests
	- FTIR, viscosity, acid number, saponification value, pH, conductivity, microscopy, particle/iron analysis, emulsion stability, foam, corrosion/stain, tribology
- 

### generic Q&A
- Tell me about yourself
	- Undergrad at Susquehanna University, considered Astronomy (first published paper in an astro journal on research at my first Summer there) 
	- Ended up liking chemistry lab more, finished with a BS in biochemistry and physics minor
	- Grad school at Penn State (UP) for chemistry working in a nanoparticle lab just starting to apply laser heating to the synthesized nanoparticles
- Tell me about your research
	- A lot of work with elastomers, mostly silicone (Sylgard 184 PDMS)
		- context of lasers + nanoparticles, and mostly with thermosetting silicone rather than lubricant formulations
		- but flow properties of the elastomer was relevant
			- performed kinematic viscosity tests according to ASTM D445
		- used parameters including flow behavior and IR spectra to update our formulation (absorption agent additive).  
			- one published paper focused on how our thermalizing additive would inherently interfere with consumer utility (because thermalizing more light means less optical transparency) and so we found through Python thermal modeling that even at visually undetectable loadings, temperatures rises sufficient for thermosetting should be accessible.   
	- Maintained vacuum pumps
- A time you had to deal with conflict
- ^etc

---
### Job Content
- video
	- worldwide supply of lubricants specifically for cold rolling steel ("rolling oils")
	- cold rolling
		- **steel strips** are passed through **work rolls** at high speed and compression
			- reversing build - several passes in the same set of coils
			- tandem build - successive passes
		- temperature ranges from ~20 C to 160 C (320 F)
		- keep cooled and lubricated by spraying **oil + water emulsion** on strip surface
		- the strip accelerates at the rolls due to the thickness reduction, which creates high sliding speed at the contact
		- term: **"roll bite"**
		- film thickness increases with mill speed (also dependent on lubricant properties)
		- film thickness decreases with oil starvation (also dependent on the emulsion properties)
		- the roll and strip surfaces are in close sliding contact
- wikipedia
	- cold rolling keeps T below recrystallization point of metal which is usually ~0.3-0.4x its melting point
		- steel melts above 1370 C, so 0.3 x 1370 C = 411 C
	- Rolling mills are often divided into roughing, intermediate and finishing rolling cages
- Chad
	- QH's steel rolling oils are used for cold rolling as oil-in-water emulsions and neat oils
	- goals include lubrication, cooling, cleaner strip surfaces, less iron-fine generation, reduced roll forces, improved roll life, productivity, cleanliness, and lower waste-treatment burden
	- Cold rolling process fundamentals
		- Cold rolling reduces steel strip thickness by passing it through work rolls
		- the lubricant must reduce friction in the roll bite, remove heat, protect surface quality, and help avoid defects 
			- defects include pickup, staining, poor cleanliness, excessive iron fines, roll wear, chatter, or inconsistent thickness.
		- “The fluid is not just a lubricant. It is part lubricant, part coolant, part surface-quality control system, and part process-control variable.”
### questions for Sarah
- where does Sarah work?  what does she do?  what are her accomplishments?
- what was the conference?
- what is the day-to-day like?
- what goes into formulating lubricants
- what papers/books does she recommend?
- chemistry
	- colloid/emulsion chemistry
		- using oil/water emulsion (is it just lubrication from oil + cooling from water?  is it just because of water's heat capacity that it's there?  Does it not worry about phase changes?)
		- surfactant hydrophilic-lipophilic balance (HLB) - does surfactant favor O/W or W/O emulsion behavior
		- critical micelle concentration (CMC) - when micelles begin to form, affecting cleaning, wetting, and emulsion behavior
		- droplet size distribution - affects stability, delivery, plate-out, filtration, and consistency
		- Zeta potential - indicator of electrostatic stabilization (not only stabilization mechanism)
		- Hard-water tolerance
		- foam control
		- pH/conductivity
		- biostability - water-based systems may support microbial growth if not controlled
	- surfactants/additives
		- base oil / ester / synthetic lubricant - lubricates, forms film, has good thermal behavior; high surface affinity
		- emulsifier (/"surfactant package") - O/W stability, wetting, plate-out, bath behavior
		- extreme pressure (/"antiwear") additives - boundary protection under high load
		- corrosion inhibitors - staining/rust
		- antioxidants - extend fluid life
		- biocides - control microbial degradation
		- defoamers
		- pH buffers - bath stability, corrosion, microbial resistance
		- couplers / solubilizers - improve compatibility of formulation components
	- tribology
		- coefficient of friction
		- wear scar / wear rate
		- boundary, mixed, hydrodynamic, and elastohydrodynamic lubrication
		- Stribeck curve - friction as a function of viscosity, speed, and load
		- viscosity (important, but not everything)
		- why lubricant will perform differently in a benchtop test vs actual mill
		- ASTM D4172 - a standard four-ball wear test used for preliminary evaluation of antiwear properties of fluid lubricants in sliding contact; it is not a rolling-mill simulation, but it is the kind of standardized tribological screen you should recognize
	- analytical tests (and why they matter)
		- FTIR - identify formulation components, oxidation, contamination, water/oil differences
			- FTIR
		- viscosity - lubricant handling, film formation, concentration, oxidation/degradation
			- ASTM D445 kinematic viscosity of petroleum products
		- Acid number / TAN - oxidation, degradation, acidic species
			- ASTM D664 covers acidic constituents in petroleum products and lubricants
		- Saponification value ester/fatty material content

Chad questions
- is water's heat capacity the main reason why it's there?  are there no big problems with phase change at the temperatures/pressures involved?
- what do "plate out" and "bath behavior" and "boundary protection" "and "wear scar" mean?
	- Boundary, mixed, hydrodynamic, and elastohydrodynamic lubrication
- zeta potential
- what is usual CMC value?
- what base oils are common?  what oils did they replace and how did they improve on them?
- what specific additives are most common specifically for these kinds of applications
- what are some tools/devices/instruments that would be used commonly in the determination of these properties?
- difference between wettability and surface affinity?
- why would a lubricant perform differently on a benchtop vs mill?
- what specifically would you look for in an FTIR to identify formulation components, oxidation, contamination, and water/oil differences?  Is FTIR not generally difficult with so much water? 

Chat questions 2
- why is it called "synthetic oil" if formulations usually begin with a base of crude oil like mineral oil does anyway?  Isn't it just mineral oil with additives?
### Questions for interviewer
- Curiosity
	- What kind of project ownership / independence should I expect? 
	- What is the balance between new product development and field-support troubleshooting?  Things like conventions?
	- What are the most common failure modes the lab is asked to investigate?
	- What tests are most predictive of mill performance?
	- Do you evaluate the metal surfaces for asperities/roughness?  Anything precise, like TEM
	- Work culture
- Brass tacks
	- Pay
	- time off
	- hiring timeline

### Questions (lingering)
- Cold rolling
	- how big of an industry is it?
	- who are the major vendors?
- Advantages of
	- hot vs cold
		-  Steelwork processing with large pieces of metal used in hotrolling: ingots, slabs, blooms, and billets
	- tandem vs reversing
	- horizontal vs vertical vs universal (rails + H beams + wide plates)
- Milling terminology
-

### sarah call tips
- "tell us about a time you've had a solve a problem" "why do you want to work here" kind of questions
- questions back "how do you like working here"