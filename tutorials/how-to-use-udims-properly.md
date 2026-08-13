---
title: How to use UDIMs properly!
source: YouTube
url: https://www.youtube.com/watch?v=yf9CPHE5BYg
author: 3DRedBox
ingested: 2026-08-13
app: "Substance 3D Painter (Painter-side portion only; most of the video is RizomUV, a third-party UV-packing tool)"
version: "not stated on screen; the Painter-side portion (UV Texel Density generator check) shows no version-specific UI markers"
tags: [udim, texture-set, uv, texel-density, generator, layers, paint-layer, basecolor]
extraction_status: complete
frames_dir: tutorials/frames/how-to-use-udims-properly/
frame_count: 7
frame_status: complete
frame_selection: content-anchored (manual timestamps chosen from transcript, not blind percentages)
---

# How to use UDIMs properly!

**Source:** [YouTube](https://www.youtube.com/watch?v=yf9CPHE5BYg)
**Author:** 3DRedBox
**Duration:** 17m19s | 1 section(s)

---

## Raw Data (for Claude Code extraction)

Frames captured — see "Captured Frames" section below.


### Full Content [0:00]
**Transcript (timestamped):**
[0:00] UDIM and keep the text density same per tile is a problem for you.
[0:16] I'm Mehdi from 2D Red Box Channel and today in this video we want to talk about how to
[0:21] keep the same text density across multi-tiles in UV.
[0:27] So, be with me in this video, we are going to explore this.
[0:31] But before that, let me introduce you the brand new course that we release for Substance
[0:37] Painter.
[0:39] Learning Substance Painter is easier than ever.
[0:42] Hey all Substance Lovers, Tech Change Seekers and awesome future artists, welcome to ultimate
[0:48] course for learning Substance Painter from Zero to Hero.
[0:58] Ready to learn how to texture with different projects, Substance Master released a brand
[1:02] new course for those who want to learn to texture with Substance Painter.
[1:08] In this course we cover from preparing the model to rendering different projects, different
[1:13] challenges.
[1:14] If you want to level up your skill in texturing, come and check the Substance Master Ultimate
[1:19] course for learning Substance Painter.
[1:22] Ok, now we are here and we have this model and we want to texture this inside Substance
[1:28] Painter.
[1:29] But there is one problem here.
[1:32] This model is so big.
[1:34] It contains so many small pieces.
[1:38] And how we are going to manage the quality inside UV and the final texture.
[1:46] And in here the first solution is to pack all the UV island inside one UV tile.
[1:54] And let's do that and compare it to the other option that we have.
[1:58] Ok, let's copy this model and I'm going to rename it UV1.
[2:05] And for sending this model to the RISOM UV, I use the bridge that's very easy and fast
[2:13] and you can use it in 3ds Max and you can find the link of this script inside the description.
[2:21] So let's put it on edits and click on send to RISOM UV.
[2:26] And when we use the RISOM bridge, it's automatically open the RISOM UV and import our model with
[2:34] the UV.
[2:36] And now I'm going to pack this UV inside the RISOM.
[2:41] And how we can achieve the best result inside the RISOM?
[2:46] We just need to go to the packing properties and change accuracy to ultra and iteration
[2:53] to something like 4 or 8 and after that we can set initial orientation to V and change
[3:03] orientation optimization to 90.
[3:07] And now I can go and click on pack.
[3:10] And as you can see, we have a perfect packing of UV inside one UV tie.
[3:18] And for bring it back to 3ds Max, we just need to press CTRL S and now we have the model
[3:25] inside 3ds Max.
[3:28] And let's add some material to this model because we want to compare this with another
[3:35] option that we are going to create.
[3:38] For this purpose, I just use a simple 1K texture and tile it 4 times because we want
[3:48] to represent the 4K texture.
[3:53] So let's apply to this model and this is the final quality that we are going to get from
[4:01] 4K texture on this model.
[4:05] Compare this pixelate issue that we have here and I'm going to copy this model again and
[4:15] rename it UDEMS 1 and let's bring it to RISOM.
[4:22] And we are in RISOM again and for increasing the quality when we want to use something
[4:30] like texturing in substance painter and create unique texture, we need to extend our UV
[4:38] tile to 2, 3 or 4 or more.
[4:42] And we call it this technique UDEMS and in RISOM we can increase UV tile spaces with
[4:52] this window, little window here.
[4:55] And let's increase it to something like 4 and I'm going to change accuracy to ultra,
[5:03] iteration 4 and initial orientation to V and orientation optimization to 90.
[5:13] And now I'm going to pack it again and now we have 4 UV tiles as you can see and let's
[5:20] save it and bring it back to 3ds Max.
[5:24] And let's give the same material to this model and now you can see we have more quality
[5:34] on this texture.
[5:36] And the reason is we have more UV tile, it means we have more UV space and when we have
[5:44] more UV space we can increase the UV island size so we have more pixel on each UV island
[5:54] and it means we have better quality compared to one UV tile.
[6:03] But the problem here is when we increase our UV tile number we may get different size of
[6:12] each UV island in different UV tile.
[6:17] So how we can solve this problem and for solving this problem we need to keep same
[6:24] pixel density when we are going to pack all the UV island in UDEMS or multiple UV tile.
[6:36] So let me bring another version here and let's call it UDEMS 2 and send it to RISO.
[6:49] Okay now we are here in RISO and the packing properties it's same that we discussed before
[6:58] and now I'm going to increase again the UDEMS to 4 tile and let's pack all the UV island
[7:10] across these tiles.
[7:12] Okay this is the final pack but it's not correct I just changed it for demonstration purpose.
[7:21] We don't get this kind of effect when we pack inside RISO UV because we use initial scale
[7:30] keep average pixel density option but in here I just want to show you what happen if we
[7:37] have different scale on each UV island.
[7:43] And the translation of this matter is we have the lower quality here and higher quality
[7:52] in here and this is the problem okay and it happens all the time when we want to use UDEMS
[8:02] in complex object okay and how we are going to solve this.
[8:08] For solving this issue we need to understand how toxial density works but it's kind of
[8:17] complex matter so let's keep it away and stick to the simple way that I'm going to show you.
[8:25] So we have map res and texial density target option here and for the map res we need to
[8:36] find out what is the final dimension that we are going to export for example from Substance
[8:42] Painter or even what is the size of the final texture that we are going to use in our material
[8:49] inside our project okay and in here it's 4k so let's put 4096 here and if we are going
[9:01] to use 2k let's put it 2048 and what's about the texial density target for this matter
[9:09] let me show you easy way okay so let's pick biggest UV island that you have okay for example
[9:19] this one this is the biggest UV island that I have and let's isolate it and just press
[9:28] on back okay and select this and pick okay as you can see we have 43 texial density target here
[9:43] okay it means we have the quality near to 4k and it's good it's good but what happened if I use
[9:57] this texial density target let's select all this UV island and press rescale and as you can see
[10:09] maybe we need more than four tiles here so let's give it eight okay and now we need to change
[10:21] texial density target to something like this I just use the map res and divide it by 100
[10:33] because I just use centimeter here okay for modeling and now it times to change some setting
[10:43] in packing properties the first one is changing initial scale to texial density and after that
[10:54] turn off scale optimization range from full to off and now it's time to use
[11:04] packing here and let's wait and see what's happening okay now after packing all the UV island in eight
[11:15] UV tile as you can see we have the great quality here but we have some space here
[11:23] and for solving this issue we can go here and select some of the UV island and bring down
[11:33] the scale of them so in this way we can save some space for these icons and pack it up all the UV islands
[11:47] in seven UV tile okay not eight but it's okay for me right now and let's save it and explore another
[11:57] option here okay now we can understand how we can keep the same size or same texial density
[12:07] when we want to pack all the UV island with udim's method okay but this is the method based on
[12:18] texial density what happened if we have some limitation for example we can just use four
[12:27] UV tile how we can keep the same size in four or three UV tile let's do that now I'm in the
[12:36] RISO and we have three tile with the udim's and I just pack all the UV island with the same packing
[12:46] properties that we discussed before and let's check the scale or texial density of each UV island
[12:55] inside each UV tile and the map res here is 4k so I need to change map res and just select
[13:06] this one and use this checker and the texial density is 24 and for this one it's 24 but we have some
[13:19] small difference in the number after dot okay and this is 23 so we have the same texial density
[13:35] almost the same but what's happened if we want to keep the same texial density when we want to have
[13:44] the three udim's okay so we have 23 and 24 okay so let's pick 22 here and I just turn off the
[14:00] scale optimization range and change initial scale to texial density and now when we
[14:08] click on the pack the texial density of each UV island should be 23 and as you can see we have 23 here
[14:20] 23 here and here so in this way we can keep the same texial density or same scale of
[14:32] UV islands in different UV tile and for the last part let me show you how we can check the texial
[14:41] density quality inside substance painter okay now we are in substance painter and whenever we import
[14:49] something like a complex model and we don't sure the UV is okay and at the end we can get
[14:58] a good quality of that we have a generator inside substance painter that we can use
[15:06] and check the quality of the UV so in here I just add generator on the paint layer go to the generator
[15:18] and just use UV texial density and let's just keep the color and whenever we have the red color
[15:30] or something like red it means we don't have enough quality inside the UV okay and for the green it
[15:41] means it's okay and we can continue but we couldn't use the lower size like 2k or 1k and we just need
[15:52] to export higher quality like 4k or 8k and when we have the blue color it means we are in a good
[16:01] position and we could use for example 2k as a final export and we get a good quality okay so in here
[16:13] for this UV we get the green color okay and now let's go I'm going to copy this layer and let's go
[16:26] to the next model and in the next model we have 8 UV tile okay and let's copy that and as you can see
[16:39] we get the blue color here so we are good and we can start our process and texture this model
[16:49] and that's it this is for this video I hope you learned something new and I can answer your
[16:56] question because we have a lot of questions about the UV u-dims and keep the same texial density
[17:03] across multi tile and this kind of question if you learned something new or like this video
[17:11] please hit the like button subscribe our channel be creative bye



---

## Captured Frames

- [3:56] tutorials/frames/how-to-use-udims-properly/frame_000.jpg
- [5:28] tutorials/frames/how-to-use-udims-properly/frame_001.jpg
- [8:55] tutorials/frames/how-to-use-udims-properly/frame_002.jpg
- [10:57] tutorials/frames/how-to-use-udims-properly/frame_003.jpg
- [15:10] tutorials/frames/how-to-use-udims-properly/frame_004.jpg
- [15:55] tutorials/frames/how-to-use-udims-properly/frame_005.jpg
- [16:32] tutorials/frames/how-to-use-udims-properly/frame_006.jpg

---

## Structured Notes

### Core Technique
Keeping texel density (pixel-per-unit resolution) consistent across every UV island when packing a UV-Tile (UDIM) layout, using RizomUV's texel-density-driven packing mode — plus how to verify the result is actually good enough directly inside Substance Painter using the built-in `UV Texel Density` generator.

### Summary
Mostly a UV-preparation video done in the third-party tool RizomUV (via a 3ds Max bridge plugin, though the concept applies in any DCC/UV tool), with a short Substance-Painter-side verification step at the end. Opens by demonstrating the actual problem UDIMs solve: packing a complex, many-small-pieces model into a single UV tile forces small UV islands and visibly pixelated 4K textures, while extending to multiple UV tiles (UDIMs) gives each island more UV space and therefore more texture resolution — but naively packing across multiple tiles can leave different islands at wildly different scales/texel densities relative to each other (demonstrated with a deliberately bad example). The fix is RizomUV's texel-density-driven packing: set `Map Res` to the actual final export resolution (4096 for 4K, 2048 for 2K, etc.), then derive a `Texel Density Target` value from the largest UV island in the scene (select it, isolate it, read its texel density, e.g. ~43 for a 4-tile pack) — if that number implies needing more tiles than currently allotted, rescale and increase the tile count accordingly (demoed going from 4 to 8 tiles, with the divide-by-100-for-centimeter-units caveat when computing texel density target from map res). Critically, `Initial Scale` in Packing Properties must be set to `Texel Density` (not the default) and `Scale Optimization` range must be turned `Off`, so RizomUV preserves the target density instead of auto-rescaling islands to save space — any resulting empty gaps are cleaned up by manually shrinking a few oversized islands to reclaim tile count (demoed reducing from 8 tiles down to 7). The same method is shown solving a tighter-constraint scenario — matching texel density across only 3 fixed UV tiles by manually dialing in a texel density target (22) partway between two islands' natural values (23 and 24) so both land on the same final number once packed. The video closes in Substance Painter: add the built-in `UV Texel Density` generator to a paint layer's Color channel to get a heatmap validation of the imported UV layout — red means insufficient resolution for the intended export size (must go higher, e.g. from 2K/1K up to 4K/8K), green means the current setting is workable but you couldn't safely go lower, and blue means there's headroom (a lower export resolution, e.g. 2K, would still look good) — demonstrated getting green on a single-tile model and copying the same generator setup onto an 8-UV-tile model for the same check.

### Key Steps
1. **Understand the baseline problem before reaching for UDIMs:** packing a complex model's many small pieces into a single UV tile forces tiny UV islands, which produces visibly pixelated results even at 4K export — demonstrated by tiling a 1K texture 4x to simulate a 4K result on a single-tile-packed model.
2. **Extend to multiple UV tiles (UDIMs) for more resolution headroom:** in RizomUV, increase the UDIM tile count (demoed 1→4) via the tile-space window, then re-pack with `Accuracy: Ultra`, `Iteration: 4-8`, `Initial Orientation: V`, `Orientation Optimization: 90` — more tiles means more total UV space, which lets island sizes grow, which directly increases per-island pixel density.
3. **Recognize the multi-tile trap:** naively packing across multiple UV tiles can leave different islands at very different scales relative to each other, producing visibly inconsistent texture quality across the model (some areas sharp, some blurry) even though the overall resolution increased — demonstrated with a deliberately mismatched pack for illustration.
4. **Set `Map Res` to your actual final export resolution** (4096 for a 4K export, 2048 for 2K, etc.) in RizomUV — this is the reference the texel density calculation is built from.
5. **Derive a `Texel Density Target` from your largest UV island**, not an arbitrary number: select and isolate the biggest island, read its texel density value (e.g. ~43), and use that as the packing target for every island in the scene.
6. **Rescale and re-tile if the derived target needs more space than currently allotted**: if a target density requires more UV tiles than you have (e.g. 4 isn't enough, so go to 8), compute a matching texel density target from Map Res (Map Res ÷ 100 when working in centimeters, per this creator's modeling unit convention).
7. **Set Packing Properties to actually honor the texel density target:** change `Initial Scale` to `Texel Density` (instead of the default automatic scaling) and turn `Scale Optimization` range from `Full` to `Off` — without this, RizomUV will silently re-optimize island sizes to save space and undo the consistent density you just calculated.
8. **Clean up leftover empty tile space after a texel-density-locked pack:** select a subset of islands and manually reduce their scale slightly to reclaim wasted space, potentially reducing the total tile count needed (demoed 8 tiles down to 7) without sacrificing the target density on the islands that matter most.
9. **Apply the same method under a fixed tile-count constraint:** when you can't add more tiles (e.g. locked to 3), read the texel density each island naturally lands at after a normal pack (e.g. 23 and 24), then manually set `Texel Density Target` to a value in that range (22), with `Initial Scale = Texel Density` and `Scale Optimization = Off`, so a final re-pack brings every island to the same density (23 across all three tiles in the demo) instead of leaving them slightly mismatched.
10. **Verify the resulting UV layout's quality directly inside Substance Painter** once imported: add the built-in `UV Texel Density` generator to a layer's Color channel (Fill or Paint layer, Generator picker) — this heatmaps the model in red/green/blue based on how much resolution headroom the UVs provide relative to the project's current export size.
11. **Read the heatmap result correctly:** red = not enough quality at the current export size, must go higher (e.g. bump from 2K/1K up to 4K/8K); green = current setting is right at the edge — usable, but don't try to go lower; blue = comfortable headroom, a lower export size (e.g. 2K) would still look fine. Repeat the same generator check on any other texture set/UV variant in the same project (demoed copying the layer setup from a 1-UV-tile model to an 8-UV-tile model) to confirm each holds up before committing to full texturing work.

### Layers / Tools / Settings
- **External tool used (not Painter):** RizomUV, connected via a 3ds Max bridge plugin (link provided by the creator) — packing properties: `Accuracy: Ultra`, `Iteration: 4-8`, `Initial Orientation: V`, `Orientation Optimization: 90`, `Initial Scale: Texel Density` (critical), `Scale Optimization: Off` (critical)
- **RizomUV concepts used:** `Map Res` (set to the real final export resolution), `Texel Density Target` (derived from the largest UV island, or manually tuned to match a fixed tile-count constraint), UDIM tile-count window
- **Substance Painter generator used:** `UV Texel Density` (Color channel), with a red/green/blue quality legend: red = insufficient resolution, green = at-the-edge but workable, blue = comfortable headroom
- **Painter layer type used for the check:** a simple `Paint` layer holding only the generator, no actual paint data — purely diagnostic
- **Texture Set List:** used to switch between UV-tile variants of the same model (1-tile vs. 8-tile) to compare texel-density results side by side

### Difficulty
Intermediate — the underlying concept (texel density) is explicitly flagged by the creator as "kind of complex" and deliberately simplified into a repeatable recipe; executing it correctly requires comfort with a third-party UV tool (RizomUV) rather than anything inside Painter itself. The Painter-side verification step (UV Texel Density generator) is beginner-friendly on its own.

### App & Version
Substance 3D Painter — version not stated on screen, and the Painter-side portion of this video (the `UV Texel Density` generator check) shows no version-specific UI markers to pin against `references/version-tracker.md`. The bulk of the video takes place in RizomUV (third-party UV-packing software, unrelated to Painter's own version history) via a 3ds Max bridge plugin.

### Tags
udim, texture-set, uv, texel-density, generator, layers, paint-layer, basecolor

---

## Related Tutorials
- [Texturing a Worn Wooden Stool in Substance Painter](texturing-a-worn-wooden-stool-in-substance-painter.md) — same creator (3DRedBox); shares the "solve texel-density problems for many-small-pieces models before entering Painter" philosophy (overlapping UVs there, texel-density-locked UDIM packing here), both explicitly framed as DCC-side prep done ahead of texturing.
- [Speed Up Your Substance Painter Workflow with This Easy Trick!](speed-up-your-substance-painter-workflow-with-this-easy-trick.md) — same creator; both are short, focused troubleshooting videos addressing a specific pipeline pain point on complex multi-piece models, solved primarily outside Painter in the DCC/UV tool.
- [Texturing Tactical Boots In Substance Painter](texturing-tactical-boots-in-substance-painter.md) — same creator; both address UV-space texel-density/consistency problems (RizomUV-side packing here, an in-Painter secondary-UV-set fix applied twice there).
- More 3DRedBox tutorials (UV-set/stencil video, NavyCap) will be cross-linked here as they are ingested — see `tutorials/INDEX.md` for the current full list.
