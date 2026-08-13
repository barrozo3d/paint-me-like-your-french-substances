---
title: Texturing Gothic Architecture in Substance 3D Painter: Part 1 | Adobe
source: YouTube
url: https://www.youtube.com/watch?v=UQkmXEWJr80
author: Adobe Substance 3D
ingested: 2026-08-12
app: "Substance 3D Painter"
version: "11.0.0+"
tags: [generator, masks, anchor-point, path-tool, height, curvature, procedural, intermediate, advanced]
extraction_status: complete
frames_dir: tutorials/frames/texturing-gothic-architecture-in-substance-3d-painter-part-1-adobe/
frame_count: 9
frame_status: complete
frame_selection: content-anchored (manual timestamps chosen from transcript, not blind percentages)
---

# Texturing Gothic Architecture in Substance 3D Painter: Part 1 | Adobe

**Source:** [YouTube](https://www.youtube.com/watch?v=UQkmXEWJr80)
**Author:** Adobe Substance 3D
**Duration:** 5m5s | 7 section(s)

---

## Raw Data (for Claude Code extraction)

Frames captured — see "Captured Frames" section below.


### Intro [0:00]
**Transcript (timestamped):**
[0:00] Hey, in today's video I'll walk you through my latest project, Agothic Hallway, and show you how I created the textures using Adobe Substance 3D Painter.
[0:08] Stick around, it's an easy and fun process.


### Base material and edge highlights [0:22]
**Transcript (timestamped):**
[0:22] I start by adding the concrete cast texture from the starter assets.
[0:27] I duplicate the layer, brighten its color, and add a black mask with a curvature generator.
[0:32] This helps highlight the edges, making them look beveled without adding extra geometry.
[0:41] I use the same texture across the whole scene, but I tweak the settings for each mesh individually.
[0:47] This way they stay consistent, but still have slight variations.
[0:50] Next, I create another layer with concrete cast, make it darker, and add a dirt grayscale through a black mask.


### Adding dirt, moss, and wear [0:52]
**Transcript (timestamped):**
[1:02] I duplicate this layer, and scale the grayscale down a bit for more depth.
[1:06] For some most details, I'll make a new layer in a brown-green tone, apply the dirt ground generator, and adjust it until I get the look that I want.
[1:20] I also add height details using the stain scratches generator, with only the height channel enabled, to make the building look older and more realistic.
[1:30] I apply this mask to the rest of the meshes, tweaking the properties slightly each time for the best results.
[1:42] Since the material still feels too clean, I add another moss layer to bring out the corners.
[1:51] For the roof tiles in the hallway corners, I use the plastic tool-worn smart material, swap its base texture for marble vane, and set the color to dark gray.
[2:03] Now it's time for some custom touches.


### Dripping details with Directional Distance Filter [2:04]
**Transcript (timestamped):**
[2:07] I create a darker layer for a dripping effect, painting just under the roof tiles, and with the directional distance filter, I control the length and smudge of the drips.
[2:16] I also add more paint or remove it by clicking the X button, and repeat this process for the lower sections of the mesh.
[2:30] I haven't textured the roof and floor yet, so I quickly do that before moving back to the walls.


### Brick patterns [2:36]
**Transcript (timestamped):**
[2:36] For the brick effect, I create a new layer, enable only the height channel, lower its value, and apply the brick generator.
[2:46] After increasing the tiling and tweaking the pattern, I paint out unwanted areas.
[2:54] I apply the same brick pattern to the ground with a dirt mask linked via anchor points, adjusting grunge and ambient occlusion for a subtle realistic look.
[3:08] I reuse it across the scene, since it emphasizes the height details nicely.
[3:15] I apply the same brick pattern to the columns, but this time I scale it up significantly to make them look like they're divided into three smaller segments.


### Decorative elements with Path Tool [3:22]
**Transcript (timestamped):**
[3:23] Now I move on to the entrance arches. I create a new layer with the height channel enabled and add a black mask.
[3:29] Using the path tool from the left menu, I choose a pattern I like, and with Symmetry turned on, start drawing a curve directly on the mesh.
[3:38] At the top of the screen, I adjust settings like size and spacing.
[3:42] I can also modify the curve itself, by clicking or adding new vertices.
[3:50] In this case, I choose one of the keld crosses and lower the spacing to bring the crosses closer together.
[3:56] Then I grab the curve and pull it all the way down to the ground.
[4:00] With the same method, I add other patterns to the walls, keeping in mind that I can adjust them at any moment, which is very convenient and saves a lot of time.
[4:31] For one of the floral patterns, I also add a bevel smooth filter to make the edges look softer.
[4:37] And that's it! This is the texturing process I use for the Gothic hallway. I hope you found it helpful.


### Outro [4:41]
**Transcript (timestamped):**
[4:43] In the next video, I'll show you how I completed the hallway with details like stained glass that bring it to life.
[4:49] Don't forget to subscribe so you don't miss it. Thanks for watching and see you soon!
[5:00] you



---

## Captured Frames

- [0:22] tutorials/frames/texturing-gothic-architecture-in-substance-3d-painter-part-1-adobe/frame_000.jpg
- [0:52] tutorials/frames/texturing-gothic-architecture-in-substance-3d-painter-part-1-adobe/frame_001.jpg
- [1:20] tutorials/frames/texturing-gothic-architecture-in-substance-3d-painter-part-1-adobe/frame_002.jpg
- [1:51] tutorials/frames/texturing-gothic-architecture-in-substance-3d-painter-part-1-adobe/frame_003.jpg
- [2:07] tutorials/frames/texturing-gothic-architecture-in-substance-3d-painter-part-1-adobe/frame_004.jpg
- [2:36] tutorials/frames/texturing-gothic-architecture-in-substance-3d-painter-part-1-adobe/frame_005.jpg
- [3:15] tutorials/frames/texturing-gothic-architecture-in-substance-3d-painter-part-1-adobe/frame_006.jpg
- [3:29] tutorials/frames/texturing-gothic-architecture-in-substance-3d-painter-part-1-adobe/frame_007.jpg
- [4:31] tutorials/frames/texturing-gothic-architecture-in-substance-3d-painter-part-1-adobe/frame_008.jpg

---

## Structured Notes

### Core Technique
Layered architectural weathering on a Gothic hallway: a Concrete Cast base with Curvature-driven fake-bevel edge highlights, stacked Dirt/Moss generator layers, a Height-only Brick generator reused at different scales (walls/floor/columns), hand-painted drip stains refined with the **Directional Distance filter**, and Path-tool-drawn decorative relief patterns (Gothic crosses, floral motifs) finished with a **Bevel Smooth filter**.

### Summary
Part 1 of Adobe's official two-part Gothic Architecture series (Part 2, "Texturing Stained Glass & Ceiling Paintings," `NCkQ1eq8a-o`, is already in this library — that video explicitly recaps this one's base texture as its starting point). Covers the full stonework pass: a reusable Concrete Cast base material (duplicated with a Curvature-generator mask for fake bevels, applied scene-wide with per-mesh tweaks for consistent-but-varied results), several stacked Dirt/Moss/Stains-Scratches generator layers for aging, a distinct smart-material swap for the roof tiles (Plastic Tool-Worn with its base texture swapped to Marble Vane), custom hand-painted drip stains shaped with the Directional Distance filter, a Height-only Brick generator pattern reused at three different scales (walls, ground — linked via anchor points to a dirt/AO mask, and columns scaled up to imply sub-segments), and Path-tool-drawn decorative relief (Gothic quatrefoil "keld crosses" and floral patterns) on the entrance arches and walls, finished with a Bevel Smooth filter for softer edges.

