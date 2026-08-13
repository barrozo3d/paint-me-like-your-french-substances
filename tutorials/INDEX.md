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
- **App:** [PENDING]
- **Version:** [PENDING]
- **Tags:** [PENDING]
- **Summary:** [PENDING EXTRACTION]
- **File:** tutorials/substance-painter-tutorial-texturing-the-coin.md


### Stylized Asset Setup in Painter: Auto-Cage, PSD Workflows & Smart Detailing | Adobe Substance 3D
- **Source:** YouTube
- **URL:** https://www.youtube.com/watch?v=LRy-Nc7B_bk
- **Author:** Adobe Substance 3D
- **App:** [PENDING]
- **Version:** [PENDING]
- **Tags:** [PENDING]
- **Summary:** [PENDING EXTRACTION]
- **File:** tutorials/stylized-asset-setup-in-painter-auto-cage-psd-workflows-smart-detailing-adobe-su.md

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
