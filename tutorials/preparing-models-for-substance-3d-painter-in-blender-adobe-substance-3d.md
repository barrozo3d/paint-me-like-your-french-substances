---
title: Preparing Models for Substance 3D Painter in Blender | Adobe Substance 3D
source: YouTube
url: https://www.youtube.com/watch?v=jCwTEEyDX3Y
author: Adobe Substance 3D
ingested: 2026-08-13
app: "Blender (model prep) + Substance 3D Painter (import/baking)"
version: "not stated on screen"
tags: [texture-set, uv, id-map, mesh-maps, baking, beginner]
extraction_status: complete
frames_dir: tutorials/frames/preparing-models-for-substance-3d-painter-in-blender-adobe-substance-3d/
frame_count: 7
frame_status: complete
frame_selection: content-anchored (manual timestamps chosen from transcript, not blind percentages)
---

# Preparing Models for Substance 3D Painter in Blender | Adobe Substance 3D

**Source:** [YouTube](https://www.youtube.com/watch?v=jCwTEEyDX3Y)
**Author:** Adobe Substance 3D
**Duration:** 6m39s | 4 section(s)

---

## Raw Data (for Claude Code extraction)

Frames captured — see "Captured Frames" section below.


### <Untitled Chapter 1> [0:00]
**Transcript (timestamped):**
[0:00] In this video, we will look at how to prepare your models before importing them into Substance 3D Painter.
[0:13] You should already have a base understanding of modeling and UV unwrapping.
[0:18] If you want to catch up on that, you can watch this video first.
[0:22] When working in Painter, you split your models into various parts to make the texturing process easier.
[0:32] You can split your model using texture sets, geometry masks, and ID maps.
[0:38] Let's learn what these are and how to use them.
[0:42] When you import a model, Painter automatically splits the model into texture sets based on the materials originally assigned to it in your previous 3D program.


### Texture Sets [0:46]
**Transcript (timestamped):**
[0:52] The name of a material becomes the name of the texture set.
[0:58] Texture sets are the main way to organize your models in Painter.
[1:04] Each texture set has its own stack of layers and exports its own set of bitmaps.
[1:10] Think of them as multiple layered documents inside your Painter file.
[1:16] Texture sets need to work together with your UV layout.
[1:20] Because each texture set is an individual layout, your UV map should be packed for each texture set.
[1:28] That means efficiently grouping the UV layouts per texture set to get the most out of your UV space.
[1:36] You can then mask and split materials within your texture sets by using either geometry masks or an ID map.
[1:46] Geometry masking relies on sub-geometry in your model.
[1:50] Keeping your model split in individual parts lets you use those parts as masks.
[1:58] You activate the geometry mask for a layer, then simply check or uncheck sub-objects from the list.
[2:06] Alternatively, you can use an ID map.
[2:10] ID maps are baked textures that contain data to make assigning materials easier.
[2:18] When your model has an ID map, you hold down CTRL while dragging materials onto your object.
[2:25] This automatically assigns the material to a specific section of your model.
[2:31] You can create these maps in a few different ways, such as assigning vertex color data in your 3D application
[2:39] or by baking maps using a second hyperlimish with different material colors for each ID section.
[2:48] Models don't need a full UV unwrap to successfully import into Painter.
[2:53] Painter has a handy auto-UV unwrap feature to do this for you.


### Auto Uv Unwrap [2:54]
**Transcript (timestamped):**
[2:58] Painters' auto-UV tools do up to three steps.
[3:02] Cut UV seams, unfold and flatten your cut UV islands and pack the flattened islands into an efficient layout.
[3:13] Each step can keep the existing UV data that you made beforehand in your 3D application.
[3:21] For example, this mesh originally had all UVs stacked on one single layout.
[3:27] But after splitting it into separate texture sets, we can let Painter repack the UVs for us
[3:33] so that we are using our separate UV tiles more efficiently.
[3:37] Now let's try this out in Blender.
[3:40] To split your model into different texture sets in Painter, you need to assign different materials to it in Blender.
[3:46] If your model is already divided into separate objects, simply apply a different material on each of them.
[3:55] Here, I'm changing the colors of each material so that we can easily tell them apart in Blender.
[4:01] But Painter will only use the name we give them to create the texture set.
[4:07] If your model is not made out of different meshes, go into Edit mode.
[4:11] Here, select the parts of your model that you want to gather in one texture set.
[4:17] Then, in the Material Properties panel, click on the plus sign to create a new material.
[4:24] When it's done, assign it to your selection.
[4:27] Don't forget to give it a proper name to make your work easier in Painter.
[4:32] Repeat that operation for each texture set you want to create.
[4:37] You can then repack your UVs to make sure your texture set has the best density possible.
[4:43] There's two ways you can do this.
[4:46] You can either click the Pack UVs function in Blender for each texture set,
[4:51] or you can let Painter do it automatically for you.
[4:55] When importing your model, check the Auto Unwrap function.
[5:00] In the Option window, you can choose to recompute only the packing.
[5:05] Painter will then reorganize your UV islands following the texture sets that you've created in Blender.
[5:11] If you want to create masks or apply different material within your texture set,
[5:16] you can create an ID map using vertex colors.
[5:20] In Edit mode, select the areas that you want to target.
[5:24] Then, switch to vertex paint mode.
[5:27] Here, tick the Paint Mask option.
[5:30] Pick a color, then click on Paint, Set vertex color, or simply press Shift K.
[5:38] In Painter, you can now bake an ID map for your model based on the vertex colors that you've just set.


### Bake an Id Map [5:40]
**Transcript (timestamped):**
[5:45] To do so, go to the baker and simply select the vertex color option under the ID tab.
[5:54] Finally, you can use the geometry itself to create masks in Painter.
[5:59] If you already have all the separate meshes that you need, then you can skip this step.
[6:05] If you want to divide your mesh further, simply go into Edit mode and select the parts you want to separate.
[6:12] Then, hit P on your keyboard and choose the method that is the most suited to your needs.
[6:18] Same as with the texture set method, don't forget to give clear names to your meshes.
[6:23] You can now use those subparts in Painter to create additional masks during your texturing work.
[6:29] And that's how you prepare your model in Blender to make the most of it in Painter.



---

## Captured Frames

- [1:04] tutorials/frames/preparing-models-for-substance-3d-painter-in-blender-adobe-substance-3d/frame_000.jpg
- [2:20] tutorials/frames/preparing-models-for-substance-3d-painter-in-blender-adobe-substance-3d/frame_001.jpg
- [3:50] tutorials/frames/preparing-models-for-substance-3d-painter-in-blender-adobe-substance-3d/frame_002.jpg
- [4:20] tutorials/frames/preparing-models-for-substance-3d-painter-in-blender-adobe-substance-3d/frame_003.jpg
- [5:00] tutorials/frames/preparing-models-for-substance-3d-painter-in-blender-adobe-substance-3d/frame_004.jpg
- [5:27] tutorials/frames/preparing-models-for-substance-3d-painter-in-blender-adobe-substance-3d/frame_005.jpg
- [5:48] tutorials/frames/preparing-models-for-substance-3d-painter-in-blender-adobe-substance-3d/frame_006.jpg

---

## Structured Notes

### Core Technique
Preparing a Blender model (demoed on a roller skate) for a clean Substance Painter import: assigning named materials to drive automatic Texture Set splitting, packing/auto-repacking UVs per texture set, and building either a vertex-color ID map or separate sub-meshes so Painter can generate masks per model region.

### Summary
Explains Painter's three model-splitting mechanisms — Texture Sets (auto-created from the material names assigned in the source 3D app; each texture set is effectively its own layered document with its own layer stack and exported bitmaps, and needs its own efficiently-packed UV layout), Geometry Masks (masking by sub-object/sub-mesh membership, toggled per-layer by checking/unchecking parts from a list), and ID Maps (baked textures encoding per-region data, letting Ctrl+drag-assign a material straight onto a specific mesh section) — then demonstrates each from the Blender side. Also covers Painter's Auto-UV Unwrap feature (up to 3 steps: cut seams, unfold/flatten islands, pack islands into an efficient layout; each step can preserve UV data already made in the source app), used here specifically to re-pack UVs efficiently across newly-split texture sets. In Blender: assign a distinctly-named material per object (or, for a single mesh, select faces in Edit Mode and assign a new named material per desired texture set) to drive automatic Texture Set creation on import; repack UVs either directly in Blender (Pack UVs) or let Painter's Auto Unwrap (Recompute Only the Packing option) handle it on import, following the material-driven texture-set split. For an ID map: in Edit Mode select target faces, switch to Vertex Paint mode, enable Paint Mask, pick a color, and paint/set vertex color (Shift+K) per region — then in Painter, bake an ID map via the Baker's ID tab with Color Source set to Vertex Color. For geometry masks: select faces in Edit Mode, press P to separate into a new sub-mesh (choosing the appropriate separation method), name it clearly, and use it later in Painter as an additional geometry mask source.

### Key Steps
1. Understand the three model-splitting mechanisms Painter offers: **Texture Sets** (one per assigned material, each its own layered document/UV layout), **Geometry Masks** (masking by sub-mesh membership), and **ID Maps** (baked per-region color data enabling Ctrl+drag material assignment).
2. On import, Painter automatically creates one Texture Set per material found on the model, using each material's name as the texture set name.
3. Each texture set needs its own efficiently packed UV layout — because texture sets are independent layouts, UV packing should be organized per texture set, not globally.
4. Painter's **Auto-UV Unwrap** can perform up to 3 steps (cut seams / unfold+flatten / pack islands) and can preserve any UV data already authored in the source app at each step — models do not need a full manual unwrap before import.
5. In Blender, to create multiple texture sets: if the model is already split into separate objects, assign a distinct, clearly-named material to each object (material name becomes the Painter texture set name — visual color-coding in Blender is just for the artist's convenience, Painter ignores it).
6. If the model is a single mesh, enter Edit Mode, select the faces for one texture set, use the Material Properties panel's **+** to create a new material, assign it to the selection, and give it a clear name; repeat per desired texture set.
7. Repack UVs after splitting into texture sets: either use Blender's **Pack UVs** function per texture set, or let Painter do it automatically on import by checking **Auto Unwrap** and, in its Options window, choosing **Recompute Only the Packing** so Painter reorganizes UV islands to match the newly-created texture sets.
8. To build an ID map via vertex color: in Edit Mode select the target region's faces, switch to **Vertex Paint** mode, enable **Paint Mask**, choose a color, then paint or use **Set Vertex Color** (Shift+K) to apply it.
9. In Painter, bake an ID map from this vertex-color data via the **Baker → ID tab**, setting **Color Source = Vertex Color**.
10. To build geometry masks: in Edit Mode, select the faces to split out, press **P** and choose the appropriate separation method to create a new sub-mesh; name it clearly — this becomes an available geometry-mask source in Painter for later masking during texturing.

### Layers / Tools / Settings
- **Blender**: Material Properties panel (+ to add/assign named materials per texture set), Edit Mode face selection, Vertex Paint mode + Paint Mask option + Set Vertex Color (Shift+K), Pack UVs, P (Separate) for splitting sub-meshes.
- **Substance 3D Painter**: Auto Unwrap import option (Options window: Recompute Only the Packing), Baker → ID tab → Color Source = Vertex Color (also Material Color / File ID / Mesh ID / Polygroup options visible in the Baker dialog), Texture Set List panel, per-layer Geometry Mask (check/uncheck sub-objects).

### Difficulty
Beginner (model/UV/material prep fundamentals, no advanced texturing).

### App & Version
Blender (model prep side, version not stated on screen) + Substance 3D Painter (import/baking side, version not stated on screen).

### Tags
`texture-set`, `uv`, `id-map`, `mesh-maps`, `baking`, `beginner`

---

## Related Tutorials
- **Preparing Models for Substance 3D Painter in Maya** (`tutorials/preparing-models-for-substance-3d-painter-in-maya-adobe-substance-3d.md`) — same 3-app prep series, Maya-side equivalent of this exact workflow (texture sets, UV packing, ID maps, geometry masks).
- **Preparing Models for Substance 3D Painter in 3DS Max** (`tutorials/preparing-models-for-substance-3d-painter-in-3ds-max-adobe-substance-3d.md`) — same series, 3ds Max-side equivalent.
- **Preparing a 3D Asset in Substance 3D Painter | 3D in After Effects Part 1** (`tutorials/preparing-a-3d-asset-in-substance-3d-painter-3d-in-after-effects-part-1-adobe-su.md`) — same channel (Adobe), same "asset preparation" framing, but downstream-focused (readying a Painter-textured asset for After Effects) rather than upstream DCC mesh prep.
