---
title: Baker Common Parameters
source: Article
url: https://experienceleague.adobe.com/en/docs/substance-3d/bakers/bakers-settings/common-parameters
author: Adobe Experience League (Substance 3D bakers documentation)
ingested: 2026-09-04
app: "[PENDING]"
version: "[PENDING]"
tags: []
extraction_status: pending
frames_dir: tutorials/frames/baker-common-parameters/
frame_count: 0
frame_status: skipped
uncertainty_frames: []
---

# Baker Common Parameters

**Source:** [Article](https://experienceleague.adobe.com/en/docs/substance-3d/bakers/bakers-settings/common-parameters)
**Author:** Adobe Experience League (Substance 3D bakers documentation)
**Duration:** unknown | 1 section(s)

---

## Raw Data (for Claude Code extraction)

Frame capture was skipped for this ingest (--skip-video). Text-only extraction.


### Full Content [0:00]
**Transcript:** Documentation Substance 3D Substance 3D Bakers Common Parameters Last update: May 1, 2026 Common parameters apply to all bakers. These parameters usually define how the bakers will behave and work with high-poly meshes but how the final textures will be generated. Some of these parameters can be overridden by specific bakers. While most of these parameters are available across all the software (including Substance Automation Toolkit), their behavior may slightly differ; or some may not be available depending on the software workflow and implementation. General Parameters These parameters affect the way bakers generate textures. Name Description Size (Default Size or Output Size) Control the baking output texture resolution (in pixels).Available values: 32 64 128 256 512 1024 2048 (default) 4096 8192 Non-square resolutions are also supported, for example: 2048x1024 (2:1 ratio). In Substance Designer this parameter can be overridden by the baker itself. Format File format of the baked textures. Not available in Substance Painter. See: How to export the baked maps . Anti-Aliasing Controls anti-aliasing which can improve the quality of baked textures and reduce aliasing where different geometries connect.To learn more about aliasing see: Aliasing on UV Seams and Aliasing on Wikipedia .Available values: None (default) Subsampling 2x2 Subsampling 4x4 Subsampling 8x8 Note: Enabling anti-aliasing can significantly increase baking time, as anti-aliasing works by computing the texture at a higher resolution and then downscaling it back to the originally selected size. This means a 2K texture with a 2x2 subsampling will actually compute a 4K texture.It is sometimes preferable to increase the number of rays in the baker rather than increasing the subsampling. It could achieve better results without waiting too long. UV Set Controls which UVs from the low-poly mesh will be used to compute the baked textures. Not available in Substance Painter. Dilation (px) Dilate/extend the pixels of the UVs outside or their border by the amount of pixels given. This operation allows to avoid seams at UV borders when these borders are not perfectly aligned to the texture pixels or when the texture resolution is reduced (ex: mipmaps). This is a post-process applied after the baking process. It can sometimes be called “padding” as well.To learn more about dilation see: Aliasing on UV Seams and Padding . Apply Diffusion If enabled, the outside of the UVs will be filled with smoothed gradient colors based on the UV borders. This process ensures that when texture size is reduced it will stays stable and not create overly visible seams (ex: mipmaps). This is a post-process applied after the baking process. Average Normals If enabled, computes the average normal of a vertex to know in which direction to send rays during the mesh matching process of baking. If disabled, the rays will follow the original vertex normals of the mesh. High-Poly Parameters The following parameters control high-poly to low-poly mesh baking (“from mesh” bakers). Name Description High Definition Meshes A list of files (or Substance package resources) that contains high-poly meshes. They are loaded into memory by the bakers when the baking process starts to compute different information and save that mesh information to textures. This list is ignored if “ Use Low as High Definition ” is enabled. Use Low as High Definition or Use Low Poly Mesh as High Poly Mesh If enabled, the high-poly mesh list provided to the bakers will be ignored and the low-poly mesh will be baked on itself instead.This parameter is useful when working with a high-poly mesh directly. For example, when baking an ambient occlusion texture for a high-poly car with this setting enabled, the ray distance is ignored and the baker will produce a perfect bake (no ray misses or geometry mismatch). Set Distance With Cage or Use Cage Indicates whether to use a cage mesh file in the baking process instead of using ray distance values. The cage controls the ray maximum distance and direction. Cage File Path to the mesh file containing the cage. Frontal Value or Max Frontal Distance Controls how far above the low-poly surface the ray should start to find any high-poly geometry along its path. This setting has no effect when a Cage is used. Rear Value or Max Rear Distance Controls how far below the low-poly surface the ray should stop to find any high-poly geometry along its path. This setting has no effect when a Cage is used. Relative to Bounding Box If enabled, ray distance and other size-based computations are based on the normalized space of the low-poly mesh. If disabled, the ray distance computation is based on units specified in the low-poly mesh when it was exported (meters, centimeters, etc).It can sometimes be useful to disable this setting and enter the ray distance manually when an object has precise measurements. Match Indicates how the bakers should match low and high-poly geometry. It can be used to filter the baking process without the need to manually move apart (explode) meshes.Possible values: Always (default): Low-poly mesh is matched with every high-poly meshes. By Mesh Name : Filter the meshes by their name to avoid matching with unwanted geometry. To learn more about matching geometry see: Matching by Name . Match Suffixes or High Poly Mesh Suffix Low Poly Mesh Suffix Mesh name suffixes to identify and group together the geometry when using the Matching By Name feature. Available suffixes: Low Poly Mesh : suffix to identify low poly meshes in the scene High Poly Mesh : suffix to identify high poly meshes in the scene Ignore Backfaces : suffix to identify meshes that should be ignored by specific bakers (like the Ambient Occlusion From Mesh ) To learn more about matching geometry see: Matching by Name . Use Skew Correction If enabled, ray direction will be computed from Average Normal or the original geometry normal depending on the input texture. Black values in the texture use the average normal computed while white values use the original mesh normal. Not available in Substance Painter. Skew Map Path to the texture file used to skew ray projection. Invert Skew Correction Invert the reading of the input texture (black becomes white and white becomes black). recommendation-more-help substance-3d-help-substance-3d-bake



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
