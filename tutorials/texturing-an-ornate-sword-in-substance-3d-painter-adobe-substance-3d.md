---
title: Texturing an ornate sword in Substance 3D Painter | Adobe Substance 3D
source: YouTube
url: https://www.youtube.com/watch?v=944ci1laePI
author: Adobe Substance 3D
ingested: 2026-08-13
app: "Substance 3D Designer (base material authoring) + Substance 3D Painter (texturing) + Substance 3D Stager (handoff)"
version: "not stated on screen; UI (Tri-Planar projection fill mode, Smart Materials with pre-built folders/masks, Send to Stager, Lazy Mouse) matches a modern Painter release, not precisely pinnable"
tags: [layers, fill-layer, paint-layer, masks, smart-material, generator, anchor-point, blend-mode, curvature, ambient-occlusion, mesh-maps, texture-set, pbr, metal-rough, basecolor, roughness, height, normal-map, alpha, procedural, tri-planar, export, intermediate, advanced]
extraction_status: complete
frames_dir: tutorials/frames/texturing-an-ornate-sword-in-substance-3d-painter-adobe-substance-3d/
frame_count: 8
frame_status: complete
frame_selection: content-anchored (manual timestamps chosen from transcript, not blind percentages)
---

# Texturing an ornate sword in Substance 3D Painter | Adobe Substance 3D

