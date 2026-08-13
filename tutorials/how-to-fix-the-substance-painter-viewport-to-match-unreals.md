---
title: How to Fix the Substance Painter Viewport to Match Unreal's
source: YouTube
url: https://www.youtube.com/watch?v=Yu8wR4df0IE
author: William Faucher
ingested: 2026-08-13
app: "Substance 3D Painter"
version: "not stated on screen; presented alongside Unreal Engine 4.26 (ray tracing referenced as a 4.26-era default)"
tags: [color-management, viewport, iray-render, pbr, intermediate]
extraction_status: complete
frames_dir: tutorials/frames/how-to-fix-the-substance-painter-viewport-to-match-unreals/
frame_count: 6
frame_status: complete
frame_selection: content-anchored (manual timestamps chosen from transcript, not blind percentages)
---

# How to Fix the Substance Painter Viewport to Match Unreal's

**Source:** [YouTube](https://www.youtube.com/watch?v=Yu8wR4df0IE)
**Author:** William Faucher
**Duration:** 7m50s | 7 section(s)

---

## Raw Data (for Claude Code extraction)

Frames captured — see "Captured Frames" section below.


### Intro [0:00]
**Transcript (timestamped):**
[0:00] Hey guys and welcome back to yet another Unreal Engine 4 tutorial.
[0:02] In today's video, we're going to be taking a look at how to use the Asus LUT to fix the default Substance Painter viewport in order to get a perfect match with the Unreal Engine 4 viewport.
[0:11] Now, before we get started, we're going to be taking a look at exactly what the problem is with the Substance Painter viewport right now and why we should be doing this fix, even if you're not using Unreal at all.
[0:21] So, let's get started.


### Why The Default Linear Viewport Is Not Good [0:23]
**Transcript (timestamped):**
[0:24] Now, as you can see, I've got a model right here with some textures on it and the first thing to come to mind is the viewport in Substance Painter is totally linear.
[0:36] It's in linear space to begin with.
[0:37] Now, Unreal Engine has an Asus color space workflow.
[0:41] So, the viewport in Unreal is going to be in Asus and any viewport in Substance Painter is completely linear.
[0:48] Now, what I mean by this is you'll see, especially in the highlights section, let's zoom in right here where we have some highlights.
[0:53] See?
[0:54] And first off, right away, you can kind of see that the highlights are totally blown out.
[0:58] They're totally clipped.
[0:59] You don't get any detail there.
[1:00] So, let's get even more of a glancing angle here and you can see this whole area here is completely clipped.
[1:06] There's no detail there and that is not good because you're going to be compensating for this.
[1:09] You're going to be adjusting your textures so that you do see some detail there.
[1:13] And when you bring it to Unreal, it's going to look completely different.
[1:16] Now, this is where the Asus LUT comes into place and this is going to help you improve and get much better results in Substance Painter.
[1:25] And not only that, you're going to be getting a perfect one-to-one match between Substance Painter and your Unreal 4 viewport.
[1:33] So, this is how you do it.


### Where to find the ACES Lut [1:35]
**Transcript (timestamped):**
[1:35] The first thing you want to do is we're going to be able to download on ArtStation.
[1:39] You're going to want to download the Asus LUT for Substance Painter.
[1:41] So, I'm going to include this link in the description below.
[1:45] Now, on the ArtStation page, you'll see a lot of other screenshots and comparisons to show you exactly what the LUT is doing and how it compares between Substance Painter and Unreal.
[1:53] So, I'll be showing you guys an example of how it looks myself in this video.
[1:57] But if you need a little bit of reassurance, there's a lot of screenshots here to prove that it does what it does.
[2:02] This right here is basically just a towmapper.
[2:06] It's a LUT that you apply in Substance Painter and this will essentially give you much, much better results in Substance Painter.
[2:14] It's a lot easier to work with.
[2:15] You get much better highlights.
[2:17] So, go ahead and download that first and foremost.
[2:20] Now, once it's downloaded, what you're going to do is you're going to go to the File button up here.


### How to Install and Enable the ACES Lut [2:21]
**Transcript (timestamped):**
[2:24] Go to Import Resources.
[2:27] Click on Add Resources.
[2:31] And when a window pops up, you're going to go find both in the folder that you've downloaded from ArtStation or Gumroad.
[2:38] You're going to click Import both the Asus UB4 log and the Asus Standard log.
[2:43] Import both of these.
[2:44] Click Open.
[2:46] Now, you're going to want to click on Undefined and set this to Color LUT to both of them.
[2:53] Import your resources to...
[2:54] I'm going to import it to my current session.
[2:57] Or I'm actually going to import it to my shelf.
[2:59] You hit Import.
[3:01] Now, once they're imported, you'll see right away, you know, what do you do with this LUT?
[3:06] So, you're going to want to go up here into Display Settings.
[3:08] There's going to be a little button right here, the second one from the top.
[3:11] Click on that.
[3:13] Activate Post Effects.
[3:15] Click on this.
[3:17] On this Tone Mapping tab, click on the little arrow.
[3:21] Make sure that Tone Mapping is checked.
[3:23] Function is set to Log.
[3:26] Okay, yes, your screen is going to get darker. This is normal.
[3:29] Now, scroll all the way to the bottom and you're going to see Activate Color Profile.
[3:34] Click on this.
[3:35] Now, it's going to get even darker.
[3:37] Click on Profile and you're going to choose Aces UE4 Log.
[3:44] Now, everything is kind of brighter. Make more sense.
[3:46] You'll see right away that it's already much more contrasty.
[3:49] There's much more punch in there.
[3:51] But the best thing is, look at our highlights now.
[3:54] Notice how our highlights have all the detail.
[3:57] Everything is there. Even at the most glancing angles, you see that, hey, look, there is detail in there.
[4:02] Let me zoom in even more and you'll see where I've before.
[4:06] If I uncheck this and uncheck this, you'll see it's totally clipped.
[4:10] There is no detail here.
[4:12] So this is how we get the Aces LUT activated.
[4:17] And, you know, just doing it before and after, you can see right away, everything just looks a lot better, especially in the highlights.
[4:24] So by default, it's at the linear and linear is not really a great color space to be working in.
[4:28] It doesn't really look good.
[4:30] And if you're doing 3D work, chances are your workflow revolves around the Aces color space workflow.
[4:37] So if you're working in Painter, you really should be using this Aces LUT, even if you're not working in Unreal.
[4:44] Now, another major benefit of this, actually the main benefit of this is,
[4:50] once you have this LUT on, the results you're going to get in Unreal Engine are going to be a perfect match.
[4:55] Have you ever had the issue where you import your textures from something Painter, you bring them into Unreal,
[4:59] and it looks completely different?
[5:01] That's why.
[5:02] This fixes that issue.
[5:04] So let's go ahead and open this same model into Unreal with the same textures and we'll do a comparison between the two.
[5:10] And you'll see the results are pretty much exactly the same.


### Comparison between Substance Painter and UE4 [5:13]
**Transcript (timestamped):**
[5:15] So I have Unreal here on the right and I've got something Painter here on the left.
[5:19] Now, of course, as you can see right now, there's already a little bit of difference right now.
[5:23] The main reason for that is because by default in the Unreal viewport as of 4.26,
[5:27] you've got ray tracing, you've got reflections, and you got shadows in here,
[5:30] whereas something Painter does not have any of those features.
[5:33] So in order to troubleshoot this and remove any kind of discrepancy between two,
[5:37] I'm going to go ahead and set Unreal to Path Tracing.
[5:40] So if you go to the little bit tab up here and click Path Tracing,
[5:44] and in something Painter, I'm going to set this to, I'm going to open the Eye Ray Renderer.
[5:48] So both of these are Path Tracers.
[5:50] Therefore, the results, you're going to be factoring out any kind of screen space effects or any kind of ray tracing effects
[5:55] that one may have and the other may not.
[5:58] So we're going to make sure that both our renders are both Path Tracers to remove any kind of inconsistencies.
[6:04] So as you can see right now, I've got the Eye Ray Renderer on, and the results are pretty much exactly the same.
[6:13] Now, Eye Ray is a little bit noisier, but you can see the colors, the highlights, everything just matches and looks pretty much the same.
[6:21] Like I said, there's a few differences that have to do more with, more to do with the depth of field,
[6:26] the angle might be slightly different, but for the most part, this is, I'm satisfied with these results.
[6:33] So seeing this right here, I'm like, yep, okay, this looks pretty much the same.
[6:36] There's no wild discrepancy between the two.
[6:40] This, having this ACE as a workflow makes things so much easier if you're working with, you know, in Unreal,
[6:47] because what you see in Painter is what you're going to get in Unreal.


### Scene setup in Unreal [6:49]
**Transcript (timestamped):**
[6:49] Just to explain a little bit what I've done here in Unreal is I went ahead and got an HDRI from HDRI Haven,
[6:56] just to make sure that, you know, the HDRI, the lighting is exactly the same in both scenes.
[7:00] I went ahead and imported that HDRI both in Painter and in Unreal.
[7:04] In Unreal, I've used the HDRI backdrop light in order to get the same kind of lighting that Painter has.
[7:10] So both these scenes are using the exact same HDRI mapping with the exact same exposure settings.
[7:15] And that's really all I have in Unreal right now.
[7:17] It's just one light, that HDRI backdrop, and that's it. Nothing else.
[7:20] So that's it, folks. It's as simple as that. Use that ACE's LUT. It is a game changer.
[7:25] It really makes things a lot easier for me.
[7:27] It's definitely been a huge improvement to my texturing workflow in something Painter.


### Outro and Thanks [7:32]
**Transcript (timestamped):**
[7:32] So guys, as always, if you have any questions whatsoever, or if you have any suggestions for future videos,
[7:36] something you would like me to cover, leave a comment down below.
[7:39] I'll get right back to you as soon as I can. I am completely open to suggestions.
[7:42] Once again, don't forget to like and subscribe, and I'll see you guys next week.



---

## Captured Frames

- [0:53] tutorials/frames/how-to-fix-the-substance-painter-viewport-to-match-unreals/frame_000.jpg
- [2:44] tutorials/frames/how-to-fix-the-substance-painter-viewport-to-match-unreals/frame_001.jpg
- [3:21] tutorials/frames/how-to-fix-the-substance-painter-viewport-to-match-unreals/frame_002.jpg
- [3:57] tutorials/frames/how-to-fix-the-substance-painter-viewport-to-match-unreals/frame_003.jpg
- [5:19] tutorials/frames/how-to-fix-the-substance-painter-viewport-to-match-unreals/frame_004.jpg
- [6:04] tutorials/frames/how-to-fix-the-substance-painter-viewport-to-match-unreals/frame_005.jpg

---

## Structured Notes

### Core Technique
Import a free third-party ACES LUT resource (two Color-LUT files: ACES UE4 Log and ACES Standard Log) and activate it through Display Settings → Post Effects → Tone Mapping (Function = Log) → Activate Color Profile → Profile = ACES UE4 Log, to replace Painter's default fully-linear viewport tonemapping — fixing blown-out/clipped highlights and producing a near-exact visual match with Unreal Engine's own ACES-based viewport.

### Summary
Diagnoses the root problem first: Substance Painter's default viewport renders in pure linear space with no tonemapping curve, so highlights clip hard with zero retained detail (demonstrated in close-up on a metal helmet surface) — this mismatch is why textures that look fine in Painter often look wrong once brought into Unreal, which uses an ACES-based color workflow. The fix is a free downloadable "ACES LUT for Substance Painter" resource (ArtStation/Gumroad): import both included files (ACES UE4 Log, ACES Standard Log) via File → Import Resources → Add Resources, set each resource's type to **Color LUT**, then import to the shelf. Activate it via the Display Settings panel (the second icon from the top) → **Activate Post Effects** → open the **Tone Mapping** tab → check **Tone Mapping**, set **Function = Log** (viewport gets noticeably darker — expected) → scroll down and check **Activate Color Profile** → set **Profile = ACES UE4 Log** (darkens further, then resolves to a more contrasty, punchier image with full highlight detail restored, confirmed by re-toggling the two checkboxes for a direct before/after). This ACES workflow is argued as worth using even outside an Unreal pipeline, since linear-only viewing is a poor working space in general. To validate the match, the same model/textures/HDRI lighting setup (same HDRI, same exposure, HDRI Backdrop light in Unreal) is compared side-by-side in both apps; because Unreal 4.26 defaults to ray tracing/reflections/shadows that Painter's viewport lacks, both apps are switched to their respective **offline path tracers** (Unreal's Path Tracing view mode, Painter's **Iray Renderer**) to remove screen-space/ray-tracing feature discrepancies from the comparison — with the ACES LUT active, the two path-traced renders match closely (Iray reads slightly noisier; only depth-of-field and minor camera-angle differences remain).

### Key Steps
1. Diagnose the problem first: zoom into a viewport highlight on a glancing angle — Painter's default linear viewport shows fully clipped/blown-out highlights with no retained detail.
2. Download the free "ACES LUT for Substance Painter" resource pack (ArtStation/Gumroad link), which contains two LUT files: ACES UE4 Log and ACES Standard Log.
3. In Painter: **File → Import Resources → Add Resources**, browse to the downloaded folder, select and import both LUT files.
4. For each imported resource, change its type from "Undefined" to **Color LUT**; choose an import destination (current session or shelf).
5. Open **Display Settings** (second icon from the top of the viewport toolbar) → **Activate Post Effects**.
6. Open the **Tone Mapping** tab, check **Tone Mapping**, set **Function = Log** (viewport darkens — expected, not an error).
7. Scroll to the bottom of the panel and check **Activate Color Profile**, then set **Profile = ACES UE4 Log** (viewport darkens again briefly, then resolves brighter/more contrasty with full highlight detail restored).
8. Verify by toggling Tone Mapping/Color Profile off and back on — confirms the direct before/after difference in highlight retention.
9. To validate a real Painter-to-Unreal match: build matching scenes in both apps using the **same HDRI** (same file imported into both, same exposure) — Unreal via an HDRI Backdrop light, Painter via its own environment lighting.
10. Because Unreal defaults (4.26-era) to ray tracing/reflections/shadows that Painter's raster viewport doesn't have, switch **both** apps to an offline path tracer for the comparison: Unreal's **Path Tracing** view mode, Painter's **Iray Renderer** — this removes ray-tracing/screen-space-effect discrepancies as a confound.
11. Compare the two path-traced renders side by side — with the ACES LUT active, colors/highlights match closely (Iray is slightly noisier by nature; remaining differences are just depth-of-field/camera-angle, not color).

### Layers / Tools / Settings
- `File → Import Resources → Add Resources` — import ACES UE4 Log + ACES Standard Log as **Color LUT** resource type
- `Display Settings → Activate Post Effects → Tone Mapping` tab: `Tone Mapping` checked, `Function = Log`
- `Display Settings → Activate Color Profile`, `Profile = ACES UE4 Log`
- `Iray Renderer` (Painter's offline path tracer, used for the Unreal-comparison render) vs. Unreal's **Path Tracing** view mode
- Matching HDRI environment imported into both apps at the same exposure (Unreal: HDRI Backdrop light)

### Difficulty
Beginner (all steps are UI toggles/imports — the value is knowing the fix exists and why, not technical complexity)

### App & Version
Not stated on screen for Substance Painter; shown alongside Unreal Engine 4.26 (ray tracing/reflections/shadows-by-default referenced as a 4.26-era Unreal behavior).

### Tags
`color-management` `viewport` `iray-render` `pbr` `intermediate`

---

## Related Tutorials
- **How to Make the Substance Painter Viewport Match Unreal Engine** (Quinn Kuslich) — alternate creator covering the same viewport-matching goal; cross-link both ways once ingested per the user's explicit instruction (same topic, alternate creators/techniques).
- [Substance 3D Painter & ACES - 01 - Color Space Fundamentals](substance-3d-painter-aces---01---color-space-fundamentals-adobe-substance-3d.md) — Adobe's own official ACES series covers the same underlying linear-vs-ACES color-space problem this LUT trick works around, from the theory side (CIE diagram, sRGB gamma curve, why ACEScg matters).
- [Substance 3D Painter & ACES - 02 - OCIO & ACEScg in Painter](substance-3d-painter-aces---02---ocio-acescg-in-painter.md) — Adobe's official, built-in alternative to this third-party LUT: Painter's native OpenColorIO/ACEScg project color-management setup achieves a related goal (consistent, non-clipped color across the pipeline) through Painter's own Color Management system rather than a Display Settings LUT hack.
