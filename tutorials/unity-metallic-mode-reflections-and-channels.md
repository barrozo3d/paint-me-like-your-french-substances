---
title: Unity Metallic Mode Reflections and Channels
source: Article
url: https://docs.unity3d.com/Manual/StandardShaderMaterialParameterMetallic.html
author: docs.unity3d.com (Unity Manual)
ingested: 2026-09-04
app: "Unity (receiving end of a Substance 3D Painter export)"
version: "Unity 6.6 (6000.6); page built 2026-09-03"
tags: [channel-packing, unity-export, game-engine, pbr, metal-rough, intermediate]
extraction_status: complete
frames_dir: tutorials/frames/unity-metallic-mode-reflections-and-channels/
frame_count: 0
frame_status: skipped
uncertainty_frames: []
---

# Unity Metallic Mode Reflections and Channels

**Source:** [Article](https://docs.unity3d.com/Manual/StandardShaderMaterialParameterMetallic.html)
**Author:** docs.unity3d.com (Unity Manual)
**Duration:** unknown | 1 section(s)

---

## Raw Data (for Claude Code extraction)

Frame capture was skipped for this ingest (--skip-video). Text-only extraction.


### Full Content [0:00]
**Transcript:** Unity - Manual: Configure reflections in prebuilt shaders Manual Scripting API unity.com Version: Unity 6.6 (6000.6) Supported Legacy Language : English English 中文 日本語 한국어 Unity Manual Version: Unity 6.6 Select a different version Language : English English 中文 日本語 한국어 Materials and shaders Prebuilt materials and shaders Configuring material properties in prebuilt shaders Configure reflections in prebuilt shaders Metallic and specular workflows Reference for metallic and specular values of real surfaces Configure reflections in prebuilt shaders Important : The Built-In Render Pipeline is deprecated and will be made obsolete in a future release. It remains supported, including bug fixes and maintenance, through the full Unity 6.7 LTS lifecycle. For more information on migration, refer to Migrating from the Built-In Render Pipeline to the Universal Render Pipeline and Render pipeline feature comparison . To configure reflections in a prebuilt shader, use the Metallic or Specular property and the Smoothness property. Select a workflow Select a material in the Hierarchy window, then in the Inspector window of the material do one of the following: If your project uses the Universal Render Pipeline (URP), set Workflow Mode to Metallic or Specular in the Surface Options section. If your project uses the Built-In Render Pipeline, set Shader to Standard to use the metallic workflow, or Standard (Specular setup) to use the specular workflow. For more information, refer to Metallic and specular workflows . Configure reflections in the metallic workflow To make a material metallic or non-metallic, set the Metallic value to 1 or 0. Values between 0 and 1 blend the two results. To control the blurriness or sharpness of the reflection, adjust the Smoothness property. To make different parts of a material more or less metallic, add a texture map to control the Metallic and Smoothness properties. For example, if you have a clothing texture with both non-metallic fabric and metallic zips and buckles. Use the channels as follows: Red channel: Metallic values Green channel: Unused Blue channel: Unused Alpha channel: Smoothness values A spaceship with a color texture, but no texture for metallic and smoothness. The whole object has a single Metallic and Smoothness value, and a flat appearance. The same spaceship model with a metallic map applied. Part of the spaceship now has a high Metallic value and appears more reflective. The metallic map. The lighter areas are values nearer 1 for metal surfaces, and the mid to low greys are values nearer 0 for non-metal surfaces. To set metallic values so they simulate real-life surfaces, refer to Reference for metallic and specular values of real surfaces . Configure reflections in the specular workflow To set the color and intensity of reflections, set the Specular color. A black specular color means no reflections, while a white specular color means full reflection. To control the blurriness or sharpness of the reflection, adjust the Smoothness property. To make different parts of a model or texture appear more or less reflective, add a texture map to control the Specular and Smoothness properties. For example, if you have a clothing texture with both non-metallic fabric and shiny plastic buttons. Use the channels as follows: Red, green, and blue channels: Specular color values Alpha channel: Smoothness values A 1000kg weight with a strong specular reflection from a directional light. The whole object has a single Specular and Smoothness value, and a flat appearance. The same model, but with a specular map assigned, instead of using a constant value. This allows the specularity to vary across the surface of the model. Notice the edges have a higher specular effect than the centre, there are some subtle colour responses to the light, and the area inside the lettering no longer has specular highlights. Additional resources Reflections Reference for metallic and specular values of real surfaces Creating Believable Visuals on the Unity Learn site Metallic and specular workflows Reference for metallic and specular values of real surfaces Copyright ©2005-2026 Unity Technologies. All rights reserved. Built from job ID 74715811. Built on: 2026-09-03. Tutorials Community Answers Knowledge Base Forums Asset Store Terms of use Legal Privacy Policy Cookies Documentation Terms of Use Do Not Sell or Share My Personal Information Your Privacy Choices (Cookie Settings)



---

## Structured Notes

### Core Technique
Unity's metallic workflow packs **Metallic in the Red channel and Smoothness in the Alpha channel**, leaving Green and Blue unused — a different layout from Godot's ORM, and the reason an export preset cannot be shared between the two engines.

### Summary
This is the Unity half of the "which packing does the target want" question, and the answer is explicit and unlike Godot's. In the **metallic workflow**, a map controlling Metallic and Smoothness uses **Red = Metallic values, Green = unused, Blue = unused, Alpha = Smoothness values**. In the **specular workflow** the same texture is read differently: **Red, Green and Blue carry specular colour, Alpha carries Smoothness**. Note also that Unity works in **Smoothness**, not roughness — the inverse of what Painter authors by default — which is exactly the kind of conversion an export preset has to perform rather than the artist doing it by hand. Workflow selection differs by pipeline: in **URP**, set **Workflow Mode** to Metallic or Specular in Surface Options; in the **Built-In Render Pipeline**, choose the **Standard** shader for metallic or **Standard (Specular setup)** for specular. ⚠️ The page carries Unity's own deprecation notice: **the Built-In Render Pipeline is deprecated** and will be made obsolete in a future release, supported through the Unity 6.7 LTS lifecycle.

### Key Steps
1. Choose the workflow: **URP** → Surface Options → **Workflow Mode** = Metallic or Specular. **Built-In** → Shader = **Standard** (metallic) or **Standard (Specular setup)**.
2. For a uniform material, set **Metallic** to 1 or 0 (values between blend the two results) and use **Smoothness** for reflection blurriness or sharpness.
3. For a varying material — fabric with metal zips and buckles is the page's example — supply a texture map and pack it as **R = Metallic, G unused, B unused, A = Smoothness**.
4. In the **specular** workflow instead, pack **RGB = specular colour, A = Smoothness**; black specular means no reflections, white means full reflection.
5. Remember Unity wants **Smoothness**, the inverse of roughness — the export preset must invert, not just re-route, the channel.
6. Use *Reference for metallic and specular values of real surfaces* to set physically plausible values.
7. ⚠️ Factor in the deprecation: the **Built-In Render Pipeline** is deprecated, supported through Unity 6.7 LTS, with migration to URP documented separately.

### Nodes / Tools / Settings
- **Metallic workflow packing**: **R = Metallic**, G unused, B unused, **A = Smoothness**.
- **Specular workflow packing**: **RGB = Specular colour**, **A = Smoothness**.
- Properties: **Metallic** (0–1, blends between), **Smoothness**, **Specular** colour.
- Pipeline selection: URP **Workflow Mode** (Surface Options); Built-In **Standard** / **Standard (Specular setup)** shaders.
- Reference: *Reference for metallic and specular values of real surfaces*, *Metallic and specular workflows*.
- ⚠️ Built-In Render Pipeline **deprecated**, supported through the Unity 6.7 LTS lifecycle.

### Difficulty
Intermediate

### Foundry App & Version
Unity 6.6 (6000.6) — documentation for the engine consuming the export, not for Painter itself.

### Tags
`channel-packing`, `unity-export`, `game-engine`, `pbr`, `metal-rough`, `intermediate`

---

## Related Tutorials
- [Godot Standard Material 3D and ORM Material 3D](godot-standard-material-3d-and-orm-material-3d.md) — the contrasting ORM layout; the two cannot share a preset.
- [Python API: export Module](python-api-export-module.md) — building either packing from script with `destChannel` / `srcChannel`.

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
