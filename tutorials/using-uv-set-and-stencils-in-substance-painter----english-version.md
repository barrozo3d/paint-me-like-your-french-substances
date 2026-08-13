---
title: Using UV set and Stencils In Substance Painter -- English version
source: YouTube
url: https://www.youtube.com/watch?v=FIvOFo-zbms
author: 3DRedBox
ingested: 2026-08-13
app: "Substance 3D Painter"
version: "not stated on screen"
tags: [layers, fill-layer, paint-layer, masks, generator, procedural, alpha, stencil, uv, texel-density, tri-planar, roughness, height, basecolor, blend-mode, intermediate, advanced]
extraction_status: complete
frames_dir: tutorials/frames/using-uv-set-and-stencils-in-substance-painter----english-version/
frame_count: 11
frame_status: complete
frame_selection: content-anchored (manual timestamps chosen from transcript, not blind percentages)
---

# Using UV set and Stencils In Substance Painter -- English version

**Source:** [YouTube](https://www.youtube.com/watch?v=FIvOFo-zbms)
**Author:** 3DRedBox
**Duration:** 24m16s | 1 section(s)

---

## Raw Data (for Claude Code extraction)

Frames captured — see "Captured Frames" section below.


### Full Content [0:00]
**Transcript (timestamped):**
[0:00] Hello everyone, welcome to this tutorial, my name is Mehdi from 2D Redbox Channel and
[0:16] today we are going to talk about how to achieve this kind of result inside Substance Painter
[0:22] with using Stencil.
[0:24] And before that, we are going to cover a new feature inside Substance Painter which is very
[0:29] useful and I used it to create this material inside Substance Painter.
[0:35] So let's go for the tutorial and before jumping into the video itself, let me introduce you
[0:42] the brand new tutorial and the course that we released for Substance Painter.
[0:50] Learning Substance Painter is easier than ever.
[0:53] Hey all Substance Lovers, TechTune Seekers and awesome future artists, welcome to ultimate
[0:59] course for learning Substance Painter from zero to hero.
[1:08] Ready to learn how to texture with different projects, Substance Master released a brand
[1:13] new course for those who want to learn to texture with Substance Painter.
[1:19] In this course, we covered from preparing the model to rendering different projects,
[1:24] different challenges.
[1:25] If you want to level up your skill in texturing, come and check the Substance Master ultimate
[1:30] course for learning Substance Painter.
[1:32] Okay, before using UV sets inside Substance Painter in our project, let me explain you
[1:40] in the concept.
[1:42] This simple cube has this UV layout.
[1:47] Due to our limitation, zero to one UV space we need to pack because we are going to texture
[1:57] it in Substance Painter.
[1:58] So we rotate this to use the much space that we can.
[2:05] And for this little space in here, we couldn't see in action, so we can decrease this section,
[2:17] this UV island.
[2:19] So this is the situation that we have.
[2:23] And if we use this technique, the drawback of that is when we want to match the size
[2:33] of the texture, not the quality.
[2:37] When we tile the texture, there is a difference as you can see in here, between this section
[2:44] and here.
[2:47] So we want to solve this issue with UV set inside Substance Painter with this new feature.
[2:57] And we have another problem here.
[3:00] The rotation, the direction of this UV island is different.
[3:06] So we have a problem here, the rotation and the size.
[3:12] And how we are going to solve this issue, this is the UV layout, but I'm going to bake
[3:22] all the data related to my textures into this UV layout.
[3:30] But I'm not going to use any rotation option inside Substance Painter to fix this issue
[3:38] or creating different layers and play with the tiling.
[3:44] So I'm going to create any UV channel here, UV channel number one, and create this UV layout.
[3:57] But the issue for this type of UV layout is we have UV cutscene all over the edges.
[4:11] And the problem is we couldn't continue our texture in here.
[4:17] And you cannot see the continuous here.
[4:20] So I create another UV set here or UV channel.
[4:26] And as you can see, the UV or the texture on the UV is continuous.
[4:35] Okay, so I'm going to save it and let's go back to the Substance Painter and explain
[4:41] what's happening inside Painter.
[4:43] Okay, now we are in Substance Painter.
[4:46] And as you can see, the UV that we're going to work on it is the rotated one.
[4:52] Okay, so I'm going to create a fill layer here.
[4:56] Let's rename it to Test.
[4:58] And in the base color, I'm going to, for example, use this fabric circle.
[5:04] And let's increase tiling to five.
[5:07] And as you can see, the rotation is not correct.
[5:11] And we have this issue here.
[5:13] Okay.
[5:14] The first solution for this kind of issue is using the Projection Triplanar.
[5:21] Okay, so it's fixed already, as you can see.
[5:26] But it's a simple cube.
[5:28] What if we have a complex shape?
[5:30] Okay, the Triplanar is not a good answer for complex shape and what we can do.
[5:39] We can change the projection to UV set.
[5:43] And in the UV set, we have UV set zero, which we can see it here.
[5:49] Okay, as you can see in the source, UV set numbers zero, it's no effect.
[5:58] So it means we can see it right now.
[6:02] And we have issue here, the size and the rotation.
[6:05] Okay.
[6:06] The UV set number one, it fix the size problem.
[6:12] Okay.
[6:13] And as you can see, we have rotation for each UV island that we create.
[6:22] But in UV set number two, we solve the size problem and we can see the continuous effect
[6:32] here.
[6:33] So in this way, we can use different UV channel inside.
[6:38] Substance painter, very easy.
[6:40] Okay.
[6:41] So let's go to the project and I'm going to show you what is the purpose of using this
[6:47] technique.
[6:49] Okay, now it's time to focus on our project.
[6:53] This video is related to how to create, I know, edge wear effect on the surface in natural
[7:01] way.
[7:02] So I skipped the wood creation material process for this video.
[7:07] So I create this smart material and I'm going to share it with you.
[7:11] You can find it in the description with the link in the description.
[7:17] And before jumping to how to use the stencil for creating realistic effect on the surface,
[7:25] let's talk about the UV set technique in this project.
[7:31] Okay.
[7:32] So we're going to create a fill layer here.
[7:34] Let's add black mask and let's add a fill.
[7:38] Okay.
[7:39] In the create skill section, let's use this one.
[7:46] Okay.
[7:47] I'm going to put it on five.
[7:49] Okay.
[7:50] The problem is according to UV layout that we create inside RISO lab, the main goal was
[7:58] using maximum space in each UV type.
[8:02] Okay.
[8:03] So for this purpose, I need to rotate each UV island 90 degree to fill out maximum space.
[8:14] So when we use direction noise on UV projection metal, as you can see, we have this kind of
[8:23] direction.
[8:24] Okay.
[8:25] And it's not good for me.
[8:30] And the first solution is change projection to triplanar.
[8:36] Okay.
[8:38] It fix so many shoe, but the problem is, okay, it's okay.
[8:44] We have this direction here, but in here, I don't want this.
[8:49] Okay.
[8:50] Maybe in here, I don't want this too because I need 90 degree direction or top down direction
[8:57] here, not left, right.
[9:00] So the triplanar, it's not a good solution for me here.
[9:06] I can do another thing.
[9:08] For example, duplicate this direction noise and mask this area that I don't want it.
[9:16] And after that, I duplicate the direction noise, change the rotation 90 degree and boom, it's
[9:23] done.
[9:24] Okay.
[9:25] But the better solution is here, UV set.
[9:31] So in UV set zero, I have this effect.
[9:36] I don't want it.
[9:37] But in UV set number one, I fix the rotation and direction by my own.
[9:48] Okay.
[9:49] And boom, as you can see, easy.
[9:56] I fix the scale and the rotation issue at the same time.
[10:02] With UV set technique.
[10:04] Let me show you what happened in the UV section.
[10:10] Okay.
[10:11] This is the UV channel number one.
[10:15] Okay.
[10:16] So the goal was reach the maximum space in UV type.
[10:22] So we've done this.
[10:24] But in UV channel number two, as you can see, the rotation and the direction, it was my
[10:34] goal and the scale around all UV island.
[10:39] Okay.
[10:41] So this is the UV set number one or UV island number two.
[10:47] And in substance painter, as you can see, I have this result.
[10:53] So the benefit of using this kind of technique for texture or field layer, it's enormous
[11:03] achievement in site substance painter.
[11:05] It's not a game changer yet, but it's a good feature.
[11:09] Okay.
[11:10] So when you use this material and you feel something wrong, you need to check the UV
[11:22] set and the source of it.
[11:27] So let's go back here.
[11:30] And we are going to talk about the edge on wear effect and create more realistic edge
[11:38] on wear effect on the surface in our material with using a stencil.
[11:43] Okay.
[11:44] So the main and the best reference for us when we want to create wood burn effect is
[11:55] using real images.
[11:57] Okay.
[11:58] So the best way is transfer all the data or the data that we want from the image to the
[12:08] texture.
[12:09] Okay.
[12:10] So we create a library for you for the wood and other things.
[12:19] You can check it on the market.
[12:23] And the technique that we are going to use for this is a stencil.
[12:29] It means you have a mask, which is created based on the real images or real board.
[12:38] And you are going to project that mask on the surface and you have a natural detail on
[12:47] the surface.
[12:48] You can find the product link in the description.
[12:52] Okay.
[12:54] Let me import all the wood stencils for imperfection to this project.
[13:04] And as you can see, we have different masks that we can use inside Substance Printer.
[13:12] And we can use this mask in two different ways.
[13:16] For the first, we can use each image or each stencil as a single image or we can create
[13:26] stencil sheet inside Photoshop and save it as a different resource imported as a stencil
[13:34] and use it inside Substance Printer.
[13:38] So let's go back to the project and start our work.
[13:41] Okay.
[13:42] And in here, I have this layer.
[13:48] Okay.
[13:49] And in this layer, I can paint any mask that I want.
[13:57] And it's going to invert for the top layer and we have this result.
[14:03] Okay.
[14:04] So let me add a fill layer and load some, for example, paint.
[14:11] Pilled.
[14:12] Okay.
[14:13] And this is the effect that we have.
[14:21] But when we use a Persistual Texture or Generator, you know, it's going to give us a generic
[14:32] result and it's not good in overall term because we need to give a unique feel to the
[14:42] material and the texture.
[14:44] Okay.
[14:45] And the fast way is using stencil.
[14:48] We can paint all the detail with the brushes inside Topson Painter, but when we use stencil
[14:55] or imperfection texture, you know, we are in the next level because the mask is ready.
[15:04] You just need to find the position and paint the detail over there.
[15:09] Okay.
[15:10] So let's use some of them.
[15:13] And after that, I'm going to apply all the detail that I want into this model.
[15:20] So for using stencil or imperfection, I need paint layer.
[15:27] Okay.
[15:29] And I need to go to the paint section.
[15:33] And here I can use the stencil.
[15:36] So let's load the first image here.
[15:42] Okay.
[15:45] And this is the stencil, the live mask.
[15:48] Okay.
[15:49] So for controlling this, I need to hold S on the keyboard.
[15:55] Okay.
[15:56] And with the right mouse button and moving mouse, we can zoom in or zoom out or a second
[16:06] scale up or scale down the stencil.
[16:11] Okay.
[16:12] For rotation S and left mouse button.
[16:17] Okay.
[16:18] For panning or reposition the mask, we use the middle mouse button.
[16:23] And for each transformation or navigation for the stencil, you need to hold S on the
[16:31] keyboard.
[16:32] Okay.
[16:33] And please be aware if your language on the windows is not on the English, it's not going
[16:42] to work.
[16:43] So this is the problem that I have all the time with the language.
[16:50] And in here, I'm going to paint all the detail here.
[16:58] Okay.
[16:59] Like this.
[17:03] Here.
[17:07] And boom.
[17:11] So after that, I can go to the regular paint, use razor or black paint and remove some area
[17:25] that I want or I don't want the paint.
[17:31] Okay.
[17:32] Like this.
[17:34] So let's go back here.
[17:37] And I'm going to use another image like this one.
[17:44] Okay.
[17:45] That's good.
[17:48] And I'm going to paint here.
[17:52] Like this.
[17:53] Let's remove it.
[17:56] Invert the color and I can control the result.
[18:05] Okay.
[18:07] Like this.
[18:10] So I can increase the height value here.
[18:21] Okay.
[18:23] Choose this one.
[18:26] Yeah, it's so much better.
[18:30] Okay.
[18:31] And let's go back to the paint.
[18:33] You can use different paints layer to control the detail.
[18:38] For example, for this section, you just need to use one paint layer.
[18:45] And for the next one, you can add another paint layer to the data separately.
[18:51] It's a better way.
[18:53] Okay.
[18:54] So this is the main method and the only thing that I'm going to use here at detail with
[19:03] the stencil in this mask.
[19:06] And I'm going to pause the video.
[19:09] And after that, I'm going to show you what's happened after that and close this tutorial.
[19:16] Okay.
[19:17] We are done.
[19:18] Let's have a breakdown of what I did.
[19:21] So for the first layer, I use metal edgeware and dirt generator.
[19:27] Okay.
[19:28] So this is the effect and we can see it in the mask.
[19:32] So there are some, you know, area that I don't want to have this effect on it.
[19:40] So I just add a paint layer, change blending mode to subtract.
[19:45] And I just paint over and remove the area.
[19:50] Okay.
[19:51] So let's go for the ground paint a scratch layer.
[19:56] It's like subtract and removing some area from the data metal edge generator to achieve
[20:05] a realistic look, not a generic one.
[20:09] Okay.
[20:10] So the next one is layer number one.
[20:14] As you can see, I use a stencil to add this kind of effect on the mask.
[20:24] The second one is like that.
[20:27] The third one, I use a stencil again.
[20:31] And this is the force and fifths.
[20:33] Okay.
[20:34] So we have all the detail that we want in front of the object like this.
[20:42] That's great.
[20:43] And for the edges, I need more intensity, but the metal edge, it's not like what I need.
[20:54] So I add another paint and work on the edges.
[21:00] As you can see, again, with the stencil, with different picture, I just project the mask
[21:06] on the surface and remove area, add some area again with the brush.
[21:13] And this is the general workflow that I followed.
[21:17] Okay.
[21:19] So as you can see, I have some detail here.
[21:25] That's good.
[21:27] So after adding all this data, I feel we can have more surface wear.
[21:36] Okay.
[21:37] So I use grunge paint scrap, but the lowest opacity, okay, like this before, after.
[21:47] And again, another grunge, crack dipped.
[21:53] And this is the result.
[21:58] Okay.
[21:59] So I push out with the level to have more clean and avoid noisy mask.
[22:11] That's good.
[22:13] As you can see, this is the result.
[22:14] But I feel the surface is not, you know, it's not complex.
[22:20] So I need to have another layer.
[22:23] So I just add a paint cover on it.
[22:27] It's a simple one.
[22:30] And in the mask, I just use the same technique.
[22:34] As you can see, let's go to the mask, turn off all those soft layers.
[22:40] For the first one, I use the dirt.
[22:43] Okay.
[22:45] And it's effect on the dirt area very slightly.
[22:49] Okay.
[22:51] And I pick some area, as you can see in here and add some details.
[23:02] Another layer of the detail here and like this.
[23:10] So the last one is subtraction layer.
[23:15] And at the end, I just want to mention the edges.
[23:19] So I remove the edges from this mask.
[23:24] So we have this result.
[23:28] And that's it.
[23:29] And if we want to paint all this detail with the brush, simple brush or even using some
[23:38] custom brushes, it's near impossible.
[23:42] But using a stencil, using images as a mask projection technique, it's a good way to
[23:50] achieve this kind of result.
[23:52] And this is for this tutorial.
[23:54] I hope you can find this useful for you.
[23:58] You can download the material in the description with the link.
[24:04] And you can reach out the product that I used here for the wood stencil again in the description.
[24:12] So have fun, be creative.
[24:14] Goodbye.



---

## Captured Frames

- [1:47] tutorials/frames/using-uv-set-and-stencils-in-substance-painter----english-version/frame_000.jpg
- [5:07] tutorials/frames/using-uv-set-and-stencils-in-substance-painter----english-version/frame_001.jpg
- [6:05] tutorials/frames/using-uv-set-and-stencils-in-substance-painter----english-version/frame_002.jpg
- [8:50] tutorials/frames/using-uv-set-and-stencils-in-substance-painter----english-version/frame_003.jpg
- [9:56] tutorials/frames/using-uv-set-and-stencils-in-substance-painter----english-version/frame_004.jpg
- [13:12] tutorials/frames/using-uv-set-and-stencils-in-substance-painter----english-version/frame_005.jpg
- [15:45] tutorials/frames/using-uv-set-and-stencils-in-substance-painter----english-version/frame_006.jpg
- [17:07] tutorials/frames/using-uv-set-and-stencils-in-substance-painter----english-version/frame_007.jpg
- [19:56] tutorials/frames/using-uv-set-and-stencils-in-substance-painter----english-version/frame_008.jpg
- [21:06] tutorials/frames/using-uv-set-and-stencils-in-substance-painter----english-version/frame_009.jpg
- [23:19] tutorials/frames/using-uv-set-and-stencils-in-substance-painter----english-version/frame_010.jpg

---

## Structured Notes

### Core Technique
Two-part technique video: (1) using a Fill layer's **UV set to UV set projection** source to independently fix a tiled pattern's scale and rotation per UV island without re-baking or hand-rotating each island, and (2) using imported real-photo **Stencils** (live on-surface projected masks, S+mouse navigation) instead of generic procedural generators to hand-place natural, non-repetitive wood-imperfection detail.

### Summary
Part 1 demonstrates the problem on a test cube: when a UV layout is packed tightly (rotated islands to save space), a tiled Fill-layer pattern reads at mismatched scale/rotation per island under normal UV projection, and Tri-Planar projection only half-fixes it (breaks on complex shapes, can't target individual faces). The fix is baking a second UV channel (UV set 1) authored purely to have correct scale/rotation per island (accepting its own UV overlaps/cuts), then setting the Fill layer's Projection to **UV set to UV set projection** with Source = that second UV set — the visible texture still renders through UV set 0's layout but reads scale/rotation from UV set 1. Demonstrated live on a real wood-cabinet project fixing a Directional Noise generator's inconsistent scratch direction across drawer faces. Part 2 covers importing wood-imperfection **Stencils** (single images or Photoshop-built stencil sheets) via the Paint tool's Stencil field, live-transforming them on the 3D surface (hold **S** + right-mouse-drag to scale, **S** + left-mouse-drag to rotate, middle-mouse-drag to pan — requires English Windows locale or the shortcut breaks), then painting/erasing through them layer by layer to build up an edge-wear and surface-imperfection pass. Ends with a full layer-stack breakdown: base Metal Edge Wear + Dirt generator layer with a Subtract paint layer removing unwanted areas, several stencil-driven paint layers adding wear detail, then two Grunge (Scratched/Dripped) low-opacity paint passes with a Levels cleanup, and a final edge-focused stencil pass plus a Subtract layer removing wear from the model's actual edges to avoid double detail.

### Key Steps
1. On the test cube, add a Fill layer with a tiled pattern (base UV projection) — observe scale AND rotation mismatch between packed UV islands.
2. Try **Tri-Planar** projection — fixes rotation/scale globally but can't be constrained per-face and breaks down on complex (non-cube) geometry.
3. In the DCC/UV tool, author a second UV channel (UV set 1) laid out purely for correct per-island scale/rotation (ignore seams/overlaps — it's never used for baking real texture data).
4. Back in Painter, set the Fill layer's **Projection → UV set to UV set projection**, **Source → UV set 1** (vs. UV set 0 = no effect / original layout) — texture now renders through UV set 0's islands but inherits scale+rotation from UV set 1.
5. Applied on the real cabinet project: a Directional Noise generator (edge-wear direction) read inconsistently per drawer face under plain UV projection; switching its projection Source to the second authored UV set fixed direction and scale simultaneously, without manually duplicating/rotating the generator per face.
6. Import wood-imperfection **Stencils** (Assets panel, single images or a Photoshop-built stencil sheet saved/imported as a stencil resource).
7. On a Paint layer, load a stencil image into the Paint tool's Stencil slot — it appears as a live semi-transparent overlay on the 3D mesh.
8. Navigate the stencil with the keyboard held down: **S + right-mouse-drag** = scale, **S + left-mouse-drag** = rotate, **middle-mouse-drag** = pan/reposition. (Note: breaks if the OS language isn't English.)
9. Paint through the positioned stencil to stamp the real-photo detail onto the surface; use the eraser/black paint afterward to remove any transferred areas that don't read naturally.
10. Repeat with additional stencil images on separate paint layers (keep each stencil pass on its own layer for independent control) — layer 1-2 use one image, layer 3 another, etc.
11. Final breakdown: base layer = Metal Edge Wear generator + Dirt generator with a Subtract-blend paint layer removing generic-looking areas; multiple stencil paint layers stack the hand-placed detail; two low-opacity Grunge (Scratched, Dripped) passes add secondary noise, cleaned up with a Levels filter to avoid a noisy mask; a final stencil pass increases edge intensity; a closing Subtract layer removes wear specifically from the model's real geometric edges (so the Metal Edge Wear generator isn't fighting the hand-placed edge detail).

### Layers / Tools / Settings
- `Fill layer → Projection` = `UV set to UV set projection`, `Source` = target UV set (0 = no effect / base layout, 1/2 = authored fix channels)
- `Fill layer → Projection` = `Tri-Planar` (partial fix, global only, breaks on complex shapes)
- `Directional Noise` generator (edge-wear direction), re-sourced from UV set 0 to a custom UV set
- Paint tool → `Stencil` field (single image or Photoshop-built stencil sheet resource)
- Stencil navigation: `S` + RMB drag = scale, `S` + LMB drag = rotate, MMB drag = pan
- `Metal Edge Wear` generator + `Dirt` generator (base mask layer)
- `Subtract` blend-mode paint layers (removing generic/edge detail)
- `Grunge Paint Scratched`, `Grunge Paint Dripped` (low-opacity secondary noise passes)
- `Levels` filter (mask cleanup after grunge passes)
- Channels affected: mask/Height (visible in captured frames as Roughness-channel mask stack)

### Difficulty
Intermediate to Advanced (UV-set projection trick is a lesser-known feature; stencil workflow is straightforward once the keyboard-modifier navigation is understood)

### App & Version
Not stated on screen; no version-gated UI markers visible in the captured frames — consistent with the pre-12.1-era UI seen across this creator's other ingested videos.

### Tags
`layers` `fill-layer` `paint-layer` `masks` `generator` `procedural` `alpha` `stencil` `uv` `texel-density` `tri-planar` `roughness` `height` `basecolor` `blend-mode` `intermediate` `advanced`

---

## Related Tutorials
- **How to use UDIMs properly!** (`tutorials/how-to-use-udims-properly.md`) — same creator, same underlying theme of UV-layout choices controlling in-Painter texture fidelity (texel density there, per-island scale/rotation here).
- **Texturing a Worn Wooden Stool in Substance Painter** (`tutorials/texturing-a-worn-wooden-stool-in-substance-painter.md`) — same creator, another case of fixing per-UV-island tiling/rotation mismatches on a real prop.
- **Speed Up Your Substance Painter Workflow with This Easy Trick!** (`tutorials/speed-up-your-substance-painter-workflow-with-this-easy-trick.md`) — same creator, same "practical workflow trick" video format.
