---
title: Texturing Stained Glass & Ceiling Paintings in Adobe Substance 3D Painter: Part 2 | Adobe
source: YouTube
url: https://www.youtube.com/watch?v=NCkQ1eq8a-o
author: Adobe Substance 3D
ingested: 2026-08-12
app: "Substance 3D Painter"
version: "not confirmed on-screen; published ~August 2025, likely 11.x/12.0.x era (approximate)"
tags: [generator, masks, anchor-point, opacity, roughness, metallic, height, normal-map, path-tool, procedural, advanced]
extraction_status: complete
frames_dir: tutorials/frames/texturing-stained-glass-ceiling-paintings-in-adobe-substance-3d-painter-part-2-a/
frame_count: 8
frame_status: complete
frame_selection: content-anchored (manual timestamps chosen from transcript, not blind percentages)
---

# Texturing Stained Glass & Ceiling Paintings in Adobe Substance 3D Painter: Part 2 | Adobe

**Source:** [YouTube](https://www.youtube.com/watch?v=NCkQ1eq8a-o)
**Author:** Adobe Substance 3D
**Duration:** 5m2s | 8 section(s)

---

## Raw Data (for Claude Code extraction)

Frames captured — see "Captured Frames" section below.


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

## Captured Frames

- [0:24] tutorials/frames/texturing-stained-glass-ceiling-paintings-in-adobe-substance-3d-painter-part-2-a/frame_000.jpg
- [0:50] tutorials/frames/texturing-stained-glass-ceiling-paintings-in-adobe-substance-3d-painter-part-2-a/frame_001.jpg
- [1:11] tutorials/frames/texturing-stained-glass-ceiling-paintings-in-adobe-substance-3d-painter-part-2-a/frame_002.jpg
- [1:42] tutorials/frames/texturing-stained-glass-ceiling-paintings-in-adobe-substance-3d-painter-part-2-a/frame_003.jpg
- [2:33] tutorials/frames/texturing-stained-glass-ceiling-paintings-in-adobe-substance-3d-painter-part-2-a/frame_004.jpg
- [2:56] tutorials/frames/texturing-stained-glass-ceiling-paintings-in-adobe-substance-3d-painter-part-2-a/frame_005.jpg
- [3:33] tutorials/frames/texturing-stained-glass-ceiling-paintings-in-adobe-substance-3d-painter-part-2-a/frame_006.jpg
- [4:05] tutorials/frames/texturing-stained-glass-ceiling-paintings-in-adobe-substance-3d-painter-part-2-a/frame_007.jpg

---

## Structured Notes

### Core Technique
Building Gothic stained-glass windows entirely in texture (Path-tool curves, exported masks driving multi-color glass panes, a Tile-generator wireframe lattice) and a peeling, moss-flecked fresco ceiling painting (imported Stock artwork + Peeling Paint filter + Ambient Occlusion filter for depth).

### Summary
Part 2 of Adobe's official two-part Gothic Architecture series (Part 1: "Texturing Gothic Architecture in Substance 3D Painter" `UQkmXEWJr80`, also in this skill's library). Covers two independent builds on the same cathedral asset: (1) stained-glass windows — window-frame detail drawn purely with the Path tool and Symmetry, Bevel-generated anchor points used to localize dirt, a glass base layer whose Opacity is driven entirely by an *exported mask* from the frame-curves layer, a Tile-generator "wireframe" lattice built from a Polygon-generator anchor point used as the tile's Custom Image Input, and multiple duplicated glass-color layers (red/blue/green) each masked by an exported luminance mask with different Levels so the colors don't overlap; and (2) a fresco ceiling painting — an Adobe Stock image UV-projected onto the ceiling mesh, aged with the Peeling Paint filter (tuned conservatively so the artwork stays legible) plus an Ambient Occlusion filter to fake depth at the peeled edges, finished with subtle mold/fade grunge passes.

