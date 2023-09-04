# Tutorial on MoleculeNodes for Illustrating Molecular Structure

[Blender](https://www.blender.org/) is a professional-grade, opensource software for 3D computer graphics. [Molecular Nodes](https://bradyajohnston.github.io/MolecularNodes/) an add-on for Blender to work with molecular structures e.g. from the Protein Databank. 

This tutorial is designed to show how it is possible to get started with MoleculeNodes.

## Installation and Setup
   1. [Download Blender](https://www.blender.org/download/) and install it. It can run on a laptop but if you have a machine with a GPU it run faster
   2. [Download MoleculeNodes](https://bradyajohnston.github.io/MolecularNodes/installation.html) and install the add-on in Blender. The add on supports importing molecular structures and using the GeometryNodes to manipulate and style the molecules. If you are have a Mac M1 or M2, you may need to install a conda environment to be able to import different types of molecular data formats.

## Getting started with Blender
Interacting with Blender is somewhat similar to PyMOL or UCSF Chimera but with a lot more control over the scene including the camera, lighting, and underlying mesh. Even to navigate around it can be a confusing at first. Fortunately there is are a large number of YouTube tutorials on how to use Blender aimed at beginners and experts. To get comfortable and get a taste for what is possible, I recommend going through the whole 17 part series [Blender Beginner Donut Tutorial](https://youtu.be/nIoXOplUvAw?si=zEotvRIJG5RB96Q6) by Blender Guru, and the [Molecular Nodes](https://www.youtube.com/@BradyJohnston/playlists) and [Blender for Biochemists](https://www.youtube.com/@BradyJohnston/playlists) series by Brady Johnston, the create of the Molecular Nodes add-on.

As you progress in learning Blender, I recommend keeping a notebook of what you learn. While not super difficult, a lot of workflows are built around hot-keys or not-so-obvious menu items, which can be difficult to remember if you don't use it often. Here is my [notebook](https://docs.google.com/document/d/1VPrr4Lk5RfgpVzDQbOud0ErJWZi_NGXNNe4Aow4PeLg/edit?usp=sharing) of things that I've learned so far. However, I recommend making it yourself so you can learn as you go.

## First render of a molecule
I'm using Blender 3.6.2 on macbook, so if you're using a more recent version some things may be slightly different.

### Setup the render engine
   1. Under the  Render panel -> Scene -> select Cycles and if you have a GPU select the device. Cycles uses physically realistic ray-tracing based on lighting.
   2. To see the render viewport Shading, on the far-right of the bar across the viewport, there should be 4 circles, select the one on the far right.
   3. To set transparent background (e.g. for a figure in a paper). Under the Render panel -> Film -> Transperent
   4. While you are setting up the and set the size and resolution of the output. In the Output panel -> Format set resolution e.g. `1080 px` x `1080 px`.
   3. To actually render the image, in the Render Toolbar (at the very top) select Render Image.

### Load the molecule
   0. Delete the default cube by selecting it and pushing `x` -> Delete
   1. Make sure the `Import: MolecularNodes` addon is installed and enabled in the Edit -> Preferences -> Add-ons.
   2. Under the Scene panel -> Molecular Nodes -> import `5ivn` from the PDB. This is a nanobody bound to a peptide from (Braun, et al., 2016, DOI: 10.1038/srep19211)
   3. Select the molecule and push `s` to scale and drag to the molecule bigger.
   4. The atoms will look like gray squares if you aren't in the `Rendered` Viewport shading mode (see above), and it will be invisible in if you haven't set the render engine to cycles (see above)

### Set up the camera
   1. Toggle the camera view from the camera icon on the upper right of the viewport.
   2. An annoying thing is that its tricky to orient the camera as an obect. A way I found that is easier is to lock the camera to the view and then move the view around. To do this click the right `<` in the very upper right of the viewport, then select the `View` -> View Lock -> Lock Camera to View. You can uncheck this when you're done so you can go back to your scene.
   3. On a mac you can use two fingers to the view around. Hold down shift to pan.

### Lighting
   1. Add light `Add` -> `Light` then select `Point`, `Sun`, `Spot`, or `Area`.
   2. E.g. to add an area light, scale it larger with `s`, and position it. Select the light then under the `Data` panel (Looks like green lighbulb), set the power and the color and other properties
   3. Basic studio lighting has a main bright light source, and one or more back and/or fill lights of complementary colors. Blender Guru has a nice [How to Make Studio Lighting in Blender](https://youtu.be/5UCc3Z_-ibs) tutorial.

### Style the molecule
   1. Select the molecule.
   2. Select the `Geometry Nodes` from the toolbar. This is flowgraph style programming environment where each node is a function that takes input and has outputs can can be wired together. The first input is `Group Input` and the last output is `Group Output`.
   3. To add a node either use the add menu or `Shift+A`.
   4. Make cartoon style. Add node -> Molecular Nodes (bottom menu item) -> Style -> Cartoon. Place it near the `MOL_style_atoms_cycles` node.
   5. Add a wire from the Atoms otuput of `MOL_color_set_common` node to the `Atoms` input of the new `Cartoon` node.
   6. To have both atoms and cartoon, add a `Join Geometry` before the `Output Group` node and wire both `MOL_style_atoms_cycles` and `Cartoon` nodes into it.
   7. Add `Molecular Nodes` -> `Selection` -> `Chain Selection`. Position it before the atoms and cartoon style objects. Select `Chain A` and pass feed the `Selection` into the cartoon node and the `Inverted` into the atoms node.
   8. To set the colors, you can also e.g. the `Molecular Nodes` -> `Color` -> `Color by Chain` and feed it into the `MOL_color_set_common` node.

### Materials
   1. Objects have materials that determine how light interacts with it.
   2. Click `Shading` from the toolbar.
   3. To create a new shader, click the `New Material` icon (looks like a copy icon) from the shader panel. Give it a good name.
   4. The default shader is the Principled BSDF and has a lot of sliders. The biggies are the `color`, `roughness`, and `subsurface scattering`. If you want it to be metalic then set the metallic slider.

