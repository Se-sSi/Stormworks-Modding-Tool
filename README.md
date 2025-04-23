
# Stormworks Modding Tool
This is a modding tool for the game Stormworks that I created. It edits the XML files to make custom blocks (**MOD BLOCK FILES**, not vehicle XML files). In the current version, surface and voxel editing is available, as well as file conversion. Many more features are planned!

# How to download 📥
To download simply download the "**Stormworks Modding Tool.exe**" file (for windows) or the MacOS files if you are using MacOS. Then run run the downloaded file.
- This can be done by clicking the "Stormworks Modding Tool.exe" file above then clicking the download button to the upper right.
- Or simply click the "code" button above and the "Download zip" and then extract the "Stormworks Modding Tool.exe" file and open it.

# How to use ❔
When you open the program, start by loading in your pre existing **custom XML mod block file** that you want to edit. Click the "**Load XML file**" button at the top of the screen and select the file you want to edit. See the chapters for further info of how to use the tool.

## Building modes 🔨
- Press the button to the left on the bottom of the screen for **surface mode** and the one to the right for **voxel mode**. Press the same button again to open the **shapes menu**, alternatively press the menu button on the far right.

### Shapes menu
- Opens a menu of all the diffrent shapes available in the current **build mode**.
- Opened by clicking the blue button to the right on the bottom of the screen.
- Alternatively press the same **build mode** button again after selecting it.

### Voxel 🔲
**Voxels** are the invisible **physical collision boxes** in-game, and the foundation for **surface** placements.
- There are **42 voxel shapes** (0-41), which define diffent collision boxes and **surface** placements.
- The voxels are not vissible in game, they are used as a foundation to put surfaces on or simply for the collision box.

### Surface 🔷
**Surfaces** are attachable (placeable) visible faces that you place on **voxel** faces.
- There are **67 surface shapes** (0-66), which define diffent surface shapes to fit with the voxel shapes.
- If the **attachment face** property is activate, the surface will be **visible** in-game (except shape 0, which is invisible).
- If the **fluid seal** property is active, but **attachment face** is not, the surface will be **invisible** but still act as a fluid seal.
- Surfaces must be placed on a voxel face (though you can remove the voxel to create floating surfaces).

### Attachment face ⬇️
An **attachment surface** is a property in the shapes menu that makes a surface, a face that you can place blocks on in-game.

### Fluid seal 💦
A **fluid seal** is a property in the shapes menu that prevents **water**, **gases** and **space** from passing through.

## Shape 🔷
- Select the shape in the **shapes menu**.
- **Voxel shapes** (0-41) define the physical collision shapes in-game.
- **Surface shapes** (0-66) define the visible surfaces in-game.

## Rotation 🔁
- Rotate objects with the **J**, **K** and **L** keys rotating the object around the X, Y, Z axies respectivley (like in Stormworks)
- Press the key **R** to rotate around the normal face axis. (usefull for **surfaces**)

## Picker 🎯
- Copy the mouse hovered shape with **middle mouse button**

## Erase 🗑
- Removes placed objects.
- ⚠️ **Undo does not work for deleted objects** in this version.

## Undo ↪️
- **Undo** removes the last placed objects in the reverse order.
- ⚠️ **Undo** does not work for deleted objects.
- **Future versions may include undo for deletions.**

## Loading an XML file 📂
- To edit anything you must **load an existing valid XML file**.
- Click the "**Load XML file**" button at the top of the screen and select your OBJ file.
- **This tool does not generate new XML files from scratch** (yet).

## Loading a visual guide 🔎
- **Load visual ghost mesh** Imports an OBJ file as a visual guide mesh for **voxel** and **surface** placement.
- Click the "**Load visual ghost mesh of obj**" at the top of the screen and select your OBJ file.
- 1 block = 0.25x0.25x0.25m.

### Generating a voxel mesh from OBJ file 📐
- **Generate voxel mesh from obj file** Generates **voxels** from an obj file
- The **vertices** in the OBJ file are **treated as the corners of the voxels** (0.25x0.25x0.25 m voxels).
- To use efficently:
- **Build** the mesh in Stormworks.
- **Export** while in the **Stormworks** editor by pressing "f11".
- **Import** the PLY file into **Blender**
- **Remove unnecessary (non voxel) vertices** (recomended).
- **Export** as **OBJ file**.
- **Load the file inside** this tool with the "GEN" button.

## Saving 💾
- Saves and **overrides** the current XML file.
- **Shortcut:** **Ctrl + S** to **save** the current XML file.
- ⚠️ **This cannot be undone, make backups before starting!**

### Save as
- Saves and **overrides** the selected XML file.
- ⚠️ **This cannot be undone, make backups before starting!**

## Opacity options 👓
### Placeables opacity
- Adjust the **opacity** of **voxels** and **surfaces** (0%-100%) by moving the slider on the far left of the screen.

### Visual mesh opacity
- Adjust the **opacity** of the visual mesh guide (0%-100%) by moving the slider to the right of the **placeables opacity** slider.

## Mirror mode 🚧
- Not implemented. (yet)

## Other features 🔧
### File converter 🔄 (temporarily removed)
- **Convert files** converts between DAE and MESH files (also works with the texture compiler for texture files).
- Click the menu at the upper left of the window and select "**Convert files**" to go **to the file converter**
- Select your **Stormworks mesh compiler** (likely at "C:/Program Files (x86)/Steam/steamapps/common/Stormworks/sdk/mesh_compiler.com").
- **Select files** to convert.
- **Choose an output folder** (defaults to source folder).
- Click "**convert**" to convert your files from *.dea* to *.mesh*.
- You can go back to the editor by clicking "**Editor**" on the upper left of the window.

#### Use operating system file explorer option
- Changes between native and Godot file explorer
- ⚠️ Native file explorer does not remember the last file conversion location.

# Disclaimer ⚠️
- **This tool will override your old XML file** when you save. Always make backups!
- **Use at your own risk.** There are many bugs.
- **Please report issues and suggest features** via [Discord]((https://discord.gg/YWDb5x6xCJ)) [GitHub](https://github.com/Se-sSi/Stormworks-Modding-Tool).

## NOTE ❗
I am NOT affiliated with the Stormworks developers.

# Need help? ❓
- **Read this README carefully!**
- If your issue is not covered. Feel free to ask me on [Discord]((https://discord.gg/YWDb5x6xCJ)) (linked below).

## Socials 🌐
- [**GitHub** (click here)](https://github.com/Se-sSi/Stormworks-Modding-Tool)
- [**Discord community server** (click here)](https://discord.gg/YWDb5x6xCJ)
- [**Steam workshop** (click here)](https://steamcommunity.com/profiles/76561198040040549/myworkshopfiles)
- [**Youtube** (click here)](https://www.youtube.com/@se-ssi)
