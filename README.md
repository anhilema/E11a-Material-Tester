# E11a-Material-Tester

This exercise is an opportunity for you to experiment with PBR Textures in Godot. The exercise is based on [Godot 3 Tutorial: PBR Materials](https://www.youtube.com/watch?v=pM5j8x71HcE). I will be providing some additional information about PBR Textures as part of today's lecture materials.

As usual, fork and clone this repository to your computer.

This exercise will invite you to adjust the materials of several sphere-like objects. Each of the objects is a mesh (called GodotBall) inside a Spatial scene. For each GodotBall, select the Mesh, and in the Inspector, select Material. For Material 0 (currently [empty]), select New Spatial Material, and then adjust the parameters as described below. The textures appear in the FileSystem panel, and can the files can be dragged from that panel to the Texture field in the inspector. 

White Plastic
 * Metallic->Metallic: 0.4
 * Roughness->Roughness: 0.35

Mirror
 * Metallic->Metallic: 1
 * Roughness->Roughness: 0.02

Dark Wood
 * Albedo->Color: R: 206, T: 147, B: 92, A: 255
 * Albedo->Texture: res://test_materials/texture_wood.png
 * Metallic->Metallic: 0.48
 * Roughness->Roughness: 0.28

Cheese
 * Albedo->Texture: res://test_materials/texture_cheese_albedo.png
 * Roughness->Roughness: 0.64
 * Normal Map->Enabled: On
 * Normal Map->Texture: res://test_materials/texture_cheese_normal.png
 * Ambient Occlusion->Enabled: On
 * Ambient Occlusion->Texture: res://test_materials/texture_cheese_ao.png
 * Depth->Enabled: On
 * Depth->Texture: res://test_materials/texture_cheese_depth.png
 * Subsurf Scatter->Enabled: On

Stones
 * Albedo->Texture: res://test_materials/texture_rock_albedo.png
 * Metallic->Metallic: 0.86
 * Metallic->Texture: res://test_materials/texture_rock_metal.png
 * Roughness->Roughness: 0.47
 * Normal Map->Enabled: On
 * Normal Map->Texture: res://test_materials/texture_rock_normal.png
 * Ambient Occlusion->Enabled: On
 * Ambient Occlusion->Texture: res://test_materials/texture_rock_ao.png
 * Depth->Enabled: On
 * Depth->Texture: res://test_materials/texture_rock_depth.png

Brick
 * Albedo->Texture: res://test_materials/texture_bricks_albedo.png
 * Metallic->Metallic: 1
 * Metallic->Texture: res://test_materials/texture_bricks_metal.png
 * Roughness->Roughness: 0.56
 * Normal Map->Enabled: On
 * Normal Map->Texture: res://test_materials/texture_bricks_normal.png
 * Depth->Enabled: On
 * Depth->Texture: res://test_materials/texture_bricks_depth.png

Wool
 * Albedo->Texture: res://test_materials/wool_albedo.png
 * Metallic->Metallic: 0.1
 * Roughness->Roughness: 0.77
 * Normal Map->Enabled: On
 * Normal Map->Texture: res://test_materials/wool_normal.png
 * Depth->Enabled: On
 * Depth->Texture: res://test_materials/wool_depth.png

Aluminium
 * Albedo->Texture: res://test_materials/aluminium_albedo.png
 * Metallic->Metallic: 0.59
 * Roughness->Roughness: 0.4
 * Normal Map->Enabled: On
 * Normal Map->Texture: res://test_materials/aluminium_normal.png
 * Anisotropy->Enabled: On
 * Anisotropy->Flowmap: res://test_materials/aluminium_flow.png

Marble
 * Parameters->Diffuse Mode: Lambert Wrap
 * Albedo->Texture: res://test_materials/marble_albedo.png
 * Metallic->Metallic: 0.1
 * Roughness->Roughness: 0.1
 * Rim->Enabled: On
 * Subsurf Scatter->Enabled: On

Wet Sand
 * Albedo->Texture: res://test_materials/sand_albedo.png
 * Metallic->Metallic: 1
 * Metallic->Texture: res://test_materials/sand_metal.png
 * Roughness->Roughness: 1
 * Roughness->Texture: res://test_materials/sand_rough.png
 * Normal Map->Enabled: On
 * Normal Map->Texture: res://test_materials/sand_normal.png

Rock
 * Albedo->Texture: res://test_materials/rock_albedo.png
 * Metallic->Metallic: 0.12
 * Roughness->Texture: res://test_materials/rock_rough.png
 * Normal Map->Enabled: On
 * Normal Map->Texture: res://test_materials/rock_metal.png
 * Ambient Occlusion->Enabled: On
 * Ambient Occlusion->Texture: res://test_materials/rock_ao.png
 * Depth->Enabled: On
 * Depth->Texture: res://test_materials/rock_depth.png

Ice
 * Parameters->Depth Draw: Never
 * Albedo->Color: R: 255, G: 255, B: 255, A: 0
 * Albedo->Texture: res://test_materials/rock_albedo.png
 * Metallic->Metallic: 1
 * Roughness->Roughness: 0.62
 * Normal Map->Enabled: On
 * Normal Map->Texture: res://test_materials/rock_metal.png
 * Ambient Occlusion->Enabled: On
 * Ambient Occlusion->Texture: res://test_materials/rock_ao.png
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
 
When you have completed the exercise, run it to ensure that everything is workign correctly. This exercise also contains an excellent example of a WorldEnvironment (and how to change environments using GDScript).

When you are done, commit and push your changes to Github, and turn in the URL of your repository on Canvas.
