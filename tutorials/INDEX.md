# Paint Me Like Your French Substances — Tutorial & Knowledge Base Index

This is the skill's growing knowledge base, covering Adobe Substance 3D Painter. Every ingested tutorial, article, and documentation page is listed here.

**To add a tutorial:** say "ingest this: [URL]" and the skill will fetch, structure, and add it here automatically.
**To add a documentation page or article:** paste the content and say "ingest this article/doc".
**To search:** look for tags matching the technique you need.

### SUBSTANCE PAINTER: Building Masks Explained
- **Source:** YouTube
- **URL:** https://www.youtube.com/watch?v=um3YRzqwYU4
- **Author:** Jared Chavez
- **App:** Substance 3D Painter
- **Version:** not specified (pre-12.1-era UI, approximate)
- **Tags:** `masks` `layers` `paint-layer` `fill-layer` `generator` `smart-mask` `curvature` `ambient-occlusion` `mesh-maps` `tri-planar` `procedural` `alpha` `blend-mode` `anchor-point` `intermediate` `advanced`
- **Summary:** Full walkthrough of every masking primitive (manual paint mask, ID color-select, generators driven by baked mesh maps, tileable/procedural grunge+scratch textures with tri-planar seam fixing, blend-mode stacking, filters, anchor points) and how to combine all of them to build complex production masks (demoed on a reptilian creature head "flaked skin" mask).
- **File:** tutorials/substance-painter-building-masks-explained.md


### REALISTIC CREATURES: HAND PAINTED TEXTURES in SUSTANCE PAINTER
- **Source:** YouTube
- **URL:** https://www.youtube.com/watch?v=ygKmaqpl2gk
- **Author:** Jared Chavez
- **App:** Substance 3D Painter
- **Version:** not specified (pre-12.1-era UI, approximate)
- **Tags:** `masks` `layers` `paint-layer` `fill-layer` `procedural` `alpha` `curvature` `mesh-maps` `basecolor` `color-management` `intermediate` `advanced`
- **Summary:** Process-level breakdown (part 2 of a personal creature project) of hand-painted skin texturing: anatomy-driven color-zone blocking (yellow=fat/bone, blue=cavities, purple=unify), large-to-small detail hierarchy, repurposing unrelated grunge materials as skin damage, edge-detect masks for peeling skin, and a post-mortem on fixing a "plasticky" skin shader and over-yellow Albedo after stepping away from the piece for months.
- **File:** tutorials/realistic-creatures-hand-painted-textures-in-sustance-painter.md


### How to TEXTURE EVERYTHING in Substance Painter
- **Source:** YouTube
- **URL:** https://www.youtube.com/watch?v=GvjfkhCW3aM
- **Author:** J Hill
- **App:** Substance 3D Painter
- **Version:** not stated on screen; Bevel Smooth filter usage places it at 11.0.0+, estimated 11.0.x-11.1.x
- **Tags:** `layers` `fill-layer` `paint-layer` `masks` `smart-mask` `smart-material` `generator` `anchor-point` `blend-mode` `curvature` `ambient-occlusion` `tri-planar` `procedural` `MatFX` `udim` `texture-set` `pbr` `metal-rough` `basecolor` `roughness` `metallic` `height` `normal-map` `emissive` `opacity` `alpha` `iray-render` `export` `export-preset` `channel-packing` `game-engine` `unreal-export` `advanced`
- **Summary:** Flagship 3h19m full-helmet texturing demo (priority creator, maximum-depth extraction) covering block-out-first material planning, base materials for metal/plastic/paint/leather/rubber/fabric/a fake-PBR "coating"/glass, anchor-point-driven multi-effect masking as the video's throughline (paint chips, leather cracks, decal grime all built from one paintable control mask referenced by multiple downstream layers), model detail added purely in texture (normal stamps + generator-driven extrusion picked up later by curvature/cavity), decals/stickers/projected text, a unifying top-of-stack "Overlays" composite pass (cavity/edge/dirt/color-variation), emissive, and a PBR-Validate-then-export-to-Unreal finish. Extremely dense — see the tutorial file's Structured Notes for exhaustive per-material step lists.
- **File:** tutorials/how-to-texture-everything-in-substance-painter.md


### How to TEXTURE in SUBSTANCE PAINTER | Creature TEXTURING
- **Source:** YouTube
- **URL:** https://www.youtube.com/watch?v=Lwep-faQVI0
- **Author:** Jared Chavez
- **App:** Substance 3D Painter
- **Version:** not specified (pre-12.1-era UI, approximate)
- **Tags:** `masks` `layers` `paint-layer` `fill-layer` `procedural` `alpha` `basecolor` `roughness` `color-management` `game-engine` `unreal-export` `advanced`
- **Summary:** Process breakdown of texturing an original xenomorph-style creature (translucent-skin reference from deep-sea fish, no fixed concept to follow): sub-dermal color blocking, a documented mid-project "everything looks wrong" struggle resolved by exporting to Unreal Engine to diagnose color under real lighting, a granite-material happy accident reused as skin discoloration, a hand-painted symmetrical head pattern, and a parallel Unreal subsurface-scattering shader pass.
- **File:** tutorials/how-to-texture-in-substance-painter-creature-texturing.md


### TEXTURING METAL from Scratch in SUBSTANCE PAINTER
- **Source:** YouTube
- **URL:** https://www.youtube.com/watch?v=-X5gKTjMGes
- **Author:** Jared Chavez
- **App:** Substance 3D Painter
- **Version:** not specified (pre-12.1-era UI, approximate)
- **Tags:** `layers` `fill-layer` `paint-layer` `masks` `smart-material` `generator` `anchor-point` `roughness` `basecolor` `metal-rough` `pbr` `ambient-occlusion` `procedural` `alpha` `intermediate` `advanced`
- **Summary:** Live layer-by-layer rebuild of a finished metal-armor texture from bare mesh to final result, organized around a big-medium-small detail pyramid: Steel smart-material base, parallel color+roughness breakup passes, complementary-color layering (blue/orange), generator-then-manual-breakup edge wear, secondary-form grunge buildup, deliberately sparse/localized rust as the tertiary focal detail, and a final anchor-point-driven flake/peel mask.
- **File:** tutorials/texturing-metal-from-scratch-in-substance-painter.md


### How to TEXTURE like a PRO with ANCHOR POINTS | Substance Painter Tutorial
- **Source:** YouTube
- **URL:** https://www.youtube.com/watch?v=l2W67e5MQuk
- **Author:** Jared Chavez
- **App:** Substance 3D Painter
- **Version:** not specified (pre-12.1-era UI, approximate)
- **Tags:** `anchor-point` `masks` `layers` `fill-layer` `paint-layer` `blend-mode` `roughness` `basecolor` `height` `emissive` `procedural` `intermediate`
- **Summary:** Dedicated anchor-point deep-dive (Allosaurus texture) covering three production use cases: reusing a finished mask to spin off fast pattern-color variants, forward-planning utility-map isolation masks (e.g. per-part roughness) while still doing base color, and building fully modular reusable "anchor point library" materials (paintable flaked-metal, paintable burn/char with emissive) from stacked anchor-referenced sub-layers combined with blend modes.
- **File:** tutorials/how-to-texture-like-a-pro-with-anchor-points-substance-painter-tutorial.md


### How to make SKIN TEXTURES in Substance Painter
- **Source:** YouTube
- **URL:** https://www.youtube.com/watch?v=s0DhvFML7oM
- **Author:** J Hill
- **App:** Substance 3D Painter
- **Version:** not stated on screen; baking-dialog UI matches pre-8.3.0 (likely predates the companion "TEXTURE EVERYTHING" video by several versions), tentative
- **Tags:** `layers` `fill-layer` `paint-layer` `masks` `generator` `curvature` `ambient-occlusion` `thickness` `tri-planar` `procedural` `blend-mode` `pbr` `basecolor` `roughness` `specular-glossiness` `normal-map` `height` `alpha` `color-management` `texture-set` `export` `export-preset` `channel-packing` `intermediate`
- **Summary:** Priority-creator, maximum-depth extraction (companion/prequel to "How to TEXTURE EVERYTHING"). Hand-painted, reference-driven PBR skin texturing: RBX imaging and cross-polarized photography as BaseColor reference, anatomy-mirrored Sub-Dermis/Dermis folder organization, the video's core repeated pattern of layered multi-scale procedural noise masks (Screen to add, Multiply to subtract) topped with a hand-paint edit pass, thickness-map- and curvature-driven lip discoloration, a custom Specular Level channel + matching export preset, Photoshop-style non-destructive adjustment layers (empty Pass-Through paint layer + HSL/Levels/Sharpen filters), and an iterate-export-render loop validated in Marmoset Toolbag rather than Painter's own viewport.
- **File:** tutorials/how-to-make-skin-textures-in-substance-painter.md


### Skew Baking & Auto Rebake in Painter 12.1 | Adobe Substance 3D
- **Source:** YouTube
- **URL:** https://www.youtube.com/watch?v=WwyElRpiQgY
- **Author:** Adobe Substance 3D
- **App:** Substance 3D Painter
- **Version:** 12.1.0 (confirmed on-screen watermark; exact match against release-notes-painter-12.1.md)
- **Tags:** `baking` `mesh-maps` `ambient-occlusion` `curvature` `thickness` `world-space-normal` `high-to-low-poly` `cage` `painter-12` `intermediate`
- **Summary:** Official Adobe walkthrough of Painter 12.1's Baking Mode changes: reorganized Mesh Map Bakers checklist with per-map quick-view/auto-rebake buttons, Common Settings split into Common/Cage/Skew Correction tabs, and the new Skew Correction paint tool (color-coded Skew Vectors overlay, Edge Protection against UV-seam artifacts) for manually fixing normal-map ray-tracing skew errors.
- **File:** tutorials/skew-baking-auto-rebake-in-painter-121-adobe-substance-3d.md


### Tempering Colors in Substance Painter | Steel Heat Effects
- **Source:** YouTube
- **URL:** https://www.youtube.com/watch?v=Y3plK51emsA
- **Author:** Dolinskyi
- **App:** Substance 3D Painter
- **Version:** not specified (modern UI, post-8.3 baking-mode era)
- **Tags:** `layers` `fill-layer` `masks` `anchor-point` `blend-mode` `smart-material` `procedural` `alpha` `roughness` `basecolor` `metal-rough` `intermediate`
- **Summary:** Short technique video building a reusable heat-discoloration/oxide-rainbow "tempering colors" effect from a 10-stop reference chart: a paintable anchor-point mask drives a 10-color gradient filter, demonstrated from scratch, then via a ready-made smart material on a suppressor (localized barrel overheating) and a subtle reference-matched slider example.
- **File:** tutorials/tempering-colors-in-substance-painter-steel-heat-effects.md



### Creating Trim Sheet UVs for Substance 3D Painter | Adobe Substance 3D
- **Source:** YouTube
- **URL:** https://www.youtube.com/watch?v=Dp2ZpGIaumA
- **Author:** Adobe Substance 3D
- **App:** Substance 3D Painter (destination only — UV prep shown in 3ds Max)
- **Version:** not specified — no Painter UI shown, DCC-side UV work only
- **Tags:** `uv` `texel-density` `game-engine` `unreal-export` `intermediate`
- **Summary:** DCC-side (3ds Max) UV-unwrap prep for a shared trim-sheet texture: grid-snapping tileable UV shells, deliberately-stretched end caps, mapping long structural sections onto one repeated tileable strip, plus deform-mesh-to-trim, thin "construction line" details, decal planes, and a grunge overlay. No Substance Painter UI appears — the trim sheet itself is the artifact that later gets painted/applied in Painter. Cross-linked with the "Create Trim Sheets in Substance 3D Painter" Part 1/2 pair.
- **File:** tutorials/creating-trim-sheet-uvs-for-substance-3d-painter-adobe-substance-3d.md


### Realistic Painted Metal in Substance Painter | M24 Grenade Texturing
- **Source:** YouTube
- **URL:** https://www.youtube.com/watch?v=SAI-lrWrtKg
- **Author:** Dolinskyi
- **App:** Substance 3D Painter
- **Version:** not specified (modern UI, post-8.3 baking-mode era)
- **Tags:** `layers` `fill-layer` `paint-layer` `masks` `generator` `anchor-point` `blend-mode` `ambient-occlusion` `curvature` `procedural` `alpha` `stencil` `tri-planar` `pbr` `metal-rough` `basecolor` `roughness` `metallic` `height` `normal-map` `color-management` `advanced`
- **Summary:** Part 2 of a personal M24 grenade texturing series — dense folder-by-folder audit of a finished painted-metal layer stack: cloned paint-variation layers (color+roughness+height together), stencil-driven hand-painted battle damage with large/medium/small compositional logic, a PBR-correct oxidized-metal-under-paint material (Metallic kept at 0.9, non-pure metalness mask), a compact 4-layer anchor-point peeling-paint recipe, a full decal build from Photoshop alpha to weathered final mask, and layered dirt/dust/curvature-cleaned generators, finished with Sharpen filters on Roughness and Base Color.
- **File:** tutorials/realistic-painted-metal-in-substance-painter-m24-grenade-texturing.md

### Texturing a Black Suit in Substance Painter
- **Source:** YouTube
- **URL:** https://www.youtube.com/watch?v=X24_IYUXOzU
- **Author:** 3DRedBox
- **App:** Substance 3D Painter
- **Version:** not stated on screen; UV-set-to-UV-set projection source is called "a new feature ... in a 10th version" — places this at 10.0.0+, pre-12.1-era UI
- **Tags:** `layers` `fill-layer` `paint-layer` `masks` `smart-material` `generator` `curvature` `anchor-point` `blend-mode` `baking` `mesh-maps` `ambient-occlusion` `udim` `texture-set` `uv` `pbr` `metal-rough` `basecolor` `roughness` `metallic` `height` `normal-map` `alpha` `procedural` `export` `export-preset` `channel-packing` `game-engine` `unreal-export` `intermediate`
- **Summary:** Full 3-UV-Tile suit texturing pipeline (jacket pinstripes, tie, dress shirt/vest, plastic accessories) built from smart materials, hand-built stripe fill layers, curvature/generator color variation, and an anchor-point-driven weave detail layer; the throughline technique is fixing pattern-direction mismatches across UV islands with a UV-set-to-UV-set fill projection source referencing a second guide UV channel authored in the DCC app. Exports to an Unreal-style PBR template and finishes with a full Marmoset Toolbag 5 lighting/render pass.
- **File:** tutorials/texturing-a-black-suit-in-substance-painter.md



### Substance 3D Painter 12.1 Beta: New Features, Faster Workflows, OpenPBR Support | Adobe Substance 3D
- **Source:** YouTube
- **URL:** https://www.youtube.com/watch?v=z-xbXtyPykI
- **Author:** Adobe Substance 3D
- **App:** Substance 3D Painter
- **Version:** 12.1.0-beta (confirmed via window title bar)
- **Tags:** `baking` `mesh-maps` `high-to-low-poly` `painter-12` `intermediate`
- **Summary:** Despite the title, this video is scoped only to Skew Correction painting and Auto Rebake (no OpenPBR or hard-surface-unwrap demo). Covers beta install paths (Creative Cloud Desktop vs. Steam), the red/green skew-direction wire overlay, performance tips (Tangent Wrap→UV brush projection for faster rebakes), Eraser/Polygon Fill as quick alternatives to manual painting, and Edge Protection. Companion to "Skew Baking & Auto Rebake in Painter 12.1" (stable 12.1.0 release, same demo mesh).
- **File:** tutorials/substance-3d-painter-121-beta-new-features-faster-workflows-openpbr-support-adob.md


