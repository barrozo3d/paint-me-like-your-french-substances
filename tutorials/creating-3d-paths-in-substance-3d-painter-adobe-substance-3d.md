---
title: Creating 3D Paths in Substance 3D Painter | Adobe Substance 3D
source: YouTube
url: https://www.youtube.com/watch?v=Ro5dADu3vpM
author: Adobe Substance 3D
ingested: 2026-08-13
app: "Substance 3D Painter"
version: "not stated on screen or in narration; this appears to be the original launch tutorial for the 3D Paths tool, which the companion '3D Path Tool Updates' video states shipped in 9.0.0 (June 2023)"
tags: [path-tool, layers, paint-layer, masks, fill-layer, blend-mode, alpha, procedural, intermediate]
extraction_status: complete
frames_dir: tutorials/frames/creating-3d-paths-in-substance-3d-painter-adobe-substance-3d/
frame_count: 7
frame_status: complete
frame_selection: content-anchored (manual timestamps chosen from transcript, not blind percentages)
---

# Creating 3D Paths in Substance 3D Painter | Adobe Substance 3D

**Source:** [YouTube](https://www.youtube.com/watch?v=Ro5dADu3vpM)
**Author:** Adobe Substance 3D
**Duration:** 5m44s | 3 section(s)

---

## Raw Data (for Claude Code extraction)

Frames captured — see "Captured Frames" section below.


### Intro [0:00]
**Transcript (timestamped):**
[0:00] Hi everyone and welcome to this video where we'll be showing you this exciting new update
[0:13] in Substance 3D Painter.


### What is the 3D Paths tool? [0:15]
**Transcript (timestamped):**
[0:16] This is the 3D Paths tool and this allows us to create brush strokes directly on our model
[0:23] using editable curves.
[0:25] What's cool about this tool that's different to using the regular paint brush tool is that
[0:30] we can dynamically change the brush's properties even after we've created our path.
[0:36] We can select a different brush, adjust the size, change the material properties and much
[0:42] more.
[0:43] This is a completely non-destructive workflow.
[0:48] We use the 3D Paths tool on paint layers, either on a regular paint layer or in a mask.
[0:55] You can paint, erase and smudge using the Paths tool.
[1:00] You'll find it located in the top left toolbar just below the eraser.
[1:05] The purpose of this tool is to be able to paint with curves around our mesh's geometry
[1:10] so we will only need the 3D viewport for now.
[1:15] Just to note, this tool currently does not work with some of our tool brushes which you
[1:20] can see here.
[1:21] This is because they are already tied to the original paint smudge and erase tools.
[1:27] There are however some new tool brushes made especially for 3D paths that we will look
[1:32] at in another video.


### Getting started with 3D Paths [1:34]
**Transcript (timestamped):**
[1:34] Right, let's jump into it.
[1:37] To start creating a path, I first make sure that I'm using a paint layer, then I select
[1:43] the pen icon for the 3D Path tool.
[1:46] I then begin clicking to add points or vertices along my path.
[1:51] You can see that when I begin creating my path, I now have this small dialogue in the
[1:56] top left of my viewport.
[1:58] This kind of works like a layer stack for my paths where I can visualize them and select
[2:03] which one I want to work on.
[2:05] But more on that later.
[2:07] By default the point interpolation is a smooth automatic bezier.
[2:11] But if I want to change it to linear, I can double click the vertex to make it a sharp
[2:16] corner.
[2:18] Another way I can do this is by selecting a vertex and clicking this icon in the top
[2:22] toolbar.
[2:24] Using this method I can click and drag multiple points or Ctrl or Command A to select all
[2:30] the points and then convert them all to corner points at the same time.
[2:36] The same approach can be taken if you want to delete multiple vertices at the same time.
[2:41] Just click and drag and then press delete on your keyboard.
[2:45] Currently we cannot edit the Bezier handles but what we can do instead is add in more
[2:50] vertices in between our existing ones.
[2:54] To do this all we need to do is hover over an existing line and click where we want our
[2:59] new vertex to sit.
[3:02] Don't be afraid to add lots of vertices, particularly if your model has quite complex geometry.
[3:08] Once you're done creating your path you can complete your path creation by pressing the
[3:12] Escape key or the Enter key.
[3:15] The next time you click on your object you will then begin making a new path.
[3:19] You can have multiple paths on one paint layer and as previously mentioned we can visualize
[3:24] these different paths in the paths window in the top left of your 3D viewport.
[3:29] Here we can right click to copy, cut, paste, duplicate and remove paths as well as double
[3:36] clicking to rename them.
[3:39] Now let's take a look at the toolbar at the top.
[3:42] Some of these properties you will recognize from the regular brush tool.
[3:46] But let's talk about what's new.
[3:49] This first icon toggles a display of the curve and vertices overlaid on your path.
[3:55] You can also toggle this visual display with the Q key.
[3:59] This next icon opens a display window where you can adjust the way your path is visualized
[4:04] on your geometry.
[4:05] This button can reverse the direction of which your curve is being created.
[4:10] This can be helpful if you want to continue your path from the other side.
[4:15] Next is the pressure slider.
[4:17] This essentially adjusts the size of your brush on a per point basis.
[4:22] You can either adjust a single vertex or multiple at the same time.
[4:27] We've looked at this icon previously.
[4:30] This is the vertex interpolation toggle.
[4:32] You can close and open your curve by having an endpoint selected and clicking this.
[4:39] This button is the same as using the delete key.
[4:43] You can switch on symmetry for your paths by clicking the mirror icon.
[4:47] And this can be toggled for each path that you create within your layer.
[4:51] So you don't have to have all paths being mirrored if you don't want to.
[4:56] You can adjust your mirror properties with the buttons next to it.
[5:01] Each path has its own brush and material properties.
[5:04] If you want your paths to share the same material properties, you can use a fill layer with
[5:09] a black mask and then add your 3D paths to a paint layer within that mask.
[5:17] If you add vertices quite far apart, you may see that you lose some of the paint.
[5:23] To fix this, you can either put an extra vertex in the middle of these points or adjust the
[5:28] projection depth in the properties panel.
[5:33] We hope this new feature helps accelerate your texturing workflow in Substance 3D Painter.
[5:40] We can't wait to see what you create.



---

## Captured Frames

- [1:46] tutorials/frames/creating-3d-paths-in-substance-3d-painter-adobe-substance-3d/frame_000.jpg
- [2:11] tutorials/frames/creating-3d-paths-in-substance-3d-painter-adobe-substance-3d/frame_001.jpg
- [2:54] tutorials/frames/creating-3d-paths-in-substance-3d-painter-adobe-substance-3d/frame_002.jpg
- [3:24] tutorials/frames/creating-3d-paths-in-substance-3d-painter-adobe-substance-3d/frame_003.jpg
- [3:49] tutorials/frames/creating-3d-paths-in-substance-3d-painter-adobe-substance-3d/frame_004.jpg
- [4:43] tutorials/frames/creating-3d-paths-in-substance-3d-painter-adobe-substance-3d/frame_005.jpg
- [5:09] tutorials/frames/creating-3d-paths-in-substance-3d-painter-adobe-substance-3d/frame_006.jpg

---

## Structured Notes

### Core Technique
The original launch tutorial for the **3D Paths tool**: paint editable, curve-based brush strokes directly on a model's geometry (rather than freehand), fully non-destructively — brush, material, and per-vertex properties can all be changed at any time after the path is drawn, since the path remains a live, editable curve rather than baked-in paint.

### Summary
Official Adobe introduction to the 3D Paths tool (demoed on a leather brogue shoe, drawing the circular "broguing" perforation pattern along the toe cap). Unlike the regular paint brush, a 3D Path is an editable curve you can keep reshaping and re-styling after the fact — change brush, size, or material properties at any point, non-destructively. The tool works on **paint layers** (regular paint layers or inside a mask) and supports paint, erase, and smudge modes; found in the top-left toolbar just below the eraser. Note: at time of this video, the 3D Paths tool did not yet work with the pre-existing tool-brushes tied to the original paint/smudge/erase tools — new tool-brushes made specifically for 3D Paths existed but were covered in a separate video. **Workflow:** with a paint layer active, select the 3D Paths pen icon and click to place points/vertices along the model's surface — a small **Paths panel** appears top-left of the viewport, functioning like a mini layer stack for all paths on that layer (visualize, select, right-click to copy/cut/paste/duplicate/remove, double-click to rename). New vertices default to smooth automatic Bezier interpolation; double-click a vertex (or select it and click the interpolation-toggle icon) to make it a sharp linear corner — this also works on multi-selections (click-drag a box, or Ctrl/Cmd+A to select all vertices) to batch-convert or batch-delete points. Bezier handles themselves aren't directly editable; the workaround is adding more vertices along the curve (hover an existing segment and click) — don't hesitate to add many vertices on complex geometry. Press **Escape** or **Enter** to finish the current path; the next click starts a brand-new path on the same layer. **Toolbar controls specific to 3D Paths:** a toggle (also bound to **Q**) to show/hide the curve-and-vertices overlay on the model; a display-settings window controlling how the path renders on the geometry; a direction-reverse button (useful for continuing a path from its other end); a per-vertex **pressure slider** (adjusts brush size per point, single or multi-selected); the vertex-interpolation toggle (smooth/corner); a close-curve button (select an endpoint, click to close the loop into a closed shape); a delete button (same as the Delete key); and a **mirror/symmetry** toggle that applies per-path within a layer (not all-or-nothing across the whole layer), with adjustable mirror-axis settings next to it. Each path carries its own independent brush and material properties by default; to make multiple paths **share** the same material, build a fill layer with a black mask and add the 3D Paths inside that mask instead of on separate paint layers. A known gotcha: widely-spaced vertices can leave visible gaps/lost paint between them — fix by adding an extra vertex partway between the sparse points, or by adjusting **Projection Depth** in the Properties panel.

### Key Steps
1. **Select or create a paint layer** (regular paint layer, or a mask) — the 3D Paths tool only works within paint-layer contexts.
2. **Select the 3D Paths pen icon** in the top-left toolbar, just below the eraser tool.
3. **Click on the model to place vertices** along the desired curve; watch the small **Paths panel** appear top-left of the viewport, tracking every path on the current layer.
4. **Leave new vertices as smooth automatic Bezier** by default, or **double-click a vertex** to convert it to a sharp linear corner; the same toggle icon in the top toolbar does this for a selection.
5. **Batch-edit multiple vertices** by click-dragging a selection box (or Ctrl/Cmd+A to select all), then apply the corner-conversion icon or press Delete to affect all selected points at once.
6. **Add intermediate vertices for finer curve control** (Bezier handles aren't directly editable) by hovering an existing path segment and clicking where you want the new point — add generously on complex geometry.
7. **Finish the current path** with **Escape** or **Enter**; your next click on the model starts an entirely new, separate path on the same layer.
8. **Manage multiple paths per layer** via the Paths panel: right-click a path to copy/cut/paste/duplicate/remove, or double-click to rename it.
9. **Toggle the curve/vertex overlay display** with the dedicated toolbar icon or the **Q** key; open the adjacent display-settings window to control how the path visualizes on the geometry.
10. **Reverse a path's direction** with its dedicated toolbar button if you need to continue drawing from the opposite end.
11. **Adjust per-vertex pressure** (effectively per-point brush size) via the pressure slider, applied to a single selected vertex or a multi-selection.
12. **Close an open path into a loop:** select an endpoint vertex, then click the close-curve button.
13. **Enable mirror/symmetry** per path (not globally per layer) via the mirror icon, and fine-tune the mirror axis with the buttons beside it.
14. **Share material properties across multiple paths:** instead of giving each path its own separate paint layer, build a fill layer with a black mask and add all the 3D Paths inside that shared mask.
15. **Fix gaps/lost paint from widely-spaced vertices:** add an extra vertex partway between the sparse points, or increase **Projection Depth** in the Properties panel.

### Layers / Tools / Settings
- **3D Paths tool** — top-left toolbar, just below the eraser; works on paint layers (including masks); supports paint/erase/smudge modes
- **Paths panel** (top-left of viewport) — per-layer list of paths; right-click copy/cut/paste/duplicate/remove; double-click rename
- **Vertex controls:** default smooth automatic Bezier vs. linear/corner (double-click or toolbar toggle icon), multi-select via click-drag or Ctrl/Cmd+A, mid-segment click to insert a vertex
- **Toolbar-specific controls:** curve/vertex overlay toggle (also **Q**), path-visualization display-settings window, direction-reverse button, per-vertex pressure slider, vertex-interpolation toggle, close-curve button, delete button, mirror/symmetry toggle (per-path) + mirror-axis buttons
- **Shared-material technique:** fill layer + black mask, with 3D Paths drawn inside that mask instead of on individual paint layers
- **Projection Depth** (Properties panel) — fixes paint-loss gaps between widely-spaced vertices
- Shortcuts: **Escape**/**Enter** to finish a path, **Q** to toggle curve overlay, **Ctrl/Cmd+A** to select all vertices, **Delete** to remove selected vertices

### Difficulty
Intermediate (the drawing mechanics are approachable, but non-destructive re-editing, mirror-per-path behavior, and the shared-material-via-mask workaround take some practice).

### App & Version
Substance 3D Painter. No version number is stated on screen or in narration in this specific video; this is evidently the original launch/introduction tutorial for the **3D Paths** tool, which — per the companion "3D Path Tool Updates" video in this same library — shipped in Painter **9.0.0** (June 2023).

### Tags
`path-tool`, `layers`, `paint-layer`, `masks`, `fill-layer`, `blend-mode`, `alpha`, `procedural`, `intermediate`

---

## Related Tutorials
- [3D Path Tool Updates in Substance 3D Painter](3d-path-tool-updates-in-substance-3d-painter-adobe-substance-3d.md) — same channel (Adobe), direct sequel: covers feature additions (path visibility toggle, selective copy/paste, freeform vertex movement, manual tangent editing) built on top of the exact 3D Paths tool introduced in this video.
- [New Path Tool Features & Improvements in Substance 3D Painter](new-path-tool-features-improvements-in-substance-3d-painter-adobe-substance-3d.md) — same channel (Adobe); covers the later, separate **Filled Path** tool (11.0.0) — a different tool generation in the same path-tool family this video's 3D Paths belongs to.
- [New Ribbon Paths in Substance 3D Painter](new-ribbon-paths-in-substance-3d-painter-adobe-substance-3d.md) — same channel (Adobe); covers the still-later **Ribbon Paths** tool (11.1.0), the third generation in the path-tool family lineage this video begins.
