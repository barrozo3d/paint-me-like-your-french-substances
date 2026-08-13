---
title: 10 New Features in Substance Painter You Didn't Know About
source: YouTube
url: https://www.youtube.com/watch?v=yebv44cOYW4
author: FlippedNormals
ingested: 2026-08-13
app: "Substance 3D Painter"
version: "not stated numerically; strongest anchor is the baking dialog listing Height/Bent Normals/Opacity as bake outputs, which release-notes-painter-8.1.md confirms were added natively in 8.1.0 (2022-06-07) — creator frames these as recently added, so this video was likely recorded around/shortly after the 8.1.x line; the Warp Projection shown here is the older manual-vertex-editing version (predates the automatic Warp-to-Geometry feature added in 12.0.0), consistent with an 8.x-era recording. Not independently confirmed beyond this cross-reference."
tags: [layers, fill-layer, paint-layer, masks, alpha, udim, texture-set, uv, baking, mesh-maps, height, opacity, export, export-preset, viewport, blend-mode, intermediate]
extraction_status: complete
frames_dir: tutorials/frames/10-new-features-in-substance-painter-you-didnt-know-about/
frame_count: 11
frame_status: complete
frame_selection: content-anchored (manual timestamps chosen from transcript, not blind percentages)
---

# 10 New Features in Substance Painter You Didn't Know About