**Source:** [YouTube](https://www.youtube.com/watch?v=944ci1laePI)
**Author:** Adobe Substance 3D
**Duration:** 18m53s | 8 section(s)

---

## Raw Data (for Claude Code extraction)

Frames captured — see "Captured Frames" section below.


### Introduction [0:00]
**Transcript (timestamped):**
[0:00] Hello again! In this video, we will fully texture the lion's heads that we sculpted in Modeler and go from this to something like this.
[0:18] Now, before we begin, a few words about the process.
[0:21] You may have noticed that we only sculpted the main shapes in Modeler
[0:25] and that the model is still lacking a lot of features to look like the final result.
[0:30] We are missing, for example, all the crisp chiseling that makes this piece unique.
[0:35] And that's because I usually like to start from a simple sculpt and leverage all the tertiary shapes through texturing.
[0:42] Not only is it easier and more efficient, but it's also less destructive, as we will soon see.
[0:50] Alright, let's open Substance Painter.


### Project set up in Painter [0:52]
**Transcript (timestamped):**
[0:53] In the previous video, we prepared our model for texturing to make our life easier, so all we have to do now is to get on mesh,
[1:01] change the resolution to 2048, and most importantly, go into the Auto Unwrapped settings.
[1:08] Our model has already been unwrapped in Modeler, so we don't need to generate new seams or islands,
[1:13] but we do need to update the packing, since we applied texture sets in the meantime.
[1:19] You can decide for the amount of UV stars you want and hit OK.
[1:23] Painter will take some time to compute and automatically split your UV islands in texture sets.
[1:29] That kind of auto-packing is not perfect and you might want to do it manually if you're expecting something very optimized,
[1:35] but in our case, this will work just fine.
[1:38] Now, the second thing we want to do is bake our model to retrieve all the information from the geometry.
[1:44] We do that by going to the texture set settings here and clicking on Bake Mesh Maps.
[1:50] Let's do a very simple bake, set the output size to 2048 and keep only the maps we need.
[2:02] Once it's done, you can shortcut through the baked map by pressing B.


### Creating a Damascene base material in Designer [2:07]
**Transcript (timestamped):**
[2:07] We are now ready to start texturing. Let's take a look at our reference.
[2:11] The most prominent feature is the Damacine surface with its delicately punched gold.
[2:18] We could make this in Painter if you wanted, but it would take a lot of time and effort and it might not be worth it.
[2:25] And that's because that kind of material can be created on its own before being applied to a specific mesh.
[2:32] To make this point clearer, we need to make the distinction between material authoring and texturing.
[2:38] Material authoring refers to creating a tileable material from scratch that can then be applied to various meshes.
[2:47] Texturing, on the other hand, is more about applying ready-made materials to specific parts of a mesh using brushes or generators.
[2:57] Substance designer, ensembler and material authoring tools. You use them to create tileable base material.
[3:06] Painter is more of a texturing tool. Each option has its pros and cons.
[3:12] You can create tileable base materials in Painter if you want, but it gets tedious pretty quickly and you'll be more limited than in Designer.
[3:20] So, let's hop into Designer to quickly make our Damacine material.
[3:25] It isn't a Designer tutorial, I'm just going to quickly walk you over what I did and as you can see, it's not a complex material.
[3:32] If you want to know more about it, you can download it in the project files and take some time to study the graph.
[3:38] Alright, so I usually start by creating some kind of background for my material.
[3:43] In this case, I wanted to have a base with soft pumps that would look like metal with imperfections.
[3:50] I did that by blending a uniform gray with a soft clouds to a noise.
[3:55] This gave me what I wanted and so all I had to do next was to add these little punch marks all over the surface.
[4:03] To do that, I studied closely the reference and watched a few videos about the art of Damacining.
[4:10] Now, let me tell you, the craftsman who made that sword guard 600 years ago probably spent a lot of time carefully punching that thin layer of gold.
[4:19] He also followed the edge flow of the face as you can see here on the nose.
[4:23] Something I want both of us, but hey, that's impressive.
[4:29] Okay, so to do that, I first created that hollow mark left by the punch.
[4:34] I made three variations of it to make it more organic and varied and then I fed them into a tile sampler,
[4:41] randomizing slightly the position, scale and luminance.
[4:45] Then to create that raised lip around the marks, I filled with the curves a bit, then warped the whole thing,
[4:53] and simply subtracted it from the metal base.
[4:57] And that's it.
[4:59] The rest is just about deriving the color and roughness from that very simple height setup.
[5:05] Once the material is finished, all we have to do is go to the share option here and send it to painter.


### Texturing the face [5:12]
**Transcript (timestamped):**
[5:13] Alright, our material has safely landed in painter's library. We can now drag and drop it onto our model.
[5:20] Right off the bat, it's not too bad, but if we take a closer look, we can spot some UV issues.
[5:26] A quick way to check the seams is to add a layer with a solid color, then mask it and add a UV border generator in the mask.
[5:35] It will help you visualize how the cuts warp around your model, and in our case, this is clearly not great.
[5:42] Good news is, painter provides us with a quick way of fixing this.
[5:47] All we need to do is go to the fill properties and switch the projection mode to Tri-Planar.
[5:53] See the difference? Perfect.
[5:57] Now let's increase the tiling and bump up the resolution to 4K.
[6:05] Alright, much better.
[6:06] Now let the texturing work begin. The first thing we want to do is to break down that uniformity and add some damage to the gold layer.
[6:15] So let's add a fill layer on top of it and search for rust material in the library.
[6:23] To control whether rust should appear, we need to add a black mask to the layer and work in that mask.
[6:30] Now in our reference, we can see that rust collects under the swirly ornaments, so let's try to replicate that.
[6:38] And this is where baked maps come in handy. Let's add a generator to our mask and choose the ambient occlusion one.
[6:46] Alt-clicking the mask lets us preview it.
[6:49] Here you can see how useful it will be for the effects we are after, because it selects all the occluded areas.
[6:55] All we need to do is to invert the values and play a bit with the contrast and balance.
[7:04] Like so. Pressing M to go back to material mode and fine tune the effect.
[7:11] Now it's still too uniform of course, so we need to keep working on it.
[7:15] I'm going to first add a blur to soften the edges, then a warp to break down the outline.
[7:26] Lastly, we can add a grunge map to make it even more organic.
[7:31] But be careful, each time we make some kind of fill operation, Painter will use the UV projection by default.
[7:38] So here it's best if we switch to Tripliner once more.
[7:42] Then we have to pick an interesting blending mode and again, spend some time testing different settings.
[7:49] Now with that first layer of rest done, we need to keep pushing and add new layers to make the effect more subtle and convincing.
[7:57] This time no need to create it from scratch, we can simply duplicate the first layer and make changes to it.
[8:04] Here going for a darker ready shade, and then adjusting the mask.
[8:09] Slope blur to further break up the lines.
[8:17] Like that.
[8:23] Now you can see the benefit of having two passes of rest like that.
[8:27] It really solves that build up effect.
[8:29] I'm going to duplicate that last layer once more, but this time I want to add random speckles of rest across the whole surface.
[8:37] So I can just clear the mask to start afresh.
[8:43] And making the rest some kind of dark brown.
[8:48] Alright, you can see that I'm doing it in a very simple way.
[8:52] And making the rest some kind of dark brown like so.
[8:58] Alright, let's add a grunge map in our mask with a fill.
[9:02] Here I'm going for paint fill.
[9:09] Increasing the tiling, adjusting the contrast and balance.
[9:22] Okay, good enough.
[9:25] Now of course it's giving us too much speckles, so in order to remove some of these I'm going to add a paint layer to the mask in subtract mode.
[9:34] Then let's look for a nice brush, this one should do, and simply remove some of the excess rest.
[9:42] Although we could have used a procedural trick to do that, I find it nice sometimes to paint things by hand and have that manual control.
[9:52] Alright, now that the rest layers are done and neatly stacked in a group, we can move on to another important feature of the model, the eyes.


### Texturing the eyes [9:54]
**Transcript (timestamped):**
[10:03] Let's create a fill layer.
[10:05] And instead of using the material mode, we can simply set the values we want for each channel.
[10:16] Now we have a problem here, and that's the fact that the height from our golden material is showing through, which we obviously don't want.
[10:25] To fix that we need to go to the height channel and set the blending mode of the layer to normal.
[10:32] And now we have a smooth layer that completely overrides what's below it.
[10:39] Keep in mind though that if you place that layer in a group, you need to change the blending mode of the group as well.
[10:46] I created a group here because I know the eyes will take many layers and I want to be able to mask them all at once, at the group level.
[10:55] So let's add a black mask to the group and simply paint in the area of the eyes.
[11:02] Perfect.
[11:06] Now we can start working on that reddish background.
[11:10] Using the same method as with the rest, duplicating the base, changing it slightly and adding generators and grunge maps to mask it out.
[11:24] Crack deep looks perfect for that.
[11:27] The UV projection also works well on this one, creating those nice radial streaks around the iris.
[11:36] Switching back to material mode. Everything looks good.
[11:44] We might just soften the height here.
[11:48] Okay.
[11:50] And with a bit more work, this is what we get. Not bad.
[11:55] Now we need to add the iris.
[11:57] And for this feature, we can take advantage of Painters' Smart Materials library.
[12:02] This will make our life easier since those materials come with ready-made masks and groups.
[12:08] Let's try Iron-old. It should match our reference pretty well.
[12:13] Drag and drop it.
[12:15] And note that it comes in a folder already.
[12:18] So we need to drag it back in the eyes group so that it applies only to the area we defined earlier.
[12:25] And see here the power of Painters' Smart Masks?
[12:28] They automatically rely on the baked map so that you barely have any manual work to do.
[12:33] Now obviously this needs a second mask in pass, so let's add a black mask and paint the irises simply by stamping the basic heart brush.
[12:44] Like so.
[12:46] For the pupil, the reference is unclear, so let's just add a fill layer and make it a fully black material with no specularity at all.
[12:58] Mask it out.
[13:00] And then carefully paint the inside.
[13:08] Alright.
[13:09] It's looking okay so far, but it's still a bit flat in my opinion.
[13:13] I'd like to make the irises pop out a bit more.
[13:17] So to do that, we can add a layer that will act on the height only.
[13:22] Simply deactivate the other channels.
[13:25] And careful now, this is a bit more technical.
[13:28] I want this layer to reuse the shape of the irises that we already painted.
[13:34] To do so, all I have to do is to go back to that layer, go in the Mask stack and add an anchor point.
[13:44] I need to add it on top of the information I want to reuse.
[13:48] So in that case, I think the basic paint layer will be enough.
[13:51] I'd rather not have something too noisy to work with.
[13:56] Rename your anchor point to make it easier to work with later.
[13:59] And now back to our height adjustment layer.
[14:02] To call for an anchor point, simply create a fill and go in the Anchor Point tab.
[14:08] There you have it.
[14:09] Now, every change that I'll make to the irises paint layer will propagate to the upper layers that use the anchor point.
[14:17] This is such a powerful feature.
[14:19] If you want to know more about it, we have a video on that topic.
[14:23] So right now the effect isn't really showing, but if we simply add a bevel to our first fill to expand it,
[14:31] we can then call for the anchor point once more,
[14:34] but this time in Subtract mode to generate that nice rim.
[14:41] With levels and a bit of tweaking, we can get the desired effect.
[14:46] At some point, we need to switch back to Material mode just to check how it looks and keep adjusting.


### Texturing the ornaments [14:54]
**Transcript (timestamped):**
[14:54] We can call the face Done and move on to the ornaments that are on the separate texture set.
[14:59] Let's first fill the whole set with a solid gold material.
[15:05] Then tweak the color to make it match our Damacine material.
[15:12] Something like that.
[15:14] Let's also adjust the roughness.
[15:18] Nice.
[15:20] Now in the reference, the bands are also thinly carved,
[15:23] and this is something that we can do with the bevel.
[15:26] We start by adding a fill layer once more, and keeping only the height channel.
[15:32] And with a few effects applied and with Lazy Mouse mode enabled,
[15:36] all we have to do is carefully draw those lines, like so.
[15:40] So we can now add the fill layer once more,
[15:44] and we can then add a fill layer once more,
[15:47] and we can add a fill layer once more,
[15:49] and we can now add a fill layer once more,
[15:52] and we can now add a fill layer once more,
[15:55] like so.
[15:58] Then to add some grain and details to that first pass,
[16:01] we create yet another fill layer for the height,
[16:04] except this time we mask it with a Grange map,
[16:08] and blur it slightly to get a wrinkled look.
[16:13] Quick level adjustments,
[16:21] and then we can go back to the Grange map to fine-tune the effect.
[16:26] I think it looks better with straight planar projection.


### Finishing touches, tips and tricks [16:31]
**Transcript (timestamped):**
[16:32] The ornaments are done,
[16:33] I want to go back to the face itself to finish a few things up.
[16:36] I won't recreate everything live, but rather show you a few tricks that I used.
[16:42] The bridge of the nose, for example, should be somehow polished,
[16:45] because it's a protruding piece, right?
[16:47] And so by creating a layer with a lighter color and a smoother height,
[16:52] we can paint that effect pretty easily.
[16:56] Like that.
[17:00] To add wear, we can follow the same logic,
[17:03] using an interesting brush with a few effects on top of it.
[17:07] And to push the details even further,
[17:09] we can polish that underlying metal a bit,
[17:12] creating a smoother patch where it's supposed to be wrapped more often.
[17:16] Simply add a layer with a lower roughness and gently paint that patch in.
[17:22] Lastly, let's zoom in on one of the larger tears.
[17:26] Let me get rid of what I did to show it again.
[17:29] If I start painting here, you see a couple of things happening.
[17:33] First, the mask is revealing the good or rest material that we already used.
[17:38] But there's also a height layer above it that controls the raised lip that you see around the edges.
[17:44] I simply used an anchor point and played with the blending modes,
[17:48] just like we did with the Aris's rim.
[17:51] This is perfect to make that tear more realistic and believable.
[17:59] Finally, for most of the gilded painting that you see on this model,
[18:02] it's a mix between loading patterns in fill mode and hand painting a few details.
[18:08] Just like this.


### Sending the model to Stager [18:12]
**Transcript (timestamped):**
[18:12] Alright, our texturing work is now finished and looks decent.
[18:17] It's time to think about staging and rendering our work.
[18:21] But the good news is we don't have to do anything manually,
[18:24] like exporting maps, reloading them elsewhere and so on.
[18:28] All we have to do is go to File, Send to, Send to Stager.
[18:33] This will automatically open Stager and load both your mesh and your textures already applied.
[18:40] Awesome!
[18:41] I'll see you in the next video to show you the steps we can follow to put our model under the best light possible.



---

## Captured Frames

- [1:44] tutorials/frames/texturing-an-ornate-sword-in-substance-3d-painter-adobe-substance-3d/frame_000.jpg
- [5:20] tutorials/frames/texturing-an-ornate-sword-in-substance-3d-painter-adobe-substance-3d/frame_001.jpg
- [6:46] tutorials/frames/texturing-an-ornate-sword-in-substance-3d-painter-adobe-substance-3d/frame_002.jpg
- [9:34] tutorials/frames/texturing-an-ornate-sword-in-substance-3d-painter-adobe-substance-3d/frame_003.jpg
- [11:57] tutorials/frames/texturing-an-ornate-sword-in-substance-3d-painter-adobe-substance-3d/frame_004.jpg
- [13:44] tutorials/frames/texturing-an-ornate-sword-in-substance-3d-painter-adobe-substance-3d/frame_005.jpg
- [15:32] tutorials/frames/texturing-an-ornate-sword-in-substance-3d-painter-adobe-substance-3d/frame_006.jpg
- [18:28] tutorials/frames/texturing-an-ornate-sword-in-substance-3d-painter-adobe-substance-3d/frame_007.jpg

---

## Structured Notes

### Core Technique
Fully texturing a sculpted-but-detail-light lion's-head sword ornament by leveraging texturing (not sculpting) for all tertiary detail: a Designer-authored Damascene gold base material, baked-mesh-map-driven weathering (AO-masked rust), anchor-point-referenced eye/iris construction, and Lazy-Mouse-drawn bevel carving for the ornament bands — closing with a one-click Send to Stager handoff.

### Summary
Demonstrates Adobe's philosophy of leveraging a simple sculpt ("Modeler") plus texture-driven tertiary detail rather than sculpting every chisel mark, explicitly framing the Designer/Painter split: Designer (or Sampler) for *material authoring* (tileable materials built from scratch), Painter for *texturing* (applying ready-made materials to specific mesh areas via brushes/generators). Project setup: Auto Unwrap re-pack (existing UVs from Modeler, just re-packing texture sets), 2048 bake at Texture Set Settings → Bake Mesh Maps. Quickly walks through authoring a Damascene (hand-punched gold inlay) material in Designer — cloudy noise metal base blended with a Tile Sampler of 3 varied hollow "punch mark" shapes (randomized position/scale/luminance), a curved/warped raised lip subtracted from the base — then Share → Send to Painter. In Painter: drags the material onto the face, diagnoses UV seam problems with a diagnostic solid-color-plus-UV-Border-generator mask trick, fixes it by switching the fill's Projection mode to **Tri-Planar** (then upping tiling and bumping resolution to 4K). Builds rust weathering in a layered, non-destructive way: base rust fill layer masked by an Ambient Occlusion generator (inverted, contrast/balance-tuned) so rust naturally collects in occluded crevices under the ornament swirls, refined with Blur + Warp + Grunge (also switched to Tri-Planar projection) and a considered blend mode; duplicates this layer for a second, darker rust pass with a Slope Blur mask tweak to avoid a uniform "buildup" look; duplicates again for a third pass of random speckled rust across the whole surface (cleared mask, grunge+Paint fill, then hand-erased in places with a Paint layer in Subtract mode over a chosen brush — deliberately manual for control, though a fully procedural approach was possible). Builds the eyes in a dedicated Group (masked once at the group level, with the group's Height blend mode also set to Normal to fully override the gold material's height showing through) — reddish background (rust-style layered masking again, this time benefiting from default UV projection which produces natural radial iris streaks), then Painter's **Smart Materials** library (an "Iron-old" material, dragged in complete with its own folder/masks, moved into the eyes group so it's constrained) for the iris base — demonstrating how Smart Materials auto-leverage baked maps for near-zero manual setup — followed by a hand-stamped heart-shaped brush mask limiting it to just the iris, plus a fully black no-specularity pupil fill hand-painted in. Iris pop-out relief is built via an **Anchor Point** technique: adds an anchor point on top of the iris paint layer, references that anchor from a new Height-only fill layer (instant reuse of the same shape with zero redraw risk — any edit to the base iris paint propagates upward automatically), then bevels the first fill and calls the same anchor again in **Subtract** mode plus a Levels adjustment to carve a raised rim around the iris — the same anchor-point+blend-mode-subtract trick is reused later on a large tear/crack detail on the face. Ornament bands (a separate texture set) get a flat gold base color-matched to the Damascene material, then hand-carved grooves via a Height-only fill layer drawn with **Lazy Mouse** enabled for smooth freehand lines, plus a secondary Grunge-masked, Blur-softened Height layer (switched to planar projection) for a wrinkled-grain finish. Finishing pass on the face: a lighter-color/smoother-height layer hand-painted onto the protruding nose bridge to fake polish-by-handling wear, a similarly-built lower-roughness "polished patch" layer for a frequently-touched area, and reuse of the same anchor-point-plus-blend-mode technique on a large facial crack for a believable raised lip. Notes most of the gilded surface decoration is a mix of loaded fill patterns plus hand-painted touch-ups. Closes with **File → Send to → Send to Stager**, which auto-transfers the mesh and all applied textures with zero manual export/reload step.

