
- ### 2025-09-22 Meeting
		- idea: pull video into DVR and use "Color Palette" mode to inform design
		- Anthony
			- messed with a few ways to make the roughness map glyph appear cool in Godot similar to Blender's Eevee, including SSR, reflection probe, and SDF-global illumination, but seemingly the best was to just add a small, colored spotlight at an angle next to the object
			- made a new candidate for creepy basement sounds by taking an orchestra-guitar piece I made, adding some Casette2 wow/flutter, and automating time stretch for like 10x its length
				- Kaya was interested in having that time manipulation happen in real time and so I should explore solutions for that including FMod
				- She also is just generally interested in FMod again, so maybe just pull it in either way
		- Talk about LD plans a little more
			- Josh still interested in joining, if only remote and if only for some of the weekend
			- Kaya will talk to Bryan about possibilities, but was open to coming over here, even if only for a day
		
- ### 2025-09-15 Meeting
	- Josh
		- controls/event blocking updates, shows on screen, will work on debugging maybe more
	- Anthony
		- made bell/button/throw switch
		- josh suggested putting them into my branched project both to see how it will all look and to be able to distribute it from everyone pulling the branch
		- kaya says maybe there'll be git complaints, let her know if it happens (and then just put on drive)
	- Kaya
		- updated the basement flying blocks and tuned up a down-draft section behind the starting floor
		- made cool texture for the 'camera too close to player' effect

- ### 2025-09-08 Meeting
	- Anthony - terrain into main project, on github, terrain updates, music/audio updates
	- Josh - new event blocking code
	- Kaya
		- discussing Foregjo repo to replace bitbucket 
		- new git commands
			- git remote add codeberg ssh://git@codeberg.org/SciuridaeSandbox/s_4_2_1_sandbox.git
			- git remote -v
			- git pull codeberg
			- git push codeberg
		- health check for connection
		- dithered transparency for when character takes up too much of camera
	- to-do
		- talk about audio updates
		- talk about LD58
			- Plan: Kaya and Anthony will meet in person and Josh will contribute remotely when he can (~4-8 hours a day when possible)
			- Maybe message 
	- home
		- maybe make pull-switch and floor button for the new basement that Kaya made

- ### 2025-09-01 Meeting
	- shave the empty space off of fx in drive
	- think on how to 'side-chain' the music when near bonfire
	- wait on Kaya noting which sounds need a little tweak to be fully desirable
		- make the glide sample more loop-able (loop remainder)
			- or make separate initial sound + loop-able sound that doesn't have such a transient
			- maybe also other 'loop' tagged samples (loop reminder on the flre-lit-2_loop and also get it longer than 4 seconds)
 
 - ### 2025-06-03 Meeting
	 - To-do
		 - scatter blender objects (flora, buildings, etc.) in a terrain world
	 - Terrain notes (mostly [tutorial 2](https://youtu.be/YtiAI2F6Xkk))
		 - holes demo
		 - porting materials from libraries (e.g., ambientcg.com)
		 - painting wetness
		 -  bake occluder 3D (in 'Terrain3D Tools')
		 - flickering fix
		 - start with procedural noise (~19:30)
		 - vegetation placement techniques - manual, proton scatter, simple grass textured, "Asset Placer" (commercial)
	 - Meeting notes


 - test terrain game
	 - add some blender objects
		 - scatter trees and flora (bushes, grass, flowers)
		 - buildings
	 - [x] cursor capture bugs
	 - [x] compass centering
	 - blink ability
		 - player feedback
			 - add sfx
			 - UI blink cooldown
			 - warp camera
		 - prevent clipping through walls
		 - add vertical killbox
	 - explore docs/video for making tunnel/cave structures
---
 - city-forest 'bullshitting platformer" level
	 - [ ] base-building structure conducive to platforming
	 - [ ] larger scale 3d platformer level design blockout
	 - Transit infrastructure
		 - [x] overpass/overhead rail
		 - [ ] trains, bridges, ladders
	 - Construction
		 - [ ] building scaffolding, beams, pulleys/lifts, crane, wrecking ball
	 - Inside of buildings
		 - [ ] shader to simulate looking in windows (i.e., [this](https://godotshaders.com/shader/interior-mapping-shader/))
	 - man-hole level changer
	 - block out alternate biomes at the boundaries of this level (N64-realism ice, dessert, etc.)
 - audio
	 - music
		 - [ ] simplify the basement track
		 - [ ] new overworld tracks (more Toby Fox, narrow the motif)
		 - [ ] new city-forest level tracks
		 - consider alternative potential uses for dynamic music system
	 - SFX (see [[SFX Checklist]])
 - animations
	 - [ ] explore the workflow that separates the animations from the model
	 - [ ] port new squirrel animations + spring joint tail wag
	 - [ ] make new ninja animations for emotes
	 - [ ] fix ninja crawl
	 - [ ] urban wildlife (rat, cat, pigeon)
- modeling
	- [ ] environment mesh + collision (care not to disrupt child structure)
	- [ ] set dressing (rocks, trees)
	- [ ] characters (original squirrel player character)
- shading/art
	- [ ] icon/svg
	- [ ] environment shaders (grass, sky, etc.)
		- remember Material Maker
	- [ ] explore hair approximation shaders for bushy squirrel tail

check out Blender 4.4 [new features](https://youtu.be/-eqPs-boihU?t=306)
check out Blender Studio [pipeline features](https://studio.blender.org/projects/project-dogwalk/3dbedf9bab5c44/) (any code available?)
check out Brackey's Lighting in Godot [YT video](https://www.youtube.com/watch?v=aRdiiWpA0AA)
### [[Task Cards]]
### [[SFX Checklist]]

