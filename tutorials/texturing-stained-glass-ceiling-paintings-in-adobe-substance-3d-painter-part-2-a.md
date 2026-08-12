---
title: Texturing Stained Glass & Ceiling Paintings in Adobe Substance 3D Painter: Part 2 | Adobe
source: YouTube
url: https://www.youtube.com/watch?v=NCkQ1eq8a-o
author: Adobe Substance 3D
ingested: 2026-08-12
app: "[PENDING]"
version: "[PENDING]"
tags: []
extraction_status: pending
frames_dir: tutorials/frames/texturing-stained-glass-ceiling-paintings-in-adobe-substance-3d-painter-part-2-a/
frame_count: 0
frame_status: pending-selection
---

# Texturing Stained Glass & Ceiling Paintings in Adobe Substance 3D Painter: Part 2 | Adobe

**Source:** [YouTube](https://www.youtube.com/watch?v=NCkQ1eq8a-o)
**Author:** Adobe Substance 3D
**Duration:** 5m2s | 8 section(s)

---

## Raw Data (for Claude Code extraction)

Frames are not captured yet. Read the timestamped transcript below, pick moments
that actually show a technique/result worth a still (not blind percentages —
even within a named chapter, verify the real moment against its timestamps), then run:
  python select_frames.py texturing-stained-glass-ceiling-paintings-in-adobe-substance-3d-painter-part-2-a <ts1> <ts2> ...
(seconds or mm:ss). This appends a "Captured Frames" section and updates the
frontmatter before you write the Structured Notes below.


### Intro [0:00]
**Transcript (timestamped):**
[0:00] Hey, welcome back to the second part of texturing Gothic architecture in Adobe Substance 3D Painter.
[0:05] Today I'll show you how I create textures for Gothic windows with colorful stained glass using generators and masks
[0:11] and an old worn fresco ceiling using the peeling paint filter. Let's dive in!


### Windows – Frame & Curves [0:18]
**Transcript (timestamped):**
[0:18] I start by finishing the window frame. Instead of adding extra geometry, I create the details using height information in the texture.
[0:24] I make a new fill layer and, with the path tool, draw curves directly on the mesh.
[0:29] I can move vertices at any time so I don't worry about perfect precision.
[0:33] I also enable symmetry and adjust its position, since the center is slightly off, to make sure all curves mirror correctly.
[0:39] I keep adding more curves to the center and lower part of the window for extra detail.
[0:46] For this layer, I use the metal sandblasted texture.


### Adding Dirt Around Details [0:50]
**Transcript (timestamped):**
[0:50] Once done, I apply a bevel filter to smooth the edges and create anchor points I will use later.
[0:56] Next, I create a new dark gray fill layer with a dirt generator.
[1:01] I enable micro height and micro normal and use the anchor points from before, so the dirt appears only around the curves of the drone.
[1:11] Then I create the glass. I add and enable the opacity channel, set roughness very low and color it dark gray.


### Glass Layer [1:12]
**Transcript (timestamped):**
[1:18] I right click the curves layer, export its mask and apply it to the glass layer's opacity.
[1:23] This makes everything transparent, except the curved details.
[1:26] I also tweak the opacity levels so the glass isn't fully transparent but still reflective.
[1:31] Using the path tool again, I add the creative medieval crosses, a classic motif and gothic architecture.
[1:39] I create a new layer and fill it with a polygon gray scale.


### Decorative Crosses & Wireframe Effect [1:40]
**Transcript (timestamped):**
[1:42] Then I add an anchor points that I will use later and fill the layer again, this time with a tile generator.
[1:48] In the properties, I set the pattern type to custom image input and select the polygon anchor points.
[1:54] This way all the tiles are filled with polygons inside.
[1:57] I play with the tiling size, both for the tile and polygon texture and tweak the position values such as offset, X and Y amounts to create a wireframe like mask.
[2:10] I also adjust the explode value for the polygon texture to make the vertical and horizontal lines thicker.
[2:15] In the color tab, I set the luminance random value to maximum and export the mask just like last time.
[2:20] I hide this layer, return to my wireframe mask, drag in the metal sandblast texture again so it matches the other details and add height information to both this and the previous layer.
[2:30] I also increase the polygontiling so the wireframe is thinner.
[2:33] I duplicate the glass layer and set its base color to dark red.


### Adding Stained Glass Colors [2:34]
**Transcript (timestamped):**
[2:37] I add the black mask and fill it with the luminance mask from before, adjusting levels to control color intensity.
[2:43] I duplicate the layer for blue glass, then again for green, making sure it has slightly different level values so they don't overlap each other.
[2:51] On top of all of these, I add a gray colored layer with roughness and metallic channels enabled.


### Leaks & Moss [2:52]
**Transcript (timestamped):**
[2:56] Now, I apply a grunge-like gray-skill texture to add realistic glass streaks.
[3:00] I repeat the process using green coloring and a different variant of the grunge-like texture to give the glass a mossy, moldy look as a final touch.
[3:08] And with that, the windows are done.
[3:10] Now we move on to creating fresco paintings for the ceilings.


### Fresco Ceiling [3:11]
**Transcript (timestamped):**
[3:13] I already have the base texture applied.
[3:15] You may have seen it in part 1, but for those who haven't, here's a quick breakdown.
[3:19] I use a main concrete cast texture, a scratcher's generator, two variants of dirt large and small, and two variants of moss concentrated around the edges.
[3:28] I tone down the moss generator and brighten its colors since I don't want too much of it inside the building.
[3:33] Next, I import the ceiling painting image from Adobe Stock that I think fits the model perfectly and drag it onto the mesh.
[3:39] I move the layer to the bottom, just above the base texture, and change its projection to UV.
[3:44] I work in both 3D and 2D view to manually adjust its size and position until I'm happy with it and set the UV wrap to repeat.
[3:52] Now, I add the peeling paint filter.
[3:55] First, I adjust the technical parameters, changing colors and lowering height range, then, back in the main settings, I tweak the peeling level and flaking values until I like the result.
[4:06] I keep the values moderate so the painting remains visible and readable.
[4:10] To add depth, I place an ambient occlusion filter above the painting layer, creating subtle shadows in the peeled areas, making it look like there's a slight gap between the paint and the concrete.
[4:21] On top of this, I add a greenish layer filled with a grunge map to simulate mold.
[4:26] I scale it down and lower its opacity so it stays subtle.
[4:29] I also create a white layer with an undergrunge map to make certain areas look faded without adding more peeling.
[4:35] With all the layers combined, I finally darken the concrete cast-based texture so it's more visible through the peeled paint.
[4:41] And that's the final result.
[4:43] I hope you enjoyed this video and learned something new.
[4:45] If you missed the first part of my texturing process, make sure to check it out and don't forget to subscribe to Adobe Substance3D's YouTube channel so you don't miss more breakdowns like this.
[4:54] Thank you for watching!



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
