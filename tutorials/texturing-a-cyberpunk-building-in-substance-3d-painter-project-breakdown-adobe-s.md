---
title: Texturing a Cyberpunk Building in Substance 3D Painter – Project Breakdown | Adobe Substance 3D
source: YouTube
url: https://www.youtube.com/watch?v=gv9R6a6VPYQ
author: Adobe Substance 3D
ingested: 2026-08-13
app: "Substance 3D Painter"
version: "not stated on screen"
tags: [layers, fill-layer, masks, generator, anchor-point, blend-mode, height, basecolor, roughness, metallic, emissive, alpha, procedural, viewport, advanced]
extraction_status: complete
frames_dir: tutorials/frames/texturing-a-cyberpunk-building-in-substance-3d-painter-project-breakdown-adobe-s/
frame_count: 8
frame_status: complete
frame_selection: content-anchored (manual timestamps chosen from transcript, not blind percentages)
---

# Texturing a Cyberpunk Building in Substance 3D Painter – Project Breakdown | Adobe Substance 3D

**Source:** [YouTube](https://www.youtube.com/watch?v=gv9R6a6VPYQ)
**Author:** Adobe Substance 3D
**Duration:** 8m11s | 10 section(s)

---

## Raw Data (for Claude Code extraction)

Frames captured — see "Captured Frames" section below.


### Intro [0:00]
**Transcript (timestamped):**
[0:00] Hi! In today's video, I'll show you a full breakdown of how I created textures for this Cyberpunk building using Adobe Substance 3D Painter.
[0:07] I'll walk you through the entire process and tell you how I achieved this effect, which is not only possible for beginners, but also fun to do.
[0:14] I start by creating the wall material. I drop a concrete texture as the base and then add a clay terracotta layer on top.


### Walls (brick material) [0:28]
**Transcript (timestamped):**
[0:35] I create a wide mask and for the fill layer, I use a brick pattern.
[0:41] I invert it, adjust the number of tiles on both the X and Y axis and scale it down until I get a satisfying effect.
[0:48] I duplicate the layer, turn off all channels except for height and increase it a little to make the bricks pop.
[0:53] I go back to the color layer and using color correct and color balance filters, adjust the colors to make them more saturated and darker.
[1:01] Next, I create a new layer filled with dark gray, add a black mask and apply the dirt generator.
[1:06] I tweak the generator's properties until I get the effect of a building covered with grease and smoke.
[1:11] In a very similar way, I add some moss accents. I drag and drop a skin vegetation texture, slightly change its color and use the 3D linear gradient generator to add some green tones to the bottom of the building.
[1:23] I also add the dripping grass generator to the same layer to add moss accents to the higher parts.
[1:28] I move all these layers into one folder, create a wide mask and paint to remove some bricks from the building's corners.
[1:39] Later, I choose a different brush, adjust its size and angle and start erasing bricks one by one to make it look like they fell off.
[1:45] I also remove bricks from other logical places, like near pipes or random damaged spots.
[1:59] Once this is done, I add a dirt layer over the concrete, group everything into one folder and add a sharpen filter set to 0.1 as the final touch.
[2:07] For the ground, I use a concrete coarse texture as the base.


### Concrete elements [2:09]
**Transcript (timestamped):**
[2:12] I drag and drop a smart material called plastic dusty and replace its fill layer with the texture I chose earlier.
[2:18] I adjust the dirt and dust masks and change their fill colors until I achieve the look that I want.
[2:23] I also create a separate dirt layer to give it an even dirtier look like a street sidewalk.
[2:32] I use the same material for other pavement elements in the curb.
[2:36] For the building corners, I switch the base texture to concrete cast, duplicate it, darken it a little
[2:42] and fill a black mask with a grunge texture to age the surface.
[2:46] I play with the scale and rotation to get it right.
[2:49] Next, I create a new layer filled with a brighter color and apply a concrete edges mask.
[2:58] Then I create another layer with only the height channel enabled.
[3:01] By lowering the height value, everything I paint now looks engraved.
[3:06] Using this technique, I paint lines in 2D view to make the concrete piece look divided into smaller sections.
[3:16] I add angle points, which I reference in my dirt layer by enabling micro height and
[3:20] micro normal in the properties.
[3:25] I adjust the dirt scale and invert it if needed.
[3:29] To make it look old and damaged, I use a cracks brush on vulnerable areas like edges and near the ground.
[3:44] I apply this material to the roof as well.


### Awning [3:49]
**Transcript (timestamped):**
[3:49] For the awning, I drag and drop a blue fabric texture.
[3:52] I change its color to red, duplicate it and make the duplicate darker.
[3:57] I add a black mask and use the fabric circle half overlap texture as the grayscale pattern.
[4:02] I adjust its rotation, scale and border width.
[4:05] Then I start stacking layers by duplicating them and changing colors and mask properties,
[4:10] creating a nice colorful fabric pattern.
[4:18] I group all layers into one folder and use oil paint and sharpen filters to blend them together.
[4:26] After that, I create a new layer filled with white at the dripping rust generator and tweak it slightly to create a damage effect.
[4:39] Similarly, I add another layer filled with dark brown and apply a dust soft mask to make the awning look dirty and dusty.


### Neons and metal details [4:47]
**Transcript (timestamped):**
[4:47] This part is probably the simplest.
[4:48] For most metal details, I use smart materials from the Substance 3D Library and just adjust dirt masks or swap based textures.
[4:56] For neons, I enable the emissive channel on the texture set settings at the layer filled with the color I want the neon to emit
[5:03] and increase the emissive intensity in the shader settings tab.
[5:06] Also, don't forget to enable glare in the display settings for the glowing effect.
[5:13] I repeat this for all neon signs, changing the emissive color to pink or green as needed.
[5:17] I explain how I created the window and glass materials in more detail in my Instagram for this collaboration,


### Windows [5:22]
**Transcript (timestamped):**
[5:25] so if you're interested, check it out.
[5:27] You can also try making them by yourself based on what I've already shown here.
[5:30] It's very easy.
[5:31] For the entrance door, I reuse the plastic dusty smart material.


### Door and window frames [5:34]
**Transcript (timestamped):**
[5:35] I adjust the color and dirt mask settings to better fit the object.
[5:39] To add interest, I create a new height layer filled with a tile generator and place it at the top of the layer.
[5:45] I tweak it a bit, but eventually switch to a stripes generator instead.
[5:48] I add ankle points and use them in a dirt layer to add wear around the raised details,
[5:53] just like I did for the concrete parts of the building.
[5:59] I lower the dirt level and darken the color.
[6:01] I use the same method for the window frame, but remember, if you're using ankle points,
[6:05] create new ones for different objects because they refer to specific object data.
[6:10] I cover the AC texturing process in more detail on Instagram,


### AC unit and smaller objects [6:13]
**Transcript (timestamped):**
[6:13] so if you're waiting for this part, head over there.
[6:15] I use lots of height, metalic, ankle points and masks.
[6:19] The process is the same for most small elements,
[6:21] and I always add tiny details like screws to boost realism.
[6:25] Since it's a city building, I usually go for a greasy, dusty look
[6:29] and almost always add grunge grayscale fills, which work great for photorealism.
[6:34] To create the tile material, I drag and drop a marble on the floor.


### Tiles material [6:37]
**Transcript (timestamped):**
[6:37] To create the tile material, I drag and drop a marble vein texture on the mesh.
[6:41] I create a new layer, increase its height and add a black mask with a checker fill.
[6:49] I do the same for the color layer.
[6:51] After adjusting the checker size and not liking the result,
[6:54] I switch to tree planner projection and tweak colors.
[6:57] I add a sharp dirt mask and some grunge leaks in the roughness layer,
[7:01] set to a low value for subtle surface wear.
[7:03] I use the same setup for interior tiles, but adjust mask contrast, marble color and tile size.
[7:12] For walls, I also use ankle points.


### Roller blinds and rug [7:16]
**Transcript (timestamped):**
[7:16] I textured the roll blinds the same way as the awning,
[7:19] starting with a fabric texture, stacking layers, changing colors and adjusting the pattern.
[7:24] For this, I use the fabric medieval flower texture.
[7:28] For the small entrance rack, I use a different fabric texture,
[7:31] then duplicate it and add a fabric diagonal layer for pattern variation.
[7:36] As a final touch, I add a mud layer, change the base color to height,
[7:40] set the blending mode to replace and paint it over the rack.
[7:43] This way, the height affects only this layer.
[7:46] I use the footprint brush, but normally you want a perfect human foot,
[7:49] so I refined with a basic brush to make it look more like a shoe print.
[7:54] And that's how I textured this Cyberpunk building.
[7:56] If you have any questions, leave them in the comments.
[7:59] Don't forget to like if you want to see more videos like this
[8:01] and subscribe to the Adobe Substance 3D channel for more in-depth project breakdowns.
[8:06] Thanks for watching!



---

## Captured Frames

- [0:14] tutorials/frames/texturing-a-cyberpunk-building-in-substance-3d-painter-project-breakdown-adobe-s/frame_000.jpg
- [0:48] tutorials/frames/texturing-a-cyberpunk-building-in-substance-3d-painter-project-breakdown-adobe-s/frame_001.jpg
- [1:39] tutorials/frames/texturing-a-cyberpunk-building-in-substance-3d-painter-project-breakdown-adobe-s/frame_002.jpg
- [3:06] tutorials/frames/texturing-a-cyberpunk-building-in-substance-3d-painter-project-breakdown-adobe-s/frame_003.jpg
- [4:10] tutorials/frames/texturing-a-cyberpunk-building-in-substance-3d-painter-project-breakdown-adobe-s/frame_004.jpg
- [5:03] tutorials/frames/texturing-a-cyberpunk-building-in-substance-3d-painter-project-breakdown-adobe-s/frame_005.jpg
- [6:41] tutorials/frames/texturing-a-cyberpunk-building-in-substance-3d-painter-project-breakdown-adobe-s/frame_006.jpg
- [7:43] tutorials/frames/texturing-a-cyberpunk-building-in-substance-3d-painter-project-breakdown-adobe-s/frame_007.jpg

---

## Structured Notes

### Core Technique
Fast-paced full-building project breakdown: every surface (brick, concrete, fabric awnings/blinds, metal, tile, rug) built from drag-and-drop base textures/smart materials plus stacked generator-driven grayscale masks (dirt, grunge, checker, tile), with a recurring anchor-point pattern (referred to as "ankle points" in the Whisper transcript — a mis-transcription of **anchor points**) linking engraved-height detail layers to downstream dirt/wear masks via Micro Height/Micro Normal.

### Summary
Adobe collaboration piece walking through texturing an entire Cyberpunk-style street-level building shopfront: layered brick walls (concrete + terracotta base, inverted/tiled brick-pattern mask, height-boosted duplicate, color-correct/color-balance saturation pass, dirt/moss generator layers, then hand-erased "fallen off" bricks with a custom brush), concrete elements (Plastic Dusty smart material re-skinned with a chosen base texture, Concrete Cast corner pieces with engraved height-channel line details referenced by anchor points into a dirt layer, finished with a cracks brush), a red/gold stacked-fabric awning pattern (duplicated masked layers blended with Oil Paint + Sharpen filters), neon signage (Emissive channel + Emissive Intensity in shader settings + viewport Glare toggle), marble-veined door/window surrounds reusing the Plastic Dusty smart material, tile flooring (checker-fill height/color layers switched to tri-planar projection when UV checker tiling looked wrong, plus Sharp Dirt and roughness grunge leaks), and a final entrance rug with a hand-painted footprint using a footprint brush refined with a basic brush for a shoe-print look. Some sub-topics (window/glass materials, AC unit texturing) are explicitly deferred to the creator's Instagram, not covered on-screen here.

### Key Steps
1. Wall base: drop a Concrete Cast texture as the base fill layer, add a Clay Terracotta layer on top.
2. New fill layer with a Brick pattern mask; invert it, adjust X/Y tile counts, and scale down until the brick read looks right.
3. Duplicate the brick layer, disable all channels except Height, and raise it slightly so bricks read with more relief.
4. On the color layer, apply **Color Correct** and **Color Balance** filters to push saturation/darken the brick color.
5. New dark-gray layer + black mask + **Dirt generator**, tuned to read as grease/smoke buildup.
6. Moss accents: drag a skin/vegetation texture, recolor it, drive placement with a **3D Linear Gradient generator** (green tint toward the base) plus a **Dripping Grass generator** for moss higher up the wall.
7. Group all wall layers into one folder; add a folder-level black mask and hand-paint to remove bricks from corners; switch to a different brush (size/angle tuned) to erase bricks one-by-one near pipes and other "logical" damage spots for a fallen-off-brick look.
8. Add a dirt layer over the whole folder, then apply a **Sharpen filter** (0.1 amount) as a final wall touch.
9. Ground/pavement: Concrete Coarse base texture; drop the **Plastic Dusty** smart material and swap its fill layer for the chosen base texture; retune its dirt/dust masks and fill colors; add a separate dirtier layer for the sidewalk look; reuse the same material on curb elements.
10. Building corners: switch base to **Concrete Cast**, duplicate + darken it, fill a black mask with a grunge texture (scale/rotation tuned) to age the surface.
11. Add a brighter-color layer masked with a **Concrete Edges** generator/mask; add a Height-only layer, lower its height value so painted strokes read as engraved (not raised) lines; paint dividing lines in 2D view to break the concrete into panels.
12. Add **anchor points** on this engraved layer, then reference them in the dirt layer by enabling **Micro Height** and **Micro Normal** in its properties — dirt now concentrates correctly along the engraved grooves; adjust dirt scale/invert as needed; finish with a **cracks brush** hand-painted on vulnerable edges/ground-adjacent areas. Same material reused on the roof.
13. Awning: drop a blue fabric texture, recolor red, duplicate + darken; add a black mask using the **Fabric Circle Half Overlap** texture as the grayscale pattern (rotation/scale/border-width tuned); stack further duplicated layers with different colors/mask tweaks to build a multi-color scalloped pattern.
14. Group the awning layers, blend them with **Oil Paint** + **Sharpen** filters; add a white layer + **Dripping Rust generator** for damage, and a dark-brown layer + **Dust Soft mask** for grime.
15. Metal details: mostly Substance 3D Library smart materials, just retuning dirt masks or swapping base textures.
16. Neon signs: enable the **Emissive** channel in Texture Set Settings on the color-filled layer, raise **Emissive Intensity** in the shader settings tab, and enable **Glare** in Display Settings for the glow; repeat per sign with different emissive colors (pink/green).
17. Entrance door/window frames: reuse the **Plastic Dusty** smart material, retune color/dirt mask; add a Height-only layer with a **Tile generator** (later swapped for a **Stripes generator**) at the top of the stack for raised trim detail; add anchor points and reference them in a dirt layer for wear around the raised details (new anchor points per object — anchor data is object-specific, not shared).
18. Small objects (AC unit etc.): same height/metallic/anchor-point/mask toolkit, plus hand-added small details like screws for realism; grunge-grayscale fills throughout for a greasy, dusty city look.
19. Tile flooring: drop a **Marble Veined** texture; new layer with raised Height + black mask filled by a **Checker** generator; duplicate the same checker approach for the color layer; when checker tiling looked wrong, switch the projection to **tri-planar** (mis-transcribed "tree planner") and retune colors; add a **Sharp Dirt** mask and grunge leaks in the roughness layer (low value) for subtle wear; same setup reused for interior tiles with adjusted contrast/color/scale, plus anchor points on the walls.
20. Rugs/blinds: roll blinds textured the same way as the awning (fabric base + stacked masked duplicates); entrance rug uses a different fabric plus a diagonal-pattern duplicate for variation; finishing touch — a mud layer with Base Color swapped for Height, blend mode set to **Replace** (so height only affects this layer), hand-painted with a **footprint brush** and refined with a basic brush for a more shoe-like print.

### Layers / Tools / Settings
- Base textures: Concrete Cast, Clay Terracotta, Concrete Coarse, Marble Veined, fabric textures
- Generators: Brick pattern, Dirt, 3D Linear Gradient, Dripping Grass, Dripping Rust, Concrete Edges, Checker, Fabric Circle Half Overlap (grayscale mask), Dust Soft mask, Sharp Dirt
- Smart materials: Plastic Dusty (reused across concrete/door/metal elements)
- Filters: Color Correct, Color Balance, Sharpen (0.1), Oil Paint
- Height-only layers for engraved/raised detail; Anchor Points + Micro Height/Micro Normal referencing (per-object, not shared)
- Brushes: custom erase brush (bricks), cracks brush, footprint brush + basic brush refinement
- Emissive channel (Texture Set Settings) + Emissive Intensity (shader settings) + Glare (Display Settings) for neon glow
- Projection: UV vs. tri-planar (switched mid-workflow for tile checker pattern)
- Blend mode: Replace (mud/footprint height-only layer)

### Difficulty
Advanced — extremely fast-paced, assumes fluency with generators, anchor points, smart materials, filters, and multi-projection masking; not a beginner step-by-step despite the creator's "possible for beginners" framing.

### App & Version
Substance 3D Painter — version **not stated on screen**; no version-gated filter/feature names (Bevel Smooth, Directional Distance, Auto-Cage, etc.) appear in transcript or captured frames, so no version floor could be pinned from this video alone.

### Tags
`layers` `fill-layer` `masks` `generator` `anchor-point` `blend-mode` `height` `basecolor` `roughness` `metallic` `emissive` `alpha` `procedural` `viewport` `advanced`

---

## Related Tutorials
- **"Complex Wooden Medieval Door Tutorial in Substance 3D Painter"** (`tutorials/complex-wooden-medieval-door-tutorial-in-substance-3d-painter.md`, video `cRKK4YOXLtQ`) — same anchor-point-driven engraved-height-to-dirt-mask pattern (Micro Height/Micro Normal referencing), applied there to a single hero door instead of a whole building.
- **"Texturing Gothic Architecture in Substance 3D Painter: Part 1"** (`tutorials/texturing-gothic-architecture-in-substance-3d-painter-part-1-adobe.md`, video `UQkmXEWJr80`) — same Adobe-official architectural-texturing genre: brick generators reused at multiple scales, dirt/moss generator stacking, anchor-point mask reuse.
- **"SUBSTANCE PAINTER: Building Masks Explained"** (`tutorials/substance-painter-building-masks-explained.md`, video `um3YRzqwYU4`) — deeper dedicated dive into the same masking-primitive toolkit (generators, tri-planar procedural breakup, anchor points) used loosely throughout this building breakdown.
- **"Creating & Reusing Smart Materials in Substance 3D Painter | Stylized Crab"** (`tutorials/creating-reusing-smart-materials-in-substance-3d-painter-stylized-crab-adobe-sub.md`, video `ZiWAe_iZ_CI`) — same Adobe-official channel; this building video reuses the built-in **Plastic Dusty** smart material across many objects the same way that video shows how to build and reuse a *custom* one.
