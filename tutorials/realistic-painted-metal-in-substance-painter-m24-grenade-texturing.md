---
title: Realistic Painted Metal in Substance Painter | M24 Grenade Texturing
source: YouTube
url: https://www.youtube.com/watch?v=SAI-lrWrtKg
author: Dolinskyi
ingested: 2026-08-12
app: "Substance 3D Painter"
version: "not specified (modern dark-theme UI, no version-pinning element visible)"
tags: [layers, fill-layer, paint-layer, masks, generator, anchor-point, blend-mode, ambient-occlusion, curvature, procedural, alpha, stencil, tri-planar, pbr, metal-rough, basecolor, roughness, metallic, height, normal-map, color-management, advanced]
extraction_status: complete
frames_dir: tutorials/frames/realistic-painted-metal-in-substance-painter-m24-grenade-texturing/
frame_count: 8
frame_status: complete
frame_selection: content-anchored (manual timestamps chosen from transcript, not blind percentages)
---

# Realistic Painted Metal in Substance Painter | M24 Grenade Texturing

**Source:** [YouTube](https://www.youtube.com/watch?v=SAI-lrWrtKg)
**Author:** Dolinskyi
**Duration:** 16m33s | 8 section(s)

---

## Raw Data (for Claude Code extraction)

Frames captured — see "Captured Frames" section below.


### Introduction [0:00]
**Transcript (timestamped):**
[0:00] Welcome to part 2 of our M24 Steel Hand Granite Texturing Series.
[0:16] And for those who haven't watched the first part yet, please do so, because I will use
[0:20] some techniques that I explained there.
[0:22] If any part of the process seems unclear, you can open the project itself and inspect
[0:27] every single layer.
[0:29] All project materials are available on my ArtStation page, including the Substance Painter project
[0:34] file, stencils, and the textures I used.
[0:37] It's like having the final answer key to the tutorial.
[0:40] Today we're tackling painted metal.
[0:42] This stage is more complex and involves several key techniques and a solid understanding of
[0:47] the PBR workflow.
[0:48] I'll break it all down step by step in simple terms.


### Paint [0:51]
**Transcript (timestamped):**
[0:52] Well, I'll start demonstrating the layers in the order I created them.
[0:56] First of all, I created paint.
[0:58] Turning on paint, and the first layer in this folder is just a fill, a dark green color.
[1:03] Roughness at 42, metallic at 0, because it's not metal.
[1:06] And this will be the base, which I will then apply in variation 1, 2, 3, 4, and all subsequent
[1:12] variations.
[1:14] I create variations in the following way.
[1:16] I duplicate this base layer.
[1:18] For example, I write that this is paint variation 01.
[1:21] I add a mask here, a fill layer, and in the fill layer, I insert for example some procedural
[1:27] texture.
[1:28] And now I just change their color.
[1:30] For example, I'll make it a little light yellow.
[1:33] This in essence will be the variation.
[1:35] This is exactly how I create all these subsequent layers.
[1:39] But I tweak not only the color, I also tweak roughness and height.
[1:43] Height variations are very important.
[1:46] This grenade is quite old.
[1:47] It has been lying around since World War II.
[1:50] If you look at photos, there are a lot of different imperfections, damages, scratches.
[1:55] The paint is not as sharp as they paint it now.
[1:58] That is, such things, old vintage objects, weapons have a very saturated height map.
[2:03] That is, it's not worth leaving such a simple surface.
[2:06] It will look unrealistic.
[2:07] So the first layer with the variation is these kinds of stripes.
[2:11] These are paint application marks.
[2:13] I add a base procedural texture, crystal 2, then blur it, then a warp filter, which gives
[2:18] a bit of life to these lines.
[2:20] With a histogram scan, I make the mask more contrasty and readable.
[2:24] We must remember that we will be looking from this distance.
[2:27] Thin, indistinct lines simply won't be visible.
[2:31] Next, I remove the uniformity.
[2:33] I add the next fill layer, insert a grunge map here and through the subtract blending
[2:37] mode.
[2:38] Next, with paint, I clean up those details where I don't want to see the mask.
[2:42] I also add an ambient occlusion generator, which also cleans up the mask where I don't
[2:47] want to see it.
[2:49] And this is how such a layer appears.
[2:51] It is darker in diffuse.
[2:53] That is, it's such a dark green color.
[2:55] Its roughness is slightly different and it has height.
[2:59] The next layer is very similar.
[3:02] In essence, the same lines, but they are blurred.
[3:04] They are bigger.
[3:06] This adds a bit of a variety.
[3:08] Because in nature, when something is painted or worn down, it cannot be uniform, meaning
[3:14] it needs to be broken up a bit.
[3:16] Somewhere it will be sharp, somewhere it will be blurry, somewhere the lines are wide,
[3:20] somewhere narrow.
[3:22] This non-uniformity is exactly what gives the effect of authenticity.
[3:26] Next layer, variation number three.
[3:29] Also differs in color.
[3:30] It is already a bit yellowish.
[3:33] Roughness is already more matte.
[3:35] Medallness is still zero, because it is still not metal.
[3:38] Next layer.
[3:39] These are already more specific yellow spots, seemingly looking like traces of rust.
[3:45] Such a contrasty dark dark orange or closer to brown color is already even more matte.
[3:50] The next variations are interesting in the sense that they work like a gradient.
[3:55] A gradient adds realism to an object, and such an object reads well from a distance.
[4:01] The layer is very simple.
[4:03] In essence, these are all masks that I take from the procedural textures library of Substance
[4:08] Painter.
[4:09] I use this mask as a stencil.
[4:11] Through the Subtract mode, I subtracted grunge plaster paint from it.
[4:15] Here, it adds such a texture overlay blending mode.
[4:20] The next layer, paint variation 07 simulates paint in the lower part.
[4:25] Such paint can be seen on references, painted simply with a standard brush.
[4:30] Next is white dirt.
[4:31] This is, in essence, white paint matte.
[4:35] This is what the main mask looks like.
[4:37] Next layer, light edges.
[4:39] Light edges adds a bit more volume.
[4:42] Often paint either wears away in contact areas or fades.
[4:47] Created very simply using metal edge wear.
[4:50] In custom grunge, this grunge is added.
[4:53] The next layer is just a variation in glossiness.
[4:56] These are fingerprints.
[4:57] The next folder is micro surface.
[5:00] Micro surface is variations in the height map.
[5:03] The first variation is the unevenness of the paint, made using a standard procedural
[5:08] texture on the height channel.
[5:10] So, the next layer is hair, as if we have a hair stuck under the paint.
[5:14] The hair mask can be found on the textures.com website.
[5:19] It looks pretty cool, especially in renders.
[5:21] Next is scratches.
[5:23] I drew them by hand, projecting them from a scratch mask.
[5:26] Next layer, separation.
[5:28] We have 01 and 02.
[5:30] They separate the details from each other by color.
[5:32] This head is made of three details and they must differ from each other.
[5:36] They cannot just be filled with a single paint.
[5:39] In an empty layer, I add an HSL perspective filter, set the blending mode to pass through.
[5:45] I isolate the needed detail with a mask and change its color.
[5:49] This is for realism.
[5:51] Next folder, metal cap, for the back part.
[5:54] The first layer changes the color of the paint, gives a more bluish tint.
[5:59] This one separates this detail.
[6:01] The next layer adds dust.
[6:03] It is made using a grunge dust white map on top.
[6:10] Dust layer settings, roughness matte, base color gray, slightly with a bluish tint without
[6:15] a height map.
[6:17] The next layer is also a color change based on curvature.
[6:20] We make it of a more gray shade like that.
[6:24] The next layer is a dirt layer.
[6:26] Well, not like dirt, but variations in color on the paint.
[6:30] A dark brown color and slightly different roughness.
[6:38] Next layer dirt, light and dark.
[6:43] This is its mask.
[6:48] Next light dirt made using a generator.
[6:57] Directional noise to give it a bit of direction.
[7:00] Such things look good on cylinders.
[7:02] We add these stripes and clean up with a brush where they are not needed.
[7:07] And right here, I add such spots under the bolts.
[7:10] Yes, and the last layer in this folder is also color variations.
[7:15] Only color, just a gray color.
[7:17] The mask is generated by this kind of generator.
[7:27] Next glossy scratches layer.
[7:29] These are glossy scratches like that, which also add variations.
[7:33] That is, our surface is matte and to make variations on this surface, you need to make them glossy.
[7:39] If our surface were glossy, I would conversely add matte variations.
[7:43] This is everything regarding this part.
[7:45] The next folder in the paint folder is extra details.
[7:49] Extra details are additional variations in the height map and color.
[7:53] Such irregularities that break through the paint.
[7:56] The mask looks like this.
[7:58] It is also created using a standard procedural texture, Rusty Leaks.
[8:02] Next, edges.
[8:04] Such a slight glossy effect.
[8:09] Also ambient occlusion slightly separates this part from the other.
[8:13] That is, in essence, these two layers just make this effect more voluminous.
[8:18] And that's all for the paint.
[8:20] All these layers need to be done very carefully.
[8:23] The main thing in the process of improvement is not to make it worse.
[8:26] Let's now create damages for our paint.
[8:28] This is a very important element.


### Paint Damage [8:31]
**Transcript (timestamped):**
[8:31] And so, the first layer I have is a generator.
[8:33] I want to add uniform wear in some places with the generator, but I will edit it very
[8:37] heavily.
[8:38] Here is the next layer.
[8:39] In essence, these are the main damages.
[8:41] I left damages from the generator only on this detail.
[8:44] I drew all these damages using a stencil.
[8:47] I will add a similar stencil to the pack with source files.
[8:51] You can use it.
[8:52] This is a real photograph of paint damages.
[8:54] We take the stencil and simply paint out these chunks of damaged paint.
[8:59] When painting, take into account such design principles as large, medium, small, that is,
[9:04] you, for example, create one large spot, create a medium spot next to it and add some tiny
[9:08] spots.
[9:09] But the mask must be contrasty so that it reads well from a distance.
[9:13] In this place, I don't have a very contrasty texture, so using blur and a subsequent histogram
[9:18] scan, I make it maximally contrasty and sharp.
[9:26] Next I created corrosion under the paint.


### Oxidized Metal [9:29]
**Transcript (timestamped):**
[9:29] This is what it looks like for me.
[9:34] If you remove paint, it looks like this.
[9:37] Let's show step by step how it was created.
[9:45] The base layer from which everything begins.
[9:48] It is set up as a grey-yellowish metal, roughness at 58 and an important point, metalness at
[9:54] 0.9.
[9:56] It's a light grey mask.
[9:57] It's not completely black because this is one of the basic principles of working with
[10:01] PBR.
[10:02] If you have metal that is not clean but oxidized, it shouldn't be clean metal on the metalness
[10:08] map.
[10:09] That is, you lower this slider a bit and then you can make the map darker.
[10:14] Next, microsurface.
[10:16] Metal is a very important element because this is old metal.
[10:19] It already has its own damages, corrosion, irregularities.
[10:23] Such grenades were made 80 years ago.
[10:25] They have survived until now.
[10:27] And metal cannot be perfectly smooth.
[10:30] Next, oxidized metal.
[10:32] Found a photo of metal on Texture.com, made a tile out of it and generated a normal map
[10:37] using bitmap to material.
[10:40] Also generated roughness, dropped it into base color, into roughness and into normal.
[10:46] This is the metal I have on top.
[10:49] Next rust.
[10:50] As you can see, it is already cut out under a mask.
[10:56] And this, if you turn off the layers, I will make the mask white to show what it looks
[11:03] like.
[11:06] This is a base rust material that can be found in the Substance Painter library.
[11:11] Here it is.
[11:13] But I changed it a bit.
[11:14] In some places I did desaturation.
[11:17] I added an empty layer and inserted an HSL into it.
[11:22] Added this kind of mask.
[11:25] Next, a yellowish layer on top.
[11:31] If you look at the damaged mask, you can see that it is added along the edges.
[11:36] This is also to vary the color of the rust a bit.
[11:39] Next, a dark layer.
[11:44] What does this dark layer represent?
[11:48] This is a fill layer, applied using this kind of mask.
[11:52] This is a standard grunge paint scratched.
[11:55] The mask is set up as oxide, a dark colored metal oxide, matte.
[12:00] And another one on top, a more spotty one like that.
[12:03] This adds contrast.
[12:05] If you look at the base color, it looks like this.
[12:09] Roughness.
[12:11] And metallic.
[12:13] And next, another folder, rust.
[12:19] The rust folder is the last one.
[12:20] It creates corrosion that breaks through the paint.
[12:24] That is, the paint wasn't damaged, but this corrosion ate it away from the inside.
[12:29] That is, a small gap got in somewhere and then the paint started to be eaten away by
[12:33] this corrosion.
[12:38] It was created using a standard procedural map, which is actually called rust.
[12:43] Here is this mask, but its contrast is turned up.
[12:47] That is, in this way.
[12:51] That's all with the corrosion.
[12:53] That is, we already have the paint, we have the corrosion underneath it.
[12:59] The surface still looks quite uniform for such an old thing.
[13:02] I add more information to the height map.
[13:06] Into the layer, I threw again this same height map generated from a photograph that I demonstrated
[13:13] earlier.


### Peeling Paint [13:17]
**Transcript (timestamped):**
[13:17] Next is the peeling paint effect.
[13:20] The first layer is anchor from the mask.
[13:25] The next one is grunge via multiply blending mode.
[13:31] Next is the blur filter to blur the edges.
[13:35] And the last layer is an inverted mask from the anchor via subtract blending mode.
[13:40] This way we get this kind of effect.
[13:44] Next, this layer is located inside a folder to which I added a mask and painted exactly
[13:52] where this effect should be.
[14:02] Let's break down how the decal was created.


### Decal [14:04]
**Transcript (timestamped):**
[14:05] As you can see, there are quite a lot of layers here.
[14:08] You can look into it in detail by opening the project.
[14:10] The link to it is below the video.
[14:12] The first layer is just the alpha of the text created in Photoshop.
[14:17] The next one is filter warp, which makes the edges ragged.
[14:21] Next is blur filter, anchor point, then procedural texture, contrast adjusting using histogram
[14:28] scan.
[14:29] And insert the information from this anchor, place it on top, meaning to remove the internal
[14:34] dots and leave them only along the edges.
[14:37] Then dirt again via multiply, then histogram to increase the contrast.
[14:43] Next is paint.
[14:44] I subtract the peeling paint mask.
[14:48] Grunge to create paint scuff slash wear in some places.
[14:55] Next is another grunge for the same purpose.
[14:58] And anchor point on top.
[15:02] The next layer.
[15:03] We insert the anchor point from the previous layer and add another grunge on top.
[15:08] This is what the final mask looks like.
[15:14] Next we have dirt.


### Dust&Dirt [15:15]
**Transcript (timestamped):**
[15:16] The first layer is grunge.
[15:18] This is from the standard procedural textures.
[15:22] Next is the dirt generator.
[15:24] Next I manually edit the mask.
[15:26] Then using curvature, I remove dirt from the edges.
[15:30] The next layer is fingerprints.
[15:34] I add high contrast spots using a stencil.
[15:44] The next layer, another dirt, but made slightly differently.
[15:48] The first layer is a generator.
[15:50] The next one is grunge via subtract mode.
[15:53] The next one is another grunge via linear dodge mode.
[16:01] Manually painting over the mask.


### Sharpen [16:08]
**Transcript (timestamped):**
[16:09] And as always, sharpen on top.
[16:12] To increase the texture sharpness, there are two sharpen filters here.
[16:17] One for roughness, the second sharpen is for color.
[16:21] That's all.
[16:22] Thank you for watching.
[16:23] You can find the project files via the link below the video.
[16:27] This pack will include stencils for making damaged paint.
[16:30] Thank you for watching.
[16:32] See you next time.



---

## Captured Frames

- [1:00] tutorials/frames/realistic-painted-metal-in-substance-painter-m24-grenade-texturing/frame_000.jpg
- [2:20] tutorials/frames/realistic-painted-metal-in-substance-painter-m24-grenade-texturing/frame_001.jpg
- [4:35] tutorials/frames/realistic-painted-metal-in-substance-painter-m24-grenade-texturing/frame_002.jpg
- [8:52] tutorials/frames/realistic-painted-metal-in-substance-painter-m24-grenade-texturing/frame_003.jpg
- [9:45] tutorials/frames/realistic-painted-metal-in-substance-painter-m24-grenade-texturing/frame_004.jpg
- [10:46] tutorials/frames/realistic-painted-metal-in-substance-painter-m24-grenade-texturing/frame_005.jpg
- [13:40] tutorials/frames/realistic-painted-metal-in-substance-painter-m24-grenade-texturing/frame_006.jpg
- [15:16] tutorials/frames/realistic-painted-metal-in-substance-painter-m24-grenade-texturing/frame_007.jpg

---

## Structured Notes

### Core Technique
Full layer-by-layer walkthrough of an aged, WWII-era painted-metal grenade head — built as six sequential folders (Paint, Paint Damage, Oxidized Metal, Peeling Paint, Decal, Dust & Dirt, finished with a Sharpen pass), each demonstrating a distinct sub-technique: stacked procedural color/roughness/height paint variations, stencil-driven hand-painted battle damage, PBR-correct oxidized-metal-under-paint, anchor-point-driven peeling paint, a fully-built decal from Photoshop alpha to weathered final mask, and layered dirt/dust generators.

### Summary
Part 2 of a personal "M24 Steel Hand Grenade Texturing Series" (project files, stencils, and textures shared on the creator's ArtStation as a reference key). Explicitly framed as more complex than part 1, requiring solid PBR understanding. The video is essentially an audit of a finished, already-built layer stack, walked top-to-bottom folder by folder: a base paint fill duplicated repeatedly into 7+ numbered "paint variation" layers (each varying color, roughness, AND height — height called out as especially important for a battle-worn 80-year-old object), separation layers using an empty pass-through layer with an HSL filter to color-differentiate the grenade's three separate mesh parts, a metal cap sub-folder (color/dust/curvature-driven variation), and a glossy-scratches layer that inverts the surface's dominant finish (matte base -> glossy scratch variation, explicitly noting the rule would flip on a glossy base). Paint Damage adds hand-stencil-painted battle damage following a large/medium/small compositional principle, with histogram-scan contrast pushes to keep masks readable at distance. Oxidized Metal builds a PBR-correct rusted-steel-under-paint material from a real photo (converted to normal+roughness via Bitmap to Material), deliberately keeping Metallic below 1.0 and the metalness mask non-pure-black/white to represent oxidized rather than clean metal. Peeling Paint uses a compact 4-layer anchor-point recipe (anchor from mask -> grunge multiply -> blur -> inverted-anchor subtract) confined to a hand-painted folder mask. Decal builds a full weathered decal stack from a Photoshop-authored text alpha through warp/blur/anchor-point/contrast/dirt/scuff passes. Dust & Dirt layers grunge, a dirt generator cleaned up with curvature (removing dirt from sharp edges) and manual paint, fingerprints via stencil, and a second dirt variant (generator + subtract-mode grunge + linear-dodge-mode grunge, manually painted over). Finishes with two Sharpen filters (one for Roughness, one for Base Color).

### Key Steps
1. **Paint folder — establish one base fill, then clone-and-vary:** create a single base paint fill layer (dark green, `Roughness` 42, `Metallic` 0 — not metal), then build every subsequent "paint variation" as a duplicate of it with a new procedural-texture-driven mask and tweaked Base Color, Roughness, and Height — height variation flagged as critical for an old, battle-worn object ("it's not worth leaving such a simple surface, it will look unrealistic").
2. **Variation 1 — paint-application stripe marks:** mask built from `Crystal 2` procedural texture -> `Blur` -> `Warp` filter (adds organic irregularity to the lines) -> `Histogram Scan` to push contrast/readability at viewing distance; uniformity broken further with a grunge map in `Subtract` blend mode, then manually cleaned up with paint and an `Ambient Occlusion` generator.
3. **Variations 2-7 — build non-uniformity deliberately:** each subsequent variation intentionally differs in blur amount, line width, and sharpness from its neighbors ("in nature, when something is painted or worn down, it cannot be uniform... this non-uniformity is exactly what gives the effect of authenticity"); later variations use masks pulled from Substance Painter's built-in procedural-texture library used as stencils, combined via `Subtract` and `Texture Overlay` blend modes for a gradient-like falloff that reads well from a distance.
4. **Paint variation 07 and "white dirt":** paint variation 07 simulates hand-brushed touch-up paint on the lower section (matched to reference photos); a separate white-matte "dirt" layer follows.
5. **Light edges via edge-wear generator + custom grunge:** simulates paint wearing away or fading at contact/high-touch points, built from a metal-edge-wear generator with an added custom grunge texture; followed by a glossiness-only variation layer simulating fingerprints.
6. **Micro Surface sub-folder — height-only detail:** standalone procedural-texture height variation for paint unevenness; a hair strand (sourced from textures.com) stuck under the paint for a "pretty cool in renders" imperfection; hand-drawn scratches projected from a scratch mask.
7. **Separation layers — differentiate the grenade's 3 mesh parts:** on an empty layer set to `Pass Through` blend mode, add an `HSL` filter, isolate each mesh detail with a mask, and shift its color independently — necessary because the head is built from three separate details that "cannot just be filled with a single paint."
8. **Metal Cap sub-folder (back part):** color shift toward a bluish tint, its own separation/isolation layer, a dust layer (grunge dust-white map, matte roughness, gray base color with a slight blue tint, no height), a curvature-driven color-shift layer (grayer tone), a dirt/color-variation layer (dark brown, differing roughness), a directional-noise dirt layer for cylinder-appropriate streak direction (cleaned with a brush) plus bolt-adjacent dirt spots, and a final generator-driven gray color-variation layer.
9. **Glossy scratches — invert the dominant finish for scratch variation:** since the base surface reads matte, scratch variation is made *glossy* to stand out (explicitly noted this logic reverses on a glossy base surface — matte scratches would be used instead).
10. **Extra Details sub-folder:** additional height+color irregularities using the `Rusty Leaks` procedural texture ("irregularities that break through the paint"), plus an edges pass (subtle glossy effect + Ambient Occlusion) to add volume and separate the part from its neighbor.
11. **Paint Damage folder — stencil-driven battle damage:** start with a heavily-hand-edited wear generator restricted to only one detail of the mesh; layer in the main damage pass hand-painted using a real damaged-paint reference photo as a `Stencil` (included in the creator's shared asset pack); apply the large/medium/small compositional principle (one large damage spot, one medium, several tiny) so the mask "reads well from a distance"; finish with `Blur` + `Histogram Scan` to maximize mask contrast/sharpness.
12. **Oxidized Metal folder — PBR-correct rust-under-paint:** base layer set as grey-yellowish metal, `Roughness` 58, **`Metallic` 0.9 (not 1.0)** — explicitly called out as a core PBR principle: oxidized/dirty metal should never be pure white on the Metallic map, so both the metalness slider and its mask are kept slightly non-maximal/non-pure-black-white.
13. **Build the oxidized-metal texture from a real photo:** sourced a metal photo from Texture.com, tiled it, ran it through `Bitmap to Material` to generate a Normal map, also generated Roughness, then fed the result into Base Color, Roughness, and Normal simultaneously.
14. **Rust — built from the library base + custom edits:** starts from Substance Painter's built-in rust material, modified with an empty pass-through layer holding an `HSL` filter for localized desaturation, a yellowish edge-following variation layer (adds rust color variety along damage-mask edges), and a dark oxide layer (grunge-paint-scratched mask, matte dark metal-oxide color) topped with a spottier contrast-boosting layer.
15. **Rust folder (paint-breakthrough corrosion, separate from the Oxidized Metal folder):** represents corrosion that ate through paint from the inside rather than damage that exposed metal directly — built from Substance Painter's built-in procedural `Rust` map with contrast pushed up; followed by re-injecting the same photo-derived height map from step 13 to add more surface irregularity appropriate to an aged object.
16. **Peeling Paint — 4-layer anchor-point recipe:** (1) an `Anchor Point` referencing the damage mask, (2) a grunge layer in `Multiply` blend mode, (3) a `Blur` filter to soften the peel edges, (4) an inverted version of the same anchor mask applied via `Subtract` blend mode — the combination produces the peeling-paint-edge look. The whole effect folder is masked by a hand-painted mask so it's confined to only where the peeling should appear.
17. **Decal — full build from Photoshop alpha to final weathered mask:** start with a text alpha authored in Photoshop; apply a `Warp` filter for ragged edges, a `Blur` filter, an `Anchor Point`, a procedural texture, and `Histogram Scan` contrast; re-insert the anchor's data on top to strip interior dots and keep only edge detail; add dirt via `Multiply` + another `Histogram Scan` contrast pass; subtract the peeling-paint mask (step 16) to integrate the decal with existing paint wear; layer two more grunge passes (paint scuff/wear) with an `Anchor Point` carried forward between them for the final composited decal mask.
18. **Dust & Dirt folder:** grunge from the built-in procedural library; a `Dirt` generator manually mask-edited, then cleaned along edges using `Curvature` (removes dirt buildup from sharp edges where it wouldn't realistically collect); a fingerprints layer built from high-contrast `Stencil` spots; a second dirt variant built from a generator + grunge in `Subtract` mode + grunge in `Linear Dodge` mode, finished with manual paint touch-ups.
19. **Sharpen — always the final layer:** two `Sharpen` filters placed at the very top of the stack, one applied to Roughness and one to Base Color, described as a standing habit ("as always, sharpen on top").

### Layers / Tools / Settings
- **Base paint layer:** dark green Fill, `Roughness` 42, `Metallic` 0
- **Procedural masks used as stencils:** `Crystal 2`, `Rusty Leaks`, built-in procedural-texture library entries, custom grunge maps, `Rust` (built-in procedural)
- **Filters:** `Blur`, `Warp`, `Histogram Scan` (repeated heavily for mask contrast/readability-at-distance), `HSL` (on empty Pass Through layers for part-separation color shifts and rust desaturation), `Sharpen` (Roughness + Base Color, final layer)
- **Generators:** metal edge-wear generator, `Ambient Occlusion` generator, `Dirt` generator, `Curvature`-driven generator (edge dirt removal), directional-noise generator
- **Masking primitives:** `Anchor Point` (peeling paint 4-layer recipe; decal build; damage-mask reuse), `Stencil` (hand-painted battle damage from a real photo reference; fingerprint spots), hand-painted masks (confining effect folders to specific areas)
- **Blend modes used:** `Subtract`, `Multiply`, `Texture Overlay`, `Linear Dodge`, `Pass Through`
- **PBR correctness rule (Oxidized Metal):** `Metallic` kept at 0.9 (not 1.0) with a non-pure-black-white metalness mask — "if you have metal that is not clean but oxidized, it shouldn't be clean metal on the metalness map"
- **External tools referenced:** Photoshop (decal text alpha authoring), `Bitmap to Material` (photo -> Normal + Roughness generation for the oxidized-metal texture), Texture.com (source photo) and textures.com (hair alpha)
- **Asset pack:** project file, stencils (including the damaged-paint stencil), and source textures shared publicly by the creator on ArtStation

### Difficulty
Advanced — assumes fluency with Painter's full toolset (anchor points, generators, stencils, multi-layer masking, PBR channel theory) and moves through dozens of layers rapidly with terse narration; best used as a structured reference/checklist (folder by folder) rather than a first-time step-along tutorial.

### App & Version
Not stated explicitly on screen. Modern dark-theme layer-stack UI with `TEXTURE SET SETTINGS` panel and standard per-layer Properties panel, consistent with the post-8.3 Baking Mode era generally seen across this skill's other ingested tutorials — nothing in-frame pins an exact version.

### Tags
layers, fill-layer, paint-layer, masks, generator, anchor-point, blend-mode, ambient-occlusion, curvature, procedural, alpha, stencil, tri-planar, pbr, metal-rough, basecolor, roughness, metallic, height, normal-map, color-management, advanced

---

## Related Tutorials
- [Tempering Colors in Substance Painter | Steel Heat Effects](tempering-colors-in-substance-painter-steel-heat-effects.md) — same creator (Dolinskyi); part of the same multi-video M24 Grenade weapon-texturing project. That video's anchor-point-driven paintable-mask technique is a simpler version of the anchor-point recipes used repeatedly here (Peeling Paint, Decal).
- See `tutorials/INDEX.md` for a possible sibling-ingested "Realistic Wood in Substance Painter | M24 Grenade Texturing" entry — this video explicitly calls itself "part 2" of that series and references techniques from "part 1"; cross-link there once/if present.