**Source:** [YouTube](https://www.youtube.com/watch?v=yebv44cOYW4)
**Author:** FlippedNormals
**Duration:** 13m14s | 11 section(s)

---

## Raw Data (for Claude Code extraction)

Frames captured — see "Captured Frames" section below.


### <Untitled Chapter 1> [0:00]
**Transcript (timestamped):**
[0:00] Hi, this is Henning for FlipNomals and in this video we are going to go through some of the best features added to Substance Painter over the last six months to a year or so.
[0:11] This software is an active development, there is tons of new good stuff added constantly and you might have missed some of these, so we are just going to go through some of our favorite new features.
[0:21] Before we get into that though, I want to talk to you about our latest course, Advanced Character Crash with Ben Erd.
[0:27] This is a fantastic course focusing on how to create this character start to finish.
[0:33] You learn advanced techniques like character sculpting, hard surface armor creation, texture painting and finally rendering the whole piece, making a really nice portfolio piece.
[0:42] So if you are interested in improving your character art, both organic and hard surface, I highly recommend this course, you are sure to learn a lot from a master like Ben.


### Locking environment to camera [0:50]
**Transcript (timestamped):**
[0:51] Back in Painter, the first feature I want to show you is that you can now link the environment to the camera instead of the world.
[0:57] Traditionally the way you are able to move the lights around is Shift Right Mask button just like this.
[1:01] The problem with this technique has been that everything that has been underneath or on top like this has been practically impossible to properly evaluate because it just isn't in light.
[1:12] They have changed this and you can now very easily link the environment to the camera.
[1:17] If you go up here to your display settings and then we just scroll down a tiny bit and here you can see the environment alignment and here you can just change this from world to camera.
[1:27] And now you can see if we rotate this around, this is always in light and you can also of course change the rotation of this.
[1:35] You can just move this around if you really want to have a specific view of this or if you want to use a different HDRI which has a different rotation.
[1:41] You can very easily do this.
[1:43] What you can see if we enable Shadows is that this actually rotates the light around and the shadows are responding to that.
[1:50] So it's really cool that you can have shadows like this which just makes the model look much better.
[1:54] We of course can turn this off for performance for reasons.
[1:57] So this is probably one of my favorite features because I'm going to be using this all the time in Painter.


### Warp Projection [2:00]
**Transcript (timestamped):**
[2:01] Next up we are going to be talking about a feature called Warp Projection.
[2:04] This is an incredible feature for warping images on top of your model.
[2:08] The way it works is first you just have to create a new fill layer.
[2:12] And then you drag the image you want to use.
[2:14] In this case we are going to give you a nice little tribal tattoo.
[2:16] And you just drag this under the slot you want, in this case the base color.
[2:21] Then just alt click on the color, nice little tip as well.
[2:24] Alt click, just clears all the other ones.
[2:26] So now we only have that.
[2:28] Then we scroll up a little bit and here you can see projection, UV protection.
[2:31] And we just change this to warp protection all the way on the bottom.
[2:35] And what this allows us to do is it allows us to move the whole thing forward like this.
[2:40] This is the same thing as a plane project.
[2:42] But it allows us to project this each point onto the model.
[2:45] So we can really warp this around.
[2:47] So if you want to give her a nice facial tattoo like this.
[2:50] The controller for this is just WENR.
[2:52] Just the same thing as a regular conventional 3D software.
[2:56] And the same thing for the settings you already have in Painter.
[2:59] So we just want to rotate this around like so.
[3:02] And then we want to give her a nice little face tattoo here on the side.
[3:04] So we can just scale this down a little bit like so.
[3:07] And then what we can do, we can go up here to the settings.
[3:10] Where you see we have some settings here that this is the third icon.
[3:14] If you hit edit, vertices, you can now go in and you can, with the move tool active,
[3:18] you can now just move this around.
[3:20] What's cool is that you can enable this little guy,
[3:23] which is going to snap it to the surface.
[3:25] So now if you just hover over this and drag, you can now just snap this to the surface.
[3:31] Which is fantastic.
[3:32] Because this just means you can really quickly warp something around like so.
[3:35] So once you can hover all the points, you're now going to have a texture,
[3:40] which has been warped properly.
[3:41] Though you can see that this goes through like so.
[3:43] So there are a few things you can do for this.
[3:45] You can change the projection depth, which is just going to move,
[3:48] you see the green lines, just going to change the depth of this.
[3:52] But sometimes this isn't possible because, just because of the geometry you're working with.
[3:57] So in that case, what you can do, you can add more resolution to the actual plane.
[4:01] You do that from the same area as you edit the vertices, which is just a third icon.
[4:06] And here you have three options.
[4:07] You have split crosswise, which is going to go horizontal and vertical.
[4:12] Horizontal, which is just going to be flat.
[4:14] And vertical, which is going to go down.
[4:15] So now you can see if we choose vertical.
[4:17] Now you can see that we have a line going through here.
[4:19] And then we can just go in and we can just click on these points.
[4:23] And then now we can add more points.
[4:25] Same thing with horizontal as well.
[4:27] Just click here and split horizontal.
[4:28] You can add another one.
[4:30] Split horizontal.
[4:31] You can add it down here.
[4:32] And now we can just go through and we can just really just make sure this fits nicely with the model.
[4:36] So a really, really handy feature for really kind of any kind of texture painting like this.
[4:42] Then of course we just go in and we just set this to multiply.
[4:45] And then we can very easily just see our result.
[4:48] And of course you can just warp this around like so.
[4:51] And once you're done, you just click on any other layer and the projection is going to disappear.
[4:57] This is actually exactly how we done it for the height map.
[5:00] You're seeing here all the pores.
[5:01] So if we just go to height, open this up and then we'll go to our warp projection.
[5:06] This is using the exact same technique I just showed you.
[5:08] Just that we're using a product here called a Flick-Momels face kit where we have a flat plane,
[5:12] which we were just wrapping on top of all this.
[5:15] And the cool thing about this is so we can still go into this and we can change it around.
[5:18] So we can go to the other vertices.
[5:19] We can just go in here and we can just go in and move this around.
[5:22] It's going to be a little slow due to the computer having a bunch of stuff to compute now.
[5:25] But it means that you can warp this around very effectively.
[5:28] So I highly recommend this for like logos, tattoos or anything like this.
[5:32] And the advantage of this is that this is procedural.
[5:34] So this means, for instance, if you have a map like this, like in this case, this is just a grayscale image.
[5:40] But if you have a color version of this, then you can just duplicate this and then you can just input the color image.
[5:46] Like if you're using XYZ textures and so on.
[5:48] So this is really, really useful if you're dealing with any kind of texture data that you have to wrap around your image.
[5:55] Or model X or warp it around.


### Working with UDIMS in Substance Painter [5:57]
**Transcript (timestamped):**
[5:57] The next new feature, which is fantastic is that Painter now supports UDEMS.
[6:01] If we hit F3 now, now we can go into our UV viewport.
[6:04] You can see that this character has UDEMS, which just means that each one of these images here, you can see 1001.
[6:10] This is just a single image, just called 1001.
[6:13] And this just means that we can have a lot more resolution than we can normally.
[6:17] This is pretty much my highest requested feature in Painter because this allows you to get significantly higher resolution.
[6:24] So this is what this looks like when you're unwrapping something in something like Blender.
[6:27] We can just see that this has just been unfolded based on the UDEM workflow as well, where each one of these is just one specific image.
[6:36] So the way you set this up is you just go to File, New.
[6:40] And then you've got to make sure, of course, that you have an FBX on OBJ that has been unfolded based on the UDEM workflow.
[6:47] Then you go to Select, you just select the file you want, hit Open.
[6:50] And then you don't have to do anything. You just simply just make sure this is ticked.
[6:54] By default, this is going to be ticked.
[6:57] So then we just hit OK. And then we don't have to save this. And then there we go.
[7:02] Now you can see that this new model now has successfully been imported based on the UDEM workflow.
[7:08] Super easy to use, very powerful.
[7:10] And if you were to export this out now, we just back in the last scene, Ctrl Shift and E.
[7:14] Then you can see that if we go to the actual template here, you can see that it has a dollar sign UDEM,
[7:21] which just means that the UDEM tag is going to be embedded into the file name.


### Export as SBSAR [7:25]
**Transcript (timestamped):**
[7:25] And speaking of exporting, you can now export out as a Substance Archive or SPSAR file,
[7:31] which is fantastic if you want to have these files be more plug-and-play and out of software that supports the Substance Archive folder.
[7:39] So what you can do, you can just go under the Global Settings,
[7:44] use Change the File tab from, in this case, PNG, then go all the way down and here you see SPSAR.
[7:50] And now you can just export this out and you are now going to get Substance Archive files that you can use in other software.
[7:57] They're adding a lot of new things like this, that it's more just workflow-friendly, pipeline-friendly.
[8:02] It's not a super big sexy feature, it's just insanely useful.
[8:06] So thank you developers of Painter for adding these features.


### Improved Eye Dropper [8:08]
**Transcript (timestamped):**
[8:08] Another feature I'm very excited about is the new Eyedropper tool or rather the improved Eyedropper tool.
[8:14] So Eyedropping has always been awkward in Painter until now, where hand painting was actually kind of a paradoxically weird thing in a software called Painter.
[8:23] Painting wasn't actually very good. So if you just have an hour paint layer and if you want to just paint by hand here,
[8:29] we can very easily do that now with a new Eyedropper tool.
[8:31] So first you do have to have this window open, so just go down to your base color and just click here, just open this up.
[8:39] And then you can just paint some kind of stuff here.
[8:41] And now if you want to just continue painting, we can now just either just click the Eyedropper tool here and you see you don't have to hold it down anymore, you just click it.
[8:49] Now we get this color, super useful. Or you can hit the I key.
[8:53] So just I for, well, I and then you just put it in here and then you can just paint like so.
[9:00] So this makes hand painting much, much easier.
[9:03] So fantastic job again to the painter devs who realized that this was a sorely missed feature.
[9:08] I've actually based my entire painting workflow around the fact that you can't really hand paint.
[9:13] So that's something I probably have to revise now with this being such a good addition to it.
[9:17] The next feature, which is absolutely brilliant is you can now add any item you find here on the asset browser to a favorites.


### Add Assets (like Brushes) to favorites [9:19]
**Transcript (timestamped):**
[9:23] So you can just right click on it, then you can hit add to favorites.
[9:26] You can see here on the top, it's going to have this night little star that's going to just move up here.
[9:31] So this is really useful.
[9:32] So if you find something that you keep using over and over again, you can just right click on them and put them all the way in top.
[9:37] And if you want to remove them, just right click and remove from favorites and that removes them.
[9:42] If you were to go to brushes now, you can see that I've already added around seven brushes, which is really useful because this means I can go in, I can just keep painting and I can keep going in and I can just keep changing this around.
[9:53] Without having to search for the brushes.
[9:56] That was one of the more frustrating things for me when actually doing hand painting, just because it was really tricky to.
[10:04] It was not tricky.
[10:05] It was just time consuming.
[10:06] You just had to keep looking for them all the time.
[10:08] So the fact you can add things now to favorites, really, really useful stuff.


### Apply Blending Mode to all layers [10:11]
**Transcript (timestamped):**
[10:13] The next feature is that you can now apply the current blending mode to all other channels.
[10:17] So let's say we change this blending mode to multiply.
[10:20] You can now right click on it and then you can apply to all other channels, which means that this layer, if we go over to go to the other channels, this is they're now going to have the same blending mode as the one we just changed.
[10:31] So if you want to change all of them at the same time, right click and then apply to all channels.
[10:36] This also works for opacity, which is really useful because we can now just change the pass here.
[10:40] And then you see now, if you go to roughness, for instance, this is not changed.
[10:45] But if you go to base color now, right click on the opacity, apply to all channels.
[10:52] You can now see that this has indeed changed in all the channels.
[10:55] Just one of those really useful workflow tips.


### Quickly re-import mesh [10:58]
**Transcript (timestamped):**
[10:58] Next up, you can now quickly reimport a mesh, which you can do by going to edit and then reimport mesh.
[11:04] This is going to just keep re importing the same mesh.
[11:07] So let's say you're texturing the model and somebody else is modeling it.
[11:10] So they might be working on an C brush or in Maya Blender, whatever it is.
[11:14] And they will just going to keep re exporting the same FBX and replacing the old one.
[11:19] You can now just control shift and R or go up here to reimport mesh.
[11:23] And now this is just going to be re imported really quickly.
[11:28] This makes iterating much faster instead of having to go in and having to go into project configuration and going in here and changing this up.
[11:35] Next up, there are three new bake types.
[11:37] If you go under texture set settings, mesh maps and bake mesh maps, you can see that we have three new mesh maps.


### New bake types [11:38]
**Transcript (timestamped):**
[11:43] One is height, then we have bent normals and then we have opacity.
[11:47] So if you want to bake any one of these, you just enable them right here.
[11:50] We are of course not going through what these actually are because there's a whole new topic, but at least you can bake height, bent normals and opacity.
[11:58] Another last feature we're going to be covering is going to be temporal anti-aliasing.


### Temporal Anti Aliasing (TAA) [11:59]
**Transcript (timestamped):**
[12:01] A really annoying feature in painter is that you see the viewport is really jagged around all the edges.
[12:06] It's just jagged and that's just a general issue.
[12:09] You see the same thing here in your eyes, but TAA or temporal anti-aliasing is going to fix that.
[12:14] If you go all the way up here to the display settings and then we scroll down just a little bit.
[12:19] And here we have activate temporal anti-aliasing.
[12:22] So click this, you can see that everything just gets smoother.
[12:25] This is, you may not even be able to see this in the video.
[12:28] I'm not sure if I can even zoom in to see it.
[12:30] I'm not sure if that's how it works, but at least you can see that this should make it quite a lot more appealing in the viewport.
[12:36] So I recommend just keeping this active and this shouldn't really impact performance.
[12:40] So it might take some time for this to activate on heavy scenes.
[12:44] So that's it for the most useful features added recently in Substance Painter.
[12:49] These features are really making a difference in my day-to-day workflow and I think they're going to improve your workflow quite a lot too.
[12:55] If you have any other features that were not covered in this video, please let us know in the comments below.
[13:00] But also be curious to hear what you think Adobe should be focusing on next in terms of features.
[13:04] So yeah, that's it for this video.
[13:06] If you enjoyed this video, make sure to leave a comment, like the video and hit the little notification bell to get a notification every single time we put out a new video.



---

## Captured Frames

- [1:17] tutorials/frames/10-new-features-in-substance-painter-you-didnt-know-about/frame_000.jpg
- [2:12] tutorials/frames/10-new-features-in-substance-painter-you-didnt-know-about/frame_001.jpg
- [3:18] tutorials/frames/10-new-features-in-substance-painter-you-didnt-know-about/frame_002.jpg
- [6:04] tutorials/frames/10-new-features-in-substance-painter-you-didnt-know-about/frame_003.jpg
- [7:44] tutorials/frames/10-new-features-in-substance-painter-you-didnt-know-about/frame_004.jpg
- [8:31] tutorials/frames/10-new-features-in-substance-painter-you-didnt-know-about/frame_005.jpg
- [9:23] tutorials/frames/10-new-features-in-substance-painter-you-didnt-know-about/frame_006.jpg
- [10:13] tutorials/frames/10-new-features-in-substance-painter-you-didnt-know-about/frame_007.jpg
- [11:04] tutorials/frames/10-new-features-in-substance-painter-you-didnt-know-about/frame_008.jpg
- [11:43] tutorials/frames/10-new-features-in-substance-painter-you-didnt-know-about/frame_009.jpg
- [12:14] tutorials/frames/10-new-features-in-substance-painter-you-didnt-know-about/frame_010.jpg

---

## Structured Notes

### Core Technique
A rapid-fire tour of ten discrete Painter feature/workflow additions, demonstrated on a horned character bust: camera-linked environment lighting, Warp Projection for wrapping flat images/alphas onto curved surfaces (used for both a facial tattoo decal and pore-detail height data), native UDIM/UV Tiles project support, SBSAR export, an overhauled click-to-pick Eyedropper, right-click favorites for any asset-browser item, one-click "apply blend mode/opacity to all channels," quick mesh reimport, three new native bake types (Height, Bent Normals, Opacity), and Temporal Anti-Aliasing (TAA) for the viewport.

### Summary
Good hub video for this creator's other Substance Painter tutorials — each feature gets a short, self-contained demo rather than deep technique-building, making it a fast reference for "how do I do X" workflow questions. **1. Camera-linked environment:** Display Settings > Environment Alignment switched from `World` (the old Shift+Right-drag lighting method, which left top/bottom surfaces permanently unlit from most angles) to `Camera`, so the HDRI lighting always follows the current view; rotation is still adjustable, and Shadows respond correctly to the now-camera-relative light. **2. Warp Projection:** on a new Fill layer with a dragged-in image (Alt-click a channel icon to isolate just that channel, e.g. Base Color), change Projection from `UV Projection` to `Warp Projection` at the bottom of the projection list — this behaves like a Plane Projection but lets each point of the projected plane be individually manipulated (`W`/`E`/`R` gizmo, same as any 3D software) and, critically, snapped directly onto the model surface via a per-vertex snap toggle in the projection's Edit Vertices mode; for surfaces too complex for the projection depth alone to handle, the plane itself can be subdivided (Split Crosswise / Split Horizontal / Split Vertical) to add more control points before snapping. Demonstrated twice: once for a Base-Color facial tattoo decal (blend mode `Multiply`), and once — using the exact same technique — for wrapping a purchased "face kit" pore/detail alpha directly into the Height channel; flagged as ideal for logos, tattoos, or any flat reference texture (including full-color XYZ scan textures) that needs to conform to curved geometry. **3. UDIM / UV Tiles support:** press `F3` for the UV viewport to see per-tile numbering (e.g. `1001`); a UDIM-unwrapped FBX/OBJ imports automatically with its UV-Tiles checkbox pre-enabled in File > New, with no extra setup required, and the `$udim` export-template token embeds the tile number into exported filenames — called out as the creator's most-requested feature for the extra resolution headroom it unlocks. **4. SBSAR export:** in the Export dialog's Global Settings, change File Type from a raster format (PNG etc.) to `SBSAR` (Substance Archive) for plug-and-play delivery into any Substance-Archive-compatible pipeline tool. **5. Improved Eyedropper:** open a channel's color swatch, then either click the eyedropper icon (no longer needs to be held down) or press `I` to sample a color directly from the canvas while painting — flagged as a long-overdue fix that specifically unblocks practical hand-painting workflows in Painter. **6. Favorites for any asset-browser item** (materials, brushes, alphas, etc.): right-click > Add to Favorites pins it to the top of its browser tab; right-click > Remove from Favorites reverses it — removes the repeated-search friction of hand-painting-heavy workflows. **7. Apply blend mode/opacity to all channels:** after setting a blend mode (or opacity) on one channel of a layer, right-click that channel's control and choose "Apply to all channels" to propagate the same setting across every other enabled channel on that layer in one action. **8. Quick mesh reimport:** Edit > Reimport Mesh (or `Ctrl+Shift+R`) re-imports the same source mesh file in place — useful when a modeler on the same project keeps re-exporting an updated FBX/OBJ under the same filename, letting the texture artist refresh geometry without re-running Project Configuration. **9. Three new bake types:** Texture Set Settings > Mesh Maps > Bake Mesh Maps now lists `Height`, `Bent Normals`, and `Opacity` as bakeable outputs alongside the established maps (not explained in depth in this video). **10. Temporal Anti-Aliasing:** Display Settings > "Activate Temporal Anti-Aliasing" smooths jagged viewport edges with negligible performance cost (may take a moment to converge on heavier scenes) — recommended to leave on by default.

### Key Steps
1. **Link environment lighting to the camera** (not the world) via Display Settings > Environment Alignment > `Camera`, so every surface stays lit as you orbit, instead of relying on manual Shift+Right-drag repositioning that leaves top/bottom areas permanently dark from most viewing angles.
2. **Use Warp Projection to wrap a flat image onto curved geometry:** new Fill layer, drag the source image into the desired channel slot (Alt-click that channel's icon to isolate it from other channels), change Projection to `Warp Projection`, position/rotate/scale it roughly with the standard `W`/`E`/`R` gizmo, then enter Edit Vertices mode (third icon in the projection's settings) and drag individual points with surface-snap enabled to conform the plane precisely to the model.
3. **Add resolution to the warp plane when the geometry is too complex for projection depth alone:** from the same Edit Vertices area, use Split Crosswise / Split Horizontal / Split Vertical to subdivide the plane and add more manipulable points before snapping each new point to the surface.
4. **Reuse the identical Warp Projection technique for non-color data** (demonstrated with a Height-channel pore/skin-detail alpha) — the same manual-plane-warp-and-snap workflow applies regardless of which channel the projected image targets, and grayscale sources can be swapped for full-color equivalents (e.g. XYZ scan textures) without changing the technique.
5. **Set up a UDIM/UV-Tiles project:** import an FBX/OBJ that was UV-unwrapped using the UDIM convention via File > New — the UV Tiles checkbox is enabled by default, requiring no manual configuration; verify tile numbering (e.g. `1001`) in the UV viewport (`F3`).
6. **Ensure exported filenames carry the UDIM tile number** by confirming the export template includes the `$udim` token (visible/editable under Ctrl+Shift+E's template settings).
7. **Export as SBSAR** for pipeline-friendly delivery by switching Export dialog > Global Settings > File Type to `SBSAR` instead of a raster image format.
8. **Sample colors while painting using the improved Eyedropper**: click the eyedropper icon (click, not hold) or press `I`, then click any point on the canvas to pick up that color for the active brush.
9. **Pin frequently-used assets (brushes, materials, alphas, etc.) to Favorites** via right-click > Add to Favorites in any asset-browser panel; remove the same way when no longer needed.
10. **Propagate a blend mode or opacity value across all channels of a layer in one action** via right-click > "Apply to all channels" on that channel's blend-mode or opacity control.
11. **Quickly refresh geometry mid-project** with Edit > Reimport Mesh (`Ctrl+Shift+R`) whenever a collaborator re-exports an updated mesh under the same source filename.
12. **Bake Height, Bent Normals, and/or Opacity as native mesh maps** by enabling them directly in Texture Set Settings > Mesh Maps > Bake Mesh Maps, alongside the standard Normal/AO/Curvature set.
13. **Enable Temporal Anti-Aliasing** in Display Settings for a smoother viewport with minimal performance cost — recommended as a default-on setting.

### Layers / Tools / Settings
- **Environment lighting:** Display Settings > Environment Alignment: `World` -> `Camera`
- **Warp Projection:** Fill layer > Projection: `UV Projection` -> `Warp Projection`; Edit Vertices mode (`W`/`E`/`R` gizmo, surface-snap toggle); plane subdivision via Split Crosswise/Horizontal/Vertical; Alt-click to isolate a single channel
- **UDIM/UV Tiles:** File > New (auto-detected from a UDIM-unwrapped mesh), `F3` UV viewport, `$udim` export-template token
- **Export:** Export dialog > Global Settings > File Type: `SBSAR`
- **Eyedropper:** click (not hold) the eyedropper icon, or press `I`
- **Favorites:** right-click any asset-browser item > Add to Favorites / Remove from Favorites
- **Channel blend-mode/opacity propagation:** right-click a channel's blend mode or opacity control > Apply to all channels
- **Mesh reimport:** Edit > Reimport Mesh / `Ctrl+Shift+R`
- **New bake types:** Texture Set Settings > Mesh Maps > Bake Mesh Maps: `Height`, `Bent Normals`, `Opacity`
- **Viewport smoothing:** Display Settings > Activate Temporal Anti-Aliasing (TAA)

### Difficulty
Intermediate — each feature is simple in isolation and clearly demoed, but several (Warp Projection's vertex-snap workflow, UDIM project setup, the blend-mode-propagation trick) assume the viewer already understands Painter's projection/channel model well enough to know when reaching for these shortcuts actually matters.

### App & Version
Not stated numerically on screen. The clearest anchor is the Baking dialog explicitly listing `Height`, `Bent Normals`, and `Opacity` as bakeable mesh maps (visible in a captured frame) — `references/release-notes-painter-8.1.md` confirms these three bakers were added natively in **Painter 8.1.0 (2022-06-07)**, and the creator frames them as a recent addition here, suggesting this video was recorded around/shortly after that release. The Warp Projection shown is the older **manual vertex-editing** version (drag + snap-to-surface + plane subdivision) rather than the automatic "Warp-to-Geometry" feature `references/version-tracker.md` dates to **12.0.0 (2026-03-09)** — i.e. this video predates that automation by a wide margin, consistent with an 8.x-era recording. Neither UDIM support's introduction date nor the improved Eyedropper's are independently confirmed in this skill's current reference files.

### Tags
layers, fill-layer, paint-layer, masks, alpha, udim, texture-set, uv, baking, mesh-maps, height, opacity, export, export-preset, viewport, blend-mode, intermediate

---

## Related Tutorials
- [Texturing a Clicker - FULL Substance 3D Painter Workflow](texturing-a-clicker---full-substance-3d-painter-workflow.md) — same creator (FlippedNormals); that video's baking step and texture-set/UDIM organization are a direct real-world application of features 3 (UDIM support) and 9 (new bake types) shown here.
- [Shading & Lighting a Character - Blender and Substance 3D Painter Workflow](shading-lighting-a-character---blender-and-substance-3d-painter-workflow.md) — same creator (FlippedNormals); the same project's UV Tiles/UDIM texture sets are visible there too, confirming this creator's consistent adoption of the UDIM workflow covered here.
- [Advanced Peeling Paint Effect in Substance 3D Painter](advanced-peeling-paint-effect-in-substance-3d-painter.md) — different creator (Javad Rajabzade); also works with a UDIM tile projection setup, a direct real-world use case for feature 3 (UDIM/UV Tiles support) covered here.