### Key Steps
1. Project setup: with the model already UV-unwrapped in Modeler, use **Auto Unwrap** just to re-pack texture sets (choose UV tile count, hit OK) rather than regenerating seams/islands from scratch.
2. Bake mesh maps via **Texture Set Settings → Bake Mesh Maps**: simple bake, 2048 output, only the needed maps selected; press **B** afterward to cycle/preview baked maps.
3. In Substance 3D Designer, author a tileable Damascene (hand-punched gold) material: a soft-clouds-noise metal background, three varied hollow "punch mark" shapes fed into a **Tile Sampler** (randomized position/scale/luminance), a curved-and-warped raised lip subtracted from the metal base, with color/roughness derived from that height setup; finish with **Share → Send to Painter**.
4. In Painter, drag the finished Damascene material from the Assets panel onto the face mesh.
5. Diagnose UV seam problems: add a solid-color fill layer, mask it, and add a **UV Border** generator to the mask to visualize exactly where seams cross the surface.
6. Fix visible seam distortion by switching the fill layer's **Projection** mode from UV to **Tri-Planar**; follow up by increasing tiling and raising resolution to 4K for a crisper result.
7. Build rust pass 1: new fill layer, search the Smart Materials/materials library for a rust material, add a black mask; mask it with an **Ambient Occlusion** generator (Alt-click the mask to preview), invert the AO values, then tune contrast/balance so rust concentrates in occluded crevices under ornament details; press **M** to return to material view and fine-tune. Layer further softened with **Blur**, broken up with **Warp**, and finished with a **Grunge map** (remember to re-switch projection to Tri-Planar on every new fill operation, since Painter defaults new fills back to UV projection) plus a deliberately chosen blend mode.
8. Rust pass 2: duplicate pass 1's layer, shift to a darker rust shade, adjust the mask with a **Slope Blur** to further break up the repeating pattern and avoid an obvious "buildup" look.
9. Rust pass 3: duplicate again, clear the mask entirely, set a dark-brown rust color, mask with a **Grunge map** via a Paint fill (increase tiling, adjust contrast/balance), then hand-remove excess speckling with a **Paint layer in Subtract mode** using a chosen brush — a deliberate manual step for artistic control even though a fully procedural approach was possible.
10. Group all rust layers together for organization.
11. Eyes: create a dedicated **Group** for every eye-related layer (so the whole set can be masked once at the group level); add a black mask to the group and paint in just the eye area.
12. Base eye fill layer: set channel values directly (not material mode); because the gold material's Height still shows through, go to the **Height channel** and set that layer's blend mode to **Normal** so it fully overrides what's below — note the containing **group's** blend mode must also be set to Normal for the override to actually take effect.
13. Reddish eye background: same layered rust-style approach (duplicate, adjust, generator+grunge masking) but left on default UV projection this time, since it happens to produce a pleasing radial-streak look around the iris.
14. Iris base: drag in a **Smart Material** (e.g. "Iron-old") from the library — it arrives in its own folder with ready-made masks; drag that folder into the Eyes group so it only affects the eye area; Smart Materials auto-leverage baked maps for near-zero manual mask setup. Add a second black mask on top and stamp a basic heart-shaped brush to constrain it to just the iris.
15. Pupil: new fill layer, fully black material with zero specularity, masked out and hand-painted carefully inside the iris.
16. Iris pop-out relief (anchor-point technique): go to the iris paint layer's mask stack and add an **Anchor Point** directly on top of the paint information to reuse (name it for clarity); create a new Height-only fill layer, disable all other channels, and in its **Anchor Point** tab reference the named anchor — any future edit to the base iris paint automatically propagates to this height layer. Add a **Bevel** to the first fill to expand it, then call the same anchor a second time in **Subtract** mode plus a **Levels** adjustment to carve a raised rim around the iris.
17. Ornaments (separate texture set): fill the whole set with a flat gold material color-matched and roughness-matched to the Damascene face material.
18. Carve the ornament bands: new Height-only fill layer, enable **Lazy Mouse** for smooth freehand strokes, and hand-draw the carved band lines directly.
19. Add grain/detail to the carved bands: another Height-only fill layer masked by a **Grunge map**, slightly blurred for a wrinkled look, fine-tuned with **Levels**; notes it read better switched to straight **Planar** projection rather than the default.
20. Face finishing touches (each demoed as a quick technique rather than fully rebuilt on camera): a lighter-color, smoother-height layer hand-painted onto the nose bridge to simulate handling-polish; a similarly-built lower-roughness "polished patch" layer for a frequently-touched protruding area; reuse of the anchor-point-plus-Subtract-blend-mode rim technique (same as the iris) on a large facial crack/tear to build a believable raised lip around the damage.
21. Most remaining gilded surface pattern work is a mix of loading pre-made fill patterns plus targeted hand-painting.
22. Handoff: **File → Send to → Send to Stager** — automatically opens Stager with the mesh and all applied textures already loaded, no manual export/reimport step required.

