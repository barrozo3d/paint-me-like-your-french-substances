---
title: Preparing Models for Substance 3D Painter in Maya | Adobe Substance 3D
source: YouTube
url: https://www.youtube.com/watch?v=Gkx96GEextY
author: Adobe Substance 3D
ingested: 2026-08-13
app: "Maya (model prep) + Substance 3D Painter (import/baking)"
version: "not stated on screen"
tags: [texture-set, uv, id-map, mesh-maps, baking, beginner]
extraction_status: complete
frames_dir: tutorials/frames/preparing-models-for-substance-3d-painter-in-maya-adobe-substance-3d/
frame_count: 7
frame_status: complete
frame_selection: content-anchored (manual timestamps chosen from transcript, not blind percentages)
---

# Preparing Models for Substance 3D Painter in Maya | Adobe Substance 3D

**Source:** [YouTube](https://www.youtube.com/watch?v=Gkx96GEextY)
**Author:** Adobe Substance 3D
**Duration:** 8m49s | 10 section(s)

---

## Raw Data (for Claude Code extraction)

Frames captured — see "Captured Frames" section below.


### <Untitled Chapter 1> [0:00]
**Transcript (timestamped):**
[0:00] In this video, we will look at how to prepare your models before importing them into Substance 3D Painter.
[0:16] You should already have a base understanding of modelling and UV unwrapping.
[0:20] If you want to catch up on that, you can watch this video first.
[0:25] When working in Painter, you split your models into various parts to make the texturing process easier.
[0:32] You can split your model using texture sets, geometry masks and ID maps.
[0:39] Let's learn what these are and how to use them.
[0:43] When you import a model, Painter automatically splits the model into texture sets,


### Texture Sets [0:47]
**Transcript (timestamped):**
[0:49] based on the materials originally assigned to the model in your previous 3D program.
[0:55] The name of the material becomes the name of a texture set.
[0:59] Texture sets are the main way to organise your model in Painter.
[1:04] Each texture set has its own stack of layers and exports its own set of bitmaps.
[1:10] Think of them as multiple layered documents inside your Painter file.
[1:16] Texture sets need to work together with your UV layout.
[1:21] Because each texture set is an individual layout, your UV map should be packed for each texture set.
[1:29] That means efficiently grouping the UV layouts per texture set, to get the most out of your UV space.
[1:37] You can then mask and split materials within your texture sets, by using either geometry masks or an ID map.


### Geometry Masks [1:42]
**Transcript (timestamped):**
[1:46] Geometry masking relies on sub-geometry in your model.
[1:51] Keeping your model split in individual parts lets you use those parts as masks.
[1:57] You activate the geometry mask for a layer, then simply check or uncheck sub-objects from the list.
[2:06] Alternatively, you can use an ID map.
[2:10] ID maps are baked textures that contain data to make assigning materials easier.
[2:18] When your model has an ID map, you hold down control while dragging materials onto your object.
[2:25] This automatically assigns the material to a specific section of your model.
[2:31] You can create these maps in a few different ways, such as assigning vertex color data in your 3D application,
[2:40] or by baking maps using a second, high poly mesh, with different material colors for each ID section.
[2:48] Each method requires a different setup when baking your ID map.
[2:54] Models don't need a full UV unwrap to successfully import into Painter.
[2:59] Painter has a handy auto UV unwrap feature to do this for you.


### Auto Uv Unwrap [3:01]
**Transcript (timestamped):**
[3:06] Painter's auto UV tools do up to three steps.
[3:11] Cut UV seams, unfold and flatten your cut UV islands, and pack the flattened islands into an efficient layout.
[3:22] Each step can keep the existing UV data you made beforehand in your 3D application.
[3:29] For example, this mesh originally had all UVs stacked on one single layout,
[3:35] but after splitting it into separate texture sets, we can let Painter repack the UVs for us,
[3:41] so that we are using our separate UV tiles more efficiently.
[3:46] Now let's try this out in Maya.


### Maya [3:47]
**Transcript (timestamped):**
[3:50] For this part, we will assume that we have already re-tapologized our model, if needed,
[3:55] and done a first pass at our UV unwrapping of it.
[3:59] To assign different texture sets for Painter, you need to assign different materials to your model inside Maya.


### Materials [4:02]
**Transcript (timestamped):**
[4:06] Some people like to use the hyper shader setup their materials,
[4:09] but personally I like to do it just by right clicking my selection and clicking assign new material,
[4:14] and then editing it in the attribute editor.
[4:17] Both get you the same result.
[4:19] It's best to assign one material to an object, but it's not required.
[4:24] Make sure to name your materials properly to keep things organized,
[4:28] as this will become the name of your texture set in Painter.
[4:32] The type of material doesn't matter, so I usually just stick a Lambo on,
[4:36] but it's a good idea to give them different colors, just so you can easily tell your texture sets apart inside of Maya.
[4:43] After assignment, you need to just make sure your UVs are packed per texture set.


### Uvs [4:45]
**Transcript (timestamped):**
[4:48] If you want to do this inside Maya, you can of course pack your shells manually,
[4:52] but the easiest way to do this is to firstly open up your UV editor and UV toolkit.
[4:58] Then select all objects from a texture set.
[5:01] You can select this manually, or you can find the material either at the top of the hyper shade,
[5:06] or by toggling assigned materials in the display settings of the Outliner.
[5:11] Right click and go to select objects with material.
[5:16] You should then see your UV shells in the UV editor.
[5:19] Click and drag to select them all, and then come down to the Arrange and Layout tab in the UV toolkit and select Layout.
[5:28] What I would also advise to do is give your shells some padding, so that when it comes to map baking, we don't get any errors.
[5:35] This means just giving your shells a couple of pixels of space between each other and the tile edges.
[5:41] We can do this by shift and left clicking on the Layout button to open the Functions options.
[5:48] From here in the Layout Settings tab, we can add a couple of pixels of padding to both our shells and our tile.
[5:56] You can also skip the packing in Maya entirely and have Painter do it automatically for you.
[6:02] Just export right after Material Assignment and toggle the Auto Unwrap option in the New Project dialog.
[6:09] Open the options and depending on if you've already cut your seams and unfolded, you can tell Painter to regenerate all the packing.
[6:17] This is done per Texture Set and gives you a good layout to start texturing with.
[6:22] There's a couple of different ways to add ID maps to your model in Painter.
[6:27] The easiest way is by using Vertex Color.
[6:30] We can split sections that we think might have different textures within a Texture Set by first selecting our sections, for example the wheels,
[6:40] and coming to Mesh Display and clicking the Apply Color option box.
[6:45] This will bring up a tool for assigning Vertex Color that we can keep open as we go on.
[6:51] I simply select the color and click Apply.
[6:55] Again, the actual color of it doesn't matter as long as all the colors are different.
[7:01] Important to note that assigning Vertex Color is not the same as assigning a new material.
[7:07] By default, Maya will display your object with Vertex Colors in the viewport,
[7:11] but if we look in our Attribute Editor, we will see that the Texture Set material is still assigned.
[7:17] You can toggle Display Colors attribute on and off in the Mesh Display menu.
[7:23] Once in Painter, you can see my handy Texture Sets are here.
[7:28] We then go into the Bake Maps dialog and select the ID selection.


### Bake Maps [7:29]
**Transcript (timestamped):**
[7:33] Make sure to set the ID map color source to Vertex Color, click Bake Selected Textures.
[7:40] Now we can see by holding down CTRL and clicking and dragging material onto our model,
[7:45] Painter shows us different sections we can apply within our Texture Set using the ID maps we've created using Vertex Colors.
[7:52] Super easy!
[7:53] To use geometry masking in Painter, just split your model into multiple objects.


### Geometry Masking [7:54]
**Transcript (timestamped):**
[7:59] If you already have a lot of separate objects, you can skip this step.
[8:03] If your mesh consists of only one or two parts,
[8:06] right-click and hold to go to your face selection mode.
[8:10] Select your faces that you want to extract and then click the Extract button to split them into new objects.
[8:17] It's a good idea to delete history after this and name your objects properly,
[8:22] just to make them easier for you to navigate inside Painter.
[8:25] Geometry masking then allows you to mask based on the separate objects that you created in Maya.


### Masking [8:26]
**Transcript (timestamped):**
[8:32] Simply click Objects to toggle inclusion or use the drop-down for shortcuts to include or exclude all objects.
[8:40] And that was a quick rundown of how to prepare your model for Painter using Maya.



---

## Captured Frames

- [4:33] tutorials/frames/preparing-models-for-substance-3d-painter-in-maya-adobe-substance-3d/frame_000.jpg
- [5:22] tutorials/frames/preparing-models-for-substance-3d-painter-in-maya-adobe-substance-3d/frame_001.jpg
- [5:50] tutorials/frames/preparing-models-for-substance-3d-painter-in-maya-adobe-substance-3d/frame_002.jpg
- [6:40] tutorials/frames/preparing-models-for-substance-3d-painter-in-maya-adobe-substance-3d/frame_003.jpg
- [7:00] tutorials/frames/preparing-models-for-substance-3d-painter-in-maya-adobe-substance-3d/frame_004.jpg
- [7:35] tutorials/frames/preparing-models-for-substance-3d-painter-in-maya-adobe-substance-3d/frame_005.jpg
- [8:10] tutorials/frames/preparing-models-for-substance-3d-painter-in-maya-adobe-substance-3d/frame_006.jpg

---

## Structured Notes

### Core Technique
Preparing a Maya model (same roller skate asset as the Blender entry in this series) for a clean Substance Painter import: material-per-texture-set assignment, per-texture-set UV shell packing with padding (via Maya's UV Toolkit Layout function or Painter's Auto Unwrap), and building ID maps via Maya Vertex Color or geometry-splitting for masking.

### Summary
Maya-side installment of the same 3-app prep series as the Blender video, covering the identical conceptual ground (Texture Sets auto-named from source-app materials, Geometry Masks by sub-object, ID Maps for Ctrl+drag material assignment, Auto-UV Unwrap's 3-step cut/unfold/pack pipeline) with Maya-specific mechanics: assigning materials via right-click → Assign New Material (any material type works, e.g. Lambert, just for organization — Hypershade setup gives the same result), naming materials clearly since the name becomes the Painter texture set name, and giving each texture set's material a distinct viewport color purely for the artist's own visual tracking. UV packing is done per texture set using Maya's UV Editor + UV Toolkit: select all objects sharing a material (via right-click → Select Objects with Material, or the Outliner's "assigned materials" display toggle), select all UV shells, then Arrange and Layout → **Layout**; Shift+click the Layout button to open its Functions options and add a couple of pixels of shell/tile padding to avoid baking errors — or skip Maya-side packing entirely and let Painter's **Auto Unwrap** (in the New Project dialog, with the option to regenerate all packing) handle it per texture set on import. Building an ID map via Vertex Color: select target faces, Mesh Display → **Apply Color** option box, pick and apply a distinct color per section (color choice itself is arbitrary, only needs to differ per section) — explicitly notes Vertex Color assignment is separate from material assignment (the texture-set material stays assigned; Display Colors is a separate viewport toggle). In Painter: Bake Maps dialog → **ID** selection, set ID map **Color Source = Vertex Color**, Bake Selected Textures — after which Ctrl+drag-dropping a material onto the model snaps it to the vertex-color-defined sections. Geometry masking: for a single/few-part mesh, face-select the target region and use **Extract** to split it into a new object (delete history and rename afterward for clarity); in Painter, geometry masks then let you toggle inclusion per split object, or use dropdown shortcuts to include/exclude all objects at once.

### Key Steps
1. Prerequisite: model already retopologized (if needed) and given a first-pass UV unwrap before this workflow begins.
2. Assign materials to drive Texture Set creation: right-click a selection → **Assign New Material** (or use Hypershade — same result), edit in the Attribute Editor; material type doesn't matter (Lambert is fine) but give each a distinct viewport color purely so texture sets are easy to tell apart while working in Maya.
3. Name materials clearly and deliberately — the material name becomes the Painter texture set name. One material per object is best practice but not required.
4. Pack UVs per texture set in Maya: open the **UV Editor** + **UV Toolkit**, select all objects sharing one material (right-click → **Select Objects with Material**, or toggle "assigned materials" display in the Outliner), select all their UV shells in the UV Editor, then use **Arrange and Layout → Layout**.
5. Add shell/tile padding to avoid baking errors: Shift+left-click the Layout button to open its Functions options, then in Layout Settings add a couple of pixels of padding between shells and at tile edges.
6. Alternative: skip Maya-side packing entirely — export right after material assignment, then in Painter's New Project dialog enable **Auto Unwrap**, open its options, and choose to regenerate packing (optionally seams/unfold too, depending on prior UV state); this repacks per texture set automatically on import.
7. Build an ID map via Vertex Color: select the faces for a sub-section (e.g. wheels within a larger texture set), go to **Mesh Display → Apply Color** (option box) to open the vertex-color assignment tool, pick a color, click Apply — repeat with a different color per distinct section. Note this is independent of material assignment (the texture-set material remains assigned; vertex color is just a separate, toggleable viewport display via **Display Colors** in Mesh Display).
8. In Painter, after import, go to the **Bake Maps** dialog, select the **ID** map, set its **Color Source to Vertex Color**, and click **Bake Selected Textures**.
9. Use the baked ID map: hold **Ctrl** while dragging a material onto the model — Painter snaps the material to whichever vertex-color-defined section you drop it on.
10. Geometry masking: if the mesh isn't already split into enough separate objects, enter face selection mode, select the faces to isolate, and use **Extract** to split them into a new object; delete history and rename the new object clearly afterward.
11. In Painter, geometry masks let you toggle each separated object's inclusion individually (click to toggle) or use dropdown shortcuts to include/exclude all objects at once when building a mask.

### Layers / Tools / Settings
- **Maya**: right-click → Assign New Material (or Hypershade); Attribute Editor; UV Editor + UV Toolkit (Select Objects with Material, Arrange and Layout → Layout, Layout Settings padding options); face selection mode + **Extract**; Mesh Display → **Apply Color** (Vertex Color assignment) and **Display Colors** toggle; Outliner "assigned materials" display toggle.
- **Substance 3D Painter**: New Project dialog **Auto Unwrap** option (regenerate packing per texture set); **Bake Maps** dialog → ID tab → Color Source = Vertex Color; Ctrl+drag material assignment onto ID-mapped sections; Texture Set List panel; per-layer Geometry Mask (toggle objects individually or via include/exclude-all shortcuts).

### Difficulty
Beginner (model/UV/material prep fundamentals, no advanced texturing).

### App & Version
Maya (model prep side, version not stated on screen) + Substance 3D Painter (import/baking side, version not stated on screen).

### Tags
`texture-set`, `uv`, `id-map`, `mesh-maps`, `baking`, `beginner`

---

## Related Tutorials
- **Preparing Models for Substance 3D Painter in Blender** (`tutorials/preparing-models-for-substance-3d-painter-in-blender-adobe-substance-3d.md`) — same 3-app prep series and same roller-skate demo asset; Blender-side equivalent workflow (materials, UV packing, vertex-color ID maps, mesh separation).
- **Preparing Models for Substance 3D Painter in 3DS Max** (`tutorials/preparing-models-for-substance-3d-painter-in-3ds-max-adobe-substance-3d.md`) — same series, 3ds Max-side equivalent.
