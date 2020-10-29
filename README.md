# Exercise-05d-Materials-Examples
Exercise for MSCH-C220, 29 October 2020

This exercise is an opportunity for you to experiment with PBR Textures in Godot. The exercise is based on [Godot 3 Tutorial: PBR Materials](https://www.youtube.com/watch?v=pM5j8x71HcE). I will be providing some additional information about PBR Textures as part of today's lecture materials.

Fork this repository. When that process has completed, make sure that the top of the repository reads [your username]/Exercise-05d-Materials-Examples. *Edit the LICENSE and replace BL-MSCH-C220-F20 with your full name.* Commit your changes.

Clone the repository to a Local Path on your computer.

Open Godot. Import the project.godot file and open the "Material Tester" project.

This exercise will invite you to adjust the materials of several sphere-like objects. Each of the objects is a mesh (called GodotBall) inside a Spatial scene. For each GodotBall, select the Mesh, and in the Inspector, select Material. For Material 0 (currently [empty]), select New Spatial Material, and then adjust the parameters as described below. The textures appear in the FileSystem panel, and can the files can be dragged from that panel to the Texture field in the inspector. 

White Plastic
 * Metallic->Metallic: 0.4
 * Roughness->Roughness: 0.35

Mirror
 * Metallic->Metallic: 1
 * Roughness->Roughness: 0.02

Dark Wood
 * Albedo->Color: R: 206, T: 147, B: 92, A: 255
 * Albedo->Texture: res://materials/texture_wood.png
 * Metallic->Metallic: 0.48
 * Roughness->Roughness: 0.28

Cheese
 * Albedo->Texture: res://materials/texture_cheese_albedo.png
 * Roughness->Roughness: 0.64
 * Normal Map->Enabled: On
 * Normal Map->Texture: res://materials/texture_cheese_normal.png
 * Ambient Occlusion->Enabled: On
 * Ambient Occlusion->Texture: res://materials/texture_cheese_ao.png
 * Depth->Enabled: On
 * Depth->Texture: res://materials/texture_cheese_depth.png
 * Subsurf Scatter->Enabled: On

Stones
 * Albedo->Texture: res://materials/texture_rock_albedo.png
 * Metallic->Metallic: 0.86
 * Metallic->Texture: res://materials/texture_rock_metal.png
 * Roughness->Roughness: 0.47
 * Normal Map->Enabled: On
 * Normal Map->Texture: res://materials/texture_rock_normal.png
 * Ambient Occlusion->Enabled: On
 * Ambient Occlusion->Texture: res://materials/texture_rock_ao.png
 * Depth->Enabled: On
 * Depth->Texture: res://materials/texture_rock_depth.png

Brick
 * Albedo->Texture: res://materials/texture_bricks_albedo.png
 * Metallic->Metallic: 1
 * Metallic->Texture: res://materials/texture_bricks_metal.png
 * Roughness->Roughness: 0.56
 * Normal Map->Enabled: On
 * Normal Map->Texture: res://materials/texture_bricks_normal.png
 * Depth->Enabled: On
 * Depth->Texture: res://materials/texture_bricks_depth.png

Wool
 * Albedo->Texture: res://materials/wool_albedo.png
 * Metallic->Metallic: 0.1
 * Roughness->Roughness: 0.77
 * Normal Map->Enabled: On
 * Normal Map->Texture: res://materials/wool_normal.png
 * Depth->Enabled: On
 * Depth->Texture: res://materials/wool_depth.png

Aluminium
 * Albedo->Texture: res://materials/aluminium_albedo.png
 * Metallic->Metallic: 0.59
 * Roughness->Roughness: 0.4
 * Normal Map->Enabled: On
 * Normal Map->Texture: res://materials/aluminium_normal.png
 * Anisotropy->Enabled: On
 * Anisotropy->Flowmap: res://materials/aluminium_flow.png

Marble
 * Parameters->Diffuse Mode: Lambert Wrap
 * Albedo->Texture: res://materials/marble_albedo.png
 * Metallic->Metallic: 0.1
 * Roughness->Roughness: 0.1
 * Rim->Enabled: On
 * Subsurf Scatter->Enabled: On

Wet Sand
 * Albedo->Texture: res://materials/sand_albedo.png
 * Metallic->Metallic: 1
 * Metallic->Texture: res://materials/sand_metal.png
 * Roughness->Roughness: 1
 * Roughness->Texture: res://materials/sand_rough.png
 * Normal Map->Enabled: On
 * Normal Map->Texture: res://materials/sand_normal.png

Rock
 * Albedo->Texture: res://materials/rock_albedo.png
 * Metallic->Metallic: 0.12
 * Roughness->Texture: res://materials/rock_rough.png
 * Normal Map->Enabled: On
 * Normal Map->Texture: res://materials/rock_metal.png
 * Ambient Occlusion->Enabled: On
 * Ambient Occlusion->Texture: res://materials/rock_ao.png
 * Depth->Enabled: On
 * Depth->Texture: res://materials/rock_depth.png

Ice
 * Parameters->Depth Draw: Never
 * Albedo->Color: R: 255, G: 255, B: 255, A: 0
 * Albedo->Texture: res://materials/rock_albedo.png
 * Metallic->Metallic: 1
 * Roughness->Roughness: 0.62
 * Normal Map->Enabled: On
 * Normal Map->Texture: res://materials/rock_metal.png
 * Ambient Occlusion->Enabled: On
 * Ambient Occlusion->Texture: res://materials/rock_ao.png
 * Refraction->Enabled: On

Toon
 * Parameters->Diffuse Mode: Toon
 * Parameters->Specular Mode: Toon
 * Albedo->Color: R: 231, G: 91, B: 25, A: 255
 * Roughness->Roughness: 0.04
 * Material->Next Pass: New Spatial Material
   * Flags->Unshaded: On
   * Parameters->Cull Mode: Front
   * Parameters->Grow: On
   * Albedo->Color: R: 7, G: 0, B: 0, A: 255
 
When you have completed the exercise, run it to ensure that everything is working correctly. This exercise also contains an excellent example of a WorldEnvironment (and how to change environments using GDScript).

Quit Godot. In GitHub desktop, add a summary message, commit your changes and push them back to GitHub. If you return to and refresh your GitHub repository page, you should now see your updated files with the time when they were changed.

Now edit the README.md file. When you have finished editing, commit your changes, and then turn in the URL of the main repository page (https://github.com/[username]/Exercise-05d-Materials-Examples) on Canvas.

The final state of the file should be as follows (replacing the "Created by" information with your name):
```
# Exercise-05d-Materials-Examples
Exercise for MSCH-C220, 29 October 2020

An exploration of PBR Materials in Godot.

## Implementation
Built using Godot 3.2.2

## References
[Godot 3 Tutorial: PBR Materials](https://www.youtube.com/watch?v=pM5j8x71HcE)

## Future Development
None

## Extra Credit
None

## Created by 
Jason Francis
```

