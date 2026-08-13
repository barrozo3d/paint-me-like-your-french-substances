---
title: 3D Path Tool Updates in Substance 3D Painter | Adobe Substance 3D
source: YouTube
url: https://www.youtube.com/watch?v=rhraMw3YVpo
author: Adobe Substance 3D
ingested: 2026-08-13
app: "Substance 3D Painter"
version: "3D Paths tool itself shipped 9.0.0 (June 2023, stated explicitly: 'you can find it in Substance 3D Painter 9.0.0 or above'); this update video's own build not stated"
tags: [path-tool, layers, paint-layer, masks, alpha, height, procedural, intermediate]
extraction_status: complete
frames_dir: tutorials/frames/3d-path-tool-updates-in-substance-3d-painter-adobe-substance-3d/
frame_count: 5
frame_status: complete
frame_selection: content-anchored (manual timestamps chosen from transcript, not blind percentages)
---

# 3D Path Tool Updates in Substance 3D Painter | Adobe Substance 3D

**Source:** [YouTube](https://www.youtube.com/watch?v=rhraMw3YVpo)
**Author:** Adobe Substance 3D
**Duration:** 3m57s | 6 section(s)

---

## Raw Data (for Claude Code extraction)

Frames captured — see "Captured Frames" section below.


### Intro [0:00]
**Transcript (timestamped):**
[0:00] Hi everyone and welcome to another update video.
[0:12] In this video we'll be talking about some awesome updates to our fantastic new 3D paths
[0:17] tool. If you haven't had a go with it yet, you can find it in Substance 3D Painter 9.0.0
[0:24] or above. And if you want to know more about the tool, you can watch these videos in the
[0:29] description. Since its release in June 2023, the 3D paths
[0:35] tool has already been received with such positivity from the Adobe Substance community, so thank
[0:40] you so much for your support and feedback on it. We've now added some new features
[0:45] that is going to make workflows with this tool even more efficient.


### Path Visibility Toggle [0:50]
**Transcript (timestamped):**
[0:51] Next up, we now have the ability to toggle path visibility. We can do this using the
[0:56] eye icon next to each path, much like other apps. This is great if you're trying out
[1:02] some different variations of your path. Next, in addition to copying and pasting


### Copy/Paste Separate Path Data [1:07]
**Transcript (timestamped):**
[1:09] paths, we now have the option to paste select data from the copied path to an existing
[1:15] path. Firstly, we can paste brush properties into
[1:19] our paths, so we can share the data found in the properties panel between our paths,
[1:24] leaving the pressure data and individual vertices intact. This means if we've created a path
[1:31] with a certain material and brush setup, we can then copy this setup to another existing
[1:37] path without overwriting the actual path data. Super handy! One thing to note with this function
[1:44] is that it only works when pasting into the same form of the tool, i.e. copying paint to
[1:50] paint or smudge to smudge or erase to erase, as these are different forms of the brush.
[1:57] We can also paste all vertex data, including individual pressure values to a chosen path.
[2:04] This works across all different forms of the tool, paint, smudge and erase.


### Move Points Freely in the 3D Space [2:11]
**Transcript (timestamped):**
[2:11] Another new feature with the 3D paths tool is that we can now move vertices freely in
[2:16] the 3D space, as opposed to only being able to snap them to our object's surface. We
[2:23] also now have the ability to move all vertices at once. We can also have these snap to the
[2:29] object's surface, however be aware that the vertices may shift slightly when moving to
[2:34] a different plane. Now, this has been a highly requested feature


### Custom Tangents [2:36]
**Transcript (timestamped):**
[2:39] since the 3D paths tool got released, and this is the ability to edit the path tangents manually.
[2:46] This means we can have full control over the tangent for each point on the path.
[2:52] When we toggle the edit tangents button, we now have two handles that we can use to edit
[2:57] the tangent of this vertex. You can combine this with toggling the corner smooth setting to
[3:03] create editable corner points too. Keep in mind that tangent handles can only be moved within the
[3:09] vertex normal plane, and cannot be moved freely in the 3D viewport like our vertices now can.
[3:16] You can hold down control or command to scale both tangents at the same time. If you hold down
[3:22] alt or option whilst moving a tangent, you can switch from smooth to corner settings.
[3:28] Keep in mind that in order to finish this action, the mouse button must be released first.
[3:34] Otherwise, it will revert back to the original setting. There is even a shortcut slot for
[3:39] toggling editing tangents manually. This is blank by default, but you can assign a keystroke if you need.


### Outro [3:47]
**Transcript (timestamped):**
[3:47] And that's all for now folks. Thank you so much for watching, and we can't wait to see what you
[3:52] create next with our fantastic 3D paths tool.



---

## Captured Frames

- [0:56] tutorials/frames/3d-path-tool-updates-in-substance-3d-painter-adobe-substance-3d/frame_000.jpg
- [1:20] tutorials/frames/3d-path-tool-updates-in-substance-3d-painter-adobe-substance-3d/frame_001.jpg
- [2:20] tutorials/frames/3d-path-tool-updates-in-substance-3d-painter-adobe-substance-3d/frame_002.jpg
- [2:55] tutorials/frames/3d-path-tool-updates-in-substance-3d-painter-adobe-substance-3d/frame_003.jpg
- [3:15] tutorials/frames/3d-path-tool-updates-in-substance-3d-painter-adobe-substance-3d/frame_004.jpg

---

## Structured Notes

### Core Technique
A round of quality-of-life updates to the **3D Paths** tool (Painter 9.0.0+, released June 2023 — note: this is a distinct, earlier tool from the later "Filled Path"/11.0.0 and "Ribbon Paths"/11.1.0 tools also in this library): per-path visibility toggling, selective copy/paste of path data (brush setup only vs. full vertex/pressure data), freeform vertex movement off the mesh surface, and fully manual tangent-handle editing for custom corner/curve control.

### Summary
Official short Adobe update video (carved wooden pillar model, then a lighthouse-pattern tin canister) covering four new 3D Paths tool features added since its June 2023 launch. **Path visibility toggle:** each path in the Paths panel now has an eye icon (matching conventions in other apps) to hide/show it individually — useful for comparing path variations without deleting anything. **Selective copy/paste:** beyond full path copy/paste, you can now paste just the **brush properties** from a copied path onto an existing path (shares material/brush setup via the Properties panel while leaving the target's own vertices and pressure data untouched) — this only works between paths using the same tool sub-mode (paint→paint, smudge→smudge, erase→erase, since these are different brush forms). Separately, you can paste **all vertex data including individual pressure values** onto a chosen path, and this variant works across all sub-modes (paint/smudge/erase interchangeably). **Freeform vertex movement:** vertices, previously locked to snapping onto the object's surface, can now be moved freely in 3D space (individually or all at once); they can still be snapped back to the surface, but doing so may shift them slightly if moving between different surface planes. **Custom tangents:** a long-requested feature — toggling "edit tangents" reveals two draggable handles per vertex for full manual control of that point's tangent/curvature, which can be combined with the Corner Smooth setting to create genuinely editable corner points. Tangent handles are constrained to move only within the vertex's normal plane (unlike the now-freely-movable vertices themselves). Hold **Ctrl/Cmd** while dragging a tangent handle to scale both handles symmetrically at once; hold **Alt/Option** while moving a tangent to toggle between smooth and corner behavior; the mouse button must be released to commit the tangent edit, or it reverts. An empty, user-assignable shortcut slot exists specifically for toggling tangent-edit mode.

### Key Steps
1. **Toggle a path's visibility** by clicking the eye icon next to its name in the Paths panel — lets you compare different path variations side-by-side without deleting or losing any of them.
2. **Copy a source path**, then when pasting onto a different existing path, choose **paste brush properties only** to transfer just the Properties-panel brush/material setup, leaving the target path's own vertex positions and pressure data intact — remember this only works within the same tool sub-mode (paint↔paint, smudge↔smudge, erase↔erase).
3. Alternatively, choose **paste all vertex data** (including per-vertex pressure values) to fully transfer the shape/pressure profile onto a target path — this mode works across all sub-modes (paint/smudge/erase can mix freely).
4. **Select a vertex (or all vertices) and drag it directly in the 3D viewport** to move it freely off the mesh surface, rather than being locked to a surface-snapped position; re-snap to the surface at any time (expect a small positional shift if snapping across a differently-angled plane).
5. **Toggle "Edit Tangents"** on a selected vertex to reveal two draggable tangent handles, giving full manual control over that point's curve tangent.
6. **Combine tangent editing with the Corner Smooth setting** to build genuinely editable, hand-shaped corner points rather than relying on automatic corner behavior.
7. Remember tangent handles are constrained to the **vertex's own normal plane** — they cannot be dragged freely through 3D space the way vertices themselves now can.
8. **Hold Ctrl/Cmd while dragging a tangent handle** to scale both of that vertex's tangent handles symmetrically together.
9. **Hold Alt/Option while moving a tangent handle** to switch that vertex between smooth and corner tangent behavior on the fly.
10. Release the mouse button to **commit** a tangent edit — if the drag is interrupted before release, the tangent reverts to its prior state.
11. Optionally **assign a custom keyboard shortcut** to the (default-blank) "toggle edit tangents manually" action for faster access.

### Layers / Tools / Settings
- **Paths panel:** per-path eye-icon visibility toggle
- **Copy/paste variants:** "paste brush properties" (Properties-panel data only, same sub-mode required) vs. "paste all vertex data" (full vertex + pressure, works across paint/smudge/erase sub-modes)
- **Vertex manipulation:** free 3D-space movement (single or all vertices), optional re-snap to surface
- **Edit Tangents** toggle — two draggable handles per vertex, constrained to the vertex normal plane
- **Corner Smooth** setting — combined with tangent handles for editable corner points
- Modifier keys: **Ctrl/Cmd** (scale both tangent handles together), **Alt/Option** (toggle smooth/corner while dragging a tangent)
- Assignable (default-empty) keyboard shortcut slot for tangent-edit toggling

### Difficulty
Intermediate (assumes prior familiarity with the 3D Paths tool's basic path-drawing workflow; these are refinement/power-user features on top of it).

### App & Version
Substance 3D Painter. The 3D Paths tool itself shipped in **9.0.0** (June 2023), stated explicitly in narration ("you can find it in Substance 3D Painter 9.0.0 or above"). This specific update video's own build/version is not stated on screen or in narration — the features described are cumulative additions since the 9.0.0 launch.

### Tags
`path-tool`, `layers`, `paint-layer`, `masks`, `alpha`, `height`, `procedural`, `intermediate`

---

## Related Tutorials
- [New Path Tool Features & Improvements in Substance 3D Painter](new-path-tool-features-improvements-in-substance-3d-painter-adobe-substance-3d.md) — same channel (Adobe); covers the later, separate **Filled Path** tool's 11.0.0 update (Projection Depth, mesh-snapping, angle-snapping, transform gizmo) — a different tool generation from this video's 3D Paths (9.0.0) updates, useful to read together to understand Painter's path-tool family lineage.
- [New Ribbon Paths in Substance 3D Painter](new-ribbon-paths-in-substance-3d-painter-adobe-substance-3d.md) — same channel (Adobe); covers the still-later **Ribbon Paths** tool (11.1.0), the third and most advanced generation in the same path-tool family, explicitly introducing the `path-tool` tag also used here.
- [Creating 3D Paths in Substance 3D Painter](creating-3d-paths-in-substance-3d-painter-adobe-substance-3d.md) — same channel (Adobe), the original launch tutorial for the exact 3D Paths tool this video's updates extend.
