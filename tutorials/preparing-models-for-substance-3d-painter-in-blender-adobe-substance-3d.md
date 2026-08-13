---
title: Preparing Models for Substance 3D Painter in Blender | Adobe Substance 3D
source: YouTube
url: https://www.youtube.com/watch?v=jCwTEEyDX3Y
author: Adobe Substance 3D
ingested: 2026-08-13
app: "[PENDING]"
version: "[PENDING]"
tags: []
extraction_status: pending
frames_dir: tutorials/frames/preparing-models-for-substance-3d-painter-in-blender-adobe-substance-3d/
frame_count: 0
frame_status: pending-selection
---

# Preparing Models for Substance 3D Painter in Blender | Adobe Substance 3D

**Source:** [YouTube](https://www.youtube.com/watch?v=jCwTEEyDX3Y)
**Author:** Adobe Substance 3D
**Duration:** 6m39s | 4 section(s)

---

## Raw Data (for Claude Code extraction)

Frames are not captured yet. Read the timestamped transcript below, pick moments
that actually show a technique/result worth a still (not blind percentages —
even within a named chapter, verify the real moment against its timestamps), then run:
  python select_frames.py preparing-models-for-substance-3d-painter-in-blender-adobe-substance-3d <ts1> <ts2> ...
(seconds or mm:ss). This appends a "Captured Frames" section and updates the
frontmatter before you write the Structured Notes below.


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

## Structured Notes

### Core Technique
[PENDING EXTRACTION]

### Summary
[PENDING EXTRACTION]

### Key Steps
[PENDING EXTRACTION]

### Layers / Tools / Settings
[PENDING EXTRACTION]

### Difficulty
[PENDING EXTRACTION]

### App & Version
[PENDING EXTRACTION]

### Tags
[PENDING EXTRACTION]

---

## Related Tutorials
[PENDING EXTRACTION]
