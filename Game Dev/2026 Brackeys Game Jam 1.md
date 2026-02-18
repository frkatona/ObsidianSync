
### 2026-02-17 Notes
- Josh has a solid negative world window, but he'd like me to take a stab at the particle effects 
	- limitation to remember: only one is usable in the world at once

### 2026-02-15 Notes - Jam Day 1
- Theme: **"Strange Places"**
	- gameplay
		- can teleport but you are taken to another dimension (a la Minecraft nether rails)
		- "place" like "placement"
			- finding lost things (point-and-click adventure? 3D detective/mystery?)
			- finding things that don't fit where they are (puzzle)
		- "place" like "dwelling"
			- door-to-door ghostbusting in a neighborhood
	- environments
		- alien world (trees, fruit, space sky)
		- weird physics (superliminal, antichamber)
- Josh's ideas:
	- puzzling to figure out what that strange thing/place is
	- mechanics ideas:
		- exploration, open world type stuff (want to pay close attention to things and move around a lot to see new things..."make them want to pay attention")
		- games where you collect knowledge (e.g., chance of sendhar (?))
- Github actions to zip and push new builds to itch?
- Fleshing out game
	- open world, isolated foresty place where items are found in strange places; focus on visual interest, mystery, exploration
		- modern technology in a dated era?
		- traces of intelligence on an alien world?
	- 'look-at-me' mechanic:
		- staring directly at certain items cause them to light; persistent staring for a threshold of time causes light to swell and culminate into a 'press e to interact'
	- first 'look-at-me' is the bonfire
		- light or smoke from fire serves as a clear visual marker to orient the player as the move through an otherwise dense, disorienting terrain
	- enemies?  fight or run/hide?

to-do
- Game
	- source of fun/actual game-loop mechanics
		- puzzle/platforming
			- find things to interact with which open doors, raise platforms, drop bridges
		- stealthing?
	- novel interest
		- line-of-sight interactions
			+ detective vision, predator vision?
		- mirror world traversal 
	- story
		- **YOU** - wake up in unfamiliar forest, don't know how you got there
		- **NEED** - lost something important (sister, teddy bear, )
		- **GO** - 
		- **SEARCH** - 
		- **FIND** - 
		- **TAKE** - 
		- **RETURN** - 
		- **CHANGE** - 
	- questions to answer
		- how did you get here?  why are you here?
			- plane crash; it's a dream; 
		- why are YOU able to swap dimensions?
			- it's related to the thing you're looking for and to the reason why you have LOS interaction powers
				- it's like a Millenium Items situation and you still have the "eye" (seeing the unseen world) or whatever piece lets you swap dimensions, but not the ones that give you power (to kill? force push? enemies), 'knowledge' (memories)
			- it's just something that happens on this island (see: why are you here?)
		- what is preventing you from leaving?  both in the grand scheme and moment to moment?
- player character
	- sculpt/make something really nice to swap out the third-person asset
- bush NPC
	- [ ] animation tree + conditions for waking, sleeping, etc.
	- [ ] detect player + activate chase + escape/caught condition
	- pathing
		- [ ] patrol across pre-defined nodes
		- [ ] wander across nav mesh
		- [x] hardcode some kind of circle or figure-8, etc.
- music
	- [ ] BGM more magical/ethereal
	- [ ] chase music (or add thumping 2x speed beat to bgm)
- sfx
	- global atmosphere:
		- wind
	- local:
		- ambient environment
			- fire, owls
		- portal (stasis, open, opening, closing, walking, walk through)
	- player 
		- [ ] step1/step2
		- [ ] jump/land
		- [ ] enter/leave/is look-mode
		- [ ] 
	- objects 
		- 
- test web build + deploy
	- gh action

- Josh glow on object --> give it to me to mess around with for merge

### 2026-02-14 meeting notes
 - Jam starts tomorrow morning (6am) and lasts 1 week
 - Tonight's meeting with Josh to briefly consider planning (timeline, meetings, template, etc.)
 - Goal:
	 - work together tomorrow and Monday and have a playable demo by Monday evening
	 - try to prioritize placeholders and not get distracted
	 - don't worry if we need to take breaks, we have a week