### Key Steps
1. Base material: add the **Concrete Cast** starter-asset texture as the base fill layer.
2. Duplicate it, brighten the duplicate's color, add a black mask driven by a **Curvature generator** — highlights edges to fake a beveled look without adding geometry.
3. Reuse this same base texture across the whole scene, but tweak settings per-mesh individually — keeps everything visually consistent while still reading as slightly varied.
4. Add another Concrete Cast layer, darkened, masked by a **Dirt** grayscale generator (black mask) for grime buildup.
5. Duplicate that dirt layer and scale its grayscale mask down for extra depth/variation.
6. New brown-green-toned layer using the **Dirt Ground** generator, tuned to taste, for moss.
7. Add height-only aging detail via the **Stains/Scratches generator** (only the Height channel enabled) — applied to the rest of the meshes with small per-mesh tweaks each time.
8. Add a second, separate moss layer specifically to emphasize corners, since the base material still read "too clean."
9. Roof tiles (hallway corners): reuse the **Plastic Tool-Worn** smart material, but swap its base texture input for **Marble Vane** and recolor it dark gray.
10. Custom dripping stains: new darker layer, hand-paint just under the roof tiles, then apply a **Directional Distance filter** to control drip length and smudge; add/remove paint via the `X` toggle; repeat the same process on the lower wall sections.
11. Texture the roof and floor (not shown in detail) before returning to the walls — a deliberate workflow-ordering choice.
12. Brick pattern: new layer, Height channel only, value lowered, apply the **Brick generator**; increase tiling and tune the pattern, then manually paint out unwanted brick areas.
13. Reuse the same brick pattern on the ground, this time masked with a dirt/ambient-occlusion combination **linked via Anchor Points**, adjusting grunge/AO for a subtle, realistic look; reused broadly across the scene since it "emphasizes the height details nicely."
14. Apply the same brick pattern to the columns, but scaled up significantly so each column visually reads as divided into three smaller segments.
15. Entrance arches: new layer, Height channel enabled, black mask added; select the **Path tool** from the left toolbar, choose a decorative curve preset, enable **Symmetry**, and draw directly on the mesh.
16. Adjust **Size** and **Spacing** at the top toolbar; reshape the curve afterward by clicking to add/move vertices.
17. Choose one of the "keld cross" (Gothic quatrefoil) presets and lower Spacing to bring the repeated crosses closer together; grab the curve and drag it all the way down the arch.
18. Repeat the same method with other decorative patterns on the walls — emphasized as a major time-saver since curves stay fully editable after the fact.
19. For one of the floral patterns, add a **Bevel Smooth filter** to soften its edges.