### Key Steps
**Stained-glass windows:**
1. Finish window-frame detail purely in height (no added geometry): new fill layer, draw curves directly on the mesh with the Path tool; move vertices freely (precision isn't critical up front); enable Symmetry and correct its center offset so curves mirror properly; add more curves toward the window's center/lower section. Apply a Metal Sandblasted texture to this layer.
2. Apply a Bevel filter to smooth the curve edges — this simultaneously generates Anchor Points reused later.
3. New dark-gray fill layer with a Dirt generator; enable Micro Height and Micro Normal, and reference the anchor points from step 2 so dirt only collects around the curve grooves.
4. Build the glass base layer: enable the Opacity channel, set Roughness very low, color dark gray.
5. Right-click the frame-curves layer → **Export mask**, then apply that exported mask to the glass layer's Opacity — this makes everything transparent except the curved frame details; fine-tune opacity so the glass still reads as reflective, not fully see-through.
6. With the Path tool again, draw decorative medieval crosses (a classic Gothic motif) onto a new layer filled with a Polygon grayscale generator; add another anchor point from this.
7. New layer filled with a Tile generator, Pattern Type set to **Custom Image Input**, feeding in the polygon anchor points so every tile cell is filled with a polygon shape — this builds a wireframe-lattice look. Tune tiling size (for both the tile grid and the polygon texture) and Offset X/Y, and increase the polygon's **Explode** value to thicken the vertical/horizontal lines.
8. In the Tile generator's Color tab, set **Luminance Random** to maximum, then export this mask the same way as step 5, for reuse as a color-variation driver.
9. Return to the wireframe layer: drag in the Metal Sandblasted texture again to match the frame, add height information to both this layer and the crosses layer, and increase Polygon Tiling further to thin the wireframe lines.
10. Duplicate the glass layer, set its base color dark red, add a black mask filled with the exported luminance mask from step 8, and adjust Levels to control color intensity/spread. Duplicate again for blue, then green — each with slightly different Levels so the three colors don't overlap.
11. Add one more gray fill layer on top with Roughness and Metallic channels enabled, unifying the glass panes' surface response.
12. Apply a grunge-style grayscale texture layer for realistic glass streaks; repeat with a green-tinted, different grunge variant for a mossy/moldy look — this completes the windows.

**Fresco ceiling painting:**
13. Recap of the Part-1 ceiling base: a main Concrete Cast texture, a Scratches generator, two Dirt variants (large + small), and two Moss variants concentrated near the edges — moss toned down and brightened so it isn't overpowering indoors.
14. Import a ceiling-painting image (sourced from Adobe Stock), drag it onto the mesh, move the layer just above the base texture in the stack, switch its **Projection to UV**, adjust size/position in both 2D and 3D views, and set **UV Wrap to Repeat**.
15. Add a **Peeling Paint filter**: first adjust its Technical Parameters (recolor, lower the Height Range), then in the main settings tune **Peeling Level** and **Flaking**, keeping values moderate so the underlying painting stays readable.
16. Add an **Ambient Occlusion filter** above the painting layer to fake a subtle shadow/gap between the peeled paint and the concrete underneath.
17. Add a greenish grunge-map layer above (scaled down, low opacity) for subtle simulated mold, plus a separate white layer using an "undergrunge" map to fade select areas without adding more peeling.
18. Finish by darkening the base concrete-cast texture underneath so it reads more clearly through the peeled-paint gaps.

### Layers / Tools / Settings
- Path tool (curves, freely-editable vertices), Symmetry
- Bevel filter → Anchor Points
- Dirt generator (Micro Height, Micro Normal), anchor-point-driven masking
- Opacity channel, exported layer masks (right-click → Export mask)
- Polygon grayscale generator, Tile generator (Pattern Type: Custom Image Input, tiling size, Offset X/Y, Explode)
- Luminance Random (Color tab), Levels adjustment
- Roughness, Metallic channels
- Concrete Cast texture, Scratches generator, Moss generator
- UV projection, UV Wrap: Repeat
- Peeling Paint filter (Technical Parameters: Height Range; main: Peeling Level, Flaking)
- Ambient Occlusion filter, grunge/"undergrunge" maps

### Difficulty
Advanced — heavy chaining of generators, anchor points, and exported/re-imported masks across many dependent layers.

### App & Version
Not confirmed from an on-screen version watermark in the captured frames (this video's UI theme doesn't show the small corner build-string other Adobe Substance3D videos in this batch display). Per external metadata this is Part 2 of Adobe's official Gothic Architecture series, published on the Adobe Substance 3D YouTube channel in August 2025 — consistent with the Painter 11.x/12.0.x era, but not independently verified against `references/version-tracker.md` from in-video evidence. Treat the version as approximate.

### Tags
`generator` `masks` `anchor-point` `opacity` `roughness` `metallic` `height` `normal-map` `path-tool` `procedural` `advanced`

---

## Related Tutorials
- **"Texturing Gothic Architecture in Substance 3D Painter: Part 1"** (`tutorials/texturing-gothic-architecture-in-substance-3d-painter-part-1-adobe.md`, video `UQkmXEWJr80`, same Adobe series, same cathedral/hallway asset) — Part 1 builds the base stonework (Concrete Cast base, Curvature-driven fake bevels, Dirt/Moss/Stains-Scratches aging, Brick generator at three scales, Path-tool decorative relief) that this Part 2 video explicitly recaps and builds on top of for the stained glass and ceiling fresco.
