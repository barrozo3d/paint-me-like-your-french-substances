---
title: New Ribbon Paths in Substance 3D Painter | Adobe Substance 3D
source: YouTube
url: https://www.youtube.com/watch?v=3zgD-wwANCs
author: Adobe Substance 3D
ingested: 2026-08-12
app: "Substance 3D Painter"
version: "11.1.0 (feature origin, stated on-screen); filmed on a later build (~12.0.0, tentative from viewport watermark)"
tags: [path-tool, alpha, opacity, roughness, metallic, height, basecolor, intermediate, advanced]
extraction_status: complete
frames_dir: tutorials/frames/new-ribbon-paths-in-substance-3d-painter-adobe-substance-3d/
frame_count: 8
frame_status: complete
frame_selection: content-anchored (manual timestamps chosen from transcript, not blind percentages)
---

# New Ribbon Paths in Substance 3D Painter | Adobe Substance 3D

**Source:** [YouTube](https://www.youtube.com/watch?v=3zgD-wwANCs)
**Author:** Adobe Substance 3D
**Duration:** 7m13s | 13 section(s)

---

## Raw Data (for Claude Code extraction)

Frames captured — see "Captured Frames" section below.


### <Untitled Chapter 1> [0:00]
**Transcript (timestamped):**
[0:00] Substance Painter 11.1 now has ribbon paths, a new advanced way to work with familiar path tools.
[0:07] So how ribbons different from the regular paint along path? Like the name suggests, paint along path repeats a brush stamp along a path.
[0:16] So it's not ideal if you want a continuous bending and repeating shapes as it overlaps its stamps.
[0:22] Ribbon paths solve that problem. They transform and repeat a texture along a path shape


### Intro [0:27]
**Transcript (timestamped):**
[0:28] with extra control for the start and end as well as options for sharp corners.
[0:33] That means it's possible to do things like transform text along paths, have a perfect gradient along a path
[0:40] and it easily lets you create your own advanced trims to wrap around a mesh.
[0:44] In short, the ribbon is the perfect tool for more precise texturing with paths.
[0:49] In this video, we will explore using these new ribbon paths.
[0:53] We look at the new presets for paths, explore the core settings for creating your own ribbon paths
[0:58] and then get into the custom ribbon tool, which is a shortcut to creating complex ribbon setups quickly.


### Vertex Stroke Width/Opacity [1:04]
**Transcript (timestamped):**
[1:04] Before we go any further, I want to point out an important change in path settings.
[1:08] All path tools, including ribbon, now split the older pressure value for each vertex into two separate controls.
[1:16] Vertex stroke width and vertex opacity, letting you control width and opacity separately instead of tying them together.
[1:23] Alright, let's start using ribbon paths.


### Empty Layer/Mask [1:24]
**Transcript (timestamped):**
[1:26] Like paint along paths, you can use them in two areas, directly in an empty paintable layer or in a mask.
[1:32] In an empty layer, you create full material data. In a mask, you only work with grayscale values.
[1:38] Once you create an empty layer mask and select the path tool, you'll see the new path presets at the top of the path properties.
[1:45] These presets are the quickest way to start creating with paths and offer a new way to quickly apply various path settings.
[1:52] The first category, Favorites, is empty.


### Favourite Paths [1:53]
**Transcript (timestamped):**
[1:55] But you can easily add your own by right clicking an existing preset or asset and picking Add to Favorites.
[2:01] You can also tell if they are ribbon or paint paths by their icon.
[2:05] Let's look at some examples.
[2:07] Smooth gradients are impossible with a regular paint along path, but with ribbons, this is now easy.


### Gradients [2:08]
**Transcript (timestamped):**
[2:13] Gradients come in a few presets, from repeating grayscale gradients to tricolor full material.
[2:18] Just like with regular brushes, make sure to keep in mind what part of the ribbon you work on.
[2:23] With this full material gradient, I make sure the alpha is set up correctly before I move to tweak the material settings.
[2:30] If you work in a mask, the material settings turn into a simple grayscale value.
[2:35] Just like with other paths, ribbon paths have a width and projection depth you probably want to tweak.
[2:40] You'll also want to make sure to add enough points on your path to conform to the surface as well as possible.


### Text Along Paths [2:46]
**Transcript (timestamped):**
[2:46] Another new possibility with ribbon paths is placing text along paths.
[2:51] There are some handy presets available for this that mainly preset text alignment and repetition.
[2:57] Pick whatever is closest to your intentions and adjust afterwards.
[3:01] The main thing to be mindful of is that your text needs to fit within the stroke the ribbon path places.
[3:06] Playing with the advanced section of the text parameters can help solve any alignment trickiness.
[3:12] The apparel section is another interesting category.


### Apparel Presets [3:13]
**Transcript (timestamped):**
[3:15] Building on the familiar stitches, these new and improved versions take the classics and expand them with new and improved stitches, seams and zippers.
[3:24] Big changes are that you can now make much sharper corners with stitches and that all of these presets nicely terminate with realistic start and end shapes, rather than just fade in and out.


### Hardsurface Details [3:34]
**Transcript (timestamped):**
[3:34] Finally, a worthwhile category is the hard surface one.
[3:38] Stacked with grip patterns, shut lines, tape and welding seams.
[3:42] A trick I'm doing here is to use the snap to mesh wireframe option and then clicking on a revertix.
[3:48] If you shift click, the created point is a sharp corner.
[3:52] Adding smooth tangents after that helps avoid some of the strange bends the path tool can make in these cases.
[3:58] If you want to move beyond the presets, let's look at making our own basic ribbon.


### Make A Basic Ribbon [3:59]
**Transcript (timestamped):**
[4:03] Pick the basic hard ribbon preset to start from a clean base and draw some initial paths to get started.
[4:09] Moving down through the settings, first you get the familiar path type, letting you switch this path between paint, ribbon, filled, erase and smudge at any time.
[4:19] The projection depth is below it and should be adjusted on a case by case basis, but keep in mind that adding more points is usually a good idea.
[4:26] Below that is the self-explanatory ribbon width and opacity.
[4:30] Before we get to the more unique settings, to use those, let's swap the alpha for something easier to read and understand.
[4:37] We'll use arrow, fire.
[4:39] Under stroke, you can then change the image orientation to better align your image to the path.
[4:45] If you set one of your vertices to sharp corner, you can test the corner modes, ranging from miter, round, bevel to cut joint.
[4:53] With cut, you can see something interesting.
[4:55] The arrows are trying to scale the whole images, never cutting off and trying to place the best amount along the path.
[5:01] This behavior is set by the stretching and tiling parameters.
[5:05] If scale mode is set to stretch and tiling to auto, they work together and try to place the amount of strokes with the least stretching.
[5:13] Changing any of these modifies and breaks that behavior.
[5:16] Let's turn on stretch between offsets only and set the tiling to custom.
[5:21] What happens now is that the first 25% of a stroke is not stretched, as well as the part past 75%.
[5:28] This stretches the inside of the arrow, but not the ends.
[5:32] Tiling mode none only starts a new stroke between sharp corners.
[5:36] There are a few more modifiers for specific behaviors, but we won't get into every detail with this video.
[5:42] Play around with them or refer to the documentation.
[5:46] What we do still want to cover is probably the most important presets.
[5:52] Custom ribbon grayscale and material.
[5:55] We mentioned before that ribbons have special support for different start and end stamps, so it'll have special stamps for sharp corners.
[6:02] These are normally only accessible through special substance files created in Substance 3D Designer,
[6:08] but we've wrapped the majority of those behaviors into these two custom ribbon presets.


### Grayscale Vs. Material [6:12]
**Transcript (timestamped):**
[6:12] The difference between the two is that the grayscale version is meant for use with simple grayscale alpha stamps,
[6:18] and only lets you paint solid color materials.
[6:21] While the material version lets you use full color images for base color,
[6:25] and has controls for roughness, metallic, and height as uniform values.


### Customize Start/End [6:29]
**Transcript (timestamped):**
[6:29] When you use them, you can always set a start, middle, and end image, along with controlling some aspects of it.
[6:37] If you turn on custom corners, you can set two additional images for a left and right sharp corner.
[6:43] These corners then get warped to match the exact angle of sharp corner you drew.
[6:48] You can build some pretty complex trim ribbons with these tools,


### Adobe Illustrator Artboards [6:49]
**Transcript (timestamped):**
[6:51] but here we've replicated one of the pattern brushes from Illustrator, using artboards straight out of Illustrator.
[6:57] You can even use the artboard functionality to pick what artboard from the source AI file to use in which context.
[7:04] So, as you can see, there's a lot possible with these new ribbon paths.
[7:08] We're excited to see what you come up with.
[7:10] Have fun!



---

## Captured Frames

- [1:38] tutorials/frames/new-ribbon-paths-in-substance-3d-painter-adobe-substance-3d/frame_000.jpg
- [2:13] tutorials/frames/new-ribbon-paths-in-substance-3d-painter-adobe-substance-3d/frame_001.jpg
- [2:46] tutorials/frames/new-ribbon-paths-in-substance-3d-painter-adobe-substance-3d/frame_002.jpg
- [3:15] tutorials/frames/new-ribbon-paths-in-substance-3d-painter-adobe-substance-3d/frame_003.jpg
- [3:38] tutorials/frames/new-ribbon-paths-in-substance-3d-painter-adobe-substance-3d/frame_004.jpg
- [4:03] tutorials/frames/new-ribbon-paths-in-substance-3d-painter-adobe-substance-3d/frame_005.jpg
- [4:53] tutorials/frames/new-ribbon-paths-in-substance-3d-painter-adobe-substance-3d/frame_006.jpg
- [6:29] tutorials/frames/new-ribbon-paths-in-substance-3d-painter-adobe-substance-3d/frame_007.jpg

---

## Structured Notes

### Core Technique
**Ribbon Paths** — a new path-tool mode (introduced Substance 3D Painter 11.1.0) that continuously transforms and repeats a texture along a path shape instead of stamping a brush along it, with dedicated presets for gradients, text, apparel, hard-surface trims, and a from-scratch **Custom Ribbon** workflow for building complex modular trims without needing Substance 3D Designer.

### Summary
Official Adobe overview explaining why Ribbon exists (regular Paint along Path repeats/overlaps brush stamps around curves — bad for continuous shapes like gradients or text; Ribbon transforms the texture itself along the path instead) and touring its features: an important underlying change where per-vertex Pressure is now split into separate Vertex Stroke Width and Vertex Opacity controls, a new Path Presets bar (Favorites/Gradients/Text/Apparel/Hard Surface categories) usable in either an empty paintable layer (full material) or a mask (grayscale), and a from-scratch custom-ribbon builder covering path type switching, projection depth, image orientation, sharp-corner modes (Miter/Round/Bevel/Cut), and Stretching & Tiling behavior. The video closes on the two most powerful presets — Custom Ribbon Grayscale/Material — which expose start/middle/end/corner image assignment (previously only possible via hand-authored `.sbs` files in Substance 3D Designer), demoed by recreating an Adobe Illustrator pattern-brush trim using AI file Artboards directly as ribbon source images.

### Key Steps
1. Understand the difference: Paint along Path repeats a single brush stamp along a path (stamps overlap on tight curves) — Ribbon instead transforms/repeats the *texture* continuously along the path shape, with explicit control over start/end and sharp corners.
2. Note the underlying change to **all** path tools (not just Ribbon): the old single per-vertex Pressure value is now split into two independent controls — **Vertex Stroke Width** and **Vertex Opacity**.
3. Ribbon (like Paint along Path) works in two contexts: an empty paintable layer (full material data — BaseColor/Roughness/Metallic/Height etc.) or a mask (grayscale values only).
4. Select the Path tool on an empty layer/mask to reveal the new **Path Presets** bar at the top of Path properties, organized into categories: Favorites (empty by default — right-click any preset/asset → Add to Favorites), Gradients, Text, Apparel, Hard Surface, plus Basic/Custom. Preset icons visually distinguish Ribbon presets from Paint-along-Path presets.
5. **Gradients** category: repeating grayscale gradients up to tricolor full-material gradients — for full-material gradients, confirm the Alpha channel is set up correctly before tuning material settings; Width and Projection Depth still apply as with other paths; add enough path points for the ribbon to conform well to curved surfaces.
6. **Text Along Paths**: presets mainly preset text alignment/repetition — pick the closest preset then adjust; text must fit within the ribbon's stroke width, and the Advanced section of the text parameters resolves alignment issues.
7. **Apparel** presets: rebuilt stitches/seams/zippers that support much sharper corners than before, and terminate with realistic start/end shapes instead of simply fading in/out.
8. **Hard Surface** presets: grip patterns, shut lines, tape, welding seams. Workflow trick shown: enable **Snap to Mesh Wireframe**, click a vertex to place a point on it, **Shift+click** to force that point to a Sharp Corner, then add Smooth Tangents afterward to avoid odd bends the path tool can otherwise produce at sharp corners.
9. To build a ribbon from scratch: start from the **Basic Hard Ribbon** preset. Key settings top to bottom: **Path Type** (switchable at any time between Paint / Ribbon / Filled / Erase / Smudge), **Projection Depth** (tune per case; adding more points usually helps), **Ribbon Width** and **Opacity**.
10. Under **Stroke**, **Image Orientation** re-aligns the alpha image to better follow the path direction.
11. Setting a vertex to Sharp Corner exposes **Corner Mode**: Miter, Round, Bevel, Cut. Cut mode scales the whole stamp image to avoid ever cutting it off, fitting the best possible stamp count along the path — this behavior is governed by the Stretching & Tiling parameters.
12. Stretching & Tiling combinations: `Scale=Stretch` + `Tiling=Auto` together minimize visible stretching. Turning on `Stretch between offsets only` + `Tiling=Custom` leaves the first 25% and last 25% of a stroke unstretched, stretching only the middle. `Tiling=None` starts a fresh stroke only between sharp corners.
13. The two most important presets for advanced work: **Custom Ribbon Grayscale** and **Custom Ribbon Material** — grayscale is for simple alpha stamps painting solid-color material; Material supports full-color BaseColor images plus uniform Roughness/Metallic/Height values.
14. Both custom-ribbon presets expose separate **Start**, **Middle**, and **End** image slots; enabling **Custom Corners** adds two more image slots for left/right sharp corners, which automatically warp to match the exact angle of the corner drawn — this is what lets you build complex modular trim ribbons that previously required hand-authored Substance Designer `.sbs` graphs.
15. Demonstrated recreating an Adobe Illustrator pattern-brush-style trim by feeding AI file **Artboards** directly in as the ribbon's source images, including choosing which artboard from the source AI file applies to which slot (start/middle/end/corner).

### Layers / Tools / Settings
- Path tool → **Path Type**: Paint / Ribbon / Filled / Erase / Smudge
- Path Presets bar: Favorites, Gradients, Text, Apparel, Hard Surface, Basic, Custom
- Vertex Stroke Width, Vertex Opacity (replaces old single Pressure value, all path tools)
- Projection Depth, Ribbon Width, Opacity
- Stroke → Image Orientation
- Corner Mode: Miter / Round / Bevel / Cut (on vertices set to Sharp Corner)
- Stretching & Tiling: Scale mode (Stretch), Tiling mode (Auto / Custom / None), Stretch between offsets only
- Snap to Mesh Wireframe, Shift+click (force Sharp Corner), Smooth Tangents
- Custom Ribbon Grayscale / Custom Ribbon Material presets — Start / Middle / End image slots, Custom Corners (left/right)
- Adobe Illustrator Artboard import as ribbon source image

### Difficulty
Intermediate for using the built-in presets; Advanced for the from-scratch Custom Ribbon / Stretching & Tiling / Custom Corners workflow.

### App & Version
**Substance 3D Painter — Ribbon Paths shipped in 11.1.0**, stated explicitly on-screen at 0:00 ("Substance Painter 11.1 now has ribbon paths"), which matches `references/release-notes-painter-11.1.md`'s headline **Ribbon tool** entry exactly — direct, unambiguous confirmation. Note: the on-screen version watermark in the captured viewport frames appears to read a later version (approximately "12.0.0"), which is expected/consistent — this is a feature-tour video made after the feature's original 11.1.0 launch, running on whatever later build was current when filmed, not the 11.1.0 launch version itself. Treat the exact captured build number as tentative (small on-screen text); the 11.1.0 origin claim is the reliable, spoken-on-camera fact.

### Tags
`path-tool` `alpha` `opacity` `roughness` `metallic` `height` `basecolor` `intermediate` `advanced`

---

## Related Tutorials
- **"New Path Tool Features & Improvements in Substance 3D Painter"** (`tutorials/new-path-tool-features-improvements-in-substance-3d-painter-adobe-substance-3d.md`, video `exE0-1ftNeE`) — same `path-tool` feature family and same 11.0.0 Filled Path tool this video builds on; covers Filled Path projection depth, snapping (mesh-wireframe + angle), and the transform manipulator rather than the Ribbon-specific presets/corner-modes this video focuses on.
- **"3D Path Tool Updates in Substance 3D Painter"** (`tutorials/3d-path-tool-updates-in-substance-3d-painter-adobe-substance-3d.md`, video `rhraMw3YVpo`) — same `path-tool` feature family; covers the earlier, distinct **3D Paths** tool (9.0.0) — path visibility toggling, selective copy/paste, freeform vertex movement, manual tangent editing — a different tool generation from this video's Ribbon Paths (11.1.0).
- **"Creating 3D Paths in Substance 3D Painter"** (`tutorials/creating-3d-paths-in-substance-3d-painter-adobe-substance-3d.md`, video `Ro5dADu3vpM`) — same `path-tool` feature family; the original launch tutorial for the earliest-generation **3D Paths** tool (9.0.0), the foundation this video's Ribbon Paths (11.1.0) builds on years later.