### Substance 3D Painter & ACES - 01 - Color Space Fundamentals | Adobe Substance 3D
- **Source:** YouTube
- **URL:** https://www.youtube.com/watch?v=hDiYqODGoHg
- **Author:** Adobe Substance 3D
- **App:** Substance 3D Painter (context-setting; no Painter UI shown in this part)
- **Version:** not specified — theory-only slide deck
- **Tags:** `color-management` `pbr` `intermediate`
- **Summary:** Part 1/3 of Michael Wilde's (ILM London) ACES series: pure color-theory slide deck covering CIE chromaticity diagrams, RGB color model vs. gamut, sRGB's non-linear gamma-2.2 transfer function, and why ACES/ACEScg (Academy color management system / its linear wide-gamut VFX-texturing color space) matters for getting Substance Painter's viewport to match other render/DCC tools. No Painter UI shown. Series continues in Part 2 (OCIO & ACEScg in Painter) and Part 3 (textures in Maya/Blender).
- **File:** tutorials/substance-3d-painter-aces---01---color-space-fundamentals-adobe-substance-3d.md


### New Ribbon Paths in Substance 3D Painter | Adobe Substance 3D
- **Source:** YouTube
- **URL:** https://www.youtube.com/watch?v=3zgD-wwANCs
- **Author:** Adobe Substance 3D
- **App:** Substance 3D Painter
- **Version:** Ribbon tool shipped in 11.1.0 (stated on-screen); filmed on a later build (~12.0.0, tentative)
- **Tags:** `path-tool` `alpha` `opacity` `roughness` `metallic` `height` `basecolor` `intermediate` `advanced`
- **Summary:** Tour of Ribbon Paths (11.1.0): continuous texture-along-path transforms vs. the older stamp-repeating Paint along Path, new Path Presets (Gradients/Text/Apparel/Hard Surface), split Vertex Stroke Width/Opacity controls, Corner Modes (Miter/Round/Bevel/Cut), Stretching & Tiling, and the Custom Ribbon Grayscale/Material presets for building complex trims (start/middle/end/corner images, even importing Adobe Illustrator Artboards) without Substance 3D Designer. Introduces the new `path-tool` tag.
- **File:** tutorials/new-ribbon-paths-in-substance-3d-painter-adobe-substance-3d.md


### Substance 3D Painter & ACES - 02 - OCIO & ACEScg in Painter
- **Source:** YouTube
- **URL:** https://www.youtube.com/watch?v=WrFqBNI6Tx4
- **Author:** Adobe Substance 3D
- **App:** Substance 3D Painter
- **Version:** OCIO added in Painter 7.4.0 (2021) per version-tracker cross-check; demo project build not shown on screen, ACES 1.2 preinstalled
- **Tags:** `color-management` `texture-set` `basecolor` `roughness` `normal-map` `export` `export-preset`
- **Summary:** Part 2/3 of Michael Wilde's ACES series: hands-on Painter Color Management setup (New Project → OpenColorIO → ACES 1.0.3/1.2/Custom config, working color space auto-set to ACEScg), OCIO "roles" (Utility sRGB Texture vs. Utility Linear sRGB), the viewport display-transform toggle, Color Data vs. Scalar Data channel distinction (checked via Texture Set Settings' 3-sphere icon) and why the display transform disables on scalar-only views, per-resource color-space overrides for imported textures and HDRIs/Environments, and export color-space defaults (floating-point exports encode in linear ACEScg).
- **File:** tutorials/substance-3d-painter-aces---02---ocio-acescg-in-painter.md


### How to texture a realistic slipper model
- **Source:** YouTube
- **URL:** https://www.youtube.com/watch?v=U5CZJAKU47s
- **Author:** 3DRedBox
- **App:** Substance 3D Painter
- **Version:** not stated on screen; the stitching panel's "PAINT ALONG PATH" title pins this to the Painter 9.x-10.x window (renamed Filled Path in 11.0.0)
- **Tags:** `layers` `fill-layer` `paint-layer` `masks` `smart-material` `generator` `curvature` `anchor-point` `blend-mode` `ambient-occlusion` `mesh-maps` `baking` `texture-set` `uv` `pbr` `metal-rough` `basecolor` `roughness` `metallic` `height` `normal-map` `alpha` `procedural` `export-preset` `advanced`
- **Summary:** Full slipper texturing (plastic sole rebuilt from a trialed smart material, herringbone fabric upper, Paint-Along-Path seam stitching) whose second half is a deep-dive into building sole tread patterns, embossed logo/text, and clean borders entirely from stacked anchor-point-referenced "placeholder mask" layers (never rendered directly) plus a Bevel/Histogram-Scan/Mask-Outline filter chain, finished with a dual-reference (Height + Normal) Ambient Occlusion pass.
- **File:** tutorials/how-to-texture-a-realistic-slipper-model.md


### Texturing Creatures for Games in Substance Painter | Full Process
- **Source:** YouTube
- **URL:** https://www.youtube.com/watch?v=dHATe4tKd_Q
- **Author:** Logan Wiesen
- **App:** [PENDING]
- **Version:** [PENDING]
- **Tags:** [PENDING]
- **Summary:** [PENDING EXTRACTION]
- **File:** tutorials/texturing-creatures-for-games-in-substance-painter-full-process.md


### Substance 3D Painter & ACES - 03 - Textures in Maya and Blender | Adobe Substance 3D
- **Source:** YouTube
- **URL:** https://www.youtube.com/watch?v=Lksg6Fum3gw
- **Author:** Adobe Substance 3D
- **App:** Substance 3D Painter (export side) + Maya + Blender (import/render side)
- **Version:** Maya 2023 (inbuilt ACES) and Maya 2019 (manual ACES 1.2 config) both shown; Blender version not stated
- **Tags:** `color-management` `export` `export-preset` `udim` `basecolor` `roughness`
- **Summary:** Part 3/3 of Michael Wilde's ACES series: exporting ACEScg-authored Painter textures and matching the Painter viewport in Maya (Arnold Standard Surface, File node Color Space = Utility sRGB Texture for color data / Utility Raw for scalar / Utility Linear sRGB for HDRIs, UDIM tiling) and Blender (OS-level `OCIO` env var, Principled BSDF, same Utility role names), verified via AOV-isolated Base Color comparison in both. Closes the 3-part color-management sequence.
- **File:** tutorials/substance-3d-painter-aces---03---textures-in-maya-and-blender-adobe-substance-3d.md


### Texturing Stained Glass & Ceiling Paintings in Adobe Substance 3D Painter: Part 2 | Adobe
- **Source:** YouTube
- **URL:** https://www.youtube.com/watch?v=NCkQ1eq8a-o
- **Author:** Adobe Substance 3D
- **App:** Substance 3D Painter
- **Version:** not confirmed on-screen; published ~August 2025, likely 11.x/12.0.x era (approximate)
- **Tags:** `generator` `masks` `anchor-point` `opacity` `roughness` `metallic` `height` `normal-map` `path-tool` `procedural` `advanced`
- **Summary:** Part 2 of Adobe's Gothic Architecture series (Part 1: `UQkmXEWJr80`, also in this library). Stained-glass windows built with Path-tool curves, Bevel-generated anchor points driving dirt placement, a glass layer whose Opacity is driven by an exported frame-curves mask, a Tile-generator wireframe lattice fed by a Polygon-generator anchor point, and duplicated red/blue/green glass layers each masked by an exported luminance mask. Plus a fresco ceiling painting (Adobe Stock image, UV-projected) aged with the Peeling Paint filter and an Ambient Occlusion filter for depth.
- **File:** tutorials/texturing-stained-glass-ceiling-paintings-in-adobe-substance-3d-painter-part-2-a.md

### Texturing Creatures for Games in Substance Painter | Full Process
- **Source:** YouTube
- **URL:** https://www.youtube.com/watch?v=dHATe4tKd_Q
- **Author:** Logan Wiesen
- **App:** Substance 3D Painter
- **Version:** not specified (modern Baking Mode UI)
- **Tags:** `layers` `fill-layer` `paint-layer` `masks` `baking` `mesh-maps` `curvature` `ambient-occlusion` `thickness` `world-space-normal` `position-map` `id-map` `blend-mode` `procedural` `tri-planar` `basecolor` `roughness` `normal-map` `color-management` `texture-set` `export` `advanced`
- **Summary:** Full real-time creature texturing pipeline: bake curvature/AO/thickness/normal from a high-poly ZBrush sculpt, layer those baked maps as color-driving utility layers (thickness tinted red + Multiply for blood-flow color), then build organic skin variation through hand-painted yellow/blue/red/green anatomical color-temperature layers integrated with tri-planar procedural grunge breakup, validated via a Color+Normal export-to-Blender/EEVEE feedback loop with Subsurface Scattering.
- **File:** tutorials/texturing-creatures-for-games-in-substance-painter-full-process.md


### Hero Assets for Fashion - 06 - Asset Texturing and Presentation | Adobe Substance 3D
- **Source:** YouTube
- **URL:** https://www.youtube.com/watch?v=us4NAWtaRic
- **Author:** Adobe Substance 3D
- **App:** Substance 3D Painter (texturing) + Substance 3D Stager (rendering/presentation)
- **Version:** not stated on screen
- **Tags:** `layers` `fill-layer` `paint-layer` `masks` `generator` `blend-mode` `baking` `texture-set` `udim` `uv` `pbr` `metal-rough` `basecolor` `roughness` `height` `normal-map` `opacity` `mesh-maps` `ambient-occlusion` `curvature` `position-map` `high-to-low-poly` `procedural` `alpha` `export` `export-preset` `channel-packing` `intermediate` `advanced`
- **Summary:** Chapter 6/6 (only Painter-relevant chapter; 1-5 are Designer/Sampler and out of scope) of Adobe's Hero Assets for Fashion series. Fully parametric (non-sculpted) dress fabric detailing: large/medium/small creases via fill layers + UV Border Distance generators + procedural noises + imported sculpt-displacement maps, French-seam flattening (Replace blend mode), Inflate/Shrink Wrap filter, Adobe-Stock crease overlay, and fully procedural stitching (two subtracted UV Border Distance generators + breakup texture) vs. Painter's built-in Stitching brush tool for manual precision work. Second half hands off to Substance 3D Stager for 3-point lighting, backdrop, camera setup, per-UV-tile map tweaks, and final PSD render.
- **File:** tutorials/hero-assets-for-fashion---06---asset-texturing-and-presentation-adobe-substance-.md


### Texturing a Worn Wooden Stool in Substance Painter 🪑
- **Source:** YouTube
- **URL:** https://www.youtube.com/watch?v=sa_5vS4s_M0
- **Author:** 3DRedBox
- **App:** Substance 3D Painter
- **Version:** not stated on screen; UI consistent with the pre-11.0-era seen in this creator's other videos
- **Tags:** `layers` `fill-layer` `paint-layer` `masks` `smart-material` `generator` `curvature` `anchor-point` `blend-mode` `baking` `mesh-maps` `ambient-occlusion` `texture-set` `uv` `pbr` `metal-rough` `basecolor` `roughness` `metallic` `height` `normal-map` `alpha` `procedural` `intermediate` `advanced`
- **Summary:** Weathered rattan-and-wood stool texturing: an overlapping-UV texel-density trick for small repeated pieces (DCC-side), a smart-material-derived wood base rebuilt into fiber/edge-wear/dirt/damage passes, a compound dual-3D-Linear-Gradient dark-area mask combined via Linear Dodge and refined with an anchor-point-referenced multiply plus hand painting, a from-scratch forced-Normal-blend "underlayer wood" material with an anchor-point-driven Soft-Light border-effect for damage edges, and a Silver-Armor-based steel material for the joinery.
- **File:** tutorials/texturing-a-worn-wooden-stool-in-substance-painter.md


### Hand Painted Workflow in Substance 3D Painter | Adobe Substance 3D
- **Source:** YouTube
- **URL:** https://www.youtube.com/watch?v=8biEy1D30Bc
- **Author:** Adobe Substance 3D
- **App:** Substance 3D Painter
- **Version:** 11.0.0+ (AutoCage feature usage confirms this floor per release-notes-painter-11.0.md)
- **Tags:** `generator` `masks` `anchor-point` `blend-mode` `ambient-occlusion` `thickness` `position-map` `high-to-low-poly` `cage` `basecolor` `procedural` `alpha` `advanced`
- **Summary:** Full value-first hand-painted pipeline on a zombie shark character: AutoCage-assisted baking, a black-and-white value map built purely from generators (AO/Light/Position), grouping the values and creating an anchor point from the group, converting that anchor point to full color via the Gradient filter, per-part local color values, the new Stylization filters as an optional inspiration pass, and finally freehand painting on top (square alpha, pen-pressure-on-opacity brush setup).
- **File:** tutorials/hand-painted-workflow-in-substance-3d-painter-adobe-substance-3d.md

### Complex Wooden Medieval Door Tutorial in Substance 3D Painter
- **Source:** YouTube
- **URL:** https://www.youtube.com/watch?v=cRKK4YOXLtQ
- **Author:** Abe Leal 3D
- **App:** Substance 3D Painter
- **Version:** 11.0.0+ (Auto-Cage baking, Assets auto-update, and Bevel Smooth filter all confirmed on-screen — all introduced in 11.0.0 per release-notes-painter-11.0.md)
- **Tags:** `layers` `fill-layer` `paint-layer` `masks` `generator` `anchor-point` `blend-mode` `baking` `mesh-maps` `ambient-occlusion` `curvature` `thickness` `world-space-normal` `position-map` `high-to-low-poly` `cage` `udim` `texture-set` `procedural` `tri-planar` `alpha` `height` `roughness` `metallic` `basecolor` `MatFX` `advanced`
- **Summary:** Adobe-sponsored showcase of fully non-destructive procedural "carving" for a multi-UDIM medieval door: Auto-Cage baking, a live-linked Photoshop-authored height-carving mask (Blur -> Bevel Smooth -> Blur Slope filter chain), a folder-level Anchor Point wired into downstream dirt/edge-wear generators' Micro Normal/Height so they correctly read into the carved crevices, Position-generator-driven moss placement, and a thickness-map-driven simulated subsurface-glow finishing trick.
- **File:** tutorials/complex-wooden-medieval-door-tutorial-in-substance-3d-painter.md


### Create Trim Sheets in Substance 3D Painter - Part 1 | Adobe Substance 3D
- **Source:** YouTube
- **URL:** https://www.youtube.com/watch?v=dE4LWGMwypc
- **Author:** Adobe Substance 3D
- **App:** Substance 3D Painter
- **Version:** not stated on screen
- **Tags:** `layers` `fill-layer` `paint-layer` `masks` `generator` `anchor-point` `blend-mode` `texture-set` `pbr` `metal-rough` `basecolor` `height` `normal-map` `opacity` `alpha` `procedural` `game-engine` `unreal-export` `intermediate` `advanced`
- **Summary:** Part 1/2 of Adobe's Create Trim Sheets series (sci-fi corridor trim sheet). Builds a Color ID map (per-zone fill layers painted via the Polygon Fill Tool, one Anchor Point per mask for later reference), then two normal-detail techniques: height-based construction lines/rivets via the Tile Generator (Capsule pattern) constrained by an anchor-referenced Levels/Multiply mask, and true normal-map decal placement via the Projection tool + auto-generated Opacity-driven cutout masks for reuse as real decal geometry in Unreal Engine. Note: this video's Whisper transcript came back mis-detected as Dutch — Structured Notes were reconstructed from surviving English technical terms cross-checked against captured frames.
- **File:** tutorials/create-trim-sheets-in-substance-3d-painter---part-1-adobe-substance-3d.md


