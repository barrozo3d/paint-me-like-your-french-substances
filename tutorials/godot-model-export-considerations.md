---
title: Godot Model Export Considerations
source: Article
url: https://docs.godotengine.org/en/stable/tutorials/assets_pipeline/importing_3d_scenes/model_export_considerations.html
author: docs.godotengine.org (Godot stable docs)
ingested: 2026-09-04
app: "Godot (receiving end of a Substance 3D Painter / Blender export)"
version: "Godot stable docs (4.x)"
tags: [godot-export, game-engine, export, uv, intermediate]
extraction_status: complete
frames_dir: tutorials/frames/godot-model-export-considerations/
frame_count: 0
frame_status: skipped
uncertainty_frames: []
---

# Godot Model Export Considerations

**Source:** [Article](https://docs.godotengine.org/en/stable/tutorials/assets_pipeline/importing_3d_scenes/model_export_considerations.html)
**Author:** docs.godotengine.org (Godot stable docs)
**Duration:** unknown | 1 section(s)

---

## Raw Data (for Claude Code extraction)

Frame capture was skipped for this ingest (--skip-video). Text-only extraction.


### Full Content [0:00]
**Transcript:** Model export considerations  Before exporting a 3D model from a 3D modeling application, such as Blender, there are some considerations that should be taken into account to ensure that the model follows the conventions and best practices for Godot. 3D asset direction conventions  Godot uses a right-handed, Y-is-up coordinate system, with the -Z axis as the camera's forward direction. This is the same as OpenGL. This implies that +Z is back, +X is right, and -X is left for a camera. The convention for 3D assets is to face the opposite direction as the camera, so that characters and other assets are facing the camera by default. This convention is extremely common in 3D modeling applications, and is codified in glTF as part of the glTF 2.0 specification . This means that for oriented 3D assets (such as characters), the +Z axis is the direction of the front, so -Z is the rear, +X is the left side, and -X is the right side for a 3D asset. In Blender, this means that +Y is rear and -Y is front for an asset. When rotating an oriented 3D asset in Godot, use the use_model_front option on the look_at functions, and use the Vector3.MODEL_* constants to perform calculations in the oriented asset's local space. For assets without an intrinsic front side or forward direction, such as a game map or terrain, take note of the cardinal directions instead. The convention in Godot and the vast majority of other applications is that +X is east and -X is west. Due to Godot's right-handed Y-is-up coordinate system, this implies that +Z is south and -Z is north. In Blender, this means that +Y is north and -Y is south. Exporting textures separately  While textures can be exported with a model in certain file formats, such as glTF 2.0, you can also export them separately. Godot uses PBR (physically based rendering) for its materials, so if a texturing program can export PBR textures, they can work in Godot. This includes the Substance suite , ArmorPaint (open source) , and Material Maker (open source) . See also For more information on Godot's materials, see Standard Material 3D and ORM Material 3D . Exporting considerations  Since GPUs can only render triangles, meshes that contain quads or N-gons have to be triangulated before they can be rendered. Godot can triangulate meshes on import, but results may be unpredictable or incorrect, especially with N-gons. Regardless of the target application, triangulating before exporting the scene will lead to more consistent results and should be done whenever possible. To avoid issues with incorrect triangulation after importing in Godot, it is recommended to make the 3D modeling software triangulate objects on its own. In Blender, this can be done by adding a Triangulate modifier to your objects and making sure Apply Modifiers is checked in the export dialog. Alternatively, depending on the exporter, you may be able to find and enable a Triangulate Faces option in the export dialog. To avoid issues with 3D selection in the editor, it is recommended to apply the object transform in the 3D modeling software before exporting the scene. Note It is important that the mesh is not deformed by bones when exporting. Make sure that the skeleton is reset to its T-pose or default rest pose before exporting with your favorite 3D editor. Lighting considerations  While it's possible to import lights from a 3D scene using the glTF, .blend or Collada formats, it's generally advised to design the scene's lighting in the Godot editor after importing the scene. This allows you to get a more accurate feel for the final result, as different engines will render lights in a different manner. This also avoids any issues with lights appearing excessively strong or faint as a result of the import process. Previous Next User-contributed notes Please read the User-contributed notes policy before submitting a comment.



---

## Structured Notes

### Core Technique
Prepare a model for Godot before it leaves the DCC: match Godot's **right-handed, Y-up, -Z-forward** axis convention, **triangulate in the modelling application** rather than on import, apply transforms, and export PBR textures separately.

### Summary
The mesh-side companion to the material page. Godot uses a **right-handed, Y-is-up** coordinate system with **-Z as the camera's forward direction** (the same as OpenGL), so +Z is back, +X is right. The asset convention is the *opposite* — an oriented asset such as a character faces the camera, so **+Z is its front**, which in Blender means **+Y is rear and -Y is front**. For assets with no intrinsic front, use cardinal directions instead: +X east, -X west, and because of the handedness, **+Z south, -Z north** (in Blender, +Y north, -Y south). On textures, the page is direct and useful for this skill: Godot uses PBR, so **any texturing program that can export PBR textures works**, naming the **Substance suite**, ArmorPaint and Material Maker — and pointing at the Standard/ORM material page for how the channels are consumed. The triangulation advice is the one that silently damages assets: GPUs only draw triangles, Godot can triangulate on import, but **results may be unpredictable or incorrect, especially with N-gons** — so triangulate in the DCC. In Blender that means a **Triangulate modifier** with **Apply Modifiers** checked in the export dialog, or a Triangulate Faces option if the exporter has one.

### Key Steps
1. Match the axis convention: Godot is **right-handed, Y-up, -Z forward**; +Z back, +X right, -X left for a camera.
2. Orient assets the opposite way — **+Z is an asset's front**, -Z rear, +X left, -X right. In Blender: **+Y rear, -Y front**.
3. In Godot code, use **`use_model_front`** on `look_at` and the **`Vector3.MODEL_*`** constants to work in the asset's local space.
4. For maps and terrain, use cardinals: **+X east, -X west, +Z south, -Z north** (Blender: +Y north, -Y south).
5. **Triangulate before exporting** — add a **Triangulate modifier** in Blender and tick **Apply Modifiers**, or enable the exporter's Triangulate Faces option. Do not rely on import-time triangulation, especially with N-gons.
6. **Apply the object transform** before export to avoid 3D selection problems in the Godot editor.
7. ⚠️ Make sure the mesh is **not deformed by bones** at export — reset the skeleton to T-pose or the default rest pose.
8. Export **textures separately** where convenient; any PBR-capable texturing tool works — the Substance suite, ArmorPaint, Material Maker.
9. Prefer to **light the scene in Godot** rather than importing lights, since engines render lights differently and imported lights often arrive too strong or too faint.

### Nodes / Tools / Settings
- Coordinate system: right-handed, **Y-up**, **-Z forward** (OpenGL-like); glTF 2.0 codifies the asset-facing convention.
- Asset orientation: +Z front / -Z rear / +X left / -X right; Blender equivalent +Y rear, -Y front.
- Cardinals: +X east, -X west, +Z south, -Z north (Blender +Y north, -Y south).
- Code helpers: **`use_model_front`** on `look_at`, **`Vector3.MODEL_*`** constants.
- Export hygiene: **Triangulate modifier** + **Apply Modifiers**, applied object transform, skeleton at rest pose.
- Textures: PBR from the **Substance suite**, ArmorPaint or Material Maker; see Standard/ORM material for channel use.
- Lighting: design in the Godot editor rather than importing from glTF/.blend/Collada.

### Difficulty
Intermediate

### Foundry App & Version
Godot (stable docs, 4.x), with Blender named as the source application throughout.

### Tags
`godot-export`, `game-engine`, `export`, `uv`, `intermediate`

---

## Related Tutorials
- [Godot Standard Material 3D and ORM Material 3D](godot-standard-material-3d-and-orm-material-3d.md) — what happens to the textures once the mesh arrives.
- [Unity Metallic Mode Reflections and Channels](unity-metallic-mode-reflections-and-channels.md) — the other engine's conventions.

---

> **Why engine documentation lives in a Substance skill.** These pages are the
> *receiving end* of a Painter export, and they answer the half Painter's own
> docs never state: **which channel packing a given engine actually wants**.
> `python-api-export-module.md` teaches the mechanism (`destChannel` /
> `srcChannel` / `srcMapType` / `srcMapName`); these teach the target. Adobe's
> Substance 3D Painter user documentation remains unreachable — re-probed
> 2026-09-04, and `substance3d.adobe.com/documentation/spdoc/...` still redirects
> to a generic 2,876-character page with zero topic hits — so the engine vendors
> are the reliable first-party source for this, and they are explicit where Adobe
> is silent.
