
### Chord progression notes
- Royal road
	- IV - V - iii - vi
- Diminished Dominant Creep-up
	- I - bii(dim) - ii - V7
	- (more broadly, to bridge any two chords a whole step apart)
- Lonely heart
	- I - bVI(7) - IV
- Get to the FOUR (aka 'minor v variations')
	- I | III7 | | vi | v - I7| IV
	- IV | III | vi | v - I7 |
	- ALSO add a passing bvi between vi and v
- Line cliche
	- vi - bVI+ - I 6/4 - \#iv^o - IV
- Transition1
	- I - bIII - IV - V---

---
Yuki Notes
- general
	- asasdf

Slides
1. ONR wants better high temperature materials
	1. (story) lots of talking about stuff before I care about it
2. Thermal protection challenges underly this interest
	1. (story) turbojet vs ramjet - unclear what the point is
		1. is the whole point to show that things get hot?
		2. (clarified that it's to show that there are reasons for both UHTCs and the more modest capabilities of B4C)
		3. Kristen's point: "delete 2000K"
3. Carbide ceramics are a good starting point
	1. Ben's point: "remake the melting temperature chart, but add lines to show where the engines lie on the chart"
4. B4C 
	1. Kristen's question "what is 15R"?
5. There are constraints on how we apply ceramic coatings today
6. Photothermal heat may offer a solution

---
### Database notes
- "Key Value" database (most basic)
	- fast (<ms), but limited space and no queries/joins/etc.
	- usually most used as a cache to speed delivery
- "Wide Column"
	- can scale horizontally
	- best for time-series, historical records, high write/low read
- Relational
	- scheme
- mysql under youtube and facebook

---
### 10/10 Nabankur meeting
- has met with Alex and (?) and ran some simulations and wanted to talk about what we're up to
- 1
	- P25108 polymer with cif (?) crystal structure (Akachukwu says "hexa ethynyl disilane", something like NUF1IM as a published structure)
	- SiCH-based polymer, did some NAQMD simulations by exciting one electron from HOMO, evaluating for 1.2 ps, analyzing the initiating reactions of the system
  2
	- calculated band participation numbers for each band
- 3
	- Density of states - occupancy at each band level
		- hole sits on the Si atoms, forming bonds initially
- 4
	- partial (until 500 fs) shows bonds, then bonds blow apart by 1.2 ps b/c it's too hot
- 5: Si-Si bond breaking
	- Si-Si crosslinks break around 58 fs after t0
	- then around 360 fs the Si are are forming with carbons
- C-C bonds are pretty stable until around 350 fs when they form bonds with the other atoms
	- around 404 fs, some C-C are still intact
- 7: Si-C bond formation
	- 296 fs some kind of condensation reaction which stays stable until close to 500 fs
		- so there's a window of ~200 fs where the bonds form without being broken?
- 8: Bond overlap
	- permanent bond breaking and formation seen for the three bonds monitored previously
	- Si-Si bond overlap goes to 0 from 0 to 200 fs and never goes up
	- C-C goes from 2 to 1 at ~150 fs and then goes to 0 around 400 fs
	- Si-C is 0 until it goes to 1 around 275 fs (graph ends at ~500 fs)
- Diffusion of elements
	- first h2 released at 871 fs.  Although H bonding shifts from one Si/C to another SiC/C before that from around 600 fs
	- there's a plateau of condensation below 600 fs, and then H2 seems to diffuse substantially afterwards
- Potential energy
	- a plateau of energy between 150 and 350 fs
- Bandgap
	- sharp drop at 100 fs indicating the systme undwent change in electronic structure signifying passage through a conical intersection which is a point degeneracy where two potential energy surfaces touch
- Temperature
	- T of Si is highest, switches to NVT at around 400 fs
	- drops at 350 fs where the highest condensation of the system could be expected after which the system temperature increases rapidly
- System evolving over time
- Silicon-carbon initial condensation
	- Si shows tetraveanetasdfasdf
- Bond Overlap
	- bond overlap  of different Si-C bonds indicate different bonds forming around 250 fs and different bonds breaking around that time due to rearrangement as seen in previous figures
- Key takeaways
	- screencaptured
Akachukwu will send the other compond for me to lase if we find something good with XRD
- otherwise will just keep chasing the polymer version of the compound 


send Sophia 3b1br
### post LD
- respond MURI email
- schedule time with Devindi
- read cover letter
- check out abetterrouteplanner app
- trash
- look up usage of assault in "sexual assault" (vs "sexual battery"?) 
- look up MRI day
- mark my/Yuki's MURI presentation in calendar
### IOOF Jam Songs
- What's Up
- Jolene
- Have You Ever Seen the Rain
---
## iphone upgrade notes
- dynamic island
- battery
- chip A14 -> A16
- Camera 12MP -> 48 MP; 2x optical zoom
- Emeregency SOS/crash detection via satellite
- Peak brightness 1200 -> 2000 nits (outdoor)
---
### website notes
- to-do
	- set time from the manifest (or otherwise extract on page load)
	- play button color and more clear in UI (big, center, visible on load from mobile)
	- download link
---
### Physics 70 years [video](https://youtu.be/d_o4k0eLoMI) notes
- 1950s - computer simulation started around 1950s
- MRIs
- Astronomy
	- 1967 - Discovery of pulsars
	- dark matter, dark energy, accelerating universe, cosmic microwave background,  pulsars, black holes (hawking radiation)
	- 2019 - first image of a black hole
- Particle physics
	- 1970s-80s-90s - tons of fundamental particles predicted and found
	- 1995 - Bose Einstein condensate
	- 2012 - Higgs Boson
---
### Vibe code song warmup helper prompt draft
I'm in the concept and early design stage stage of a webpage and I'd like your feedback on its helpfulness and simplicity/clarity of purpose.  I'd like to streamline vocal warmups and vocal self-evaluation for beginners through a stylish, interactive, step-by-step process where a columnar roadmap of steps presented as tabs such that the state within that roadmap are visible, but not intrusive.  Otherwise, the major visual elements on the webpage would be the current task in the step and the relevant interactive tool within the step.  For concepts that may be confusing to a beginner (e.g., passagio), a non-intrusive question mark icon would sit near the relevant words and reveal a snippet of helper text on hover.  

The warmup steps would include (1) Stretches, (2) Arpeggios, and (3) Sirens, while the self-evaluation would include (4) Range and (5) Passaggio Determinations.  All steps should be available to click between at will, but the user should feel visually guided to use them in the given order and for the allotted time (where applicable).  

The Stretches tasks would include neck (head rolls), shoulders (arm windmills), back (torso twists), and jaw (yawns).  Images of each will be on screen, as well as a timer which counts down from 2 minutes on click, simply directing the user to perform each at will for that time (no additional micro-managing).  After the timer finishes, the button to the next session would gently flash.

The Arpeggios tasks would include humming, lip trills, and vowels.  A piano would appear on the screen stretching from C3 to C5 with the A3 note highlighted.  The user would be prompted to select a comfortable starting note, triggering audio of the 5 note scale arpeggio.  A "repeat" button would repeat the arpeggio, and left and right arrow buttons flanking that button would trigger the arpeggio a semitone down or up, respectively.  While the keyboard is on screen, a checkbox would be visible titled "single note" which would make single notes play in place of the arpeggios.  Also visible while the the keyboard is on screen would be a series of thin bars running along the bottom of the keyboard visualizing the ranges corresponding to the ranges of six major voice types.  When a note is played, any bar overlapping that note would briefly and subtly change color.   Another timer for 3 minutes would be on screen.


The Sirens task would show a vertical bar which fills and empties at a rate of about 6 seconds per cycle, prompting the user to move their voice from their lowest to highest notes with even volume and timbre.  A timer for 1 minute would be on screen.

The Range and Passaggio tasks would use the same keyboard visual as the Arpeggios.  I'm still conceptualizing the best way to have the user know when their voice has weakened or strained sufficiently to return as they stray from their comfortable range.  Similarly, I'm unsure how specifically to have them navigate finding their passaggio, though I feel it's important to include  


side thoughts
- Should sirens start in arpeggios (slides)?
- soft palette lifting with "mmm-ah"
- Suggest a vowel for up vs down or "mee may mah moh moo"?
- Revealed hint text would suggest an intuitive visualization where applicable (e.g., try to imagine your voice here causing a candle flame to lean away from you without flickering)
- Beyond emulating artists, imitate environmental sounds and do character voices while trying to actively focus on the location of sympathetic vibrations in your head, neck, and body, or any other feeling
	- singer ideas? 
	- environment?
	- character ideas?  
		- Nasally - Urkle, Spongebob
		- Kermit?

### DaVinci Resolve Notes
- YT [color management](https://youtu.be/hgVqUATQSMg) for phone
	- color space transform for Pixel 8 Pro
		- "input space is" rec2020 HLG
		- "output" rec709

### music videos to note or remove
- 5 songs for guys
	- Lovely Day (B2-E4; comfortably chest-centric) 
	- Breakfast at Tiffany's (B2-D4; also pretty chesty)
	- Let Her Go (D3-E4; small range with bright voices)
	- Love Yourself (B2-B3)
	- Chasing Cars (E3-D4)
- Vocal resonance
	- resonators: larynx, pharynx, oral cavity, nasal cavity
- open mic
	- come up with better sign language for mixing levels
	- improve the microphone graphic and print it
---
- Ben recommended: (1) algorithms to live by, (2) super mario optimization

thinking of buying (removed from amazon cart)
- cable tester (# Mackie Cable Tester, 5-way switch Battery-Powered Connector Test, Black, (MTest-1)) - $35 today (8/25/25)
	- look used, try out Tim's
- CO2 [tank](https://www.amazon.com/VEVOR-Aluminum-Cylinder-Adjustable-Dispensing/dp/B0DXKZ14SY?sr=8-1) for soda stream replacement - $138 

### Blender video editing [video](https://youtu.be/n77Viu93pYI)
- after opening new video editor project, add a new window as a dope sheet and select View -> Sync Visible Range in both it and the sequencer
- show thumbnails and waveforms
- Open panels for histogram, chroma, vectorscope, luma waveform, and RGB parade
- Apply color balance as a modifier to an adjustment layer strip
	- start adjusting value of lift/gamma/gain
		- shift+drag for fine adjustments, monitor the vector
		- use eye button to mute and see change difference
- (something about streamlining animation) - pin scene
- 't' as a hotkey for keyframe interpolation modes
	- alternatively, use the graph editor to fine-tune
- Save a starter file with desirable settings and default file paths

### Misc. to-do
 - Watch
	 - [ ] Flow
	 - current anime season
		 - [ ] Kaiju no 8 [S02](https://www.miruro.to/watch?id=178754)
	 - older anime
		 - [ ] My Life as a Vending Machine [S01](https://www.miruro.tv/watch?id=153360&ep=1)
 - Play 
	 - [ ] Hades
	 - [ ] Hollow Knight --> Silksong
	 - [ ] Undertale --> Deltarune
	 - [ ] Darkest Dungeon
	 - [ ] Rain World
	 - [ ] Return of the Obra Dinn
 - Code
	 - [ ] Song scroller with more complete feature set and UI
	 - [ ] Color grade with sliders in Marimo
### Closed Tabs
- [Learn Git Branching](https://learngitbranching.js.org/?locale=en_US)
- [Tiger VNC](https://tigervnc.org/)
- [Selenium](https://pypi.org/project/selenium/)
- what is `pip install -e`?
- https://threejs.org/manual/#en/installation
- 3B1Br and Sebastian Lague Neural Network videos
- wiki islamic holidays
- setting frames to video length blender
- youtube [vibe coding microsoft](https://www.youtube.com/watch?v=eo9UKLqfjhI)
- hotkeys for obsidian commit and push
- esp button clicker game
- coding adventures: rasterizer
- w3 python reference list and string methods
- https://en.wikipedia.org/wiki/In-band_signaling
- https://www.instructables.com/Tales-From-the-Chip-LM386-Audio-Amplifier/
- https://en.wikipedia.org/wiki/Amplifier#:~:text=An%20amplifier%20is%20defined%20as,power%20gain%20greater%20than%20one.&text=An%20amplifier%20can%20be%20either,in%20almost%20all%20electronic%20equipment.
- https://www.youtube.com/watch?v=aRdiiWpA0AA
- [special search characters](https://www.digitalthirdcoast.com/blog/5-easy-symbols-google-work)
- https://zen-browser.app/download/
- https://www.masteringthemix.com/products/eq-academy
- [well posed vs ill posed problem](https://www.statisticshowto.com/well-posed-ill/)
- https://en.wikipedia.org/wiki/Barkhausen_stability_criterion
- https://en.wikipedia.org/wiki/Nyquist_stability_criterion
- Open source tools list
	- drawing - https://excalidraw.com/
	- penpot, ardour, applflowy, drone (ci/cd), 
- YT
	- [Building a Nanodrop Style UV/Vis Spectrometer](https://www.youtube.com/@thethoughtemporium)
	- [Object-oriented vs functional programming in typescript](https://youtu.be/fsVL_xrYO0w)
	- [Andre Kelley DoD](https://youtu.be/IroPQ150F6c)
	- [Every type of capacitor](https://youtu.be/Fwng7mRuOVw)
	- [simulating 256 bytes RAM](https://www.youtube.com/watch?v=HGkuRp5HfH8)
	- Ben Eater [8-bit Computer](https://youtu.be/HyznrdDSSGM?list=PLowKtXNTBypGqImE405J2565dvjafglHU)
	- [shadow math ](https://youtu.be/MuvuxHXLzls)
	- Ample Bass [1](https://youtu.be/2WrbDEUMPU0) and [2](https://youtu.be/bfB4tkRIp8M)
	- [Walking Basslines on Keyboard](https://www.youtube.com/watch?v=1ohTb1El06o)
	- [DIY Mass Spec](https://www.youtube.com/watch?v=nIKhUizkXxA&t=449s)
	- [Lighting in Godot](https://www.youtube.com/watch?v=aRdiiWpA0AA)
	- Legal Eagle - [Supreme Court Trans Rights](https://youtu.be/S80ivPamBoM)
	- Legal Eagle - [Religious Parents](https://youtu.be/Go3-HnVxres)
	- [LibGodot](https://youtu.be/L06KBOWCsSk)
	- [Andor Luthen Speech](https://youtu.be/-3RCme2zZRY)
	- Josh recommended YT video on Godot signals - https://youtu.be/w6jXgaWHo1s
	- Yt Crystals Upconversion - https://youtu.be/7WT0qZdHT5M
	- https://youtu.be/NSB6JrP--F4
	- [Complete guide to recording in FL Studio](https://youtu.be/qTh4COvhIs0)
	- music - [kishi bashi](https://youtu.be/5BiirTWso0s) (sophia recommendation) 
	- Ian Hubert - [talking about art in the woods](https://youtu.be/6LWZqmba0uw)
	- AI replacing humans going poorly - https://youtu.be/QX1Xwzm9yHY
	- FL Studio Emphasis [overview video](https://youtu.be/U3zeQ2A7xNI)
	- [Rhythm Guitar Tips](https://www.youtube.com/watch?v=Uo70TeO6B9E)
	- [12k hours blender user tips](https://youtu.be/n677HB7GbpQ)
	- [Blender Hades Modeling Inside Look](https://www.youtube.com/watch?v=cYJ6d1ifSqA)
	- [Stop Growing Lawns](https://www.youtube.com/watch?v=KLYMjPNppRQ )
	- [Hidden Gems on Ali Express](https://youtu.be/VyqljSodp6k)
	- [Marquees Brownlee Android Update](https://youtu.be/j7W2v_FmCuE)
	- ["Hotspot texturing for the omnisiah"](https://youtu.be/qU7EjGv3iiE)
	- [Good React (js) tutorial](https://youtu.be/E8lXC2mR6-k) 
	- [Computerphile SQL injection](https://youtu.be/ciNHn38EyRc)
	- [making digitcore sounds Vital](https://youtu.be/y4w_mNuhxmw)
	- 

[](https://www.youtube.com/@Blargis3d)
- https://learngitbranching.js.org/?locale=en_US
- https://leetcode.com/problems/longest-common-prefix/description/
- 3DP - "snap-fit joints"
- https://wokwi.com/rust
- https://docs.godotengine.org/en/stable/tutorials/shaders/your_first_shader/your_first_3d_shader.html
- mounting onto acrylic -face -photo
- https://www.w3schools.com/cpp/cpp_functions_lambda.asp
- https://github.com/google-gemini/gemini-cli
- chemical composition of dirt
- UCUPaint latest version
- Silo TV Series
- https://da4all.github.io/toolkit/
- FL delete 'd' vs e
- put sample on k junction
- focusrite scarlett mute speakers but not monitor
- https://github.com/ur-whitelab/chemcrow-publicm
- music pack jam ([shrimpo](https://datafruits.fm/shrimpos/fall-fruix-2025))
- Jain - Come (music video from Seana, lots of VFX)
- 9/12 Polyfjord Blender VFX video (30 min)
- Sophia music - https://www.tunemymusic.com/share/Lk6gS7JTkl
- [physics of music video](https://youtu.be/tCsl6ZcY9ag)
- Hank Green
	- [Electricity About to be Like Housing](https://youtu.be/39YO-0HBKtA)
	- [Caffeine](https://youtu.be/p-Dy2pcdBSU)
- how to use color palette and chrome sphere for vfx?
- https://en.wikipedia.org/wiki/Isaac_Newton%27s_occult_studies
- https://www.usatoday.com/story/news/nation/2025/02/12/tesla-cybertrucks-inspire-backlash-amid-elon-musks-political-work/78358688007/
- go-to tenor gifs to favorite
- sharpening mower blades
- https://www.colour-science.org/
- pixel update notes
- Google Pixel 8 PRO Focus and Exposure Lock for photo and video
- buy dry ice near me
- 

---
## FL Notes
### FL 2025 [YT](https://youtu.be/nKK0TRFwB7g) Notes
- Playlist - per-clip editing
	- cut clips are unique by default
		- do none of them share volume or anything?  Is it only when you cut them?
	- alt + 2x-M1 = clip properties, including pitch, reverse, and time shift
- Loop starter
- channel rack 4 bar seems to repeat for >4 lengths

### For Eric live collab:
- MIDI Bass
	- re-watch kontakt demo
	- try ample bass (see if there are any good patterns)
	- explore extracting bass from [GTab](https://gprotab.net/) tracks
	- find free MIDI pattern downloads
		- generally
		- that come with the new Kontakt bass player
- [x] Try out Jacob Collier's free choir plugin
---
## YT Audio Comment Response
'''
Well, who I think it's good for is people with a simple 2x2 interface and an SM7B. No other preamps or anything else. This is for two reasons. 

The mic preamps on entry level 2x2 audio interfaces often don't provide sufficient gain to get the best power and performance out of an SM7B and the headphone preamp on those interfaces often times don't provide ample volume output. So, what happens a lot of time is beginners often record things in at loud volume levels (like at -6 dB or louder). Then they go to track vocals and they wonder why the output of the vocal is so low in comparison to all the other tracks. Instead of turning down all the other tracks and turning up the headphone preamp when tracking vocals, they end up keeping the levels of all other tracks where they are and just try to record vocals the best they can but the vocal gets buried and they can't deliver their best vocal performance. So, if you have a cloud lifter, it helps in this scenario. 

Also, it provides the proper amplification to ensure you're getting the best out of an SM7B or ribbon mic. But studios or people with a selection of high end mic pres don't need a cloudlifter at all so they wouldn't use one. The preamp they chose would provide sufficient amplification from the start. I'd say it's something good to have if you're just starting out with an entry level budget interface, and then to keep around the studio as you become more experienced as well because you may run out of mic pre's and you can end up finding a good use for it. Bottom line is if you have good preamps on your interface or have dedicated mic preamps, it's not needed. It's for people who don't have these things and don't
'''

Thanks for such a detailed response!  I do think I see where you're coming from for microphones that are low-sensitivity (e.g., the SM7b) combined with weak-preamps (e.g., many entry-level interfaces) in situations where the user is quiet and distant from the microphone (e.g., whispery podcasts).  I do find that a bit niche, combined with choosing to purchase a >$400 microphone alongside a <$100 interface, but it happens.

That said, to the first point, it seems that beginners would be better served by simple/free solutions, like turning down their mix and taking one ear out of their headphones.  I understand that "just turn down" is an (unironically) infamously difficult lesson to teach a newcomer, but it feels non-ideal to recommend an expensive hardware purchase to solve a mouse-click issue.

To the second point—and I want to be clear that I do not mean this as snarky as it sounds—you're not getting the BEST out of your microphone unless you're using gold-plated, silver-core electronics with dielectric potting in a faraday cage booth lined with >6" rock wool pads.  To the best of my knowledge, there are no interfaces around the Cloudlifter price point that don't add more gain than your SSL 2 at the ~60% from the video.  And there seem to be a few examples around YouTube of people recording soft dialogue in a similar setup where the gain-matched noise is (to my ears) imperceptibly different between interface and Cloudlifter.  And for recording vocal

---


### Blender-Godot [Blog-post](https://studio.blender.org/blog/our-workflow-with-blender-and-godot/) Notes
- .blend imports deemed unhelpful for multi-person workflows
- Collection Exports
	- 'rather than exportin ga file in its entirety, we could set up dedicated collections to export multiple individual assets, allowing us to set up the export settings for all assets in advance'
	- 'also allows to have additional data for reference in a file without polluting export data'
	- 'question was how to nest assets without exporting the nested assets redundantly -> custom code'
		- blender extension and godot plugin for correctly re-creating the asset from the blender export inside godot found at the end of the article (though it is 'not fully fleshed out')
- Asset Separation
	- asset collections (e.g., branches on trees, trees in forests) need to be allowed to be edited/exported separately and their references in Godot should be re-created
- Pipeline breakdown
	- asset pipeline that worked for different asset types and relied on naming conventions
	- Export data to game files
		- Blender extension assigns an ID to assets that don't have one and register it to an index .json file for Godot to find
		- make sure collection instances are cleared of their instanced geometry for asset separation
---
## First pass blackbody thermometry shopping list

| Qty | Description                                                 | Thorlabs Part # | Est. Price (USD) | Notes                               |
| --- | ----------------------------------------------------------- | --------------- | ---------------- | ----------------------------------- |
| 1   | Fast Si photodiode detector, 200–1100 nm, 5 GHz, SMA output | DET08A/M        | $845             | 532–850 nm range                    |
| 1   | Ext. InGaAs detector, 800–2600 nm, 1.1 GHz, BNC output      | DET10D2         | $1,230           | 850–2200 nm range                   |
| 1   | Bandpass filter, 532 nm, 10 nm FWHM, 1"                     | FB530-10        | $330             |                                     |
| 1   | Bandpass filter, 650 nm, 10 nm FWHM, 1"                     | FB650-10        | $330             |                                     |
| 1   | Bandpass filter, 850 nm, 10 nm FWHM, 1"                     | FB850-10        | $330             |                                     |
| 1   | Bandpass filter, 1064 nm, 10 nm FWHM, 1"                    | FBH1064-10      | $388             |                                     |
| 1   | Bandpass filter, 1550 nm, 12 nm FWHM, 1"                    | FB1550-12       | $367             |                                     |
| 1   | Bandpass filter, 2200 nm, 12 nm FWHM, 1"                    | FB2200-12       | $521             |                                     |
| 1   | 1" filter holder, SM1-threaded                              | SM1FH           | $55              | For easy filter swapping            |
| 1   | SM1 (1") lens tube, 10 mm                                   | SM1L10          | $33              | For filter mounting                 |
| 1   | SM1 to C-Mount adapter (for detector mounting)              | SM1T2           | $33              | For lens tube to detector interface |
| 1   | 50 mm post                                                  | TR50/M          | $16              | For vertical mounting               |
| 1   | Post holder                                                 | PH2/M           | $27              | For post mounting                   |
| 1   | Base plate                                                  | BA1/M           | $23              | For table mounting                  |
| 1   | SMA(m) to BNC(m) RG-58 cable, 2 ft                          | CA2862          | $26              | For DET08A/M to scope               |
| 1   | BNC(m) to BNC(m) RG-58 cable, 2 ft                          | CA2602          | $19              | For DET10D2 to scope                |
| 1   | 50 Ω BNC terminator                                         | T4119-50        | $25              | For scope input termination         |

---
## Chelsea jobs

- Intelligence Analyst
	- Government
		- CIA, NSA, FBI, DoD ("Open Source Analyst" or "Intelligence Research Specialist")
	- Private
		- Booz Allen Hamilton, Raytheon, Palantir (near DC), IST Research, Leidos
- Legal Researcher
	- law firms in any city found on Indeed/Glassdoor ("Litigation Support Specialist" or "Paralegal - Research Focused")
- UX Researcher Apprenticeship (x)
- Policy Analyst/ Program Evaluator (Think Tank)
	- American Institutes for Research, Brookings, RAND, state/local government
	- Harrisburg-based policy groups, Pennsylvania Department of Education
	- "Policy Analyst," "Program Evaluation Specialist," "Research Associate"
- Knowledge Management Specialist
	- organizations in healthcare, engineering, and education (e.g., Penn State Health, Geisinger, UPMC)
	- "Information Specialist," "Knowledge Manager," "Taxonomy Analyst"
- Grant Writer or Research Development Officer
	- Penn State, Bucknell, nonprofit hospital

Creative tabs dump
 - Blender 4.5 features [YT](https://youtu.be/wPhA0imjvVs)
 - Blender Godot workflow [YT](https://studio.blender.org/blog/our-workflow-with-blender-and-godot/)
 - FL VFX Scripting Tutorial [YT](https://youtu.be/sB5otomxtu4)
	 - Dogwalk Release Party [YT](https://youtu.be/7eRlX4b3HEU)
 - 'suggest markdown in Fruity Notebook 2'
 - what to grow with tomatoes, how to compost, how to water tomatoes
 - Music Indie Game from Scratch [YT](https://youtu.be/3USobO6qRHE)
 - DBD 9.1 [patch notes](https://forums.bhvr.com/dead-by-daylight/kb/articles/514-9-1-0-ptb-patch-notes)
 - UK Censored Internet [YT](https://youtu.be/RFUUy0DKxvk)
 - 'PIP subtitles'

---
## Growing Tomatoes

- **Planting**
	- in late Spring/early Summer, after soil has warmed to ~60 C (danger of nighttime frost has passed)
- **Support**
	- stakes, cages, and trellises to keep upright, sun-exposed, and circulated
- **Watering**
	- water deeply (~4"), infrequently (1/wk), and consistently (for Ca update)
	- make soil moist but not soggy
	- water directly at the base, avoiding wetting foliage (spreading disease)
	- water in the morning to allow the foliage to dry before nightfall, reducing risk of fungus
	- young transplants need daily, established plants ~1-2 inches per week depending on soil drainage (more drainage -> more water) and heat
	- almost ripe --> reduce watering further to prevent cracking and blossom end rot
- **Pruning**
	- pinch suckers (remove side shoots) to focus plant's energy on production
	- remove lowest branches to mitigate diseases borne from soil contact
- **Composting**
	- apply around the base of the plants to retain moisture and suppress weeds
- **Grow**
	- 3-4 weeks to get large/green and then another 3-4 weeks to ripen on the vine
	- smaller varieties (e.g., cherry) may ripen as quickly as 4 weeks from flower to harvest
	- a 'blushed' tomato (started to show color) can be picked and ripen indoors at room temp
	- remove when they are slightly soft to the touch
- **Harvest**
	- pick at the 'breaker stage' when they begin to show color and let them finish ripening indoors
	- no more than a week after full ripening to avoid splitting, overripening, and attracting pests

---
## Discord tech illiterate how-to
## Anthony's Quick Guide to Discord

Hi! Anthony here! Since a few of us are brand new to Discord, I just wanted to point out what I feel are the 3 most important tips:

## 1. No money needed :money_with_wings:
You do not have to buy anything on Discord.
- if you see “Nitro,” “Shop,” or anything that asks for money → just back out

## 2. Getting around :compass:
When you open Discord on your phone, the first things you'll see are:
- Direct Messages (the top-leftmost button)
  - these are your 1-on-1 chats, like texts
- our "OMN Crew" group (the green icon with a white microphone)
  - where we coordinate gatherings and share pictures
- other groups
  - if you choose to join or create other groups, you will see them at the left edge, along with our group

When you tap on a group, that group's *channels* will appear
- tap on a *text* channel (channels with the '#' icon, e.g., "# meeting-plans")  to view its contents and write your own messages for the group
  - *note: sent messages will generally only be visible in a specific channel, like with this message and the "# general" channel*
- channels with unread messages will appear bold
- don't worry about *voice* channels (channels with speaker icons) — they are like group calls, but we usually do not use them

*Tip: if you get lost, look at the left-hand column — that’s where all your servers are.  If you don't see the servers, try pressing the back button at the top, or closing/re-opening to return to the servers*

## 3. Notifications :bell:
If you feel that Discord pings have become unwelcome or overwhelming:
- enter the group, tap on the server name at the top, and select “Notifications”
  - by default, you receive push notifications for each message sent — change that here (e.g., select "Nothing" in "Server notification settings" and uncheck "Mobile Push Notifications") 


:white_check_mark: That’s it! If you can:
1. Open this server
2. Read/reply to messages
3. Manage notifications
…you’re set. Everything else is extra.

## Extra things (optional) :sparkles:
You don’t need these right away, but talk to me if you'd like to learn more about:
- Reactions/Emojis: add a little :thumbsup: or :joy: under someone’s message
- Messages: replying, editing, deleting, pinning, formatting, hyperlinking
- Files: sharing pictures, videos, audio, PDFs, etc
- Events: creating and coordinating real life gatherings with Discord sign-ups
- Voice channels: hop on a call where you can talk, share your screen, or stream video from your camera if you'd like
- Other groups: create your own group or join an existing community.  This platform is popular for people with shared interests to gather and share funny pictures and stories via text or in spontaneous group calls

*note that what I've referred to as a "group" in these messages you will usually see called a "server"*

**And again: all of these features are free.  Do not pay for anything.**