### Texturing Gothic Architecture in Substance 3D Painter: Part 1 | Adobe
- **Source:** YouTube
- **URL:** https://www.youtube.com/watch?v=UQkmXEWJr80
- **Author:** Adobe Substance 3D
- **App:** Substance 3D Painter
- **Version:** 11.0.0+
- **Tags:** `generator` `masks` `anchor-point` `path-tool` `height` `curvature` `procedural` `intermediate` `advanced`
- **Summary:** Part 1 of Adobe's two-part Gothic Architecture series (Part 2, "Texturing Stained Glass & Ceiling Paintings," `NCkQ1eq8a-o`, also in this library). Full stonework pass on a Gothic hallway: reusable Concrete Cast base with a Curvature-generator mask for fake bevels, stacked Dirt/Moss/Stains-Scratches generator layers for aging, a Plastic Tool-Worn smart material swap (Marble Vane) for roof tiles, hand-painted drip stains shaped with the Directional Distance filter, a Height-only Brick generator reused at three scales (walls, anchor-point-masked ground, scaled-up columns), and Path-tool-drawn decorative relief (Gothic "keld cross"/floral patterns) finished with a Bevel Smooth filter. Version floor 11.0.0+ confirmed via two independent filter names (Directional Distance, Bevel Smooth) matching release-notes-painter-11.0.md.
- **File:** tutorials/texturing-gothic-architecture-in-substance-3d-painter-part-1-adobe.md


### 🎨 Texturing Women's Shorts with Lace Trim in Substance Painter 🎨
- **Source:** YouTube
- **URL:** https://www.youtube.com/watch?v=6eRY49oxJNI
- **Author:** 3DRedBox
- **App:** Substance 3D Painter
- **Version:** not stated on screen; UI consistent with the pre-12.1-era seen across this creator's other videos
- **Tags:** `layers` `fill-layer` `paint-layer` `masks` `generator` `anchor-point` `blend-mode` `alpha` `procedural` `basecolor` `roughness` `height` `normal-map` `opacity` `metallic` `smart-material` `texture-set` `iray-render` `viewport` `intermediate` `advanced`
- **Summary:** Garment texturing (floral AI-generated pattern + crochet lace trim) starting from viewport/shader calibration (ACES tone mapping, Bent Normal, Alpha Blending), Marvelous-Designer-baked wrinkle alphas applied as Height data and routed through a Pass-Through Height-to-Normal effect layer via a channel-specific (not layer-wide) blend-mode trick, an AI-generated tiling pattern masked by an anchor-point-referenced UV-island selection, and an opacity-channel-driven lace decal system (two variants combined via Linear Dodge, sharpened with a Levels-on-Opacity filter) duplicated across every strap via anchor points instead of layer copies.
- **File:** tutorials/texturing-womens-shorts-with-lace-trim-in-substance-painter.md

### Paint On Baked Maps To Fix Issues | Substance Painter
- **Source:** YouTube
- **URL:** https://www.youtube.com/watch?v=oRkgEuGKPtw
- **Author:** Stu Lloyd (CG Stu)
- **App:** Substance 3D Painter (Steam Edition)
- **Version:** not specified beyond "Steam Edition" (confirmed in title bar)
- **Tags:** `layers` `fill-layer` `paint-layer` `masks` `baking` `mesh-maps` `ambient-occlusion` `normal-map` `uv` `texture-set` `blend-mode` `alpha` `color-management` `intermediate`
- **Summary:** Focused problem-solving tutorial on hand-repairing baked-map artifacts (AO and Normal) directly in the layer stack without re-baking: expose AO/Normal as Replace-mode channels, rebuild a base fill from the real baked map, then use a Fill-layer-holding-the-baked-map + Pass-Through paint layer trick so Clone Stamp/Blur/Smudge brushes sample and repair the actual baked data instead of a transparent layer. Demonstrated fixing dodgy eye-socket AO blotches and warped normal-map edges.
- **File:** tutorials/paint-on-baked-maps-to-fix-issues-substance-painter.md


### Create Trim Sheets in Substance 3D Painter - Part2 | Adobe Substance 3D
- **Source:** YouTube
- **URL:** https://www.youtube.com/watch?v=QoVWM-IKmFw
- **Author:** Adobe Substance 3D
- **App:** Substance 3D Painter + Unreal Engine (final scene) + 3ds Max (UV unwrap)
- **Version:** not stated on screen
- **Tags:** `layers` `fill-layer` `masks` `generator` `anchor-point` `smart-material` `blend-mode` `curvature` `ambient-occlusion` `pbr` `metal-rough` `basecolor` `roughness` `metallic` `height` `normal-map` `opacity` `alpha` `procedural` `uv` `game-engine` `unreal-export` `advanced`
- **Summary:** Part 2/2 of Adobe's Create Trim Sheets series. Finishes the trim sheet's base color pass entirely with Anchor-Point-referenced fill layers (masking every zone from Part 1's Color ID map, combined via Add/Linear Dodge blend mode), builds a proper decal cutout (Opacity-only Cutout layer + Extract Alpha), adds text decals with grunge breakup, and introduces a "Master Anchor" (pass-through filter + anchor point combining all normal/height details) referenced by Micro Normal/Micro Height fields on Dirt (Sharp Dirt smart material) and Edge Highlights (Curvature generator) layers. Closes with the finished trim sheet's UV unwrap in 3ds Max and full deployment across a real-time Unreal Engine 5 sci-fi corridor scene.
- **File:** tutorials/create-trim-sheets-in-substance-3d-painter---part2-adobe-substance-3d.md


### Substance Painter Tutorial: Texturing the Coin
- **Source:** YouTube
- **URL:** https://www.youtube.com/watch?v=7kV4Q4UBvl4
- **Author:** Abe Leal 3D
- **App:** Substance 3D Painter
- **Version:** not stated on screen; UI consistent with this creator's other ingested 11.0.0+-pinned tutorial, tentative
- **Tags:** `layers` `fill-layer` `masks` `generator` `baking` `mesh-maps` `ambient-occlusion` `curvature` `cage` `texture-set` `pbr` `metal-rough` `basecolor` `roughness` `metallic` `height` `alpha` `procedural` `blend-mode` `export` `export-preset` `game-engine` `unreal-export` `intermediate`
- **Summary:** Small game-prop pipeline (brief Maya retopology/UVs, then Painter baking+texturing) for a treasure coin: bakes 4 duplicate low-polys into one Texture Set so procedural rust/wear/scratch mask stacks (Dirt generator, tileable grunge masks, Metal Edge Wear generator, Clouds, scratch masks, AO-driven cavity rust with inverted Levels) read differently per coin from shared settings alone, no per-coin hand-painting. Includes an Alt+click channel-isolation UI tip and export to Unreal Engine.
- **File:** tutorials/substance-painter-tutorial-texturing-the-coin.md


### Stylized Asset Setup in Painter: Auto-Cage, PSD Workflows & Smart Detailing | Adobe Substance 3D
- **Source:** YouTube
- **URL:** https://www.youtube.com/watch?v=LRy-Nc7B_bk
- **Author:** Adobe Substance 3D
- **App:** Substance 3D Painter
- **Version:** 11.0.0+
- **Tags:** `mesh-maps` `high-to-low-poly` `cage` `generator` `masks` `height` `path-tool` `procedural` `intermediate`
- **Summary:** Foundation-setup video (no painting yet) covering Auto-Cage baking (adaptive cage that eliminates manual tightness tuning against red "matching error" artifacts), a PSD-based Auto-Update texture pipeline (edit in Photoshop, refresh instantly everywhere in Painter), and a height-only Path-tool + Smooth Bevel filter trick for sculpting stylized rim ornaments using only texture. Version floor 11.0.0+ confirmed via three independent markers (Auto-Cage, Auto-Update, Smooth Bevel filter) matching release-notes-painter-11.0.md.
- **File:** tutorials/stylized-asset-setup-in-painter-auto-cage-psd-workflows-smart-detailing-adobe-su.md


### Texturing an ornate sword in Substance 3D Painter | Adobe Substance 3D
- **Source:** YouTube
- **URL:** https://www.youtube.com/watch?v=944ci1laePI
- **Author:** Adobe Substance 3D
- **App:** Substance 3D Designer (base material) + Substance 3D Painter (texturing) + Substance 3D Stager (handoff)
- **Version:** not stated on screen
- **Tags:** `layers` `fill-layer` `paint-layer` `masks` `smart-material` `generator` `anchor-point` `blend-mode` `curvature` `ambient-occlusion` `mesh-maps` `texture-set` `pbr` `metal-rough` `basecolor` `roughness` `height` `normal-map` `alpha` `procedural` `tri-planar` `export` `intermediate` `advanced`
- **Summary:** Lion's-head sword-ornament texturing demonstrating Designer-vs-Painter division of labor: a Damascene gold material authored in Designer (Tile Sampler punch marks) sent to Painter, Tri-Planar projection fixing UV seam issues on an organic sculpt, multi-pass AO-generator-masked rust weathering (three duplicated/varied passes plus hand-painted cleanup), Smart-Material-driven iris construction, and an anchor-point-plus-Subtract-blend-mode technique for carved relief (iris rim, facial crack) reused from Jared Chavez's dedicated anchor-point tutorial. Ornament bands hand-carved with Lazy Mouse. Closes with one-click Send to Stager handoff.
- **File:** tutorials/texturing-an-ornate-sword-in-substance-3d-painter-adobe-substance-3d.md


### How to Create a Realistic Poison Bottles Material Using Substance Painter
- **Source:** YouTube
- **URL:** https://www.youtube.com/watch?v=386o64sxSpw
- **Author:** 3DRedBox
- **App:** Substance 3D Painter
- **Version:** not stated on screen; "PAINT ALONG PATH" tool panel pins this to the Painter 9.x-10.x window
- **Tags:** `layers` `fill-layer` `paint-layer` `masks` `generator` `anchor-point` `blend-mode` `alpha` `procedural` `MatFX` `texture-set` `uv` `pbr` `metal-rough` `basecolor` `roughness` `metallic` `height` `normal-map` `opacity` `ambient-occlusion` `mesh-maps` `export` `export-preset` `channel-packing` `iray-render` `advanced`
- **Summary:** Glass-bottle texturing: a Translucency/Absorption-channel glass shader handed off to Marmoset Toolbag for a ray-traced glass render, ornate carved-ornament detail built from alphas plus a custom Pass-tool brush with radial symmetry, and anchor-point-driven mask reuse across separate folders — a Pass-Through "Ornament Plus" collector layer feeds the carved-detail height data into every generator inside the metal smart material, and the Glass folder subtracts all four ornament masks so the etched pattern reads through the glass too.
- **File:** tutorials/how-to-create-a-realistic-poison-bottles-material-using-substance-painter.md


### Texturing a Cyberpunk Building in Substance 3D Painter – Project Breakdown | Adobe Substance 3D
- **Source:** YouTube
- **URL:** https://www.youtube.com/watch?v=gv9R6a6VPYQ
- **Author:** Adobe Substance 3D
- **App:** Substance 3D Painter
- **Version:** not stated on screen
- **Tags:** `layers` `fill-layer` `masks` `generator` `anchor-point` `blend-mode` `height` `basecolor` `roughness` `metallic` `emissive` `alpha` `procedural` `viewport` `advanced`
- **Summary:** Fast-paced full-building project breakdown covering layered brick walls (concrete+terracotta base, inverted brick mask, height-boosted duplicate, hand-erased "fallen off" bricks), concrete elements (Plastic Dusty smart material reuse, engraved-height anchor-point-linked dirt masks), a stacked-fabric awning pattern, neon emissive signage (Emissive channel + Emissive Intensity + viewport Glare), tri-planar-projected checker tile flooring, and a hand-painted footprint rug detail. Anchor points referred to as "ankle points" in the Whisper transcript (mis-transcription). No version-gated features referenced — version not pinned.
- **File:** tutorials/texturing-a-cyberpunk-building-in-substance-3d-painter-project-breakdown-adobe-s.md


### Preparing Models for Substance 3D Painter in Blender | Adobe Substance 3D
- **Source:** YouTube
- **URL:** https://www.youtube.com/watch?v=jCwTEEyDX3Y
- **Author:** Adobe Substance 3D
- **App:** Blender (model prep) + Substance 3D Painter (import/baking)
- **Version:** not stated on screen
- **Tags:** `texture-set` `uv` `id-map` `mesh-maps` `baking` `beginner`
- **Summary:** 1/3 of a cross-DCC prep series (Blender/Maya/3DS Max). Explains Painter's three model-splitting mechanisms — Texture Sets (auto-named from source-app materials), Geometry Masks (sub-mesh membership), ID Maps (baked per-region data for Ctrl+drag material assignment) — and Auto-UV Unwrap (cut/unfold/pack, preserves existing UV data). Demoed in Blender on a roller skate: material-per-texture-set assignment, UV repacking (Blender Pack UVs or Painter's Recompute Only the Packing), vertex-color ID-map painting + Painter's Baker ID-tab Vertex Color bake, and mesh separation (P) for geometry masks.
- **File:** tutorials/preparing-models-for-substance-3d-painter-in-blender-adobe-substance-3d.md


### Substance Painter Tutorial for Beginners - Texturing A Rock 3D Model
- **Source:** YouTube
- **URL:** https://www.youtube.com/watch?v=hKg_N96EUjA
- **Author:** 3DWolf
- **App:** Substance 3D Painter (Substance Edition)
- **Version:** not stated on screen beyond "Substance Edition"
- **Tags:** `layers` `fill-layer` `masks` `generator` `smart-mask` `curvature` `texture-set` `pbr` `roughness` `height` `basecolor` `tri-planar` `procedural` `alpha` `blend-mode` `beginner`
- **Summary:** Short beginner rock-column texturing pass: Tri-Planar concrete base, Curvature-generator edge lightening, channel-restricted (height/roughness-only) Fill layers for surface detail and scratches, a Rust Coarse smart material driven by the built-in Ground Dirt Smart Mask, a Dirt-generator broad-rust pass, and a hand-painted mask confining a Large Rust Leaks streak texture to specific faces.
- **File:** tutorials/substance-painter-tutorial-for-beginners---texturing-a-rock-3d-model.md


