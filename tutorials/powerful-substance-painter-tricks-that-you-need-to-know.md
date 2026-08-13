---
title: Powerful Substance Painter Tricks That You Need To Know
source: YouTube
url: https://www.youtube.com/watch?v=XXEgE2rJ09c
author: Dolinskyi
ingested: 2026-08-13
app: "Substance 3D Painter"
version: "not stated on screen"
tags: [layers, paint-layer, masks, generator, anchor-point, blend-mode, procedural, alpha, metal-rough, roughness, height, basecolor, texture-set, viewport, intermediate, advanced]
extraction_status: complete
frames_dir: tutorials/frames/powerful-substance-painter-tricks-that-you-need-to-know/
frame_count: 11
frame_status: complete
frame_selection: content-anchored (manual timestamps chosen from transcript, not blind percentages)
---

# Powerful Substance Painter Tricks That You Need To Know

**Source:** [YouTube](https://www.youtube.com/watch?v=XXEgE2rJ09c)
**Author:** Dolinskyi
**Duration:** 26m26s | 9 section(s)

---

## Raw Data (for Claude Code extraction)

Frames captured — see "Captured Frames" section below.


### Intro [0:00]
**Transcript (timestamped):**
[0:00] In this video I want to share some of the techniques I personally use while working in Substance Painter.
[0:05] I'll walk you through my viewport setup, show some useful hotkeys and demonstrate different methods for creating various effects,
[0:12] from simple surface details to more advanced material tricks.
[0:16] Whether you're just starting out or already experienced with Substance Painter,
[0:21] I hope you'll find something new and practical to improve your workflow.


### Viewport setting [0:27]
**Transcript (timestamped):**
[0:27] Let's start with the viewport settings.
[0:30] First, change the environment to a studio one, preferably without any colored lighting.
[0:36] The most popular choice is Tomaco Studio. Although it's not black and white, it doesn't affect the colors too much.
[0:43] Next, change the environment alignment from world to camera.
[0:47] In this mode, the environment map follows the camera position and lights up the areas you're currently looking at.
[0:54] Then, adjust the focal length. This is individual preference.
[0:58] I prefer when the lens doesn't distort the model too much, as it makes the proportions easier to read.
[1:04] You can set temporal anti-aliasing to maximum. It helps reduce the staircase effect along the models.
[1:12] Set anesthetropic filtering to 8 and Mipmap bias to 2. This affects the texture sharpness at a distance.
[1:20] Next, go to the shader settings and set them to very high.
[1:24] You can also choose Ultra, but the difference between very high and Ultra is minimal.
[1:30] And in a heavy scene, Ultra might slow down the viewport performance.
[1:36] If ambient occlusion bothers you, you can tone it down.
[1:43] If you want more accurate ambient occlusion rendering,
[1:47] enable bent normals.
[1:53] That's it for the viewport settings.


### Hotkeys [1:56]
**Transcript (timestamped):**
[1:56] Quick object selection across different texture sets.
[2:00] Hold Ctrl plus Alt and right click on an object.
[2:03] This automatically switches to the texture set that the object belongs to.
[2:08] Very convenient when you have many sets in the scene and can't always remember their names.
[2:13] Next, Alt plus left click on the eye icon of a texture set isolates that set from others without
[2:19] switching to it. Alt plus Q isolates the objects of the current texture set.
[2:32] Let's move on. Change the blending mode on all texture channels in just a couple of clicks.
[2:38] For example, when you need to apply sharpen to every channel.
[2:40] Simply change the blending mode on any channel.
[2:43] Right click, choose apply to all channels. Done.
[2:48] Next feature, isolating a single channel.
[2:52] Hold Alt and left click on the channel you want to keep visible.
[2:59] And finally, sometimes you import dozens of textures.
[3:03] Instead of changing their type one by one, select all textures with shift,
[3:08] set the desired type on one of them and it will be applied to all selected textures.


### Parkerizing damage [3:17]
**Transcript (timestamped):**
[3:20] Let's look at some texturing techniques.
[3:23] We'll create a damaged mask for metals with Parkerized or so-called gun metal materials.
[3:30] As we can see in the reference, this type of coating gets damaged in a way that visually
[3:35] creates a grainy effect. Let's try to recreate that effect.
[3:41] Create a layer with pure metal.
[3:52] Add a black mask and inside the mask, create a paint layer where we'll draw the damage.
[3:57] Add white noise and set its blending mode to subtract.
[4:13] Adjust the tiling to get the desired grain size using the reference as a guide.
[4:18] Above it, add a histogram scan and tweak the position value to around 0.9 to 0.95.
[4:32] You can rename the paint layer to something like plus.
[4:39] By making the brush tip semi-transparent, we can start painting the damage.
[5:18] Based on real photos of surface damage.
[5:48] Another method I often use when working with generators.


### Mask reveal [5:59]
**Transcript (timestamped):**
[6:06] Add a metal edge wear generator.
[6:10] On top of it, add a paint layer. Fill the entire model with black.
[6:20] Change the blending mode to multiply.
[6:27] Now, by painting with white, you reveal the generator only in the areas where you need it.
[6:40] Remember to add red just to remind everyone of where you'reab azt that metal is.
[6:50] We've got a lot of colors, we've got white, white, dark, light,我不 codeEng,
[6:54] Alright, another cool feature is working with decals.


### Decals [7:09]
**Transcript (timestamped):**
[7:15] Let's create a random decal in Photoshop.
[7:25] I'll be using a black and white alpha.
[7:28] It's easier this way to control color parameters and other channels.
[7:42] Give the decal to a folder.
[7:52] Now drag and drop the decal onto our model in the spot where we want to place it.
[8:05] It landed a bit crooked.
[8:08] The angle from which you project the decal also matters.
[8:42] Now switch to Edit Vertices mode.
[8:56] We'll slightly modify the grid to make it easier to align the decal with the surface.
[9:11] Then go back to Edit Vertices and press the Surface Tool button.
[9:16] Now we can snap the decal's vertices to the object's surface.
[9:21] It is allowing us to position it more organically.
[9:24] This looks especially good on complex shapes and organic surfaces, for example placing
[9:29] markings on cables and so on.
[9:31] There are endless ways to use it.
[9:53] Let's refine the look of our decal a bit.
[10:47] Another super useful feature is Auto Update Resources.
[11:17] In the bottom right corner of the Assets panel, click the button with the arrows.
[11:22] In the new window, check the boxes next to Asset Panel and resources used in project.
[11:28] Open your previous decal in Photoshop.
[11:31] Let's change the text to something else.
[11:47] Now, just save file and go back to Substance Painter and Magic.
[11:59] This is especially handy when you have dozens of decals all over the model and need to quickly
[12:03] change a font or when the logo design has been updated, you just save the PST file and
[12:09] you're done.
[12:39] A few simple techniques for working with plastic.


### Mold seam [13:03]
**Transcript (timestamped):**
[13:07] Let's create a mold seam on the AR-15 grip.
[13:11] Add a new layer and in its mask, add a gradient linear 2 or 3 with transition from white to
[13:18] black to both sides.
[13:26] Just because my grip isn't perfectly aligned to the axis, placing the gradient is a little
[13:30] bit tricky.
[13:37] Disable the Repeat option.
[13:47] Adjust it so it forms a thin line but not absolutely sharp.
[14:13] Turn off the Base Color Channel and enable the height.
[14:21] Place it along the center of the grip.
[14:29] On top of the fill layer, add a slope blur to create slight distortion.
[14:47] Then use a regular blur to soften the mask a bit and push it with levels to add contrast,
[14:53] make the line thinner.
[15:17] Done.
[15:18] If you want, you can refine it further with a brush so it doesn't look too uniform.


### Plastic damage [15:23]
**Transcript (timestamped):**
[15:25] Keep working with plastic.
[15:27] Let's make a damaged mask.
[15:29] Add a new layer with a black mask and a paint layer.
[15:35] In the channels, enable only height.
[15:38] In the paint layer, draw the damage using alphas.
[16:01] Make the mask more contrasty to remove unnecessary noise.
[16:17] Add Diffuse, slightly lighter than the base color.
[16:24] Add Glossiness, a bit more matte than the main glossiness.
[16:37] On top, add an anchor point.
[16:44] Give the layer to base and duplicate it.
[16:55] Completely clear the mask, add a fill layer and insert the anchor from the previous layer
[17:00] into it.
[17:03] On top of that, add a blur filter.
[17:09] Then add another fill layer above it, using the same anchor but set the blending mode
[17:14] to subtract.
[17:20] Decrease the height on the top layer and decrease it on the bottom one to create depth.
[17:39] The scratch looks noisy, so you can add blur to the base layer and also adjust it with
[17:45] levels on top so it reads better from a distance.
[18:16] You can continue painting your scratches by selecting the first one.
[18:24] Select the first base layer, go to paint and keep painting.
[18:44] I'm not creating perfect damage here, I'm just demonstrating the tool that can help
[18:49] you make it more interesting.
[18:51] This plastic is quite durable, so deep scratches like these are not very common.
[18:56] The final result should rely on your references and artistic sense.


### Weld seam [19:06]
**Transcript (timestamped):**
[19:10] The last part of the video will be a bit experimental.
[19:15] I want to add a rainbow effect on the metal around the welding seam.
[19:21] As you know, there are standard tools in Substance Painter that allow you to create a welding
[19:26] seam.
[19:27] Let's create a random curve.
[19:31] The idea is to add that rainbow effect that appears from metal heating around the seam.
[19:37] We already created the rainbow effect in the previous video, the link to it is in the description.
[20:00] So the first thing we need to do is extract the information from the mask of the created
[20:04] seam.
[20:17] Now blur this mask, expanding it around the seam.
[20:28] Since the rainbow effect doesn't appear directly on the seam, but only around its perimeter,
[20:34] we need to exclude the seam from the blurred mask.
[20:46] It's important to have a wide gradient range from white to black.
[20:50] This way we'll get the full color spectrum of heat tinting.
[21:16] The contour looks a bit too sharp in the center, so let's add some blur.
[21:38] Add an anchor point so we can use this mask later in the tempering colors smart material.
[21:55] Instead of the default mask that comes with the smart material, we'll use the one we just
[22:00] created.
[22:14] Right now we can see only yellow tones, that's because our mask isn't bright enough, so
[22:18] we need to increase its contrast.
[22:21] We can do that with levels and also subtract the seam itself from this effect.
[22:28] At maximum heating the metal gives a light bluish color, almost white.
[22:33] So I want to adjust the contrast to bring out that white shade.
[22:58] We also need to get rid of the sharp edges, since they don't look natural.
[23:20] Well this is already something closer to reality.
[23:30] We can also play with the blending mode.
[24:30] I don't quite like that the effect looks too uniform.
[24:42] In reality, when working with a welding torch it can't look perfectly even, a hand might
[24:47] shake or some areas might be overheated, some under heated.
[24:52] So let's add a procedural texture on top to break up that uniformity.
[24:57] I'm doing this for the first time so I might not pick the right texture right away.
[25:14] I think some kind of noise will work best here.
[25:18] Something like this more or less, I think.
[25:27] This is basically a ready to use tool for real objects, for weapons or anything that
[25:32] requires a welding seam.
[25:55] I'll experiment a bit more with roughness since it's still an oxide layer.
[26:14] That's it for now.
[26:15] Thanks for watching.
[26:17] If you have any cool substance techniques, effect creation tips or workflow optimization
[26:22] tricks, share them in the comments.
[26:25] Grow together.



---

## Captured Frames

- [0:40] tutorials/frames/powerful-substance-painter-tricks-that-you-need-to-know/frame_000.jpg
- [2:05] tutorials/frames/powerful-substance-painter-tricks-that-you-need-to-know/frame_001.jpg
- [4:20] tutorials/frames/powerful-substance-painter-tricks-that-you-need-to-know/frame_002.jpg
- [6:15] tutorials/frames/powerful-substance-painter-tricks-that-you-need-to-know/frame_003.jpg
- [8:10] tutorials/frames/powerful-substance-painter-tricks-that-you-need-to-know/frame_004.jpg
- [9:15] tutorials/frames/powerful-substance-painter-tricks-that-you-need-to-know/frame_005.jpg
- [11:20] tutorials/frames/powerful-substance-painter-tricks-that-you-need-to-know/frame_006.jpg
- [14:00] tutorials/frames/powerful-substance-painter-tricks-that-you-need-to-know/frame_007.jpg
- [16:45] tutorials/frames/powerful-substance-painter-tricks-that-you-need-to-know/frame_008.jpg
- [21:00] tutorials/frames/powerful-substance-painter-tricks-that-you-need-to-know/frame_009.jpg
- [23:30] tutorials/frames/powerful-substance-painter-tricks-that-you-need-to-know/frame_010.jpg

---

## Structured Notes

### Core Technique
A grab-bag of 8 personal workflow tricks (viewport setup, hotkeys, and 6 texturing techniques) for firearm-reference hard-surface work, culminating in a **weld-seam heat-tinting/rainbow oxide effect** that explicitly reuses the mask this same creator built for the already-ingested "Tempering Colors in Substance Painter" smart material via an Anchor Point.

### Summary
**Viewport settings**: Studio Camera environment (no colored lighting), Environment Alignment set to camera-following (not world) so lighting always favors the current view angle, personal-preference focal length to minimize distortion, Temporal Anti-Aliasing at maximum, Anisotropic Filtering 8 / Mipmap Bias 2 for distance sharpness, Shader Settings at Very High (Ultra gives minimal extra quality for a viewport-performance cost), Ambient Occlusion toned down or Bent Normals enabled for more accurate AO. **Hotkeys**: `Ctrl+Alt+Right-click` on any object jumps straight to its Texture Set (no need to hunt the list); `Alt+Left-click` a texture set's eye icon isolates it without switching selection; `Alt+Q` isolates the current texture set's objects; right-click any channel's blend mode → **Apply to all channels** (e.g. to push a Sharpen filter onto every channel at once); `Alt+Left-click` a channel icon to isolate just that channel; when importing many textures, select them all with Shift then set the resource type on just one to apply it to the whole selection. **Parkerizing/gun-metal damage**: a pure-metal Fill layer, black mask, nested Paint layer; add a White Noise texture set to **Subtract** blend mode with tiling matched to reference grain size, then a **Histogram Scan** filter above it with Position ≈0.9-0.95 to threshold it into a fine grain pattern; paint the damage by hand with a semi-transparent brush tip guided by real damage-photo references. **Mask reveal trick**: add a Metal Edge Wear generator, then a Paint layer above it filled entirely black and set to **Multiply** — painting white on that paint layer selectively reveals the generator only where painted, giving hand-guided control over an otherwise fully-automatic generator mask. **Decals**: build a black-and-white alpha decal in Photoshop (easier to control color/other channels downstream than a color decal), group it in a folder, drag onto the model, then fix a crooked/misaligned placement by switching to **Edit Vertices** mode to reshape the projection grid and using the **Surface Tool** to snap the decal's vertices to the actual mesh surface for organic-surface placement (e.g. markings on cables) beyond what a flat Warp/Planar projection alone achieves. **Auto Update Resources**: enable via the arrows-icon button in the bottom-right of the Assets panel, checking both "Asset Panel" and "resources used in project" — after that, re-saving a source PSD (e.g. changing decal text) in Photoshop automatically refreshes the resource back in Painter with no manual re-import, extremely useful for iterating decal text/logos across many placements. **Mold seam (plastic)**: a new Fill layer with a **Gradient Linear 2/3** mask (white-to-black-to-white, Repeat disabled) aligned along a grip's center axis, Base Color channel disabled and Height enabled, refined with a **Slope Blur** filter for irregular distortion, then a regular **Blur** plus **Levels** to thin/sharpen the line into a realistic seam, optionally hand-touched with a brush for asymmetry. **Plastic damage/scratches**: a black-masked Paint layer with only Height enabled, hand-painted scratch alphas, contrast-cleaned with Levels; add Diffuse (slightly lighter than base) and Glossiness (more matte) variants; capture the scratch mask as an **Anchor Point**, then build the scratch's actual depth from *two* Fill layers referencing that same Anchor Point — one blurred with reduced positive Height (the raised/worn lip) and one set to **Subtract** blend mode with reduced negative Height (the carved groove) — giving a scratch real dimensional depth rather than a single flat height dip; additional Blur+Levels tames noise so it reads correctly from a distance; new scratches are added by reselecting the original base paint layer and continuing to paint (the anchor-fed depth layers update automatically). **Weld seam rainbow/heat-tint effect (the video's most advanced trick)**: after creating a standard Painter weld seam, extract/copy that seam's own mask, **Blur** it outward to expand around the seam (not directly on it — subtract the seam itself from the blurred result, since the heat-discoloration halo surrounds a weld seam rather than sitting on top of it), keep a wide white-to-black gradient range for full color-spectrum heat tinting, blur the contour further to avoid an unnaturally sharp edge, then capture that processed mask as a new **Anchor Point** and swap it in as the mask source on the creator's own **Tempering Colors** smart material (see the companion "Tempering Colors in Substance Painter" video, also in this library) in place of its default mask. Boost contrast with Levels (and subtract the seam itself again) to properly bring out the near-white maximum-heat tone and the blue tones at peak temperature; soften remaining sharp edges; experiment with the smart material's blend mode; finally break up the effect's otherwise too-uniform look with a procedural noise texture layered on top (simulating uneven real-world welding-torch heat) and a touch of extra Roughness variation for the oxide layer.

### Key Steps
1. Viewport: Environment = Studio Camera (or similarly neutral studio HDRI), Environment Alignment = camera-following, personal focal length, TAA = maximum, Anisotropic Filtering = 8, Mipmap Bias = 2, Shader Settings = Very High, tone down AO or enable Bent Normals for accuracy.
2. Hotkey: `Ctrl+Alt+Right-click` an object to jump directly to its Texture Set.
3. Hotkey: `Alt+Left-click` a texture set's eye icon to isolate it without switching selection; `Alt+Q` isolates the current texture set's objects.
4. Hotkey: right-click any channel's blend mode → **Apply to all channels** to propagate a change (e.g. Sharpen) across every channel at once.
5. Hotkey: `Alt+Left-click` a channel icon to isolate just that channel in the properties view.
6. Hotkey: when importing many textures, Shift-select them all then set the resource type on one to apply it to the whole selection.
7. Parkerizing damage: pure-metal Fill layer → black mask → nested Paint layer; add a **White Noise** texture on **Subtract** blend mode (tiling matched to reference grain size) then a **Histogram Scan** filter (Position ≈0.9-0.95) above it to threshold into a fine grain; hand-paint damage with a semi-transparent brush guided by real reference photos.
8. Mask-reveal trick: **Metal Edge Wear** generator, then a black-filled Paint layer on **Multiply** above it — painting white selectively reveals the generator only where painted, adding hand control to an automatic generator mask.
9. Decals: build a black-and-white alpha in Photoshop (not color, for easier downstream channel control), group in a folder, drag onto the model; fix crooked placement via **Edit Vertices** (reshape the projection grid) + the **Surface Tool** (snap decal vertices to the actual mesh surface) for accurate placement on complex/organic geometry.
10. Enable **Auto Update Resources** (arrows-icon button, bottom-right of Assets panel; check "Asset Panel" and "resources used in project") so re-saving a source PSD in Photoshop live-updates the resource in Painter with no manual re-import.
11. Mold seam: Fill layer with **Gradient Linear 2/3** mask (white-black-white, Repeat off) aligned along the part's axis, Base Color off / Height on, **Slope Blur** for irregular distortion, regular **Blur + Levels** to thin/sharpen into a realistic seam line, optional hand touch-up.
12. Plastic scratch damage: black-masked Paint layer (Height only), hand-painted alphas, Levels contrast cleanup, plus Diffuse/Glossiness variant layers.
13. Capture the scratch mask as an **Anchor Point**; build real scratch depth from two separate Fill layers referencing that Anchor Point — one Blurred with reduced positive Height (raised lip), one on **Subtract** blend mode with reduced negative Height (carved groove) — rather than one flat height dip.
14. Add new scratches by reselecting the original base paint layer and continuing to paint — the anchor-referenced depth layers update automatically.
15. Weld-seam heat-tint: after building a standard Painter weld seam, extract/copy its mask, **Blur** it outward around the seam (subtracting the seam itself from the result, since heat discoloration halos the seam rather than covering it), keep a wide gradient range for full heat-color spectrum, blur the contour further for a natural edge.
16. Capture the processed halo mask as a new **Anchor Point** and use it as the mask source on the **Tempering Colors** smart material (from the companion video) in place of its default mask.
17. Refine with Levels (increase contrast, subtract the seam again) to bring out near-white peak-heat and blue maximum-temperature tones; soften remaining sharp edges; experiment with blend modes.
18. Break up the effect's uniformity with a procedural noise layer on top (simulating uneven real welding heat) plus extra Roughness variation for a believable oxide layer.

### Layers / Tools / Settings
- Viewport: Studio Camera environment, camera-aligned environment, TAA max, Anisotropic Filtering 8, Mipmap Bias 2, Shader Quality Very High, Bent Normals
- Hotkeys: `Ctrl+Alt+RMB` (jump to texture set), `Alt+LMB` on eye icon (isolate set), `Alt+Q` (isolate current set's objects), `Alt+LMB` on channel (isolate channel), right-click blend mode → Apply to all channels
- `White Noise` texture (Subtract), `Histogram Scan` filter (Position ~0.9-0.95)
- `Metal Edge Wear` generator + black Paint layer (Multiply) for hand-guided generator reveal
- Decal workflow: black-and-white Photoshop alpha, `Edit Vertices` mode, `Surface Tool` (vertex-to-mesh snapping)
- `Auto Update Resources` (Assets panel arrows-icon button)
- `Gradient Linear 2/3` mask (Repeat off), `Slope Blur`, `Blur`, `Levels`
- `Anchor Point` (scratch depth: two Fill layers, one Blur+reduced-positive-Height, one Subtract+reduced-negative-Height)
- Weld seam: seam-mask extraction, `Blur` (expand halo), `Anchor Point` (feeds into the `Tempering Colors` smart material's mask slot), `Levels`, procedural noise breakup, Roughness variation

### Difficulty
Intermediate to Advanced — assumes familiarity with generators, anchor points, and blend modes; the weld-seam rainbow effect explicitly builds on the creator's own separate Tempering Colors smart material.

### App & Version
Not stated on screen; UI consistent with this creator's other modern-era ingested Substance Painter videos.

### Tags
`layers` `paint-layer` `masks` `generator` `anchor-point` `blend-mode` `procedural` `alpha` `metal-rough` `roughness` `height` `basecolor` `texture-set` `viewport` `intermediate` `advanced`

---

## Related Tutorials
- [Tempering Colors in Substance Painter | Steel Heat Effects](tempering-colors-in-substance-painter-steel-heat-effects.md) — same creator (Dolinskyi); this video's weld-seam rainbow effect explicitly reuses that video's Tempering Colors smart material, swapping in a custom Anchor-Point-fed mask built from the weld seam's own blurred/expanded mask.
- [Realistic Painted Metal in Substance Painter | M24 Grenade Texturing](realistic-painted-metal-in-substance-painter-m24-grenade-texturing.md) — same creator; shares the compact 4-layer anchor-point peeling/damage-mask philosophy this video's two-Fill-layer scratch-depth trick (raised lip + carved groove from one shared anchor) builds on.
- [Realistic Wood in Substance Painter | M24 Grenade Texturing](realistic-wood-in-substance-painter-m24-grenade-texturing.md) — same creator, same M24 Grenade project series — cross-link once ingested.
