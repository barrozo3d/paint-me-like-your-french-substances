---
class: topic-reference
verified: no
sources: []
last_verified: never
version_basis: "unknown"
# WARNING: written from model memory, not ingested from a source.
# Do not cite as authority. If a tutorial disagrees, the tutorial wins.
---
# Export & Game-Engine Pipeline

## Export Presets
Painter ships built-in **export presets** (File → Export Textures, or `Ctrl+Shift+E`) that define which output files get produced from which combination of channels — e.g. the "Unreal Engine 4 (Packed)" preset packs BaseColor(RGB) + a packed OcclusionRoughnessMetallic(RGB) map, matching Unreal's expected texture layout. Presets ship for Unreal Engine, Unity (Standard/HDRP/URP variants), Godot's PBR layout, glTF, Arnold/USD-friendly unpacked sets, and a generic "Document channels" pass-through.

## Channel Packing
- **Packing** means combining multiple single-channel outputs (each 0-1 grayscale) into the R/G/B/A slots of one output texture, cutting texture-fetch and file-count cost in the target engine — e.g. Unreal's ORM convention: R=Occlusion, G=Roughness, B=Metallic in one texture.
- Custom packing is authored in the **Export Preset Editor** (Edit → Export Presets → New) by dragging a source channel (or a per-channel-selected map) into a target output's R/G/B/A slot.
- Packing choices must match what the target engine's shader/material actually expects — packing into the wrong slot order (e.g. swapping G/B) silently produces a plausible-looking but wrong material once imported.

## Texture Sets & UDIMs on Export
- Each Texture Set exports its own file set by default, with a filename token pattern (`$mesh`, `$textureSet`, `$channel`, `$udim`, etc.) configurable per preset — get this token pattern right before a large batch export, since renaming hundreds of exported files after the fact is painful.
- UDIM projects export one file per tile per channel unless the target format/engine expects a single virtual-texture UDIM set (some newer pipelines, e.g. certain USD/MaterialX setups, consume the UDIM tile sequence directly).

## Resolution, Format, Bit Depth
- Export resolution is set per Texture Set (can differ per set — e.g. a hero prop at 4K, background/trim texture sets at 1K/2K) independent of the in-app working/painting resolution.
- Output format (`.png`, `.tga`, `.exr`, `.tif`, `.jpg`) and bit depth (8/16/32-bit) are chosen per output map in the preset — Normal maps should stay 16-bit where the target pipeline supports it; 8-bit normals show visible banding on smooth curved surfaces.
- Color space matters on export the same way it does for painting (see `foundations-pbr-texturing-theory.md`): BaseColor/Emissive as sRGB, data maps (Roughness/Metallic/Normal/Height/AO) as linear/raw — most export presets set this correctly by default, but a custom preset must set it explicitly per output.

## Game Engine Specifics (brief)
- **Unreal:** default material expects sRGB BaseColor, a packed ORM (or split O/R/M), tangent-space Normal in DirectX (or OpenGL, configurable per-material) green-channel convention — verify which convention the target Unreal material uses, since Painter's Normal can be flipped per Texture Set Settings.
- **Unity (URP/HDRP):** expects a Metallic/Smoothness pack in some pipelines (note: **Smoothness = 1 - Roughness**, not Roughness directly) — using a raw Roughness export against a Smoothness-expecting shader inverts the material's shininess.
- **Godot:** PBR export preset targets Godot's StandardMaterial3D channel layout (ORM packing supported natively since Godot 4).

## Common Gotchas
- Exporting before all Texture Sets are baked and all layers are filled leaves some channels at their default flat value (often black) in the export — always do a final visual pass over every Texture Set before a real export.
- A preset built for one project's channel set breaks silently (empty/black outputs for missing channels) when reused on a project with a different enabled-channel list — presets are per-Texture-Set-Settings, not universally portable without checking.
- Mismatched Normal map green-channel convention (OpenGL vs. DirectX) between what Painter exported and what the target engine expects is the single most common "why does my normal map look inverted/inside-out" bug — check Texture Set Settings → Normal Map Format before export, not after import.