### Advanced Peeling Paint Effect in Substance 3D Painter
- **Source:** YouTube
- **URL:** https://www.youtube.com/watch?v=VE8aILV053Y
- **Author:** Javad Rajabzade
- **App:** Substance 3D Painter
- **Version:** not stated on screen; UDIM multi-tile workflow and modern generator/anchor-point UI, tentative
- **Tags:** `layers` `fill-layer` `paint-layer` `masks` `generator` `anchor-point` `blend-mode` `height` `roughness` `basecolor` `alpha` `procedural` `udim` `texture-set` `intermediate` `advanced`
- **Summary:** Advanced fully-procedural peeling/blistering paint mask on a fire hydrant: Metal Edge Wear generator + blurred companion combined via Lighten, 3D Voronoi Fractal noise combined via Divide, a Levels-invert/Histogram-Shift/Levels cleanup chain, captured as an Anchor Point referenced by a paint-color layer, an edge-detail pass, and a Bevel-filter erosion trick. Introduces a paint-driven "reveal window" (black-mask paint layer + generator set to Multiply Light) to confine uniform procedural wear to hand-painted areas only.
- **File:** tutorials/advanced-peeling-paint-effect-in-substance-3d-painter.md


### Preparing Models for Substance 3D Painter in Maya | Adobe Substance 3D
- **Source:** YouTube
- **URL:** https://www.youtube.com/watch?v=Gkx96GEextY
- **Author:** Adobe Substance 3D
- **App:** Maya (model prep) + Substance 3D Painter (import/baking)
- **Version:** not stated on screen
- **Tags:** `texture-set` `uv` `id-map` `mesh-maps` `baking` `beginner`
- **Summary:** 2/3 of the cross-DCC prep series (same roller-skate asset as the Blender entry). Maya-side Texture Set/Geometry Mask/ID Map workflow: right-click Assign New Material per texture set, UV Toolkit Layout with shell/tile padding (or Painter's Auto Unwrap regenerate-packing option), Vertex Color-based ID maps (Mesh Display → Apply Color, distinct from material assignment) baked in Painter's Bake Maps ID tab, and geometry masking via face Extract into new objects.
- **File:** tutorials/preparing-models-for-substance-3d-painter-in-maya-adobe-substance-3d.md


### Speed Up Your Substance Painter Workflow with This Easy Trick!
- **Source:** YouTube
- **URL:** https://www.youtube.com/watch?v=_oSPDoX37lM
- **Author:** 3DRedBox
- **App:** Substance 3D Painter
- **Version:** not stated on screen; "PAINT ALONG PATH" tool panel pins this to the Painter 9.x-10.x window
- **Tags:** `layers` `fill-layer` `paint-layer` `masks` `smart-material` `blend-mode` `baking` `mesh-maps` `ambient-occlusion` `texture-set` `pbr` `metal-rough` `basecolor` `roughness` `height` `normal-map` `alpha` `beginner` `intermediate`
- **Summary:** Short troubleshooting technique for the Pass tool (Paint Along Path) mis-detecting neighboring geometry on complex models with tightly-packed closed surfaces: after baking, duplicate the mesh in the DCC app, detach and spatially "explode" its small pieces apart (without touching materials/UVs), re-import via Project Configuration to paint detail cleanly on isolated surfaces, temporarily drop the Ambient Occlusion channel to suppress spacing-mismatch artifacts, then switch back to the original mesh for final render.
- **File:** tutorials/speed-up-your-substance-painter-workflow-with-this-easy-trick.md


### Creating & Reusing Smart Materials in Substance 3D Painter | Stylized Crab | Adobe Substance 3D
- **Source:** YouTube
- **URL:** https://www.youtube.com/watch?v=ZiWAe_iZ_CI
- **Author:** Adobe Substance 3D
- **App:** Substance 3D Painter
- **Version:** 11.0.0+
- **Tags:** `layers` `fill-layer` `masks` `smart-material` `generator` `anchor-point` `blend-mode` `curvature` `tri-planar` `procedural` `texture-set` `basecolor` `intermediate` `advanced`
- **Summary:** Converts a hand-built, project-specific stylized-crab shell material into a portable, reusable Smart Material: layer-renaming hygiene, tri-planar-projected mask textures for UV-independence, swapping hand-painted UV-specific layers for empty placeholder paint layers, then right-click → Create Smart Material. Demonstrates dragging the result onto multiple meshes and a brand-new project, re-skinning via folder-level Gradient/HSL Perception filters, and propagating tweaks project-wide via Instantiate across Texture Sets. Version floor 11.0.0+ confirmed via an explicit name-check of the "6 new filters" batch matching release-notes-painter-11.0.md.
- **File:** tutorials/creating-reusing-smart-materials-in-substance-3d-painter-stylized-crab-adobe-sub.md


### Preparing Models for Substance 3D Painter in 3DS Max | Adobe Substance 3D
- **Source:** YouTube
- **URL:** https://www.youtube.com/watch?v=xuLRnFBvLyI
- **Author:** Adobe Substance 3D
- **App:** 3ds Max 2022 (model prep) + Substance 3D Painter (import/baking)
- **Version:** 3ds Max 2022 confirmed on screen; Painter version not stated
- **Tags:** `texture-set` `uv` `id-map` `mesh-maps` `baking` `beginner`
- **Summary:** 3/3 of the cross-DCC prep series (same roller-skate asset as Blender/Maya entries). 3ds Max-side Texture Set/Geometry Mask/ID Map workflow: Compact Material Editor per-texture-set material assignment, Unwrap UVW + Arrange Elements UV packing (or Painter's Auto Unwrap regenerate-packing option), Vertex Paint modifier-based ID maps (Fill/Paint tools, remember to disable vertex color display before exiting) baked via Painter's Baking dialog ID Color Source, and Edit Poly + Detach for geometry-mask sub-objects.
- **File:** tutorials/preparing-models-for-substance-3d-painter-in-3ds-max-adobe-substance-3d.md


### 3Dconnexion SpaceMouse in Substance 3D Painter | Adobe Substance 3D
- **Source:** YouTube
- **URL:** https://www.youtube.com/watch?v=PvZYHYQ3_uc
- **Author:** Adobe Substance 3D
- **App:** Substance 3D Painter
- **Version:** not stated on screen; SpaceMouse support introduced in Painter 8.0.0
- **Tags:** `viewport` `beginner`
- **Summary:** Short hardware tip: configuring a 3Dconnexion SpaceMouse (all models natively supported) via the separate 3Dconnexion Settings app — Navigation Mode (Object/Camera/Helicopter + Lock Horizon), Rotation Center pivot behavior, and Buttons (radial menus on Compact, direct Painter keyboard-shortcut binding on Enterprise/Pro). Notes Painter can't navigate via SpaceMouse and paint with mouse/tablet simultaneously.
- **File:** tutorials/3dconnexion-spacemouse-in-substance-3d-painter-adobe-substance-3d.md


### How to create a paint peeling effect in Substance Painter
- **Source:** YouTube
- **URL:** https://www.youtube.com/watch?v=JnWvMys9xNk
- **Author:** Wes McDermott
- **App:** Substance 3D Painter
- **Version:** not stated on screen; creator notes filter-native blend modes as a then-recent feature, tentative
- **Tags:** `layers` `fill-layer` `paint-layer` `masks` `generator` `anchor-point` `blend-mode` `ambient-occlusion` `MatFX` `height` `roughness` `basecolor` `alpha` `procedural` `tri-planar` `smart-material` `texture-set` `intermediate` `advanced`
- **Summary:** Exhaustive from-scratch build of a reusable Paint Peeling Smart Material: a dirt-generator+grunge mask stack sculpted via Blur/Levels/Warp/Slope-Blur (Warp and Slope Blur using filter-native blend modes Multiply/Min with Perlin noise), captured once as an Anchor Point and referenced by 4 downstream layers (cracks-inside subtraction, a Mask-Outline-driven peel-height layer, a colored Peel Edge accent, and manual paint control), finished with HBAO ambient occlusion and gradient-remapped color variation.
- **File:** tutorials/how-to-create-a-paint-peeling-effect-in-substance-painter.md


### Footwear Texturing from Start to Finish – Live Tutorial in Substance 3D Painter | Adobe Substance 3D
- **Source:** YouTube
- **URL:** https://www.youtube.com/watch?v=s59xbaF4Q14
- **Author:** Adobe Substance 3D
- **App:** Substance 3D Painter
- **Version:** not stated on screen
- **Tags:** `layers` `fill-layer` `masks` `blend-mode` `texture-set` `pbr` `roughness` `height` `normal-map` `emissive` `stencil` `alpha` `uv` `viewport` `intermediate`
- **Summary:** Live project breakdown for a performance-inspired sneaker: rapid material assignment (leather/fabric/plastic/knit/vinyl/carbon fiber) with a small consistent palette, reused across parts via copy → Paste Layer as Instance rather than re-tuning. Adds Emissive-channel glow to vinyl accent panels, layered Multiply/Screen blend-mode surface flecks, a Height-slider logo emboss/deboss, and a hexagon-stencil-masked outsole detail. Whisper mis-detected large transcript stretches as Arabic — notes reconstructed from clear English fragments + frames, same approach as the Create Trim Sheets Part 1 tutorial. Version not stated on screen.
- **File:** tutorials/footwear-texturing-from-start-to-finish-live-tutorial-in-substance-3d-painter-ad.md


### Creating Fabric stitches for Footwear with Anchor Points in Substance 3D Painter | Substance 3D
- **Source:** YouTube
- **URL:** https://www.youtube.com/watch?v=dIO6cJiE7JM
- **Author:** Adobe Substance 3D
- **App:** Substance 3D Painter
- **Version:** not stated on screen
- **Tags:** `anchor-point` `masks` `layers` `fill-layer` `paint-layer` `blend-mode` `height` `basecolor` `roughness` `alpha` `particle-brush` `intermediate`
- **Summary:** 1/3 of a footwear anchor-points series. Paints stitches with the built-in Stitches brush on a base layer, adds an Anchor Point, then builds a Deform layer (negative Height, anchor-referenced mask with Extract Alpha, double-blur transition trick) and a Color layer (Base Color+Roughness, same anchor referencing) — both automatically apply to any future stroke on the base layer, demonstrated by swapping in a different brush for a plain seam line that still gets the same denting/color treatment. Also shows isolating mesh parts (e.g. hiding laces) while painting.
- **File:** tutorials/creating-fabric-stitches-for-footwear-with-anchor-points-in-substance-3d-painter.md


### How to use UDIMs properly!
- **Source:** YouTube
- **URL:** https://www.youtube.com/watch?v=yf9CPHE5BYg
- **Author:** 3DRedBox
- **App:** Substance 3D Painter (Painter-side portion only; most of the video is RizomUV)
- **Version:** not stated on screen; no version-specific UI markers in the Painter-side portion
- **Tags:** `udim` `texture-set` `uv` `texel-density` `generator` `layers` `paint-layer` `basecolor`
- **Summary:** Mostly a RizomUV UV-packing tutorial (via 3ds Max bridge) on keeping texel density consistent across every UV island in a UDIM/UV-Tile layout — Map Res + Texel-Density-Target-derived packing, Initial Scale set to Texel Density with Scale Optimization off — closing with a Substance-Painter-side verification step using the built-in `UV Texel Density` generator (red/green/blue quality heatmap) to confirm the imported UVs actually support the intended export resolution.
- **File:** tutorials/how-to-use-udims-properly.md


### Realistic Texturing Tips in Substance Painter
- **Source:** YouTube
- **URL:** https://www.youtube.com/watch?v=_qirDRMN1WI
- **Author:** FastTrack Tutorials
- **App:** Substance 3D Painter
- **Version:** not stated on screen
- **Tags:** `layers` `fill-layer` `masks` `generator` `blend-mode` `roughness` `basecolor` `metallic` `height` `alpha` `procedural` `texture-set` `intermediate`
- **Summary:** Five realism tips on a stacked metal pot, all from stock procedural maps: noise-driven roughness/color breakup with channel blend mode set to Overlay, a hand-painted multi-color heat-discoloration gradient, layered grime (Dirt generators, Moisture noise, Galvanic Large, Multiply/Subtract) with manual brush cleanup, procedural dents from inverted Cells/Clouds noise, and a dried-drip stain using Painter's built-in Leak Small texture.
- **File:** tutorials/realistic-texturing-tips-in-substance-painter.md


### Creating Sole Patterns for Footwear with Anchor Points in Substance 3D Painter | Adobe Substance 3D
- **Source:** YouTube
- **URL:** https://www.youtube.com/watch?v=AoGXdldOWQA
- **Author:** Adobe Substance 3D
- **App:** Substance 3D Painter
- **Version:** not stated on screen
- **Tags:** `anchor-point` `masks` `layers` `fill-layer` `paint-layer` `blend-mode` `height` `basecolor` `roughness` `procedural` `alpha` `intermediate`
- **Summary:** 2/3 of the footwear anchor-points series. Hand-paints a sole shape (negative-Height fill + Blur-smoothed mask), adds an Anchor Point, then chains it through a Sole Color layer (anchor-referenced mask + Levels cleanup) and a Pattern layer (tiled library pattern, Height-channel mask set to Max/Lighten blend so it only raises detail, confined to the sole via a second anchor-referenced Multiply mask) plus an independent Pattern Color pass via a second anchor point. Viewport Displacement/Tessellation enabled as a sculpting aid.
- **File:** tutorials/creating-sole-patterns-for-footwear-with-anchor-points-in-substance-3d-painter-a.md


### 6 Powerful New Filters in Substance 3D Painter | Adobe Substance 3D
- **Source:** YouTube
- **URL:** https://www.youtube.com/watch?v=aCi0RG9-9so
- **Author:** Adobe Substance 3D
- **App:** Substance 3D Painter
- **Version:** 11.0.0
- **Tags:** `layers` `masks` `generator` `anchor-point` `procedural` `height` `alpha` `basecolor` `roughness` `normal-map` `viewport` `intermediate` `advanced`
- **Summary:** Official Adobe feature-tour of the "6 new filters" batch: Anisotropic Kuwahara (edge-preserving stylized blur), Bevel Smooth (pixel-artifact-free bevels on Height layers/masks), Directional Distance (UV-space directional drips/smears), Grayscale Conversion (color-to-mask derivation), Quantize (posterized/vector flat-shading — confirmed parameters Color Amount/Contour Smoothing/Dithering/Distance Color Space/Apply To Alpha/Alpha Threshold), and Stylization (full hand-painted asset conversion). This is the primary/authoritative 11.0.0 version-pin source cited by several other tutorials in this library.
- **File:** tutorials/6-powerful-new-filters-in-substance-3d-painter-adobe-substance-3d.md


### Texturing a Clicker - FULL Substance 3D Painter Workflow
- **Source:** YouTube
- **URL:** https://www.youtube.com/watch?v=RTvgwZj-5Rw
- **Author:** FlippedNormals
- **App:** Substance 3D Painter
- **Version:** not stated numerically; baker and brush-favoriting called out as "new"/"fairly new" features, tentative
- **Tags:** `layers` `fill-layer` `paint-layer` `masks` `generator` `curvature` `ambient-occlusion` `mesh-maps` `world-space-normal` `position-map` `high-to-low-poly` `baking` `cage` `udim` `texture-set` `uv` `pbr` `basecolor` `roughness` `height` `alpha` `procedural` `tri-planar` `blend-mode` `iray-render` `viewport` `color-management` `advanced`
- **Summary:** Professional creature-texturing workflow on a fan-sculpted Clicker (The Last of Us) bust: per-channel-separated layer groups (Color vs. Roughness), curvature/AO-driven procedural masks combined with deliberate hand-painting, iterative Iray/external-render feedback as a mandatory checkpoint, Tri-Planar marble noise for organic skin, a combined-Color+Roughness exception for blood, an AO-hand-correction-then-Curvature-then-Levels mask chain for mushroom growths, and a Polygon Fill Tool UV-mode click-to-mask trick for per-tooth variation.
- **File:** tutorials/texturing-a-clicker---full-substance-3d-painter-workflow.md


### Texturing a shawl in substance painter
- **Source:** YouTube
- **URL:** https://www.youtube.com/watch?v=urA-oaoqfpM
- **Author:** 3DRedBox
- **App:** Substance 3D Painter
- **Version:** not stated on screen; UI consistent with the pre-12.1-era seen across this creator's other videos
- **Tags:** `layers` `fill-layer` `paint-layer` `masks` `generator` `curvature` `anchor-point` `blend-mode` `texture-set` `ambient-occlusion` `pbr` `metal-rough` `basecolor` `roughness` `metallic` `height` `normal-map` `alpha` `procedural` `intermediate` `advanced`
- **Summary:** Dense garment build (embroidered shawl, two fabrics) organized around a single reusable "Edge Border" anchor-point mask that nearly every subsequent layer — library fabric patterns, three stitch types (Top Stitching/Golden/Middle, all Material-mode not Pass-tool), an imported Midjourney design, a pop-up emboss + beadwork accent, and two closing curvature-driven highlight/sheen passes — references via Subtract or direct-load; by the end, roughly 8-9 anchor points are simultaneously active across the stack.
- **File:** tutorials/texturing-a-shawl-in-substance-painter.md


### Achieve Stunning Stylized Textures in Substance 3D Painter | Adobe Substance 3D
- **Source:** YouTube
- **URL:** https://www.youtube.com/watch?v=WYbp7SY-wEo
- **Author:** Adobe Substance 3D
- **App:** Substance 3D Painter
- **Version:** 11.0.0
- **Tags:** `layers` `masks` `generator` `ambient-occlusion` `curvature` `procedural` `basecolor` `roughness` `metallic` `normal-map` `iray-render` `viewport` `intermediate` `advanced`
- **Summary:** Dedicated deep-dive on every Stylization filter sub-menu: Brush Strokes (splattered shapes, follow-surface orientation), Brush Stroke Effects (per-channel color/normal overrides), Smoothness (per-channel anisotropic Kuwahara smoothing), Colorize (uniform tint + grunge), Gradient (1/2-color blends), Baked Lighting (fake diffuse/specular response), and Edges and Cavities (curvature-driven contouring). Companion deep-dive to "6 Powerful New Filters" — same demo scene and B-roll credit confirm the pairing. Version 11.0.0.
- **File:** tutorials/achieve-stunning-stylized-textures-in-substance-3d-painter-adobe-substance-3d.md


### Creating a Leather Material for Footwear with Anchor Points in Substance 3D Painter | Substance 3D
- **Source:** YouTube
- **URL:** https://www.youtube.com/watch?v=xXad_mS7K9s
- **Author:** Adobe Substance 3D
- **App:** Substance 3D Painter
- **Version:** not stated on screen
- **Tags:** `anchor-point` `masks` `layers` `fill-layer` `paint-layer` `smart-mask` `generator` `blend-mode` `curvature` `ambient-occlusion` `height` `basecolor` `roughness` `procedural` `tri-planar` `alpha` `advanced`
- **Summary:** 3/3 of the footwear anchor-points series (longest and most complete). Two chained anchor points: a Leather_Roughness_Base (Roughness + AO generator + Blur + Levels) anchor drives Edge Highlights, Dirt (AO-referenced + Dirt generator Multiply), and Overall Highlights (white fade + Grunge Multiply, Tri-Planar seam fix); a second folds/creases anchor (hand-painted Height mask + Creases Soft texture, Tri-Planar rotation via E to align with flex joints) drives Folds Color via generator Micro Height anchor-referencing with Invert, plus fold-specific Dirt via an Add-mode anchor-referenced fill.
- **File:** tutorials/creating-a-leather-material-for-footwear-with-anchor-points-in-substance-3d-pain.md


### How to Enable Auto-Updates in Substance 3D Painter | Adobe Substance 3D
- **Source:** YouTube
- **URL:** https://www.youtube.com/watch?v=13B82VtLuQY
- **Author:** Adobe Substance 3D
- **App:** Substance 3D Painter
- **Version:** 11.0.0
- **Tags:** `layers` `masks` `alpha` `beginner`
- **Summary:** Short feature explainer for the Auto-Updater panel (Assets panel toggle + Resources used in project toggle, both off by default): externally re-saved image files (Photoshop PSDs) and Substance 3D Designer filter graphs sent via "Send to Substance 3D Painter" now refresh live in the layer stack with no manual reload/redrag. Covers the Skip assets when their parameters mismatch safety toggle for the Designer round-trip. Version 11.0.0 stated explicitly on screen.
- **File:** tutorials/how-to-enable-auto-updates-in-substance-3d-painter-adobe-substance-3d.md


### Shading & Lighting a Character - Blender and Substance 3D Painter Workflow
- **Source:** YouTube
- **URL:** https://www.youtube.com/watch?v=2lHAio4DoWw
- **Author:** FlippedNormals
- **App:** Substance 3D Painter (paired with Blender)
- **Version:** not stated numerically; UDIM workflow, AgX color management on the Blender side
- **Tags:** `texture-set` `uv` `udim` `basecolor` `roughness` `color-management` `export` `export-preset` `pbr` `advanced`
- **Summary:** Cross-platform sequel to "Texturing a Clicker" — mostly Blender-side shading/lighting/rendering (out of this skill's scope, summarized briefly), but the Painter-relevant core is a "texturing software as master" discipline: the finished project exports down to just Base Color + Roughness per texture set, and any color correction discovered during Blender look-dev must be reproduced back on the actual Painter Fill-layer colors and re-exported rather than left as a permanent shader-graph adjustment.
- **File:** tutorials/shading-lighting-a-character---blender-and-substance-3d-painter-workflow.md


### Texturing Tactical Boots In Substance Painter
- **Source:** YouTube
- **URL:** https://www.youtube.com/watch?v=--CvtUlcVMs
- **Author:** 3DRedBox
- **App:** Substance 3D Painter
- **Version:** not stated on screen; "PAINT ALONG PATH" tool panel pins this to the Painter 9.x-10.x window
- **Tags:** `layers` `fill-layer` `paint-layer` `masks` `generator` `curvature` `anchor-point` `blend-mode` `texture-set` `uv` `pbr` `metal-rough` `basecolor` `roughness` `metallic` `height` `normal-map` `alpha` `procedural` `tri-planar` `advanced`
- **Summary:** Broad technique-survey build (plastic sole, steel/copper hardware, three fabric surfaces, Pass-tool stitching, anchor-point-driven logo/text decals) covering Curvature/Metal-Edge/Dirt/Inflate-Shrink-Wrap/UV-Border generators, a Galvanize+Tri-Planar copper-flake filter, and — used twice — an in-Painter fix for UV-island texel-density/tiling mismatches by switching a mask's pattern source to a dedicated secondary UV set. Decals use Anchor Point + Extract Alpha for dynamic transparent-PNG masks.
- **File:** tutorials/texturing-tactical-boots-in-substance-painter.md


### Substance 3D Stager - Rendering assets from Substance 3D Painter | Adobe Substance 3D
- **Source:** YouTube
- **URL:** https://www.youtube.com/watch?v=raGhfzhzVdU
- **Author:** Adobe Substance 3D
- **App:** Substance 3D Painter (export handoff only) + Substance 3D Stager (primary focus)
- **Version:** not stated on screen
- **Tags:** `export` `viewport` `intermediate`
- **Summary:** Stager-primary video; the entire Painter-side content is one step — File → Send to → Send to Substance 3D Stager on a finished robot character, which auto-wires every exported map into matching Stager materials. Documented at survey depth per this skill's Painter-only scope: Stager environment/terrain setup, HDRI lighting + rotation (same Shift+right-drag gesture as Painter), displacement tessellation, physical Area Light face-normal snapping, and PSD render export (material/object/depth passes) for a Photoshop post-pass (sky composite, fog and Lens-Blur depth of field driven by the depth pass). Cross-linked with the ornate-sword and Hero Assets for Fashion videos, which both use the same Send-to-Stager handoff.
- **File:** tutorials/substance-3d-stager---rendering-assets-from-substance-3d-painter-adobe-substance.md


### New Path Tool Features & Improvements in Substance 3D Painter | Adobe Substance 3D
- **Source:** YouTube
- **URL:** https://www.youtube.com/watch?v=exE0-1ftNeE
- **Author:** Adobe Substance 3D
- **App:** Substance 3D Painter
- **Version:** 11.0.0
- **Tags:** `path-tool` `layers` `masks` `paint-layer` `height` `normal-map` `alpha` `viewport` `intermediate`
- **Summary:** Tour of the 11.0.0 Filled Path tool's new capabilities: Filled Path shapes with adjustable Projection Depth (green normal-direction stripes), shift-click straight-line drawing, duplicate/convert-type and cross-layer "Paste All Vertices" syncing, mesh-wireframe snapping (Shift+Z, vertices/edges/edge centers), 45°-increment angle snapping (Ctrl+Shift, configurable step + reference space), and a 3D transform-manipulator gizmo for moving multiple selected points at once. Version 11.0.0 stated explicitly on screen.
- **File:** tutorials/new-path-tool-features-improvements-in-substance-3d-painter-adobe-substance-3d.md


### 10 New Features in Substance Painter You Didn't Know About
- **Source:** YouTube
- **URL:** https://www.youtube.com/watch?v=yebv44cOYW4
- **Author:** FlippedNormals
- **App:** Substance 3D Painter
- **Version:** not stated numerically; new-bake-types (Height/Bent Normals/Opacity) cross-references to Painter 8.1.0 (2022-06-07), tentative
- **Tags:** `layers` `fill-layer` `paint-layer` `masks` `alpha` `udim` `texture-set` `uv` `baking` `mesh-maps` `height` `opacity` `export` `export-preset` `viewport` `blend-mode` `intermediate`
- **Summary:** Feature-tour hub video: camera-linked environment lighting, Warp Projection (manual vertex-editing + surface-snap, for tattoos/decals and Height-channel detail alphas alike), native UDIM/UV Tiles support, SBSAR export, an overhauled click-to-pick Eyedropper, asset-browser Favorites, one-click blend-mode/opacity propagation across all channels, quick mesh reimport, 3 new bake types, and Temporal Anti-Aliasing.
- **File:** tutorials/10-new-features-in-substance-painter-you-didnt-know-about.md


### Warp Projection in Substance 3D Painter | Adobe Substance 3D
- **Source:** YouTube
- **URL:** https://www.youtube.com/watch?v=6_8CCf6v-uM
- **Author:** Adobe Substance 3D
- **App:** Substance 3D Painter
- **Version:** 7.4.0 confirmed on-screen; narration says the feature was added in 7.3.1 — see version-tracker cross-reference note in the file (Warp Projection itself predates 12.0.0's "Automatic warping" enhancement, they are not the same version event)
- **Tags:** `layers` `fill-layer` `masks` `alpha` `procedural` `uv` `viewport` `intermediate` `advanced`
- **Summary:** Fill-only Warp Projection mode: an editable on-surface grid (Transform Warp vs. Edit Vertices, Shift+W surface snapping, W/E/R hotkeys, Split Warp Horizontally/Vertically for local density) for manually bending a 2D image onto 3D geometry. Basic case on a red arrow alpha; advanced case wraps a TexturingXYZ face scan onto a differently-proportioned sculpted head, including Projection Depth tuning, snap-to-surface point placement, and the key tip of cropping stubborn regions (e.g. the mouth) into their own separately-aligned warp layer rather than over-densifying one grid. **Version note:** on-screen build is 7.4.0, contradicting an assumption that Warp Projection was introduced in 12.0.0 — 12.0.0 instead added an automatic "Warp to Geometry" assist on top of this older manual tool.
- **File:** tutorials/warp-projection-in-substance-3d-painter-adobe-substance-3d.md


### Izakaya's Paradigm, Chapter 3: Substance 3D Painter | Adobe Substance 3D
- **Source:** YouTube
- **URL:** https://www.youtube.com/watch?v=_HcSf9i4kIY
- **Author:** Adobe Substance 3D
- **App:** Substance 3D Painter
- **Version:** not stated on screen
- **Tags:** `layers` `paint-layer` `procedural` `alpha` `emissive` `basecolor` `beginner`
- **Summary:** Artist-philosophy piece (French interview, translated), Chapter 3 of a multi-app project-breakdown series — mostly interview B-roll rather than a software walkthrough. Describes a working principle: build a complex procedural base pass first, then hand-paint a deliberately illustrative 2D-style layer on top (flat colors, visible brush marks, texture-baked highlights rather than renderer-generated light), treating texturing and lighting as co-developed and iterative through to final render. Also covers real-world texture sampling and importing Photoshop brushes into Painter.
- **File:** tutorials/izakayas-paradigm-chapter-3-substance-3d-painter-adobe-substance-3d.md


### Speeding Up Character Texturing with Smart Masks - Substance Painter
- **Source:** YouTube
- **URL:** https://www.youtube.com/watch?v=qkRJjA5rTcY
- **Author:** FlippedNormals
- **App:** Substance 3D Painter
- **Version:** not stated numerically; Scattering channel added via Texture Set Settings > Channels > "support by shader", consistent with a modern shader-driven channel model, tentative
- **Tags:** `layers` `fill-layer` `paint-layer` `masks` `smart-mask` `blend-mode` `basecolor` `roughness` `height` `alpha` `texture-set` `pbr` `intermediate`
- **Summary:** Reusable character-region Smart Mask library workflow: hand-paint a saturated single-channel mask per recurring facial/character region (eye soft, eyelids, eye sharp, mouth, nose, ears, horns), save each as a Smart Mask (not Smart Material) under a consistent naming prefix, then drag independent (non-live) copies into new Fill layers across Color, Roughness, and Scattering/Subsurface channels for near-instant block-in on a new character. Closes with a local-grading trick: a Pass-Through Levels paint layer masked by a reused smart mask to confine a correction to one region only.
- **File:** tutorials/speeding-up-character-texturing-with-smart-masks---substance-painter.md


### Anchor Point Magic 01 - Double Layer Setup in Substance 3D Painter | Adobe Substance 3D
- **Source:** YouTube
- **URL:** https://www.youtube.com/watch?v=Ix4eknncFU0
- **Author:** Adobe Substance 3D
- **App:** Substance 3D Painter
- **Version:** not stated on screen
- **Tags:** `anchor-point` `masks` `layers` `fill-layer` `paint-layer` `generator` `blend-mode` `basecolor` `roughness` `metal-rough` `intermediate`
- **Summary:** 1/4 of Adobe's foundational Anchor Point Magic series (bronze valve model). Two duplicate paint layers (White_Paint, Blue_Paint) share one Metal-Edge-Wear mask via an Anchor Point + fill-with-Anchor-Points-tab reference + independent Levels retuning. Demonstrates the critical rule that anchors can only be referenced by layers positioned above them (bottom-to-top resolution), and that anchors are fully live/dynamic (a new paint layer added below the anchor propagates through immediately). Note: Whisper transcript came back mostly Dutch (language-ID artifact); notes reconstructed from surviving English terms + frame verification.
- **File:** tutorials/anchor-point-magic-01---double-layer-setup-in-substance-3d-painter-adobe-substan.md


### Using UV set and Stencils In Substance Painter -- English version
- **Source:** YouTube
- **URL:** https://www.youtube.com/watch?v=FIvOFo-zbms
- **Author:** 3DRedBox
- **App:** Substance 3D Painter
- **Version:** not stated on screen; no version-gated UI markers, consistent with this creator's other pre-12.1-era videos
- **Tags:** `layers` `fill-layer` `paint-layer` `masks` `generator` `procedural` `alpha` `stencil` `uv` `texel-density` `tri-planar` `roughness` `height` `basecolor` `blend-mode` `intermediate` `advanced`
- **Summary:** Two-part technique video: fixing per-UV-island tiling scale/rotation mismatches with a Fill layer's `UV set to UV set projection` source referencing a second, purpose-built UV channel (no re-baking or per-island manual rotation needed), demoed on a test cube then a real wood-cabinet project's Directional Noise edge-wear generator; then a real-photo Stencil workflow (S+RMB scale, S+LMB rotate, MMB pan) for hand-placing natural, non-repetitive wood-imperfection detail, finished with a full layer-stack breakdown (Metal Edge Wear + Dirt generator base, stencil paint layers, low-opacity Grunge passes, edge-focused cleanup).
- **File:** tutorials/using-uv-set-and-stencils-in-substance-painter----english-version.md


### Tips & Tricks in Substance 3D Painter to Make Semi-Realistic Textures | Adobe Substance 3D
- **Source:** YouTube
- **URL:** https://www.youtube.com/watch?v=ng-Wb7RaYHU
- **Author:** Adobe Substance 3D
- **App:** Substance 3D Painter
- **Version:** Beta (window title only; no numeric version stated)
- **Tags:** `layers` `fill-layer` `paint-layer` `masks` `generator` `procedural` `alpha` `curvature` `thickness` `blend-mode` `basecolor` `roughness` `height` `normal-map` `texture-set` `pbr` `advanced`
- **Summary:** Conference talk + live demo by character artist Anna B on texturing a stylized skin bust via a "three skin layers" model: Sub Dermal (flat red base + noise-generator redness + hand-painted veins + purple under-eye tint) under Dermis (semi-transparent noisy-brush skin mask + sun damage + freckles via Warp filter + curvature-masked blackheads + thickness-masked lip darkness + reused veins + makeup shading), topped with a Specular layer (used instead of Metallic, since skin isn't metal) and a Roughness layer (wet lips, oily T-zone). Core principle: many individually-subtle layers compound into realism. Q&A covers career advice and a cross-app HDRI-matching tip for color consistency between Painter and external renderers.
- **File:** tutorials/tips-tricks-in-substance-3d-painter-to-make-semi-realistic-textures-adobe-substa.md


### How to Texture NavyCap In Substance Painter in English
- **Source:** YouTube
- **URL:** https://www.youtube.com/watch?v=dGmVGU7aHb4
- **Author:** 3DRedBox
- **App:** Substance 3D Painter
- **Version:** not stated on screen; "newest version" name-checked for the duplicate-path-preserves-settings stitching feature, not otherwise pinned
- **Tags:** `layers` `fill-layer` `paint-layer` `masks` `smart-material` `generator` `anchor-point` `blend-mode` `baking` `mesh-maps` `ambient-occlusion` `curvature` `thickness` `high-to-low-poly` `world-space-normal` `texture-set` `uv` `pbr` `basecolor` `roughness` `height` `normal-map` `alpha` `procedural` `particle-brush` `intermediate` `advanced`
- **Summary:** Military-cap texturing pipeline built on two throughline techniques: baking Curvature/Thickness from a separate TurboSmooth-subdivided high-poly stand-in (same UVs) to eliminate low-poly mesh-wire edge artifacts in those two mesh maps, and an anchor-point-driven dynamic mask combination (two Anchor Points, second set to Soft Track blend) so a folder's mask self-updates instead of needing a manual Subtract layer. Also covers Wrap Projection for placing a fabric patch decal across a UV seam, a free Height-from-Base-Color-reference noise trick, and duplicating a placed stitch Path (geometry preserved) to reuse it with a different stitch-style preset.
- **File:** tutorials/how-to-texture-navycap-in-substance-painter-in-english.md


### Custom Fonts in Substance 3D Painter | Adobe Substance 3D
- **Source:** YouTube
- **URL:** https://www.youtube.com/watch?v=QSVgnyiDADc
- **Author:** Adobe Substance 3D
- **App:** Substance 3D Painter
- **Version:** 10.0.0 (stated in narration + confirmed via on-screen cache-usage readout)
- **Tags:** `layers` `fill-layer` `masks` `alpha` `texture-set` `MatFX` `procedural` `beginner`
- **Summary:** Official feature-tour of the new Text resource type (10.0+): drag text onto a model/layer/channel/mask like any other resource; live-edit content/font/size/alignment/color plus Advanced spacing/offset/background/resolution in the Properties panel; swap fonts non-destructively without losing other parameters. Ideal grayscale input for MatFX SBSAR materials (Spray Paint, Stickers, Stamps, Wood Carvings, Metal Engraving). Covers font sourcing (OS-installed auto-load, custom library folders, drag-drop or File > Import Resources import, licensing-restriction blocking, RTL/unsupported-glyph handling).
- **File:** tutorials/custom-fonts-in-substance-3d-painter-adobe-substance-3d.md


### How to Fix the Substance Painter Viewport to Match Unreal's
- **Source:** YouTube
- **URL:** https://www.youtube.com/watch?v=Yu8wR4df0IE
- **Author:** William Faucher
- **App:** Substance 3D Painter
- **Version:** not stated on screen; shown alongside Unreal Engine 4.26
- **Tags:** `color-management` `viewport` `iray-render` `pbr` `intermediate`
- **Summary:** Fixes Painter's default fully-linear viewport (hard-clipped, detail-less highlights) by importing a free third-party ACES LUT resource (ACES UE4 Log + ACES Standard Log, set to Color LUT type) and activating it via Display Settings > Post Effects > Tone Mapping (Function=Log) > Activate Color Profile > Profile=ACES UE4 Log — producing a near-exact visual match with Unreal's own ACES-based viewport. Validated with a same-HDRI, same-exposure side-by-side comparison using both apps' offline path tracers (Painter's Iray Renderer vs. Unreal's Path Tracing mode) to remove ray-tracing/screen-space-effect discrepancies from the test.
- **File:** tutorials/how-to-fix-the-substance-painter-viewport-to-match-unreals.md


### Native Illustrator File Support in Substance 3D Painter | Adobe Substance 3D
- **Source:** YouTube
- **URL:** https://www.youtube.com/watch?v=_lMpyz0Vhx8
- **Author:** Adobe Substance 3D
- **App:** Substance 3D Painter
- **Version:** 10.0.0-BetaFMX (confirmed via on-screen cache-usage readout)
- **Tags:** `layers` `fill-layer` `masks` `alpha` `blend-mode` `texture-set` `basecolor` `roughness` `height` `normal-map` `color-management` `procedural` `intermediate`
- **Summary:** Official feature-tour (juice-carton packaging example) of native .ai import: drag a whole Illustrator document onto the 3D view (Warp Projection material), 2D/UV view (UV material), or Layer Stack (UV fill in a chosen channel); each artboard becomes swappable via a file-type-specific Artboard dropdown, with Resolution/Crop/Scope controls and lossless vector scaling. Layers built from the import take normal Painter filters (Drop Shadow, Levels, HSL, Outline+Emboss+metallic). Projection mode (Warp vs. UV) is switchable after placement; reloading the source .ai file propagates edits non-destructively.
- **File:** tutorials/native-illustrator-file-support-in-substance-3d-painter-adobe-substance-3d.md


### How to Make the Substance Painter Viewport Match Unreal Engine
- **Source:** YouTube
- **URL:** https://www.youtube.com/watch?v=UOcNnu2uW1Y
- **Author:** Quinn Kuslich
- **App:** Substance 3D Painter
- **Version:** not stated on screen
- **Tags:** `color-management` `viewport` `iray-render` `roughness` `metallic` `pbr` `unreal-export` `beginner`
- **Summary:** Same fix as the companion William Faucher video, same underlying Brian Leleux ACES LUT pack: File > Import Resources (ACES Standard Log + ACES UE4 Log, set to Color LUT, imported to the Library shelf for persistence) > Display Settings > Environment Opacity 100% > Tone Mapping (Restore Defaults, Function Linear to Log) > Activate Color Profile > ACES_UE4_log. Framed specifically around getting an accurate in-viewport read of Roughness/Metallic values before importing to UE4; closes with a MetaHuman side-by-side comparison and a note that matching HDRIs in both apps is needed for a true 1:1 lighting match.
- **File:** tutorials/how-to-make-the-substance-painter-viewport-match-unreal-engine.md


### 3D Path Tool Updates in Substance 3D Painter | Adobe Substance 3D
- **Source:** YouTube
- **URL:** https://www.youtube.com/watch?v=rhraMw3YVpo
- **Author:** Adobe Substance 3D
- **App:** Substance 3D Painter
- **Version:** 3D Paths tool shipped 9.0.0 (June 2023, stated explicitly); this update video's own build not stated
- **Tags:** `path-tool` `layers` `paint-layer` `masks` `alpha` `height` `procedural` `intermediate`
- **Summary:** Update-tour of the (earlier, distinct) 3D Paths tool: per-path visibility toggle (eye icon), selective copy/paste (brush-properties-only vs. full vertex+pressure data, with same-sub-mode restriction on the former), freeform vertex movement off the mesh surface (with optional re-snap), and manual tangent-handle editing (two handles per vertex, Ctrl/Cmd to scale both together, Alt/Option to toggle smooth/corner) combinable with Corner Smooth for hand-shaped corners.
- **File:** tutorials/3d-path-tool-updates-in-substance-3d-painter-adobe-substance-3d.md


### Preparing a 3D Asset in Substance 3D Painter | 3D in After Effects Part 1 | Adobe Substance 3D
- **Source:** YouTube
- **URL:** https://www.youtube.com/watch?v=aZ8bzxuZ-pM
- **Author:** Adobe Substance 3D
- **App:** Substance 3D Painter
- **Version:** not stated/legible
- **Tags:** `layers` `fill-layer` `paint-layer` `masks` `blend-mode` `texture-set` `pbr` `metal-rough` `basecolor` `roughness` `metallic` `height` `normal-map` `opacity` `viewport` `alpha` `beginner`
- **Summary:** Beginner fundamentals video (Part 1/2, smartwatch asset; Part 2 covers After Effects and is out of scope). Covers paint vs. fill layers, environment/lighting basics (World vs. Camera alignment), sourcing/applying smart materials with Tiling, black-mask + Object Fill (Mesh Fill) per-part masking, applying 2D Illustrator textures and SVG vector decals (dragged onto the 3D model directly), and building a working glass material via a custom Opacity channel plus Shader Settings' Alpha Blending toggle. Finishes with a layer-reorder fix (bottom-to-top compositing) for a graphic's background color.
- **File:** tutorials/preparing-a-3d-asset-in-substance-3d-painter-3d-in-after-effects-part-1-adobe-su.md


### Baking in Substance 3D painter 8.3 | Adobe Substance 3D
- **Source:** YouTube
- **URL:** https://www.youtube.com/watch?v=hYtHp4IXvsM
- **Author:** Adobe Substance 3D
- **App:** Substance 3D Painter
- **Version:** 8.3.0 — exact match confirmed against `references/release-notes-painter-8.3.md`
- **Tags:** `baking` `mesh-maps` `high-to-low-poly` `cage` `ambient-occlusion` `curvature` `thickness` `position-map` `world-space-normal` `id-map` `texture-set` `opacity` `python-scripting` `python-api` `intermediate` `advanced`
- **Summary:** First-party feature-launch tour of the then-new dedicated Baking Mode (F8/croissant icon): interactive viewport with live cage/high-poly/low-poly overlays (exponential cage sliders, red mismatch highlighting), a Baking Log tracking mesh loading/mismatches, non-blocking bakes, and a synchronize/desynchronize system for Common Settings and individual bakers per Texture Set — including selective Match by Mesh Name for animated/removable parts (demoed on a dragon then a submachine gun). Every feature independently confirmed against this skill's own release-notes-painter-8.3.md.
- **File:** tutorials/baking-in-substance-3d-painter-83-adobe-substance-3d.md


### Substance Painter Beginner To Pro - Course
- **Source:** YouTube
- **URL:** https://www.youtube.com/watch?v=UCKwN3QA_FM
- **Author:** TriGon
- **App:** Substance 3D Painter
- **Version:** not stated on screen; modern Baking Mode UI consistent with a post-8.3-era build
- **Tags:** `layers` `fill-layer` `paint-layer` `masks` `smart-material` `smart-mask` `generator` `anchor-point` `blend-mode` `baking` `mesh-maps` `ambient-occlusion` `curvature` `high-to-low-poly` `cage` `id-map` `texture-set` `pbr` `metal-rough` `basecolor` `roughness` `metallic` `height` `normal-map` `alpha` `tri-planar` `procedural` `export` `export-preset` `channel-packing` `game-engine` `unreal-export` `beginner` `intermediate` `advanced`
- **Summary:** Flagship 2h48m zero-to-production foundations course (26 chapters, one leather-belt-and-buckle asset): layers/channels/masking/smart-materials/filters fundamentals, then a full real pipeline — ZBrush-to-Painter baking (cage tuning, matching-error heatmap, Match by mesh name, ID map via Vertex Color), ID-map-driven blocking-out, a fully non-destructive filter-and-Pass-Through material-building method (the throughline technique — copy a base mask onto a filter layer instead of hand-editing color so everything stays reactive to later changes), a primary/secondary/tertiary Tri-Planar-noise breakup recipe for realistic variation, Anchor Points introduced for mask reuse, Smart Material save/reuse with a personal naming convention, AO/Curvature baked-map refinement, environmental wear/storytelling (blood + dust Smart Materials/Masks, cross-material edge wear), a final top-of-stack grading pass, and export settings. Companion to two other TriGon courses in this library (escalating skill level) — cross-linked.
- **File:** tutorials/substance-painter-beginner-to-pro---course.md


### Creating 3D Paths in Substance 3D Painter | Adobe Substance 3D
- **Source:** YouTube
- **URL:** https://www.youtube.com/watch?v=Ro5dADu3vpM
- **Author:** Adobe Substance 3D
- **App:** Substance 3D Painter
- **Version:** not stated; original launch tutorial for the 3D Paths tool (9.0.0, per the companion "3D Path Tool Updates" video)
- **Tags:** `path-tool` `layers` `paint-layer` `masks` `fill-layer` `blend-mode` `alpha` `procedural` `intermediate`
- **Summary:** Original launch tutorial for the 3D Paths tool (leather-shoe brogue-pattern demo): paint editable, non-destructive curve-based strokes directly on geometry on a paint layer or mask. Covers vertex placement/Bezier vs. corner interpolation, the Paths panel (per-layer path management), toolbar controls (curve overlay toggle/Q, direction-reverse, per-vertex pressure, close-curve, per-path mirror/symmetry), the shared-material-via-fill-layer-and-black-mask workaround, and fixing paint gaps from widely-spaced vertices (extra vertex or Projection Depth).
- **File:** tutorials/creating-3d-paths-in-substance-3d-painter-adobe-substance-3d.md


### Anchor Point Magic 02 - Micro Normals & Micro Height in Substance 3D Painter | Adobe Substance 3D
- **Source:** YouTube
- **URL:** https://www.youtube.com/watch?v=HL5mZdzzgIg
- **Author:** Adobe Substance 3D
- **App:** Substance 3D Painter
- **Version:** not stated on screen
- **Tags:** `anchor-point` `masks` `layers` `fill-layer` `generator` `smart-mask` `curvature` `ambient-occlusion` `height` `normal-map` `procedural` `intermediate` `advanced`
- **Summary:** 2/4 of Adobe's foundational Anchor Point Magic series (bronze valve, embossed "MADE IN SP" stamp plate). Teaches referencing an Anchor Point through a Dirt generator's **Micro Height** and **Micro Normal** fields (under Micro Details) so the generator's grime placement reacts to a separate layer's height or normal detail without hand-painting — including the Levels+Invert fix for dirt gathering on the wrong side of the detail, and the critical "anchor goes on the layer, not a mask" + mandatory Reference Channel = Normal steps for the Micro Normal variant. Note: Whisper transcript came back mostly Dutch (language-ID artifact); notes reconstructed from surviving English terms + frame verification.
- **File:** tutorials/anchor-point-magic-02---micro-normals-micro-height-in-substance-3d-painter-adobe.md


### Substance Painter Tutorial -  Beginner To Advanced
- **Source:** YouTube
- **URL:** https://www.youtube.com/watch?v=qcQPItAXxgE
- **Author:** TriGon
- **App:** Substance 3D Painter
- **Version:** not stated on screen
- **Tags:** `layers` `fill-layer` `masks` `smart-material` `smart-mask` `generator` `blend-mode` `baking` `mesh-maps` `ambient-occlusion` `curvature` `id-map` `texture-set` `pbr` `basecolor` `roughness` `height` `alpha` `tri-planar` `procedural` `export` `export-preset` `game-engine` `unreal-export` `beginner` `intermediate` `advanced`
- **Summary:** Personal-workflow course (1h21m) on a wooden barrel (note: Whisper transcript consistently mis-hears "barrel" as "boot"): never use Painter's stock Materials/Smart Materials directly — build custom Fill-layer bases and drive every adjustment through Pass-Through filters (never a second Fill layer) so nothing breaks when base values change later. Covers color/roughness variation via Tri-Planar-masked HSL filters, ID-map-driven per-part detail isolation, Curvature-map-driven edge damage via Smart Masks (using a Base layer not a filter so underlying detail correctly disappears in damaged zones), a Warp-filtered secondary-detail pass, explicit Primary/Secondary Details grouping, a top Effects group with Curvature-Overlay depth + PBR Validator check, weathering/environmental storytelling (dust/blood/mud), and closing hand-painting guided by the procedural shapes already on the model. Companion to two other TriGon courses in this library — cross-linked.
- **File:** tutorials/substance-painter-tutorial---beginner-to-advanced.md


### Anchor Point Magic 03 - Paint Peel Effect in Substance 3D Painter | Adobe Substance 3D
- **Source:** YouTube
- **URL:** https://www.youtube.com/watch?v=0V_81uje7d8
- **Author:** Adobe Substance 3D
- **App:** Substance 3D Painter
- **Version:** not stated on screen
- **Tags:** `anchor-point` `masks` `layers` `fill-layer` `paint-layer` `generator` `blend-mode` `height` `alpha` `procedural` `advanced`
- **Summary:** 3/4 of Adobe's Anchor Point Magic series (bronze valve, same asset as 01-02). A more advanced double anchor-reference technique for a paint-peel bump effect: a paint layer's crack mask (Mask Builder Legacy generator, inverted) gets an Anchor Point; a separate Height-only layer references that anchor twice — once inverted + Blur-softened (the bump itself, at the crack edges), once non-inverted + Multiply blend (clips the blur bleed back to just the edges) — finished with manual black hand-painting for art direction. Note: Whisper transcript came back mostly Dutch (language-ID artifact); notes reconstructed from surviving English terms + frame verification.
- **File:** tutorials/anchor-point-magic-03---paint-peel-effect-in-substance-3d-painter-adobe-substanc.md


### Anchor Point Magic 04 - Rust Fade Effect in Substance 3D Painter | Adobe Substance 3D
- **Source:** YouTube
- **URL:** https://www.youtube.com/watch?v=LmtepSmnRQs
- **Author:** Adobe Substance 3D
- **App:** Substance 3D Painter
- **Version:** not stated on screen
- **Tags:** `anchor-point` `masks` `layers` `fill-layer` `paint-layer` `generator` `smart-mask` `blend-mode` `height` `basecolor` `roughness` `metallic` `procedural` `advanced`
- **Summary:** 4/4, series finale (same bronze valve asset as 01-03). Chains every prior technique into one system: a rust material's mask (referencing the White_Paint anchor, inverted) drives a matching glow (double reference: inverted+Blur+Levels for the bump, non-inverted+Multiply to clip the bleed — same trick as video 03), a Micro Height reference pulls the embossed text into the rust (technique from video 02), and a Dripping Rust generator's leaks are spatially confined to only appear near existing rust via the same invert+blur+Multiply-clip trick applied at the **folder** level (masks work on folders, not just layers) — all fully hand-paintable throughout via the underlying White_Paint mask.
- **File:** tutorials/anchor-point-magic-04---rust-fade-effect-in-substance-3d-painter-adobe-substance.md


### Substance Painter  - Creating Profesional Textures
- **Source:** YouTube
- **URL:** https://www.youtube.com/watch?v=eVRWXPJPjyE
- **Author:** TriGon
- **App:** Substance 3D Painter
- **Version:** not stated on screen
- **Tags:** `layers` `fill-layer` `paint-layer` `masks` `smart-mask` `generator` `id-map` `blend-mode` `curvature` `ambient-occlusion` `world-space-normal` `texture-set` `pbr` `basecolor` `roughness` `height` `alpha` `tri-planar` `procedural` `export` `intermediate` `advanced`
- **Summary:** Silent, unnarrated 168-minute speed-texturing follow-along on the same wooden barrel as the companion "Beginner To Advanced" video — the creator explicitly skips narration since he "already explained it in the previous video." No usable audio (Whisper hallucinated song lyrics over background music for the whole runtime); Structured Notes reconstructed entirely from 16 frames spread across the full video. Shows a more advanced pass: ID-map-masked wood/metal materials, rust hoops, layered dust/grunge weathering, a composite Curvature+AO+World-Space-Normal Mask Builder (Legacy) generator for edge damage, extensive hand-painting, and a closing HSL Perception + Color Correct grade before export. Cross-linked with the companion narrated video (read that one first for technique explanations) and the Beginner To Pro course.
- **File:** tutorials/substance-painter---creating-profesional-textures.md


### Substance Painter Beginner Tutorial for Unreal Engine 5
- **Source:** YouTube
- **URL:** https://www.youtube.com/watch?v=dXDWFPHkeZM
- **Author:** Unreal Sensei
- **App:** Substance 3D Painter
- **Version:** not stated on screen; Unreal Engine 5 (Nanite) on the engine side
- **Tags:** `layers` `fill-layer` `paint-layer` `masks` `smart-material` `generator` `anchor-point` `blend-mode` `baking` `mesh-maps` `ambient-occlusion` `curvature` `texture-set` `uv` `pbr` `metal-rough` `basecolor` `roughness` `metallic` `height` `normal-map` `alpha` `tri-planar` `procedural` `particle-brush` `export` `export-preset` `game-engine` `unreal-export` `beginner` `intermediate`
- **Summary:** Exceptionally thorough 2h55m foundations course (25 chapters, two assets — a mascot character then a Sci-Fi Crate) covering Fill-layer PBR basics, Tri-Planar texture projection, mask-building from stacked/blended generator+fill+paint effects (Dirt via baked AO, Metal Edge Wear via baked Curvature), per-channel independent blend-mode/opacity, Smart Material creation/reuse, exhaustive brush/symmetry/distance paint-tool controls, multi-Texture-Set blending, the Height-vs-Normal-channel distinction, hand-sculpting real height detail with Anchor-Point-fed Micro-Height generator inputs, and the full pipeline into Unreal Engine 5 Nanite tessellated displacement (custom export template, Use Height, Enable Tessellation, Displacement Scaling). One of the most exhaustive single tutorials in this library.
- **File:** tutorials/substance-painter-beginner-tutorial-for-unreal-engine-5.md


### Powerful Substance Painter Tricks That You Need To Know
- **Source:** YouTube
- **URL:** https://www.youtube.com/watch?v=XXEgE2rJ09c
- **Author:** Dolinskyi
- **App:** Substance 3D Painter
- **Version:** not stated on screen
- **Tags:** `layers` `paint-layer` `masks` `generator` `anchor-point` `blend-mode` `procedural` `alpha` `metal-rough` `roughness` `height` `basecolor` `texture-set` `viewport` `intermediate` `advanced`
- **Summary:** 8-trick grab bag: viewport/hotkey setup, a White-Noise+Histogram-Scan parkerizing-damage grain mask, a black-Paint-layer-on-Multiply trick for hand-guiding an automatic generator's reveal, black-and-white Photoshop decals placed with Edit Vertices + Surface Tool snapping, Auto Update Resources for live PSD re-linking, a Gradient-Linear mold seam, a two-Fill-layer (raised-lip + carved-groove) Anchor-Point scratch-depth technique for plastic damage, and — the video's centerpiece — a weld-seam rainbow heat-tint effect built by blurring/expanding the seam's own mask, capturing it as an Anchor Point, and feeding it into the creator's own Tempering Colors smart material in place of its default mask.
- **File:** tutorials/powerful-substance-painter-tricks-that-you-need-to-know.md


### Realistic Wood in Substance Painter | M24 Grenade Texturing
- **Source:** YouTube
- **URL:** https://www.youtube.com/watch?v=I3v-ESX4DxQ
- **Author:** Dolinskyi
- **App:** Substance 3D Painter
- **Version:** not specified (modern UI, consistent with this creator's other M24 Grenade series videos)
- **Tags:** `layers` `fill-layer` `masks` `generator` `anchor-point` `blend-mode` `ambient-occlusion` `procedural` `alpha` `stencil` `basecolor` `roughness` `height` `metal-rough` `color-management` `advanced`
- **Summary:** Part 1 of the M24 Grenade series (prequel to Tempering Colors / Realistic Painted Metal), texturing the wooden handle from a dark/mid/light three-tone reference framework where nearly every layer group derives its mask from one shared Anchor Point off the base texture. Key tricks: building Roughness/Height by reusing the base layer's own Base Color data via the Reference Channel dropdown, an AO-driven Dirt generator used in reverse (to remove dark-tone treatment from ZBrush-baked damage rather than add dirt), a Height-blend-mode switch to strip micro-detail from dark tones for a lacquer-like glossy/matte variation, and light-tone damage built from Painter's own stock wood texture used as a stencil. Deliberately restricted to only stock Painter grunges/stencils throughout. Cross-linked with the two later grenade-series videos and the Anchor-Point-centric "Powerful Tricks" video.
- **File:** tutorials/realistic-wood-in-substance-painter-m24-grenade-texturing.md


### How to Paint Realistic Skin in Substance Painter
- **Source:** YouTube
- **URL:** https://www.youtube.com/watch?v=jrDHqY96beY
- **Author:** FlippedNormals
- **App:** Substance 3D Painter
- **Version:** not stated on screen
- **Tags:** `layers` `fill-layer` `paint-layer` `masks` `procedural` `tri-planar` `blend-mode` `alpha` `basecolor` `color-management` `advanced`
- **Summary:** Entirely hand-painted-first (no photo projection) skin color-map workflow: one folder per channel, one flat-color Fill layer per named skin tone (Base/Red/Redder/Yellow/Blue/Darker), each masked by a nested Paint layer, fully re-gradable by changing a single Fill layer's color later. Covers favorite skin-painting brushes (Dirt2, Dots/Dots Erase, Cracks, Cotton/Smooth Noise, Mold), then layers in Tri-Planar procedural masks (BNW Spots 3, 3D Berlin Noise, Grunge) all set to Soft Light blend once hand-painting hits its practical time limit, and closes with a ZBrush round-trip — a Levels-pushed displacement map and a hand-authored poly-painted pimple mask (ZBrush Color→Fill Object + RGB-intensity painting, exported via Multi Map Exporter as Poly Paint) fed back in as additional Fill-layer masks.
- **File:** tutorials/how-to-paint-realistic-skin-in-substance-painter.md


### Creating environment materials and meshes in Substance 3D Painter
- **Source:** YouTube
- **URL:** https://www.youtube.com/watch?v=JMtw05Cj1gE
- **Author:** Wes McDermott
- **App:** Substance 3D Painter (primary) + Substance 3D Stager (render preview) + Unreal Engine 5 (Nanite delivery)
- **Version:** not stated on screen
- **Tags:** `layers` `fill-layer` `masks` `generator` `anchor-point` `blend-mode` `ambient-occlusion` `texture-set` `uv` `tri-planar` `pbr` `basecolor` `roughness` `height` `normal-map` `alpha` `procedural` `particle-brush` `export` `export-preset` `channel-packing` `game-engine` `unreal-export` `texel-density` `advanced` `expert`
- **Summary:** Advanced technique for authoring real tileable environment geometry (not just texturing a prop): Tri-Planar + Physical-Size projection for auto-correct material tiling, real Shader-Settings displacement/tessellation, Clone-tool multi-channel tiling fixes, Horizon-Based AO and Height-to-Normal filters, blending two ground materials via a live, Levels-reactive Compare Mask (Add Mask with Height Combination), an Anchor-Point-fed Dirt generator Micro Normal input to work around a mesh with no baked mesh maps, Stager ray-traced displacement validation, Smudge-tool fixes for jagged displacement edges, and exporting the actual displaced/tessellated mesh (Recompute Vertex Normals disabled) as a Nanite mesh for Unreal Engine 5.
- **File:** tutorials/creating-environment-materials-and-meshes-in-substance-3d-painter.md


### Zbrush to Substance Painter Bridge! NEW TOOL!
- **Source:** YouTube
- **URL:** https://www.youtube.com/watch?v=KzoJkdqyn7E
- **Author:** Abe Leal 3D
- **App:** Substance 3D Painter (receiving end) + ZBrush 2026.2 (sending end, via the ZBrush-to-Substance Bridge plugin)
- **Version:** ZBrush 2026.2 confirmed on screen; Painter version not stated
- **Tags:** `baking` `mesh-maps` `high-to-low-poly` `cage` `id-map` `udim` `texture-set` `uv` `masks` `ambient-occlusion` `world-space-normal` `curvature` `thickness` `height` `normal-map` `opacity` `intermediate`
- **Summary:** Demo of the ZBrush-to-Substance Painter Bridge plugin: one-click send auto-detects a sub-tool's lowest/highest subdivision as low/high-poly, auto-configures the Painter project (Automatic Cage, ZBrush template) and optionally auto-bakes mesh maps with zero manual Baking-dialog setup. Confirms working (if unofficial) UDIM support via UV-only edits between sends, a Force UV Auto-Unwrap option for UV-free quick tests, a Send PolyPaint feature that bakes ZBrush polygroup/paint color directly into a Painter texture draggable into the ID map slot for instant Color-Selection masking, a Decimation-Master-based path for high-poly-only assets (Subdivision Level = Current), and Per-PolyGroup multi-texture-set export.
- **File:** tutorials/zbrush-to-substance-painter-bridge-new-tool.md


### Optimizing Textures - How to Pack Masks Like a Pro
- **Source:** YouTube
- **URL:** https://www.youtube.com/watch?v=yZA_QMeZU0Q
- **Author:** Abe Leal 3D
- **App:** Substance 3D Painter (channel packing/export) + Unreal Engine 5 (material graph reconstruction)
- **Version:** not stated on screen
- **Tags:** `texture-set` `channel-packing` `export` `export-preset` `basecolor` `roughness` `metallic` `normal-map` `ambient-occlusion` `curvature` `thickness` `height` `alpha` `masks` `generator` `procedural` `blend-mode` `game-engine` `unreal-export` `color-management` `advanced` `expert`
- **Summary:** Advanced channel-packing beyond the standard Unreal Engine 4 Packed export: deletes the standalone Normal map entirely, repacking Normal X/Y into a custom texture's R/G channels (Roughness in B, Metallic in Alpha) since Unreal's DeriveNormalZ node can mathematically reconstruct the missing Blue/Z channel at render time (via Append+Subtract0.5+Multiply2, or a single Constant Bias Scale node). The freed BaseColor-Alpha slot carries a custom Painter User Channel ("blood") built from generators/grunges as a from-scratch procedural mask, reconstructed in Unreal via Lerp/Min nodes to drive both color and glossiness, and finally exposed as a live Material Instance scalar parameter for real-time on/off blood damage — down to just two 4K textures per asset. Cross-linked with this creator's Bridge and Texturing the Coin videos.
- **File:** tutorials/optimizing-textures---how-to-pack-masks-like-a-pro.md


### HOW TO MASTER TEXTURing in SUBSTANCE PAINTER
- **Source:** YouTube
- **URL:** https://www.youtube.com/watch?v=nM0FTa2p9yo
- **Author:** Jared Chavez
- **App:** Substance 3D Painter
- **Version:** not specified
- **Tags:** `layers` `masks` `ambient-occlusion` `roughness` `basecolor` `beginner` `intermediate`
- **Summary:** Talking-head/slide-deck methodology video (no live layer-building) laying out Jared Chavez's repeatable 3-phase texturing process, mapping primary/secondary/tertiary sculptural forms onto texturing: Phase 1 Blockout (color blocking + clean "fresh off the factory floor" material definition), Phase 2 Color & Roughness Breakup (~80-90% of final quality — subtle wear/edge-wear/grime value shifts, hue/saturation embellishment, roughness variation), Phase 3 Detail (sparse, high-contrast graphic damage — scratches/tears/blood — then a final global dirt/grime pass applied across the whole character, not per-material). Painter viewports/layer stacks appear only as B-roll validation, not step-by-step. Cross-linked with this creator's Building Masks Explained, both creature-texturing videos, and Texturing Metal from Scratch.
- **File:** tutorials/how-to-master-texturing-in-substance-painter.md


### HOW to Make a Peeled Paint Effect with ANCHOR Points | SUBSTANCE PAINTER
- **Source:** YouTube
- **URL:** https://www.youtube.com/watch?v=mLsXRzm7K0c
- **Author:** Jared Chavez
- **App:** Substance 3D Painter
- **Version:** not specified
- **Tags:** `layers` `fill-layer` `paint-layer` `masks` `anchor-point` `blend-mode` `height` `generator` `procedural` `particle-brush` `intermediate` `advanced`
- **Summary:** Direct continuation of Chavez's Building Masks Explained: builds a freehand-paintable lifted/flaking metal-edge paint-peel effect from a single Anchor Point referenced twice — one reference grown via Blur/Levels, a second identical reference set to `Subtract` blend mode cancels the interior, leaving only the grown edge ring (the lifted lip). Edge irregularity added via Warp/`Blur Slope` (Maximum blend) and layered Clouds/Grunge noise (Multiply/Overlay). Second demo extends the same architecture to pressure-sensitive dents/bubbling. Cross-linked with Building Masks Explained, Anchor Point Magic 03, Advanced Peeling Paint Effect (Javad Rajabzade), and How to create a paint peeling effect (Wes McDermott).
- **File:** tutorials/how-to-make-a-peeled-paint-effect-with-anchor-points-substance-painter.md


### SUBSURFACE SCATTERING: Subsurface Scattering in SUBSTANCE PAINTER for UNREAL ENGINE 5
- **Source:** YouTube
- **URL:** https://www.youtube.com/watch?v=mjLiJ5yjto0
- **Author:** Jared Chavez
- **App:** Substance 3D Painter
- **Version:** not specified
- **Tags:** `thickness` `masks` `generator` `curvature` `blend-mode` `layers` `fill-layer` `paint-layer` `game-engine` `unreal-export` `export` `advanced`
- **Summary:** SSS follow-up to Chavez's Neomorph creature texturing video: hand-paints a custom "Scattering" channel (white=max light transmission, black=fully bone-blocked, grays in between) starting loosely from a baked Thickness map, using per-region Paint layers (Stomach/Feet/Hands/ribcage) + `Levels - Scattering` adjustments + Blur for soft transitions + Curvature generator for edge detail, plus a non-physical "fake mass" belly-darkening trick for readability. Exports into an Unreal Engine 5 `SubsurfaceProfile` asset (Mean Free Path, Extinction Scale, Scattering Distribution, etc.) for final shader tuning. Cross-linked with both creature-texturing videos, Master Texturing, Unreal Sensei's UE5 tutorial, and Optimizing Textures (custom-channel-to-engine-asset pattern).
- **File:** tutorials/subsurface-scattering-subsurface-scattering-in-substance-painter-for-unreal-engi.md


### SUBSTANCE PAINTER: SMART MATERIALS Demonstration
- **Source:** YouTube
- **URL:** https://www.youtube.com/watch?v=pFUXJiTToc8
- **Author:** Jared Chavez
- **App:** Substance 3D Painter
- **Version:** not specified
- **Tags:** `smart-material` `smart-mask` `anchor-point` `masks` `blend-mode` `layers` `fill-layer` `paint-layer` `generator` `procedural` `particle-brush` `opacity` `emissive` `height` `intermediate` `advanced`
- **Summary:** Product-demo tour of a commercial 12-material anchor-point-driven Smart Material pack, doubling as an architecture lesson: every material is a folder with one base "Paint Here" layer that drives all secondary anchor-referenced effects (HSL variation, Lifted Edge, cracks, bubbling, dents) automatically. Covers Paint Peeled (starts blank by design), Bullet Hole (Opacity punch-through), Dent Chipped Paint (pressure drives dent depth + paint erosion together), Bubble (scaled-up Dirt 3 generator), Damaged/Black Leather (material-chaining: drag one Smart Material underneath another's active layer), mask-preset integration (reposition + `Linear Dodge` blend to make a dropped-in mask read with existing paint layers), Rust Streak, Burnt Streak, Burnt Emissive (pressure-driven live Emissive-channel glow), Burnt Fabric Holes (Opacity burn-through), Fabric Tear/Torn Cloth, and Tape (Sticker Shape brush-driven outline). Cross-linked with Building Masks Explained, Peeled Paint Anchor video, Texturing Metal from Scratch, Master Texturing, and Substance3D's Stylized Crab Smart Material creation video.
- **File:** tutorials/substance-painter-smart-materials-demonstration.md


### How to TEXTURE in SUBSTANCE PAINTER | ORC TEXTURES
- **Source:** YouTube
- **URL:** https://www.youtube.com/watch?v=lbMaYHlflp0
- **Author:** Jared Chavez
- **App:** Substance 3D Painter
- **Version:** not specified
- **Tags:** `layers` `fill-layer` `paint-layer` `masks` `blend-mode` `procedural` `tri-planar` `stencil` `roughness` `basecolor` `height` `curvature` `texture-set` `export` `game-engine` `beginner` `intermediate` `advanced`
- **Summary:** Full-character project breakdown of an orc bust (story-first: cave-dweller pale skin, stolen high-status armor). Metal: base + procedural breakup, stencil-placed gold trim, two-tier rust (subdued cavity rust + punchy hero-scratch rust), orange/blue complementary color-nuance layer. Leather: Base Color then Roughness breakup with organic-shaped grunge maps, edge-lightening, procedural cracking. Cloth stain/discoloration breakup. Teeth/gums: marble-noise veining + a thin transitional mesh to seat tooth/gum geometry (reused later for eye/eyelid). Skin: 3-frequency-band discoloration (large/medium/small), tiling-splatter sunburn base + hand-painted raised flaking-skin Height detail. Continuous Marmoset Toolbag round-tripping throughout. Cross-linked with both creature-texturing videos, Texturing Metal from Scratch, Master Texturing, Subsurface Scattering, and FlippedNormals' skin-painting video.
- **File:** tutorials/how-to-texture-in-substance-painter-orc-textures.md


### How to MAKE HAND PAINTED TEXTURES and SUBSTANCE PAINTER | Dragonite
- **Source:** YouTube
- **URL:** https://www.youtube.com/watch?v=VPSYen29WbU
- **Author:** Jared Chavez
- **App:** Substance 3D Painter
- **Version:** not specified
- **Tags:** `paint-layer` `layers` `fill-layer` `masks` `ambient-occlusion` `curvature` `blend-mode` `basecolor` `smart-material` `beginner` `intermediate`
- **Summary:** Full personal-project pipeline (ZBrush sculpt/pose → Painter texture → external render); Painter section (~5:17-8:44) extracted at primary depth. Speeds up start by exporting a Smart Material from a prior similar project (`UnderGradient`/`HighLight`/`2_tone_gradient` base layers), then hand-paints color/blood/light-value directly on top (graphic-not-photoreal blood shape to match a stylized concept), finishing with AO-tinted color + curvature accentuation layers. ZBrush Transpose Master posing and subsurface-scattering render glow noted briefly as pipeline context, out of Painter scope. Cross-linked with Smart Materials Demonstration, Master Texturing, Orc Textures, and FlippedNormals' realistic-skin video.
- **File:** tutorials/how-to-make-hand-painted-textures-and-substance-painter-dragonite.md


### How to make HAND PAINTED SKIN Textures in SUBSTANCE PAINTER
- **Source:** YouTube
- **URL:** https://www.youtube.com/watch?v=GcI60mKZU0k
- **Author:** Jared Chavez
- **App:** Substance 3D Painter
- **Version:** not specified
- **Tags:** `paint-layer` `fill-layer` `layers` `masks` `ambient-occlusion` `curvature` `blend-mode` `procedural` `particle-brush` `basecolor` `baking` `advanced` `expert`
- **Summary:** Fully hand-painted (no scan/photo projection) realistic skin color map on an elderly priest bust, built as two tiers: a Subdermal group (base Red + AO-masked brighter Red + broad scattered Yellow for bone + localized Blue for beard/under-eye + sparse Purple for eyes/lips) followed by an Epidermal group (base skin color via reduced-Flow Dirt brush so subdermal breakup shows through, then a 3-zone face breakdown worked non-sequentially, Curvature-masked+Levels-clamped pore/cavity emphasis, Cracks-brush capillaries, sculpted-guide vein tracing, and a final Marble/Vein-pattern procedural for surface complexity). Lips + waterline "Caramel" color as final touches. Cross-linked with FlippedNormals' realistic-skin video, both creature-texturing videos, Orc Textures, Subsurface Scattering, and Adobe's Semi-Realistic Textures talk.
- **File:** tutorials/how-to-make-hand-painted-skin-textures-in-substance-painter.md


### How to Make  HAND PAINTED POKEMON in Substance Painter | Tutorial
- **Source:** YouTube
- **URL:** https://www.youtube.com/watch?v=ZbrZR-9iX_Q
- **Author:** Jared Chavez
- **App:** Substance 3D Painter
- **Version:** not specified
- **Tags:** `paint-layer` `fill-layer` `layers` `masks` `ambient-occlusion` `blend-mode` `procedural` `particle-brush` `basecolor` `beginner` `intermediate`
- **Summary:** "Paris" (demonic Parasect) — the origin project later referenced/reused in Chavez's Dragonite video. Foundation-then-freehand workflow: base color + gradient, AO used for hue-shifted (not just darkened) shadow color, brushstroke-grain procedurals for happy accidents, then a single freehand Paint layer using a modified Palette Knife brush with a "never undo strokes" discipline. Continuous Marmoset Toolbag round-tripping from the start of hand-painting. Secondary asset (hand) built by copying the body's base layers then HSL-cooling for warm/cool contrast. Cross-linked with Dragonite, Smart Materials Demonstration, Hand Painted Skin Textures, Master Texturing.
- **File:** tutorials/how-to-make-hand-painted-pokemon-in-substance-painter-tutorial.md


### HOW to Make UDIMS for UNREAL ENGINE
- **Source:** YouTube
- **URL:** https://www.youtube.com/watch?v=fonCA0jiEF8
- **Author:** Jared Chavez
- **App:** Substance 3D Painter
- **Version:** not specified
- **Tags:** `udim` `texture-set` `baking` `mesh-maps` `thickness` `export` `unreal-export` `game-engine` `uv` `texel-density` `intermediate` `advanced`
- **Summary:** Verify check confirmed: primarily Maya UV work + UE5 Virtual Texture setup (~6 of 8 chapters), Painter appearing as one pipeline stage — extracted at proportionate depth. Same Neomorph creature as the Subsurface Scattering video. Maya: joint-based UV cuts, texel-density-matched 6-tile UDIM layout, split-and-decimate high-poly export. Painter: mandatory `Use UV Tile` import toggle, Thickness-map seam-discontinuity manual fix, standard tile-aware export. UE5: Enable Virtual Texture Support project setting, Material Editor wiring, VT thumbnail badge as load-success indicator. Cross-linked with Subsurface Scattering (same character), How to use UDIMs properly! (3DRedBox), UV Set and Stencils, Baking in Painter 8.3.
- **File:** tutorials/how-to-make-udims-for-unreal-engine.md


### How to MAKE POKEMON in Zbrush and Substance Painter | Gengar
- **Source:** YouTube
- **URL:** https://www.youtube.com/watch?v=MJxjI4pwY3g
- **Author:** Jared Chavez
- **App:** [PENDING]
- **Version:** [PENDING]
- **Tags:** [PENDING]
- **Summary:** [PENDING EXTRACTION]
- **File:** tutorials/how-to-make-pokemon-in-zbrush-and-substance-painter-gengar.md

---

## Tag Reference

Approved tag pool (see `SKILL.md` → "Approved tag pool" for the authoritative list):

```
layers, fill-layer, paint-layer, masks, smart-material, smart-mask, generator, anchor-point,
blend-mode, baking, mesh-maps, ambient-occlusion, curvature, thickness, position-map, id-map,
world-space-normal, high-to-low-poly, cage, udim, texture-set, uv,
pbr, metal-rough, specular-glossiness, basecolor, roughness, metallic, height, normal-map,
emissive, opacity, iray-render, viewport,
particle-brush, alpha, tri-planar, procedural, MatFX, stencil,
python-scripting, plugin, python-api, ui-plugin,
export, export-preset, channel-packing, game-engine, unreal-export, unity-export, godot-export,
color-management, texel-density,
beginner, intermediate, advanced, expert, painter-12, path-tool
```
