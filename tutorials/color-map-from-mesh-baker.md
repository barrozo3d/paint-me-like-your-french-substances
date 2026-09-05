---
title: Color Map from Mesh Baker
source: Article
url: https://experienceleague.adobe.com/en/docs/substance-3d/bakers/bakers-settings/color-map-from-mesh
author: Adobe Experience League (Substance 3D bakers documentation)
ingested: 2026-09-04
app: "Substance 3D Painter / Designer / Automation Toolkit"
version: "Adobe Substance 3D bakers documentation, last update 2026-05-01"
tags: [baking, id-map, mesh-maps, high-to-low-poly, intermediate]
extraction_status: complete
frames_dir: tutorials/frames/color-map-from-mesh-baker/
frame_count: 0
frame_status: skipped
uncertainty_frames: []
---

# Color Map from Mesh Baker

**Source:** [Article](https://experienceleague.adobe.com/en/docs/substance-3d/bakers/bakers-settings/color-map-from-mesh)
**Author:** Adobe Experience League (Substance 3D bakers documentation)
**Duration:** unknown | 1 section(s)

---

## Raw Data (for Claude Code extraction)

Frame capture was skipped for this ingest (--skip-video). Text-only extraction.


### Full Content [0:00]
**Transcript:** Documentation Substance 3D Substance 3D Bakers Color Map from Mesh Last update: May 1, 2026 This Color Map from mesh baker projects color properties from a high definition mesh into a texture. It can be used to bake polypaint or material IDs to create selection masks. Available in: Substance Designer Substance Automation Toolkit Substance Painter Parameters Parameter Description Color Source Controls from which property of the high-poly mesh the color generation should be based on.Possible values: Vertex Color : reads the vertex color save it into the texture. Color are interpolated from vertex to vertex. Material Color : reads the material color assigned to a polygon face. Mesh ID : assign a color per object found. Polygroup / Submesh ID : assign a color per sub-object (also called element). Color Generator Defines how the color is generated when the Color Source is set to Mesh ID or Polygroup/Submesh ID .Possible values: Random : each object or sub-object is colored by a randomly generated color. Hue Shift : each object or sub-object is colored by a unique color based on a hue. Grayscale : each object or sub-object is colored by a unique grayscale value. recommendation-more-help substance-3d-help-substance-3d-bake



---

## Structured Notes

### Core Technique
**Color Map from Mesh** projects a **colour property of the high-poly mesh** — vertex colour, material colour, mesh ID or polygroup ID — into a texture. It reads properties, **not an existing texture**, which is why it cannot carry a scan's albedo across.

### Summary
This is the baker people reach for when they want to move a scan's colour onto a retopo mesh, and understanding why it does not do that is the whole point. Its **Color Source** enumerates what it can read: **Vertex Color** (interpolated vertex to vertex), **Material Color** (the material assigned to a polygon face), **Mesh ID** (a colour per object), and **Polygroup / Submesh ID** (a colour per sub-object). Every one of those is a *property carried on the geometry*. A photogrammetry scan normally carries its colour as a **UV-mapped texture file**, not as vertex colours — so this baker has nothing to read, and the transfer must go through **Transferred Texture from Mesh** in Designer instead. Where it genuinely fits is its stated purpose: **baking polypaint or material IDs to create selection masks**. The **Color Generator** applies only when the source is Mesh ID or Polygroup/Submesh ID, offering **Random**, **Hue Shift** (a unique hue per object) or **Grayscale** (a unique grey per object). Unlike the transfer baker, this one **is available in Painter** as well as Designer and the Automation Toolkit.

### Key Steps
1. Pick **Color Source** to match what the high-poly actually carries: **Vertex Color**, **Material Color**, **Mesh ID**, or **Polygroup / Submesh ID**.
2. Use **Vertex Color** for polypaint — e.g. a ZBrush sculpt painted per-vertex; colours interpolate from vertex to vertex.
3. Use **Material Color** where the high-poly has materials assigned per face.
4. Use **Mesh ID** or **Polygroup / Submesh ID** to generate selection masks per object or sub-object.
5. Set **Color Generator** for those two ID sources: **Random**, **Hue Shift** (unique hue per object) or **Grayscale** (unique grey value per object).
6. ⚠️ **Do not expect it to transfer a scan's texture.** If the high-poly's colour lives in a UV-mapped image rather than on the vertices, this baker has nothing to read — use **Transferred Texture from Mesh** in Substance Designer.
7. Combine with the common parameters — cage or max distance — as with any "from mesh" bake.

### Nodes / Tools / Settings
- **Color Map from Mesh** — available in **Substance Painter**, Designer and the Automation Toolkit.
- **Color Source**: `Vertex Color` (interpolated), `Material Color` (per polygon face), `Mesh ID` (per object), `Polygroup / Submesh ID` (per sub-object).
- **Color Generator** (Mesh ID / Polygroup only): `Random`, `Hue Shift`, `Grayscale`.
- Stated purpose: baking **polypaint** or **material IDs** to create **selection masks**.
- ⚠️ Reads geometry-borne colour properties, **never an existing texture file**.

### Difficulty
Intermediate

### Foundry App & Version
Substance 3D Painter, Designer and the Automation Toolkit.

### Tags
`baking`, `id-map`, `mesh-maps`, `high-to-low-poly`, `intermediate`

---

## Related Tutorials
- [Transferred Texture from Mesh Baker](transferred-texture-from-mesh-baker.md) — what to use instead when the colour is a texture, not a vertex property.
- [Baker Common Parameters](baker-common-parameters.md) — the cage and ray-distance settings shared by both.

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
