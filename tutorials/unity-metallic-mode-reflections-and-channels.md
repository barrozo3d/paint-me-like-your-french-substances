---
title: Unity Metallic Mode Reflections and Channels
source: Article
url: https://docs.unity3d.com/Manual/StandardShaderMaterialParameterMetallic.html
author: docs.unity3d.com (Unity Manual)
ingested: 2026-09-04
app: "[PENDING]"
version: "[PENDING]"
tags: []
extraction_status: pending
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
