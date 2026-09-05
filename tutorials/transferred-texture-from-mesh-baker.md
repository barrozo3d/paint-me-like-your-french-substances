---
title: Transferred Texture from Mesh Baker
source: Article
url: https://experienceleague.adobe.com/en/docs/substance-3d/bakers/bakers-settings/transferred-texture-from-mesh
author: Adobe Experience League (Substance 3D bakers documentation)
ingested: 2026-09-04
app: "Substance 3D Designer / Substance Automation Toolkit (NOT available in Substance 3D Painter)"
version: "Adobe Substance 3D bakers documentation, last update 2026-05-01"
tags: [baking, high-to-low-poly, uv, normal-map, advanced]
extraction_status: complete
frames_dir: tutorials/frames/transferred-texture-from-mesh-baker/
frame_count: 0
frame_status: skipped
uncertainty_frames: []
---

# Transferred Texture from Mesh Baker

**Source:** [Article](https://experienceleague.adobe.com/en/docs/substance-3d/bakers/bakers-settings/transferred-texture-from-mesh)
**Author:** Adobe Experience League (Substance 3D bakers documentation)
**Duration:** unknown | 1 section(s)

---

## Raw Data (for Claude Code extraction)

Frame capture was skipped for this ingest (--skip-video). Text-only extraction.


### Full Content [0:00]
**Transcript:** Documentation Substance 3D Substance 3D Bakers Transferred Texture from Mesh Last update: May 1, 2026 The Transferred texture from mesh baker allows to convert a texture from one a mesh to another based on their respective UVs. This baker also supports the transfer or normal maps (which require special conversions). In order to work, both meshes need UV definitions. Available in : Substance Designer Substance Automation Toolkit Parameters Parameter Description Texture File Path to the input texture file that will be transferred. UV Set Mesh UVs to use on the high-poly mesh to read the texture and project it onto the low-poly mesh. Filtering Mode Defines how the pixel interpolation of the texture should be done.Possible values: Nearest : No interpolation, use the closest pixel found to a given position. Precise but can create aliasing. Bilinear (default): Use the four nearest pixels to a given position. No aliasing but can be blurry. Normal Map If enabled, indicates to the baker that the input texture to transfer is a normal map. This indicates the baker to apply special conversions to the texture to make it compatible with the target mesh. Map Type Defines what type of normal map the input texture is.Possible values: World Space Tangent Space (default) Normal Orientation Defines the normal format of the input texture if Map Type is set to Tangent Space .Possible values: OpenGL DirectX (default) recommendation-more-help substance-3d-help-substance-3d-bake



---

## Structured Notes

### Core Technique
**Transferred Texture from Mesh** converts an existing texture from one mesh onto another **through their respective UVs** — the operation for carrying a photogrammetry scan's colour onto a retopologised mesh. It is a **Substance 3D Designer** baker, and it is **not available in Painter**.

### Summary
This is the direct answer to "how do I transpose a texture from a 3D-scanned asset onto a retopologised asset", and the first thing it settles is *which application*: the baker is **available in Substance Designer and the Substance Automation Toolkit only**. **Substance 3D Painter cannot transfer a texture from a high-poly mesh to a low-poly one at all** — which is why searching Painter's bakers for the operation turns up nothing and why the nearest-looking option (Color Map from Mesh) does something different. The hard requirement is UVs: **both meshes need UV definitions**, since the transfer reads the texture through the high-poly's UVs and projects it onto the low-poly's. A photogrammetry scan normally satisfies this — it arrives as a dense mesh with a UV-mapped albedo — which is exactly the case the baker is built for. **Filtering Mode** chooses the interpolation: **Nearest** is precise but aliases, **Bilinear** (default) avoids aliasing at the cost of some blur. Normal maps are handled specially: enable **Normal Map** to tell the baker the input needs conversion, then declare its **Map Type** (World Space or **Tangent Space**, default) and, for tangent space, its **Normal Orientation** (**OpenGL** or **DirectX**, default) — getting that pair wrong is the classic inverted-green-channel failure.

### Key Steps
1. Work in **Substance 3D Designer** (or the Automation Toolkit) — this baker does not exist in Painter.
2. Confirm **both meshes carry UVs**. Without them the transfer cannot run; this is the one non-negotiable prerequisite.
3. Set **Texture File** to the input texture being transferred — the scan's albedo.
4. Set **UV Set** to the UVs **on the high-poly mesh** that the texture should be read through before projection onto the low-poly.
5. Choose **Filtering Mode**: **Bilinear** (default) for smooth results, **Nearest** when precision matters more than aliasing.
6. For a normal map, enable **Normal Map** so the baker applies its conversions rather than treating it as flat colour.
7. Set **Map Type** — **Tangent Space** (default) or **World Space** — to match the source.
8. For tangent space, set **Normal Orientation** to **DirectX** (default) or **OpenGL** to match the source's convention.
9. Pair this with the **Common Parameters** — cage or max frontal/rear distance — which govern how the rays find the high-poly surface on a noisy scan.

### Nodes / Tools / Settings
- **Transferred Texture from Mesh** baker — **Substance Designer** and **Substance Automation Toolkit**; ⚠️ **not Substance Painter**.
- **Texture File** — the input texture to transfer.
- **UV Set** — the high-poly UVs used to read the texture before projecting onto the low-poly.
- **Filtering Mode** — `Nearest` (no interpolation, precise, can alias) / `Bilinear` (default, four nearest pixels, no aliasing, can blur).
- **Normal Map** (toggle) → **Map Type** (`World Space` / `Tangent Space`, default) → **Normal Orientation** (`OpenGL` / `DirectX`, default).
- Requirement: **both meshes must have UV definitions**.

### Difficulty
Advanced

### Foundry App & Version
Substance 3D Designer and the Substance Automation Toolkit. **Not Substance 3D Painter** — the page's own "Available in" line is the authority, and it is the reason this question has no Painter-only answer.

### Tags
`baking`, `high-to-low-poly`, `uv`, `normal-map`, `advanced`

---

## Related Tutorials
- [Baker Common Parameters](baker-common-parameters.md) — cage, max frontal/rear distance and matching, which control how the transfer finds the scan surface.
- [Color Map from Mesh Baker](color-map-from-mesh-baker.md) — the Painter baker people reach for by mistake, and what it actually does.

---

> **Provenance, and a correction worth keeping.** These come from
> `experienceleague.adobe.com/en/docs/substance-3d/bakers/...`, which **is
> reachable** — verified 2026-09-04 with the final URL and topic-hit check, not a
> bare status code. This is a **real exception** to this skill's standing finding
> that Adobe's documentation is unreachable: the Painter **user guide** and the
> **Python API** paths still 404 or redirect to a generic page, and `helpx.adobe.com`
> times out entirely from here — but the **bakers** doc set is live and specific.
> The earlier conclusion was right about the paths it tested and **over-generalised
> to "Adobe docs are unreachable"**. Probe the doc set you actually need.
