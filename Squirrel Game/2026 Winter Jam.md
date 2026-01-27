Theme: "**Constantly overworked**"

Ideas:
- elf present factory
	- present automation, a la factorio
	- darker - impossible not to make some mistakes, have to prioritize resources and lie to Santa (a la Papers Please)
- santa delivering presents overnight
	- driving/flying the sleigh (racer with speedups, SM64 rings/coins), precarious rooftop landings
	- slippery rooftop walking, squeezing in chimney, stealthing past kids to tree, milk+cookies pickup
- winter resale worker (manager, cashier?)
- signing christmas cards
- mall santa (idk, visual novel-esque?)
- winter driveway maintenance (shoveling + salting)
	- simulation
		- visually satisfying 'particle wiping' brush effect
		- embodying the feelings of the shovel skidding along lightly dusted surface and of the sudden resistance when wet snow rapidly piles up
		- push space to toss over your back...hold duration = throw farther
	- snake-like (one snake for shove, other for salt, have to return for energizing cocoa)
- christmas lights (rhythm game syncing songs to lightshow)

To-do
- figure out forge.squirrelracer login problems
	- josh is resetting password (but I could just upload to github for now anyway)

Settling on sokoban/cozy cafe thing (though maybe theme would be better to pivot to elf factory)

ask Josh to push build so I can try a deploy
# Assets

Audio
- music
	- [x] main menu ✅ 2026-01-24
	- [x] bgm ✅ 2026-01-24
	- [x] victory/credits ✅ 2026-01-24
- sfx
	- UI
		- [x] button click ✅ 2026-01-24
	- player
		- [x] walk (step 1/step 2) ✅ 2026-01-24
		- [x] push ✅ 2026-01-24
	- environment
		- [x] block pushed ✅ 2026-01-24
		- [x] block slide (1 tile? continuous?) ✅ 2026-01-24

3D assets
- characters
	- player
		- [x] mesh ✅ 2026-01-24
		- [x] textures ✅ 2026-01-24
		- [x] animations ✅ 2026-01-24
	- enemies/NPCs? (other elf character animated to be tossing new packages into drop-off area)
- environment
	- [ ] pick-up area (workshop drop-off)
	- [ ] drop-off area (santa's sleigh)
	- [ ] storage room
	- [ ] snowy outdoors (snowfall with 3d particles?)
	- floor surfaces
		- [x] walking (wood planks, concrete?) ✅ 2026-01-24
		- [x] sliding (icy/shiny, arrows?) ✅ 2026-01-24
		- [x] launching (animated closing circles) ✅ 2026-01-24
- props
	- [x] xmas trees ✅ 2026-01-24
	- [ ] xmas lights
	- [x] tables ✅ 2026-01-24
	- [x] storage racks ✅ 2026-01-24
- interactive/animated elements
	- [x] conveyor belt ✅ 2026-01-24
	- moveable packages
		- [x] wooden crates ✅ 2026-01-24
		- [ ] cardboard boxes


- [x] Butler
- [x] add more time to hectic jazz bgm ending to prevent cutoff sound
- fix animations 
	- [x] continue loop until another animation is called (and don't call idle until keys are released) ✅ 2026-01-25
	- [x] create looping push animation ✅ 2026-01-25
	- [x] foreman animations - idle, idle-impatient, and button-push ✅ 2026-01-25
	- [x] swap push animation in Godot ✅ 2026-01-25
- [x] shelves casting shadows but not walls ✅ 2026-01-25
	- probably back-face culling problem, fixable in godot or don't cull in blender?  actually maybe best to make the walls cubes anyway in case the camera angle sees past them on the bottom of the level

- [x] working menu system (splash screen, opening menu) ✅ 2026-01-25
- [x] replace placeholder box with crate ✅ 2026-01-24
- [x] (fuck it) jiggle bone on hat ✅ 2026-01-25

- [x] design basic room layout style ✅ 2026-01-25


Josh
- [ ] establish a 'clear' or 'fail' condition for next level, win game, or game over
- [x] track/show score/sense of progression ✅ 2026-01-25
- [x] UI (timer, score, pause/options/exit/volume controller) ✅ 2026-01-25

- [ ] design puzzle layout
- web fuckiness
	- [x] UI scaling at small and large resolutions ✅ 2026-01-25
	- [ ] audio - wiper keeps happening (is it linked to any box movement?)
- [ ] make "continue" more prominent in the 'level complete' modal
	- [ ] change "restart game" text to "restart level" (it does restart level, not game)
- change camera
	- [ ] zoom out with scroller?
	- [ ] default to higher position at sharper angle?
- [ ] separate sound for ice sliding
- [ ] slow timing of feet audio triggers in Godot
- [ ] tune window alpha
- [ ] remove misleading options from pause menu (e.g., 'interact')
- [ ] thumbnail/cover/main menu art
- [ ] window sills to windows

are we allowed to submit 6 hours late or only edit the submission?

puzzle elements
- walls
- other boxes
- floor obstacles
- levitating obstacles
- conveyers
- ice

advanced mechanics
- brute forcing a block against the conveyer flow
- looping boxes in a lift so one has to wait and becomes pushable
- blocking the ice/conveyer path (with another box or the player character)
	- racing against the conveyer belt + ice to get into the necessary position to block the crate in time
- blocking your own slippery ice path with a pre-placed crate

### tutorial draft
- goal: fill the delivery tiles (white) with the crates of presents (red bow tie blocks)
- how to play: push the crate blocks in the direction that you walk into them (move with WASD) one tile at a time until they reach the delivery tiles
- tile types
	- generic obstacles (trees, barrels, and desks) block movement from all directions
	- floater obstacles block the player, but crates can be pushed both under and through them
		- stacked blocks function as floaters, allowing the bottom block to be pushed out from under the other
	- conveyer tiles push one tile in the direction of the arrow (only effect blocks)
		- the player has the strength to push blocks against an opposing conveyor belt
	- ice tiles push one tile in the direction of movement (effects both blocks and the player)
		- caution: a block dropped from a height will break through ice tiles and sink into them (though they are only one block deep)
	- lift tiles propel blocks up and forward in the direction of arrow, useful for accessing raised conveyer tiles

check for other brute force solutions to minimize
working bgm
'e' on terminal -> easter egg sound
end round after delivery
quieter footsteps
sound (jingle?) for crashing through ice


### submission scoring
**1.** **Enjoyment** - how fun it was to play the game
**2. Presentation** - how well the visuals, sound, colors, etc work together
**3. Concept** - the game's idea; storyline, mechanic, etc
**4. Use of theme** - how well the theme is integrated
**5. Use of prerequisite** - how well the prerequisite is integrated
**6. Controls** - how the game feels when playing it (snappy? delayed? smooth?)

Josh asks: for anything new placed in a level, add to the `scenes/gameobjects` folder
- if there are decorations maybe a separate decorations folder
### version control notes

- resetting
	- `git fetch --all`
	- `git reset --hard origin/main`
- misc
	- `git merge --abort`
	- `git stash --all`
- asdf
	- `butler push boxesgame.zip akatona/boxes-for-the-big-man:web`

- Qs
	- space vs : vs / for origin main