### Layers / Tools / Settings
- **Substance 3D Designer**: Tile Sampler (randomized position/scale/luminance for punch marks), Curve/Warp nodes, Subtract blend for the Damascene raised-lip effect; Share → Send to Painter.
- **Bake Mesh Maps** (Texture Set Settings), 2048 output; press B to preview baked maps.
- **Fill layer Projection mode**: UV (default, reset on every new fill) vs. **Tri-Planar** (fixes seam distortion on organic sculpted surfaces) vs. **Planar** (used for the ornament grain pass).
- **Generators**: UV Border (seam diagnostic), Ambient Occlusion (rust placement, inverted + contrast/balance tuned).
- **Filters**: Blur, Warp, Slope Blur, Bevel, Levels.
- **Grunge maps** (via Paint fill) for organic rust/grain breakup.
- **Paint layer in Subtract mode**: manual removal of excess procedural detail (rust speckles).
- **Groups**: used to mask multiple related layers (all eye layers) at once; group-level blend mode must match child-layer blend mode overrides (Height → Normal) for the override to propagate correctly.
- **Smart Materials library**: "Iron-old" material for the iris base, dragged in as a ready-made folder with pre-built masks that auto-leverage baked maps.
- **Anchor Point**: added to a base paint layer's mask stack, referenced by later Height-only fill layers (Normal mode for base relief, Subtract mode + Levels for a carved rim) — reused for both the iris pop-out and a facial crack/tear detail.
- **Lazy Mouse**: enabled for smooth freehand height-channel line carving on the ornament bands.
- **File → Send to → Send to Stager**: one-click mesh+texture handoff, no manual export step.

