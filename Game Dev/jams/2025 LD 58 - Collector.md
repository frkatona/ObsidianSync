### final countdown to-do
- countdown timer + end screen (show scores/winner/back-to-menu)
- input camera direction
- volume - escape key into volume slider (or mute in the corner)
- fix 90 degree interactable bookshelf rotation offset runtime bug (at least the one in the right building)
- maybe
	- hook polish
	- trap logic
		- move the trigger further away, think on a more ideal position, create maybe 2x around what might be seen as the most desirable tooth collection routes
		- make it obvious they are dangerous  when they're raised (metallic shader, time-varying emission, ambient sound effect?)
	- house witch patrol path doesn't repeat after first pass 
		- maybe keep that, but have her stare down one of the important doors time for like the latter half to disrupt the flow of the round
	- where are we on the lights budget?  can we add another interactable floor lamp to the right building or outside?
	- sound fx when outside (reverb outside vs low-pass inside?)
	- hook up sounds/animations (at least death, anything else? )
		- Kaya was hoping for more sound fx of basically any kind as well
	- get teeth more readable (outline shader?)
	- kid/dad models
		- fix idle animations or remove

### then
- figure out LD team thing 

modeling/animating to-do
- fairy re-do for good player character
	- [x] wand, wings
	- [x] hair/hat
	- [x] jiggle dress
- interactive pop-up traps
	- [x] spike trap from floor
	- [ ] anvil drop
- kid
	- need new anim for interact w/ player?
- Josh wants some paintings on the walls
---
### audio to-do
- music
	- [x] title music
	- [x] game music (indoor vs outdoor?  outdoor wind woosh?)
- sfx
	- player
		- [x] fairy float movement
		- pickup
			- [x] tooth (/kid interact?)
			- [x] environment interact (? switch, door, etc.?)
			- [ ] other pickup?
		- [x] caught
	- parents
		- [x] ambient proximity danger
		- [x] player found (/round over?)
	- UI
		- match
			- [x] UI select
		- multiplayer
			- [x] match found
			- [x] match starting
- [x] script effects with Godot's audio bus
	- (nevermind, audio bus effects don't get transferred for some reason)
	- (same with action inputs from the input editor)
	- though maybe I could just write down my ideal audio bus settings and then see if the last build can just dial it in manually?
- Kaya wants some more interesting sounds, anything will do
---
### other to-do
- add more obstacles
- custom shaders in godot
	- wand/hat
- main menu?
	- getting separate audio into main menu, lobby, and game?
- how to play, controls intro?
- fix input vs camera direction
- volume slider
- getting teeth more readable (bigger?  outlined/fresnel?  at an angle or facing camera?)
- itch upload
	- canvas scaling text
	- dark mode background on itch.io page
- lobbies
	- problem if people make lobbies and don't ready up if they're the first lobbies people see?
	- a back button
- joining LD team (so all our game reviews contribute to our game's boost)
- splash/load screen (2:1, 4:3 something)...team squirrel, teeth maybe 
---

### feature ideas
- father (/witch/ mother)
	- [x] animated to walk around map
	- [ ] bounce back on closed door
- kids
	- [ ] animate around map
	- [ ] colliding with player gives bonus
		- (extra (3?) teeth or a powerup (2x speed?  refresh your dash/phase?)
- 3 rounds of increasing impactfulness of interactives (implement all on same level and then remove modularly):
	- [ ] round 1 - turn off/on lights
	- [ ] round 2 - introduce parents; switch parents directions (on collision with closed door?)
	- [ ] round 3 - switch paths (like trolley tracks, opening one = closing another) and kill switches
- abilities
	- dash/lunge
		- [ ] logic
		- [ ] UI
		- [x] animations
	- wand hooks and pull a tooth towards you (can collide with another witch)
		- [ ] logic
		- [ ] UI
		- [x] animations
	- phase through obstacles (slow blink?)
		- [ ] logic
		- [ ] UI
		- [x] animations

- Josh idea - local physics on the kids chairs (will that need to be taken off network syncing somehow?)
- progressing
	- [ ] transition to next "level"
	- [ ] screen to show who won/points
- pudge hook wand
- buy emotes or clothes stuff with total accumulated teeth

---
### tell kaya/josh
- added sound for active flying
- added input keys for various animations, but couldn't figure out best way to use them in the existing script (tested dance and that works)
---
### Concepts
- hobbyist collection
	- stamps, stickers, baseball cards
	- critters (pokemon?)
	- curator (art?)
	- pawn shop
- evidence
	- detective/private eye
- money
	- debt collector
	- busker, homeless
	- savings (newspaper clippings/coupons)
- game parts
	- card game
	- jigsaw puzzle
- scavenger (hunter/gatherer)
- pieces of self
	- voltron?
- funnel/bottleneck
- upgrades (a la mobile games)
- Tooth fairy
	- kids <7
	- horror? stealth?
### before
- shopping - soda, healthy snacks
- clothes - washed
- stylize some materials (3D)
- play around with sprites for potential 2D
- play around with FMOD
	- General FMOD Tutorial [video](https://youtu.be/RfzshDQILr8)
	- Integrating into Godot [video](https://youtu.be/7kD7Q3O5P-s)
- practice character modeling, rigging, animating, and basic shading
- make most basic 3D game (followalong with Brackeys coding and 3D game videos)
- discuss with Kaya and Josh
	- traveling to Kaya?
		- packing
			- computer
			- monitor
			- audio stuff
	- version tracking/collaboration

### timeline
- Friday night (6:00 PM to 11:30 PM)
	- concepts
	- prototyping
- Saturday
	- implementing core game loop
	- polishing concepts and context
	- basic designs for character, items, environment, etc.
	- basic music
- Sunday
	- push test builds
	- test multiplayer with third parties





### Kaya notes
- Next witch export
	- set origin to feet
	- rename animations to loop (start or end with "loop" or "cycle")
### misc notes
- ssh key -> with old **
