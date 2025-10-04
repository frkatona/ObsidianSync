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
	- horror version
		- 
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




### Blender Godot Pipeline Plugin Notes
Q: what specifically can this pipeline do that is impossible or difficult with Blender 4.5 and Godot 4.5?

A: The Blender Godot Pipeline offers several functionalities that are either impossible or more difficult to achieve when using Blender 4.5 and Godot 4.5 with default import hints:

- **Combining Shape Types with Body Types** (5:30-5:38): The pipeline allows you to combine any shape type (like primitive or tri-mesh collisions) with any body type (static, rigid, area, animatable body 3D), which is not possible with Godot's built-in import hints.
- **Custom Material Application and Consistency** (6:59-7:04): While you can use custom materials in Godot, the pipeline's path setter functionality allows you to link materials from Blender to Godot, ensuring that custom materials are consistently applied upon re-import without breaking the representation.
- **Attaching Scripts** (10:32-10:51): The pipeline provides a direct way to attach Godot scripts to exported objects from within Blender using a path setter, streamlining the process of adding behavior.
- **Modifying Collision Layers and Masks** (11:14-11:45): You can easily set collision layers and masks for objects directly in Blender, which is then reflected in Godot, offering more control over collision behavior than standard import options.
- **Embedding Packed Scenes** (13:32-13:44): The pipeline enables you to embed Godot packed scenes directly into your exported scene from Blender, allowing you to control the placement and instantiation of complex scenes within your Blender design.
- **Automatic Handling of Duplicated Scene Geometry** (13:46-14:09): The pipeline automatically manages the duplicated scene nodes that Godot creates upon import by "queue freeing" them on ready, preventing performance issues that might arise from having two copies of your scene.
- **Proper Instancing and Resource Management** (15:00-15:02): The pipeline ensures that mesh resources are correctly tied to the glTF file and handles instancing properly, avoiding concerns about resources being duplicated or made local unnecessarily.
- **Nav Mesh Creation** (15:16-16:17): The pipeline simplifies the process of setting up navigation meshes by allowing you to define them in Blender and export them as a .tres file, which can then be used by Godot for navigation.