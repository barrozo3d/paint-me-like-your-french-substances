---
title: Preparing Models for Substance 3D Painter in 3DS Max | Adobe Substance 3D
source: YouTube
url: https://www.youtube.com/watch?v=xuLRnFBvLyI
author: Adobe Substance 3D
ingested: 2026-08-13
app: "[PENDING]"
version: "[PENDING]"
tags: []
extraction_status: pending
frames_dir: tutorials/frames/preparing-models-for-substance-3d-painter-in-3ds-max-adobe-substance-3d/
frame_count: 0
frame_status: pending-selection
---

# Preparing Models for Substance 3D Painter in 3DS Max | Adobe Substance 3D

**Source:** [YouTube](https://www.youtube.com/watch?v=xuLRnFBvLyI)
**Author:** Adobe Substance 3D
**Duration:** 6m51s | 5 section(s)

---

## Raw Data (for Claude Code extraction)

Frames are not captured yet. Read the timestamped transcript below, pick moments
that actually show a technique/result worth a still (not blind percentages —
even within a named chapter, verify the real moment against its timestamps), then run:
  python select_frames.py preparing-models-for-substance-3d-painter-in-3ds-max-adobe-substance-3d <ts1> <ts2> ...
(seconds or mm:ss). This appends a "Captured Frames" section and updates the
frontmatter before you write the Structured Notes below.


### <Untitled Chapter 1> [0:00]
**Transcript (timestamped):**
[0:00] In this video, we look at how to prepare your models before importing them into Substance 3D Painter.
[0:16] You should already have a base understanding of modeling and UV and wrapping.
[0:19] To catch up on that, we have another video for you to watch first.
[0:24] When working in Painter, you split your models into various parts to make the texturing process easier.
[0:32] You can split your model by using texture sets, geometry masks, and ID maps.
[0:39] Let's learn what these are and how to use them.
[0:44] When you import a model, Painter automatically splits the model into texture sets based on the materials originally assigned to the model in your previous 3D program.
[0:54] The name of a material becomes the name of the texture set.
[1:00] Texture sets are the main way to organize your model in Painter.
[1:03] Each texture set has its own stack of layers and exports to its own set of bitmaps.
[1:10] Think of them as multiple layer documents inside your Painter file.
[1:18] Texture sets need to work together with your UV layout.
[1:21] Because each texture set is an individual layout, your UV map should be packed for each texture set.
[1:29] That means efficiently grouping the UV layouts per texture set to get the most out of your UV space.
[1:39] You can then mask and split materials within your texture sets by using either geometry masks or an ID map.
[1:47] Geometry masking relies on sub-geometry in your model.
[1:51] Keeping your model split in individual parts lets you use those parts as masks.
[1:57] You activate the geometry mask for a layer, then simply check or uncheck sub-objects from the list.
[2:07] Alternatively, you can use an ID map.
[2:11] ID maps are big textures that contain data to make assigning materials easier.
[2:15] When your model has an ID map, you hold down CTRL while dragging materials onto your object.
[2:21] This automatically assigns the material to a specific section of your model.
[2:33] You can create these maps in a few different ways, such as assigning vertex color data in your 3D application,
[2:40] or by baking maps using a second, high-poly mesh with different material colors for each ID section.
[2:47] Each method requires a different setup when baking your ID map.
[2:51] Models don't need a full UV unwrap to successfully import into Painter.
[2:56] Painter has a handy Auto-UV unwrap feature to do this for you.


### Auto Uv Unwrap [2:57]
**Transcript (timestamped):**
[3:02] Painters' Auto-UV tools do up to three steps.
[3:05] Cut UV seams.
[3:08] Unfold and flatten your cut UV islands.
[3:12] And pack the flattened islands into an efficient layout.
[3:16] Each step can keep the existing UV data that you made beforehand in your 3D application.
[3:24] For example, this mesh originally had all UVs stacked on one single layout.
[3:29] But after splitting it into separate texture sets, we can let Painter repack the UVs for us
[3:34] so that we're using our separate UV tiles more efficiently.
[3:39] Now let's try this out in 3ds Max.


### Texture Sets [3:42]
**Transcript (timestamped):**
[3:42] Let's start with texture sets.
[3:45] To assign different texture sets, you need to assign different materials inside 3ds Max.
[3:50] It's easiest to do this with a compact material editor, as that one gives you a better overview of your materials and their names.
[3:57] You start with creating a material for each texture set that you'd like to end up with in Painter,
[4:00] and then you name them properly because it helps to keep things organized.
[4:05] The type of material doesn't really matter, but it's a good idea to give them different colors so you can easily tell your texture sets apart inside 3ds Max.
[4:13] Once your materials are ready, you just assign them to your selection, or you drag and drop them into the viewport on specific objects.
[4:21] It's best to assign one material to an object, but you don't really have to do that specifically.
[4:26] After assignment, you need to make sure your UVs are packed per texture set.
[4:31] If you want to do this inside Max, the easiest way is to select all objects from a texture set, add a Unwrap UVW modifier, and then open the UV editor.
[4:41] Then use the Arrange Elements tool to pack your shells within the UV range.
[4:46] I personally prefer the Pack Normalize option, or you can just pack things manually also.
[4:51] You can also skip the packing inside Max and have Painter do it all automatically for you.
[4:57] Just export after the material assignment, and toggle the Auto Unwrap option in the New Project dialog.
[5:03] Then you open the options, and depending on if you already cut your seams and unfolded, you can tell Painter to regenerate all packing.
[5:11] This is done per texture sets, and it gives you a good layout to start texturing with.
[5:16] Then to do ID maps with vertex colors, you select your objects and you add a vertex paint modifier to all of them together.
[5:25] Then you go into vertex paint edit mode.
[5:27] You'll need to toggle the vertex color display in the bar to the left at the top, and then just use the Fill and Paint tools to assign unique colors to mesh parts.
[5:37] So you select a face or a sub-object and you assign colors.
[5:40] Remember to turn off the vertex color display before you exit the modifier because it's not done automatically.
[5:46] Once in Painter, go into the baking dialog after import, and make sure to set the ID map color source to vertex color.


### Prep for Geometry Masks [5:55]
**Transcript (timestamped):**
[5:55] And then last, to prep for geometry masks, that's pretty easy.
[5:59] So to use it in Painter, you just split your model into multiple objects.
[6:03] If you already have a lot of separated objects, you can just skip this step.
[6:06] But if your mesh consists of only one or two parts, go into Edit Poly mode and select sub-objects and then use Detach to split them into new objects.
[6:17] It's a good idea to name your objects properly because it just makes it easier to navigate in Painter.
[6:23] Once you get to Painter, geometry masking then lets you mask based on those objects from 3ds Max.


### Masking [6:24]
**Transcript (timestamped):**
[6:29] Simply click objects to toggle inclusion, so on or off, or use the drop-down on the right for shortcuts to include or exclude all objects.
[6:38] You can exclude all and then just click a few to include them.
[6:41] And that's all there is to basic mesh preparation in 3ds Max. Good luck with it.



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