### Layers / Tools / Settings
- Concrete Cast texture, Curvature generator, Dirt generator, Dirt Ground generator, Stains/Scratches generator (Height channel only)
- Plastic Tool-Worn smart material (base texture swapped to Marble Vane)
- Directional Distance filter, `X` (paint/erase toggle)
- Brick generator (Tiling)
- Anchor Points (dirt/AO mask linking/reuse)
- Path tool (curve presets, Symmetry, Size, Spacing, vertex editing)
- Bevel Smooth filter

### Difficulty
Intermediate to Advanced — mostly generator/mask layering (accessible), with Path-tool decorative work and anchor-point mask reuse pushing into more advanced territory.

### App & Version
**Substance 3D Painter 11.0.0+** — this video uses both the **Directional Distance filter** (step 10) and the **Bevel Smooth filter** (step 19), and `references/release-notes-painter-11.0.md` lists both by name as new in 11.0.0 ("6 new filters: stylization, quantize, anisotropic Kuwahara, bevel smooth, directional distance, grayscale conversion"). Two independent filter confirmations in one video — a strong, unambiguous version floor. Exact build not shown on screen.

### Tags
`generator` `masks` `anchor-point` `path-tool` `height` `curvature` `procedural` `intermediate` `advanced`

---

## Related Tutorials
- **"Texturing Stained Glass & Ceiling Paintings in Adobe Substance 3D Painter: Part 2"** (`tutorials/texturing-stained-glass-ceiling-paintings-in-adobe-substance-3d-painter-part-2-a.md`, video `NCkQ1eq8a-o`) — direct continuation of this video on the same Gothic-hallway asset; Part 2 explicitly recaps this video's Concrete Cast/Scratches/Dirt/Moss base ("You may have seen it in part 1") before building stained-glass windows and a fresco ceiling on top of it. Read Part 1 (this file) before Part 2 for the full picture.
- **"New Ribbon Paths in Substance 3D Painter"** (`tutorials/new-ribbon-paths-in-substance-3d-painter-adobe-substance-3d.md`) — same Path-tool feature family (`path-tool` tag) used here for the decorative crosses/floral relief; that video covers the Path/Ribbon tool in much greater depth (presets, corner modes, custom start/end/corner images).
- **"Texturing a Cyberpunk Building in Substance 3D Painter – Project Breakdown"** (`tutorials/texturing-a-cyberpunk-building-in-substance-3d-painter-project-breakdown-adobe-s.md`, video `gv9R6a6VPYQ`) — same Adobe-official architectural-texturing genre: brick generators reused at multiple scales, dirt/moss generator stacking, anchor-point mask reuse, applied there to a whole cyberpunk-street building instead of a Gothic hallway.
- **"6 Powerful New Filters in Substance 3D Painter"** (`tutorials/6-powerful-new-filters-in-substance-3d-painter-adobe-substance-3d.md`, video `aCi0RG9-9so`) — the official Adobe feature-tour video for Directional Distance and Bevel Smooth, both used here (dripping stains under roof tiles; softened decorative relief), and the primary source for this video's 11.0.0 version pin.
- **"New Path Tool Features & Improvements in Substance 3D Painter"** (`tutorials/new-path-tool-features-improvements-in-substance-3d-painter-adobe-substance-3d.md`, video `exE0-1ftNeE`) — explains the underlying Filled Path/snapping mechanics behind the decorative-relief technique used here.
