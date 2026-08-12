---
title: Substance 3D Painter 12.1 Beta: New Features, Faster Workflows, OpenPBR Support | Adobe Substance 3D
source: YouTube
url: https://www.youtube.com/watch?v=z-xbXtyPykI
author: Adobe Substance 3D
ingested: 2026-08-12
app: "Substance 3D Painter"
version: "12.1.0-beta"
tags: [baking, mesh-maps, high-to-low-poly, painter-12, intermediate]
extraction_status: complete
frames_dir: tutorials/frames/substance-3d-painter-121-beta-new-features-faster-workflows-openpbr-support-adob/
frame_count: 8
frame_status: complete
frame_selection: content-anchored (manual timestamps chosen from transcript, not blind percentages)
---

# Substance 3D Painter 12.1 Beta: New Features, Faster Workflows, OpenPBR Support | Adobe Substance 3D

**Source:** [YouTube](https://www.youtube.com/watch?v=z-xbXtyPykI)
**Author:** Adobe Substance 3D
**Duration:** 9m4s | 1 section(s)

---

## Raw Data (for Claude Code extraction)

Frames captured — see "Captured Frames" section below.


### Full Content [0:00]
**Transcript (timestamped):**
[0:00] Hi, welcome to this video about Substance 3D Painter Beta 12.1.
[0:05] This beta version features SKU painting and baking, auto rebake, open PBR and the new hard
[0:12] surface unwrap mode.
[0:14] This video was specifically focused on the SKU baking and the auto rebake.
[0:18] Now before we get into that, let's take a quick look where you can find and access this
[0:21] beta first.
[0:23] First option is on Creative Cloud Desktop.
[0:26] From home, if you go to apps and then click on beta at the top here, scroll down, you
[0:33] should see the Substance 3D Painter Beta.
[0:35] Just click install and it should install it.
[0:38] The good thing about using this method is that you can keep both the old and the newer
[0:43] beta version at the same time.
[0:46] The other option is to use Steam.
[0:47] So if I go to Steam, go to your library, find Substance 3D Painter, right click, go to properties
[0:55] and find the game versions and betas.
[0:58] You should see that under the default public version, there's a 12.1 beta.
[1:03] Click that and it should start installing instantly.
[1:07] Keep in mind that if you do it on Steam, you replace your current version with the beta
[1:10] version.
[1:11] You cannot have two versions at the same time.
[1:14] Very very important to state as well is that we do not recommend that you use this beta
[1:19] for any serious production work.
[1:21] See it as a test only.
[1:23] Because that you open and save in the beta cannot be opened in the older versions, things
[1:27] might change and there might be general instability.
[1:30] See this testing only.
[1:34] Now let's get into this and take a look at what the SKU baking and auto rebake is about.
[1:39] I have a file open here and this is a fairly low poly file just to show you.
[1:44] It's a radio that has a very low poly mesh wireframe.
[1:49] Let's get started with this.
[1:50] Let's go into the baking mode and we have to fulfill a few requirements first before we
[1:55] can start using this SKU baking.
[1:57] The first one is we have to load a high poly.
[2:00] So I'm going to open this here, load my high poly and see it has been placed in here.
[2:07] Now I don't even have to do an initial bake, but just to make it go a bit quicker, I'm
[2:12] going to turn off everything except the normal map because that is where SKU is the most
[2:16] visible.
[2:17] I'm going to click bake selected textures.
[2:22] I'm also going to turn off the high poly mesh and cage wireframe so we see things a bit
[2:26] better and then we'll take a look at the actual problem that's happening here.
[2:31] So because this is such a low poly mesh, you see we're getting very strong skewing artifacts
[2:35] such as here at the bottom or here because of the way the rays are traced, the bakes come
[2:42] out very distorted and not the most representative of the actual high poly mesh that we have
[2:47] here.
[2:48] SKU baking, the SKU painting is here to fix that for you.
[2:52] So how do you use it exactly?
[2:54] Well, you scroll down in the common settings and you find the SKU correction or you can
[2:59] also use this little tab at the top.
[3:01] Click it to jump down immediately to SKU correction.
[3:05] You click on paint SKU correction and you enter into a new mode.
[3:10] You can now paint inside the baking mode and paint these SKU correction errors out.
[3:14] So for example, if we find this one at the bottom here, going to reduce the size of my
[3:19] brush just a little bit, paint, you see that it rebakes and my SKU problem has been solved.
[3:28] Let's do that again.
[3:29] And what you see at the same time happening is that these red wires that represent the
[3:32] bake directions are also modified.
[3:35] The red ones are the old average normal directions.
[3:38] The green ones are a specific corrected version where the rays are traced in the correct direction.
[3:44] So at the same time, you might not have noticed, but it's automatically rebaking as well.
[3:48] So every time I finish a stroke, the project rebakes and I see the update here.
[3:55] This is a new feature we've added as well to pair together with the SKU mapping.
[4:00] And if you look closely to the common settings that we have over here, a few things have
[4:03] changed.
[4:05] There are three new icons in here and the auto rebake is this last one.
[4:10] Keep in mind, these icons are going to change.
[4:11] We're actually in the process of designing new ones.
[4:14] So in a later version, these will not be the same.
[4:17] The last one means that auto rebake is active.
[4:20] That means that this specific mesh map will be rebaked as soon as a change is detected.
[4:26] It toggles automatically when you enter a SKU painting mode.
[4:29] But if you turn it off, then you have to manually trigger a bake.
[4:33] So I paint here, I have to click bake, select the textures to do a baking in.
[4:38] It's actually much easier if you keep it on.
[4:40] Performance wise, some remarks, this is on a MacBook M3 and it's set to 2K size.
[4:46] It's actually fairly responsive because it's baking a single map and it does an optimization
[4:50] where it only bakes the changed area.
[4:52] But let me just increase the sub sampling of it to show you how fast that responds.
[4:57] First bake is a bit slower, obviously.
[5:00] But right now, if I paint some more here, you see that it's a bit slower by four sub sampling.
[5:08] A trick if you want this to be faster is you can go down to the brush projection and set
[5:14] it from tangent wrap to UV and you should get much faster responses as well.
[5:19] See, it's almost instant when you do it that way.
[5:23] Now painting is nice, that's one thing, right?
[5:25] So you can go over and manually find all the corrected areas.
[5:28] But it takes a bit of time.
[5:30] It gives you the control but it takes a bit of time.
[5:33] So there might be other methods that you want to use for this.
[5:36] So specifically, what you can do instead is you can use some of the familiar painting
[5:40] tools.
[5:41] Well, the first one is the eraser, which is obviously a simple one.
[5:43] You just erase your painted areas, the ones that are marked in blue.
[5:47] But you can also use the polygon fill tool.
[5:50] So if I click on polygon fill, I can actually fill entire polygons with white.
[5:58] So the color picker at the top here shows you what color you're picking.
[6:00] It's the same polygon fill tool as in painting mode.
[6:03] And this area here, if I click it, it gets rebaked and you see that it's much quicker
[6:08] than painting these out manually.
[6:10] If you're experienced with skew maps, if I turn off the wireframe here, I go and leave
[6:15] the skew painting mode.
[6:19] This might give you some seams.
[6:20] If you look closely here, you're seeing seams.
[6:22] That is because when you're painting skew maps, you want to avoid painting over edges
[6:27] and if you're using a polygon fill, that's a fairly blunt tool.
[6:31] You don't have control over specific edges.
[6:33] That's why we've added a new option to help you edge protection.
[6:37] If you turn this on, it enables a new extra mask that protects your edges.
[6:42] By default, it's fairly big, but if I reduce the distance, so let me just make that quite
[6:46] a bit smaller, something like that, you see that automatically the edges are protected.
[6:55] This means that you can actually work fairly quick if you just turn on the, if you use
[7:00] the polygon fill tool to select whole areas and you never have to worry about painting
[7:06] over edges.
[7:07] In theory, you could even select your entire mesh with the polygon fill tool and just have
[7:12] everything filled like that.
[7:15] My work in some cases might not in others.
[7:18] Then maybe just a little focus on some of these other buttons here.
[7:21] We've added a few extra ones, Exit skew painting.
[7:24] The first button is to show mesh maps quickly.
[7:27] If you want to just see your normal map, you click that icon and it totals to the mesh mode.
[7:31] The exact same as using this dropdown here is just a faster access.
[7:35] These are not baked, so they won't work, but you can only have one active at a time.
[7:39] The other button next to that, the one in between the seeing the mesh map and over rebake,
[7:43] is a quick single rebake.
[7:46] So say I would turn everything on now because I've corrected my skew.
[7:49] I'm going to turn off thickness.
[7:50] I'll bake my selected textures.
[7:56] And if I go into ID and I decide that I want to use something different here, say I want
[8:00] to use sub mesh.
[8:02] I don't want to rebake everything and I don't want to toggle these states.
[8:06] I can just simply click this single bake icon to do a quick rebake of just that map.
[8:11] It means that you don't have to use the checkboxes on this button here.
[8:14] You can just quickly bake an individual map here when it is visible.
[8:18] That's about it for the auto rebake and the skew correction.
[8:22] There's not that much more to say about it.
[8:24] Maybe the last thing that I could point out is in skew mode under skew vectors.
[8:28] You can actually control the length and the density of these vectors.
[8:31] If you get very close, they might be very dense, so you can reduce their density.
[8:36] You can increase the length and you can also play with the opacity.
[8:41] If you don't want them, you just set the opacity down to zero.
[8:44] There's not that much more to it.
[8:47] We are looking for feedback on this.
[8:49] You can actually make use of our Discord channel or the Adobe Community forums to tell us what
[8:54] you think about this release and help us shape the feature before we go for the final release.
[9:00] Thanks and have fun with this feature.
[9:02] Let us know what you think.



---

## Captured Frames

- [0:38] tutorials/frames/substance-3d-painter-121-beta-new-features-faster-workflows-openpbr-support-adob/frame_000.jpg
- [1:44] tutorials/frames/substance-3d-painter-121-beta-new-features-faster-workflows-openpbr-support-adob/frame_001.jpg
- [2:31] tutorials/frames/substance-3d-painter-121-beta-new-features-faster-workflows-openpbr-support-adob/frame_002.jpg
- [3:19] tutorials/frames/substance-3d-painter-121-beta-new-features-faster-workflows-openpbr-support-adob/frame_003.jpg
- [4:17] tutorials/frames/substance-3d-painter-121-beta-new-features-faster-workflows-openpbr-support-adob/frame_004.jpg
- [5:14] tutorials/frames/substance-3d-painter-121-beta-new-features-faster-workflows-openpbr-support-adob/frame_005.jpg
- [5:58] tutorials/frames/substance-3d-painter-121-beta-new-features-faster-workflows-openpbr-support-adob/frame_006.jpg
- [6:42] tutorials/frames/substance-3d-painter-121-beta-new-features-faster-workflows-openpbr-support-adob/frame_007.jpg

---

## Structured Notes

### Core Technique
How to install the Substance 3D Painter 12.1 Beta, and a deep, performance-focused walkthrough of its headline **Skew Correction painting** and **Auto Rebake** features (same feature covered in the shipped-12.1.0 video "Skew Baking & Auto Rebake in Painter 12.1", but from the beta build with extra speed-tuning tips).

### Summary
Despite the title namechecking OpenPBR and the new hard-surface unwrap mode, the video explicitly narrows scope to only Skew Baking and Auto Rebake ("This video was specifically focused on the SKU [skew] baking and the auto rebake" — OpenPBR/unwrap are not demonstrated here). Covers two install paths for the beta (Creative Cloud Desktop "Beta" tab vs. Steam beta branch — Steam replaces your current install, CCD can run both side by side) plus an explicit warning not to use the beta for production (project files saved in it aren't openable in older versions). The bulk of the video repeats and extends the Skew Correction / Auto Rebake workflow: color-coded skew-direction wires (red = old average normal direction, green = corrected direction after a fixed stroke), practical speed tips (switch Brush Projection from Tangent Wrap to UV for near-instant rebakes; sub-sampling raises quality but slows rebakes), the Eraser and Polygon Fill as faster alternatives to manual painting, Edge Protection to stop Polygon Fill from bluntly painting over UV seams, and the quick per-map "view mesh map" / "single rebake" buttons next to Auto Rebake.

### Key Steps
1. Install the beta via Creative Cloud Desktop → Apps → Beta tab → find "Substance 3D Painter (Beta)" → Install (keeps old + beta side by side), **or** via Steam → Library → Substance 3D Painter → Properties → Betas tab → select the `12.1 beta` branch (replaces the current install; cannot run both from Steam).
2. Do not use the beta for production work — project files saved in it are not backward-compatible with older stable versions, and instability is expected.
3. In Baking Mode, load a High Poly mesh (required before Skew Correction becomes available).
4. Disable all mesh maps except Normal (skew is most visible there) and bake once to see the problem — a low-poly mesh produces visibly distorted, skewed bakes from how rays are traced.
5. Open Skew Correction (scroll down in Common Settings, or use the dedicated top tab to jump straight to it) and click **Paint Skew Correction** to enter paint mode.
6. Paint directly over a skewed area; the stroke automatically triggers a rebake on release. The overlay wires update live: **red** = old average normal (ray) direction, **green** = the corrected direction after painting.
7. Auto Rebake is one of three new icons added to Common Settings in this beta (icons are explicitly noted as placeholder/WIP, subject to change before final release); it auto-enables the moment you enter Skew Painting mode, and rebakes only the changed region for speed — turning it off means you must manually click Bake to see corrections.
8. Performance tip: on a MacBook M3 at 2K output, single-map incremental rebakes are fast by default; raising sub-sampling (e.g. to 4x) slows them down noticeably.
9. Speed trick: switch **Brush Projection** from `Tangent Wrap` to `UV` for near-instant rebake response while painting skew corrections.
10. Faster-than-manual-painting alternatives: the **Eraser** removes painted (blue) correction areas; **Polygon Fill** fills entire polygons white in one click for a quick, blunt correction pass (same tool as regular Painting mode; color picker shows the fill color).
11. Polygon Fill can introduce new seam artifacts because it doesn't respect edges — enable **Edge Protection** to auto-mask UV borders/hard edges, and tune `Edge distance` (how far the protection reaches) smaller for tighter protection.
12. Additional per-map quick-action buttons next to Auto Rebake: one instantly previews a given mesh map (only one active at a time, doesn't trigger a real bake), the other does a single quick rebake of just the currently visible/selected map — useful when you change one setting (e.g. switch an ID map source to sub-mesh) without wanting to re-bake or re-toggle every checked map.
13. Skew Vectors display settings (under "Skew vectors") let you adjust vector length, density, and opacity — set opacity to 0 to hide the overlay entirely.

### Layers / Tools / Settings
- Skew Correction (`Paint Skew Correction` / `Stop painting`), Skew Vectors (length, density, opacity)
- Auto Rebake toggle (per-map, one active at a time) + quick "view mesh map" button + single quick-rebake button
- Edge Protection (`Edge distance`, `Edge contrast`)
- Eraser, Polygon Fill (color picker)
- Brush Projection (`Tangent Wrap` vs `UV` — UV is faster for skew painting)
- Mesh Map Bakers checklist (Normal, World Space Normal, AO, Curvature, Position, Thickness, Height, Bent Normals, Opacity)
- High Poly mesh assignment (Cage settings)

### Difficulty
Intermediate — same audience as the shipped-12.1.0 skew video; adds beta-installation logistics and performance tuning on top.

### App & Version
**Substance 3D Painter 12.1.0-beta** — confirmed directly from the application window title bar visible in every captured frame ("Adobe Substance 3D Painter Beta 12.1.0-beta..."). Cross-referenced against `references/release-notes-painter-12.1-beta.md`: the feature set demonstrated here (Skew Painting/baking, Edge Protection, Auto Rebake) matches that file's documented beta scope. Note: the beta's own release-notes file flags its date as "~2026-04-07 (unverified — secondary source)"; this video doesn't provide a clean enough on-screen date to independently confirm that estimate, but the beta-branch identity itself is a firm, direct confirmation that this feature set really did ship as a Beta release ahead of 12.1.0 stable.

### Tags
`baking` `mesh-maps` `high-to-low-poly` `painter-12` `intermediate`

---

## Related Tutorials
- **"Skew Baking & Auto Rebake in Painter 12.1"** (`tutorials/skew-baking-auto-rebake-in-painter-121-adobe-substance-3d.md`, video `WwyElRpiQgY`) — same feature, same demo mesh (the low-poly radio), shipped-stable 12.1.0 companion video. This beta video adds performance-tuning details (Tangent Wrap→UV brush projection trick, sub-sampling cost) and beta-install logistics not covered in the stable-release video; the stable video covers the reorganized Mesh Map Bakers checklist and Common/Cage tabs in more general detail. Read together for the fullest picture of this feature.
