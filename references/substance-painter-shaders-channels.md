# PBR Channels & Shaders

## Channel Set
Painter paints into a per-Texture-Set list of enabled channels, added via the "+" at the bottom of the Layers panel or set in the project's **Texture Set Settings**. Common channels:

| Channel | Purpose | Typical bit depth / range |
|---|---|---|
| BaseColor (Albedo) | Diffuse/base surface color, no baked lighting | 8-bit sRGB |
| Roughness | Microsurface roughness, 0 = mirror, 1 = fully diffuse | 8-bit linear/grayscale |
| Metallic | 0 = dielectric, 1 = metal (binary in practice — avoid mid-values except at material transition edges) | 8-bit linear/grayscale |
| Normal | Tangent-space surface detail, usually the baked high-to-low normal plus hand-painted detail on top | 16-bit, OpenGL or DirectX convention (green channel flips) |
| Height | Displacement/parallax source, also drives some generators (edge wear reads height deltas) | 16-bit linear/grayscale |
| Emissive | Self-illumination, HDR-capable in export | 8/16/32-bit |
| Opacity | Alpha/cutout transparency | 8-bit grayscale |
| AO (if separate from baked mesh map) | An authorable ambient-occlusion channel distinct from the baked mesh-map AO used in masks | 8-bit grayscale |

## Metal/Rough vs. Specular/Glossiness
- **Metal/Rough** (Disney/glTF-style) is Painter's default and the standard for Unreal, Unity (URP/HDRP), and most modern game/USD pipelines: BaseColor + Metallic + Roughness.
- **Specular/Glossiness** is the older workflow (still used by some legacy pipelines/Substance Designer graphs): Diffuse + Specular (RGB) + Glossiness. Switching workflows in Painter's Project Configuration changes which channels are exposed and how the built-in shaders interpret them — it is a per-project setting, not something toggled per-layer.
- Converting between the two loses information both ways (metal/rough can't perfectly reconstruct a colored specular response, and vice versa) — pick the workflow the target engine expects at project creation rather than converting after the fact.

## OpenPBR (default workflow as of 12.1)
- Starting with Painter 12.1 (2026-06-22), **OpenPBR** — a standardized, cross-application material definition — is the default shading workflow, alongside the legacy Metal/Rough and Specular/Glossiness options (still available as a per-project Project Configuration choice).
- OpenPBR is designed to carry a material's full definition (including coat, sheen, and other layered-response parameters beyond classic metal/rough) consistently across apps that support it, reducing lossy conversion when a material moves between Painter, Designer, and other OpenPBR-aware tools.
- Check `references/version-tracker.md` before assuming which workflow a given project should target — OpenPBR being the *default* for new projects doesn't mean every target engine already consumes it; most game engines still expect metal/rough on export as of this writing.

## Shader Presets / Viewport
- The **iray** renderer (View → renderer, or the Iray panel) gives a physically-based path-traced preview for lookdev/marketing stills — much slower than the default raster viewport, not used during active painting.
- The default **raster viewport** shader ("pbr-metal-rough" or "pbr-spec-gloss" depending on project workflow) is a fast approximation good enough for real-time painting feedback; it will not exactly match a target engine's actual lit result (Unreal/Unity apply their own tonemapping, IBL, exposure).
- Custom shader presets (`.sbsar`-based, under **Shader Settings**) can expose game-specific channels (e.g. a Detail Normal, Anisotropy, Clear Coat, or Subsurface channel for a custom engine shader) beyond the default set — needed when matching a proprietary engine material model.

## Common Gotchas
- Painting Metallic values other than pure 0 or 1 (aside from a 1-2px anti-aliased edge at material transitions) produces physically implausible results in most PBR renderers — this is one of the most common beginner mistakes.
- Height channel painting affects the Normal preview in-viewport (via the height→normal blend) but does NOT automatically bake into the exported Normal map unless "Normal from height blending" is enabled in Texture Set Settings — otherwise Height exports as its own separate map for the engine's parallax/displacement/tessellation pipeline.
- BaseColor must stay sRGB and Roughness/Metallic/Height must stay linear on export — an engine importing a roughness map through an sRGB-decoding pipeline will get visibly wrong (usually too dark) roughness.
