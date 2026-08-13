---
title: Texturing a Cyberpunk Building in Substance 3D Painter – Project Breakdown | Adobe Substance 3D
source: YouTube
url: https://www.youtube.com/watch?v=gv9R6a6VPYQ
author: Adobe Substance 3D
ingested: 2026-08-13
app: "[PENDING]"
version: "[PENDING]"
tags: []
extraction_status: pending
frames_dir: tutorials/frames/texturing-a-cyberpunk-building-in-substance-3d-painter-project-breakdown-adobe-s/
frame_count: 0
frame_status: pending-selection
---

# Texturing a Cyberpunk Building in Substance 3D Painter – Project Breakdown | Adobe Substance 3D

**Source:** [YouTube](https://www.youtube.com/watch?v=gv9R6a6VPYQ)
**Author:** Adobe Substance 3D
**Duration:** 8m11s | 10 section(s)

---

## Raw Data (for Claude Code extraction)

Frames are not captured yet. Read the timestamped transcript below, pick moments
that actually show a technique/result worth a still (not blind percentages —
even within a named chapter, verify the real moment against its timestamps), then run:
  python select_frames.py texturing-a-cyberpunk-building-in-substance-3d-painter-project-breakdown-adobe-s <ts1> <ts2> ...
(seconds or mm:ss). This appends a "Captured Frames" section and updates the
frontmatter before you write the Structured Notes below.


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