### Difficulty
Advanced (Designer material authoring, Tri-Planar seam fixing, multi-pass generator-and-hand-blended weathering, anchor-point relief carving).

### App & Version
Substance 3D Designer (base material authoring) → Substance 3D Painter (texturing) → Substance 3D Stager (final handoff, not detailed in this video — covered in the "next video" referenced at the end). No Painter version number stated on screen; the feature set (Tri-Planar fill projection, Smart Materials with pre-built folders, Lazy Mouse, Send to Stager) is consistent with a modern Painter release but not precisely pinnable to a single point version.

### Tags
`layers`, `fill-layer`, `paint-layer`, `masks`, `smart-material`, `generator`, `anchor-point`, `blend-mode`, `curvature`, `ambient-occlusion`, `mesh-maps`, `texture-set`, `pbr`, `metal-rough`, `basecolor`, `roughness`, `height`, `normal-map`, `alpha`, `procedural`, `tri-planar`, `export`, `intermediate`, `advanced`

---

## Related Tutorials
- **Substance 3D Stager - Rendering assets from Substance 3D Painter** (`tutorials/substance-3d-stager---rendering-assets-from-substance-3d-painter.md`, if ingested) — the natural follow-on video referenced at the end of this tutorial ("I'll see you in the next video... best light possible"), covering the Stager side of this exact Send-to-Stager handoff.
- **How to TEXTURE like a PRO with ANCHOR POINTS | Substance Painter Tutorial** (`tutorials/how-to-texture-like-a-pro-with-anchor-points-substance-painter-tutorial.md`) — Jared Chavez's dedicated anchor-point deep-dive; this video's iris-relief and facial-crack techniques both directly apply the anchor-point-plus-blend-mode-subtract pattern taught there.
