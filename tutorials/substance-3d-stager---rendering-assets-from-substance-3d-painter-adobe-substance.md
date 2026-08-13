---
title: Substance 3D Stager - Rendering assets from Substance 3D Painter | Adobe Substance 3D
source: YouTube
url: https://www.youtube.com/watch?v=raGhfzhzVdU
author: Adobe Substance 3D
ingested: 2026-08-13
app: "Substance 3D Painter (export handoff only) + Substance 3D Stager (primary focus of this video)"
version: "not stated on screen"
tags: [export, viewport, intermediate]
extraction_status: complete
frames_dir: tutorials/frames/substance-3d-stager---rendering-assets-from-substance-3d-painter-adobe-substance/
frame_count: 5
frame_status: complete
frame_selection: content-anchored (manual timestamps chosen from transcript, not blind percentages)
---

# Substance 3D Stager - Rendering assets from Substance 3D Painter | Adobe Substance 3D

**Source:** [YouTube](https://www.youtube.com/watch?v=raGhfzhzVdU)
**Author:** Adobe Substance 3D
**Duration:** 17m24s | 10 section(s)

---

## Raw Data (for Claude Code extraction)

Frames captured — see "Captured Frames" section below.


### Intro [0:00]
**Transcript (timestamped):**
[0:00] In this video, I'm going to walk you through the process of taking an object that was textured
[0:12] in Substance Painter and rendering that in Substance Stager.
[0:15] So you can see that I have this robot character.
[0:17] The model was created in medium by my coworker Giovanni Neckpill.
[0:21] And so now all the textures are completed and I'm ready to go into the rendering process.
[0:26] So all I need to do is come up here to file and choose Send to Substance 3D Stager.
[0:32] So we're now going through an exporting process.


### Exporting [0:35]
**Transcript (timestamped):**
[0:36] Here you can see that Substance Stager is now loading in the model that was exported.
[0:40] All of the textures that were exported from Substance Painter are going to be hooked up
[0:44] into Stager materials and everything's going to be applied and ready to go for me to start
[0:49] staging and rendering the scene.


### Environment [0:53]
**Transcript (timestamped):**
[0:53] Okay, so just like that, you can see that we have a robot here in my 3D view.
[0:58] And like I said, all of the materials are applied.
[1:01] Okay, so let's start creating a little environment for this robot character.
[1:04] So I'm going to import in a 3D model that I'm going to use for a ground plane.
[1:08] I have a terrain that was modeled by another coworker named Vladimir Petkovich.
[1:12] Vlad modeled this terrain in ZBrush and I was able to export in the OBJ.
[1:16] Just simply drag and drop it right here into the Stager viewport to import the model.
[1:20] Here in the scene view, you can see that I have the object.
[1:23] Now it was called Group 1.
[1:24] Let's just make sure we just name this something that's a little bit more recognizable, so
[1:27] I'll call it Ground.
[1:29] Now you'll also notice here that some of my ground is being cut off and that's because
[1:33] if I come over to the Environment tab and I take a look at the ground properties, this
[1:37] ground plane is enabled.
[1:38] That's typically used as like a shadow catcher.
[1:41] I'm not really going to be using that here in this case, so I'm just going to disable
[1:44] it.
[1:45] Now I see the entire model.
[1:46] Okay, so with this in place, let's go ahead and go back here to the art robot.
[1:50] And let's position this art robot here in the scene or more specifically on the ground
[1:55] plane.
[1:56] So I can use the Move tool to position.
[1:58] However, I can also just simply click and drag here on the pivot point and you can see
[2:02] this pivot point will actually snap the robot along the surface normal here of the ground
[2:07] plane geometry, which is really cool.
[2:09] Nice way to position objects.
[2:11] All right, so I think I'm going to go with something maybe like this.
[2:14] I can always tweak this after the fact, but here, I think we'll do something like this.
[2:19] And what I'm looking at is possibly doing a shot where I frame up my object where we
[2:24] have some nice terrain here in the foreground and in the background and right here in the
[2:28] mid ground is where I'm actually going to do the main focus here for my character.
[2:32] All right, the next thing I'd like to do is start to get some texturing here on this
[2:37] ground plane.
[2:38] And so I'm just going to use a substance material for that.
[2:41] So here you can see that I'm browsing the substance 3D assets website and I found a nice substance
[2:47] material that's going to work perfect for this ground terrain.
[2:49] And I can download this SPS AR material.
[2:52] So now that I've already done that, I can simply take that substance material and then
[2:56] just drag and drop it here onto the ground plane.
[2:58] So here you can see that I'm dragging in the substance material and I'll just drop it right
[3:02] here on the ground plane.
[3:03] And that is going to apply this material to the terrain mesh.
[3:07] Now here under the ground object in the material tab, you can see that I have all of the parameters
[3:13] that are accessible through the substance material to make changes.
[3:16] In my case here, I definitely want to change this resolution.
[3:18] So I'm going to upgrade this here to 2048.
[3:22] And then I'm also going to go through and just repeat this material on the surface.
[3:26] So for the repeat value, I think I'll set this to say something like a six by six on
[3:29] the X and Y repeat.
[3:30] All right.
[3:31] So I think this is going to work for me for now.
[3:34] Next thing I'll do is start to take a look at maybe setting up my camera as well as the
[3:37] all important lighting here for my scene.
[3:41] So at the top of the toolbar, I'm going to click this create camera button, which is
[3:44] going to create a new camera.
[3:45] Instead of fault, it's set to 1920 by 10 a.
[3:48] I can always change this output size, but this is going to be the resolution actually
[3:51] going to work with the camera framing that I want to use is something more in line of
[3:55] what you see here.
[3:56] Of course, I could change my focal length if I want, but I think what I have at this 50
[4:00] millimeters is going to work well enough.
[4:02] Okay.
[4:03] So now let's start to take a look at the overall lighting.
[4:06] So what I can do to begin with is just come over to the top of the toolbar and enable
[4:10] my ray tracing.
[4:11] So already we're starting to get some nice shadowing here from enabling my ray tracing.
[4:15] If I look at the options, you'll notice that I'm rendering here with my GPU.
[4:21] So now I just need to adjust the environment lighting.
[4:24] If I come over here to the scene hierarchy and choose environment underneath the lights
[4:28] category, here you can see I can adjust the global lighting, which is a high dynamic range
[4:33] image.
[4:34] I can adjust things like intensity and rotation by holding down shift and using my right mouse
[4:38] button left to right, I can interactively adjust the rotation here of this light very
[4:43] similar to how I would work in substance painter.
[4:46] I definitely do not want to use this studio interior.
[4:49] So I'm going to come over here to the starter assets and I'm going to select the light option
[4:53] and then scroll down here towards the bottom and you can see a range of HDR images that
[4:58] we ship in substance stager.
[5:00] You can also import your own if you like.
[5:02] But in my case here, I think I'm going to go with this Corsica beach.
[5:05] I'll just left click and you can see here it's applied this new environment light.
[5:10] Now I'll hold down shift right mouse button left to right again to adjust this new light
[5:14] angle for that HDR.
[5:16] So we'll try something like this for now.
[5:18] Okay, so one of the issues that I'm having here with my ground plane is, well, I don't
[5:22] have any displacement.
[5:24] This looks very flat and boring.
[5:26] So let's take care of that now.
[5:27] I'm going to select the ground itself, the ground mesh and underneath the object, you'll
[5:32] notice here that we have this displacement setting.
[5:34] So now I'm going to enable the displacement option and stages now going to go through
[5:39] the process of test relating the geometry based on the tessellation mode.
[5:44] So in my case here, it's set to per triangle fixed by default, but I might actually set
[5:49] this to just an overall total face budget and I'll leave it at 10,000 for now.
[5:54] It's really nice that you can set the specific face budget number that you want.
[5:59] Okay, we're not really seeing too much happen here.
[6:01] And that's because I need to adjust my material settings.
[6:04] So again, I'm have my ground selected.
[6:06] I'm going to jump over to my material tab and then scroll down to where I have the height
[6:10] information.
[6:11] So we'll expand the height value and I have this height scale.
[6:14] I can really punch this.
[6:16] So what I'm going to do here is set this to a value of six.
[6:20] Okay, so now we're starting to see some nice displacement here.


### Displacement [6:21]
**Transcript (timestamped):**
[6:25] Again, holding down the shift key and my right mouse button, as I start to adjust my lighting,
[6:30] we can see how we're starting to get some just different results here.
[6:33] And that's actually looking pretty cool.
[6:35] Now, of course, at any time, I can always jump back over here to the object and increase
[6:39] this face budget so that I can get a much higher quality result on the overall displacement
[6:44] here from my scene.
[6:45] But for now, this is going to be fine because I'm still just kind of working up what I want
[6:48] this scene to basically look like.
[6:50] All right, so something else I could do is maybe take a look at maybe doing a little
[6:54] bit of a sky replacement here.
[6:56] So the background plate for the camera is just this gray background.
[7:00] If I select the camera, I can come over here to, let's say, the background and add an image
[7:04] here.
[7:05] Well, I have a sky image that I'd like to use.
[7:07] So let me just come over here to my second monitor and just grab it.
[7:10] I'll just drag and drop it right here to this background input.
[7:13] So I'll grab the image.
[7:14] It's a PNG file and just place it right here on the background.


### Accent Lights [7:17]
**Transcript (timestamped):**
[7:18] So now I have this sky in place.
[7:20] Okay, so something else I'd like to do, it's a little dark here.
[7:24] So maybe I would like to add a little bit of an accent light.
[7:27] So here I'm just click my dropdown and go back to my viewport camera.
[7:30] So you'll notice here that I'm able to look at my view, that displacement on the terrain
[7:35] is looking pretty cool.
[7:36] And we're also able to work with that interactively here in our ray tracer.
[7:39] So what I'm going to do is now underneath the starter assets, I'm still under the lights
[7:43] category.
[7:44] Let's scroll up here towards the top and take a look at these physical lights.
[7:48] So I have some physical lights that I can drag into the scene, maybe a spotlight or directional
[7:53] light.
[7:54] I think I'll try to maybe use this area light.
[7:56] And so what I'm going to do is just left click and drag the area light.
[7:59] And you can see that I can actually have the light point directly to a specific face normal
[8:04] here on my robot.
[8:05] So if I'm looking to maybe add a little bit of a highlight here to the side of the robot,
[8:09] I'm just going to align the light here to this side of the robot's face.
[8:13] That area light is now pointing directly at that face normal.
[8:16] Okay, with that in place, I'll now move the light out slightly and just make some adjustments.
[8:22] So I'll go through and rotate this guy.
[8:24] Maybe what I could do is come over here to say something like the exposure and I'll just
[8:28] increase this a bit.
[8:30] Now I'll tell you what, let's take a look at what this is doing through our camera view.
[8:34] So we'll jump over to our camera view.
[8:36] And like I said, I can also maneuver or manipulate this light and get something more in line
[8:41] of what I want to do.
[8:42] I was really just looking at getting a nice little rim lighting going on here.
[8:46] So like I said, that's what I'm truly trying to focus on.
[8:49] So let's get something like this.
[8:50] I'm just going to play with this slightly here to get this in place.


### Color [8:54]
**Transcript (timestamped):**
[8:54] If the exposure value, if I set that too high, I can always kind of feather that back by
[8:59] just decreasing the overall intensity.
[9:00] So you can see what that's doing here.
[9:02] Something else that might be kind of interesting is just to play around with the color value.
[9:06] So if we come over here to the color and we take a look at our temperature, we can use
[9:11] a warm kind of tinted value or maybe something a little bit more cool.
[9:15] Actually I think I'm going to just move this over here to this kind of warm value and we'll
[9:19] go with something like maybe like this.
[9:21] Okay.
[9:22] So with that in place, what I can do is also hold down the shift right mouse button left
[9:26] to right again to kind of continue to play around with the lighting here for that environment
[9:30] background.
[9:31] So I'm just rotating that HDR in the background, which is also changing some of that directional
[9:35] light from that scene as well.
[9:37] We can also jump over to the environment itself underneath lights and I can increase or decrease
[9:42] the intensity here as well.
[9:45] Okay.
[9:46] So now that we have this in place, I'm kind of liking this little bit of contrast.
[9:49] We're going to have some shadowing here.
[9:50] I have this area light providing some light and then again, a little bit more shadows.
[9:55] So we get this nice little contrast kind of helping to maybe focus a little bit on my
[9:59] robot character.
[10:01] I can also jump over to my camera and enable depth of field and I can set a focus point.
[10:06] So if we focus right on the robot, we can adjust our blur amount.
[10:10] This lets us have some nice kind of depth of field again to help focus our eye to our
[10:14] robot character.
[10:15] Well, one problem with this though is you'll notice that because that background plate
[10:19] that we have added to our cameras, just a 2D image, that depth of field is not really
[10:23] able to appropriately affect that background plate.
[10:26] All right.
[10:27] So for now, what I'm going to do is just disable this depth of field and I'm going to go ahead
[10:30] and just save my scene.
[10:32] So now I'd like to go ahead and render my scene.
[10:34] Before I do that, I'm going to jump over here to my ground and increase my face budget here
[10:39] for the actual tessellation.
[10:41] So now I'm just going through and just trying some different values.
[10:44] I ended up using 7 million, which is a lot, but Stature can handle this pretty well.
[10:49] Okay.


### Rendering [10:50]
**Transcript (timestamped):**
[10:50] So now that I've increased that polygon budget here for the tessellation, I'm going to jump
[10:55] over here to my render tab.
[10:57] I'm going to save my scene and I'm going to crank out a render.
[11:00] So you'll notice here from the export settings, I have the camera.
[11:04] This is the shot camera that I want to work with.
[11:06] You can have multiple cameras and you can cue them up here.
[11:09] In my case, I'm just going to be rendering with this one camera.
[11:11] So it's set to 1920 to 80.
[11:13] And I'm going to export as a PSD file.
[11:17] And I'm specifically using this PSD file format because Stature is going to export with some
[11:21] additional layer passes such as depth, material and object selection, which I can use to create
[11:28] various post effects inside an image editing application.
[11:32] So I'm going to set this to PSD.
[11:33] You can see that we have a 16 bit or a 32 bit per channel option.
[11:37] I'm going to leave this at 16 bit and then simply click the render button here to perform
[11:41] a render.


### Post Effects [11:42]
**Transcript (timestamped):**
[11:43] So now that the render is complete, I can come over here to the render status and click
[11:46] this button here to show in folder or edit in Photoshop.
[11:50] So now I'm going to run through the process of editing my render to add some various post
[11:54] effects.
[11:55] I'll run through this process pretty quickly and you can use any image editing application
[11:59] that you prefer.
[12:00] In my case here, I'm just going to use Photoshop.
[12:03] So I'll click the edit in Photoshop button and you can see this is going to open Photoshop.


### Photoshop Post Effects [12:07]
**Transcript (timestamped):**
[12:08] Stature is going to create a few additional layers.
[12:10] As I had mentioned previously that we can use in this post effects process.
[12:14] So for example, if I come over here to the additional layers, you can see that we have
[12:18] a layer for material selection masks.
[12:21] We have another layer for object selection.
[12:23] And then finally we have a depth pass.
[12:26] Here you can see that we have our rendered image, which has been denoised.
[12:30] Stature does a denoising pass which removes all the noise from the render.
[12:34] This is what the original render looks like, quite noisy.
[12:37] However, this pass, which is denoised, is going to give us a nice clean result.
[12:42] So with this layer visible, you'll notice that we have our background transparency back,
[12:45] which is great because I can do a sky replacement here.
[12:48] So I'm just going to grab the sky that I used in Stature and just drag and drop it here to
[12:52] the canvas.
[12:53] And then I'm just going to drag that here below the rendered image.
[12:57] So now I have my sky back.
[12:59] This is going to let me do a little bit of transformation.
[13:01] So I'll use the transformation tool and then I'm going to perform a non uniform scale to
[13:06] basically better represent the curvature of the sky.
[13:09] So I think I want to go with something more like this.
[13:11] All right.
[13:12] So now that I have that in place, I'm going to go ahead and just merge visible these two
[13:16] layers.
[13:18] Now in this layer, I'm going to come up here to filter and I'm just going to use my camera
[13:21] raw to add a few effects.
[13:23] Now typically I would convert this to a smart object so that I could add multiple effects,
[13:28] keeps things non destructive.
[13:29] But here in just in this case for this demonstration, I'm just going to just add the filter directly
[13:33] and just kind of bake this in.
[13:35] So if I go to the basic tab, I can play with things like the exposure.
[13:39] So I'm just going to bring the exposure up slightly, play around with things like the
[13:43] contrast here for clarity.
[13:46] I'm going to increase this value.
[13:48] And then if I come over here to my effects, I can add in some vignetting here.
[13:53] So we'll add a little bit of vignetting and then click OK.


### Depth Pass [13:57]
**Transcript (timestamped):**
[13:58] So that gives us a slight bit of grading here to the image already a little bit better with
[14:01] the contrast.
[14:03] Now I can start to use this depth pass.
[14:05] So I'm going to come over here to the additional layers and take a look at this.
[14:08] I have a problem here where the background is black.
[14:11] I have some missing data.
[14:12] This is just that camera background that I use for the sky.
[14:15] So it had transparency.
[14:16] There was an actual like full 3D scene that I could use here for that depth.
[14:21] So no problem.
[14:22] I can just fix this.
[14:23] What I'm going to do is I'm just going to create a new layer and I'll just fill this
[14:27] with white.
[14:29] Let's just drag this below the depth.
[14:31] Let's come over here to the depth layer and I'm going to grab just the one tool here and
[14:34] just quickly select the black and delete it.
[14:37] And there we go.
[14:38] So now we have basically the full range and then I'll merge these two layers down and
[14:42] we'll call this depth.
[14:44] All right.
[14:45] So this is going to be our depth pass.
[14:46] I'm going to use this a couple ways.
[14:48] Number one, let's add some fog.
[14:49] So what we're going to do here is come over here to the layer stack and I'm going to add
[14:53] a new layer and we'll just call this fog.
[14:57] And I'm going to just sample maybe a value range here from the cloud in the background.
[15:01] So let's just say something like that works and then we'll just fill that layer.
[15:05] So now I'm going to add a layer mask to that layer and I'm going to fill this layer mask
[15:09] with my depth information.
[15:11] So we'll come up here to the depth control a to select the layer and copy it.
[15:16] Then I'll come over here to the layer mask alt left click to enter into the layer mask
[15:20] and then paste in the depth information.
[15:23] Now when I jump back to my layer, I can see that I now have this fog pass working for
[15:27] me.
[15:28] So easily now I can come over here to the layer mask itself and just run like a levels to
[15:33] adjust the actual fog.
[15:40] Okay.
[15:46] I think something like that's going to work pretty well and we'll click okay.
[15:49] And you can see that that really adds a lot to the image.
[15:52] So if we turn off the fog, this is what we had before and now we have some nice atmospheric
[15:55] perspective.
[15:57] So next I'd like to add some depth of field.
[15:59] So I could take this rendered image and I'm just going to duplicate this layer for now.
[16:04] And what I'm going to do is just create a layer mask on this and then I also want to
[16:08] use that depth information.
[16:10] So I'll select the depth layer control a to cop to select it all control C to copy it.
[16:15] Let's jump back here into the layer mask and paste it in.
[16:18] Okay.
[16:19] So we'll come back to the layer.
[16:21] Now what I'm going to do is just right click on this layer mask and just disable the layer
[16:24] mask.
[16:25] The reason I'm using this layer mask is because I'm going to come over here to filter and choose
[16:29] blur and use lens blur.
[16:31] Now the lens blur is going to look here at the layer mask as the source.
[16:36] Now what I can do is come over here to set my focal point and I'll select the robot.
[16:41] And now as I adjust the radius, you can see here that I can add my depth of field as a
[16:45] post effect, which is driven by the depth layer that I rendered out of Stager.
[16:50] Now we'll just click okay to apply this depth of field effect.
[16:54] Now I'm feeling like the fog is just a little bit too intense.
[16:57] That's no problem.
[16:58] I can just select the layer and just simply feather this back here by dropping the opacity.
[17:02] So I'm just going to give it a slight hint of some atmospheric perspective.
[17:08] As you can see, it's pretty quick to send assets from painter to Stager and build a
[17:12] simple scene for rendering.
[17:14] I hope you've enjoyed this quick look at Stager.
[17:16] Thanks a lot for watching and I'll see you next time.
[17:20] Bye.



---

## Captured Frames

- [0:26] tutorials/frames/substance-3d-stager---rendering-assets-from-substance-3d-painter-adobe-substance/frame_000.jpg
- [0:40] tutorials/frames/substance-3d-stager---rendering-assets-from-substance-3d-painter-adobe-substance/frame_001.jpg
- [6:14] tutorials/frames/substance-3d-stager---rendering-assets-from-substance-3d-painter-adobe-substance/frame_002.jpg
- [11:13] tutorials/frames/substance-3d-stager---rendering-assets-from-substance-3d-painter-adobe-substance/frame_003.jpg
- [12:18] tutorials/frames/substance-3d-stager---rendering-assets-from-substance-3d-painter-adobe-substance/frame_004.jpg

---

## Structured Notes

### Core Technique
The entire Painter-side contribution to this video is a single action — **File → Send to → Send to Substance 3D Stager** on a fully-textured model — after which Stager auto-imports the mesh with every exported map already wired into matching Stager materials, no manual texture export/reimport required. Everything past that point (environment building, lighting, rendering, Photoshop post-effects) is Stager/DCC-side and outside this skill's core Painter scope; documented here only at survey depth per this skill's own scope boundary, since the video itself is Stager-primary.

### Summary
Demonstrates the Painter-to-Stager pipeline on a finished robot character (modeled in Medium, textured in Painter). The only Painter-side step is the export: **File → Send to Substance 3D Stager**, which pushes the mesh and every painted map straight into a new Stager scene with materials already hooked up and ready to light/render — this is the one technique from this video that's directly this skill's concern, and it matches the same "Send to Stager" handoff used in other Adobe Painter tutorials in this knowledge base (e.g. the ornate-sword and Hero-Assets-for-Fashion videos). The remainder of the video (documented briefly, Stager being out of this skill's scope) covers: importing a separate ground/terrain OBJ and positioning the robot on it (drag-to-snap along the surface normal), applying a downloaded Substance material to the terrain (resolution 2048, 6x6 UV repeat), camera creation (50mm, custom output resolution), enabling ray-traced (GPU) preview, swapping the default HDRI environment for a bundled "Corsica Beach" HDRI and rotating it interactively (Shift + right-mouse-drag, same gesture as Painter's own HDRI rotation), enabling mesh displacement on the terrain (tessellation face-budget mode, Height Scale pushed to 6, later increased to a 7-million-face budget before final render), adding a 2D sky-image background plate on the camera, adding a physical Area Light that can snap-align to a specific face normal for rim lighting (adjusting exposure, intensity, and color temperature), toggling Depth of Field (disabled here because the flat 2D background plate doesn't support it), and finally rendering via the Render tab as a 16-bit **PSD** (chosen specifically because Stager bakes in extra Photoshop layers: material-selection mask, object-selection mask, and a depth pass) at the shot camera's resolution. The video closes with a Photoshop post-pass using those extra layers: compositing a proper sky in place of the flat background, Camera Raw grading (exposure, contrast/clarity, vignette), rebuilding a broken depth pass (filling missing background depth data with white before merging), using the depth pass as a layer-mask source to add distance fog (color-sampled from the sky, masked by copy-pasted depth data, refined with Levels) and post-render Depth of Field (Lens Blur filter driven by the same depth-derived layer mask, focal point set on the robot).

### Key Steps
1. **(Painter)** With texturing complete, go to **File → Send to → Send to Substance 3D Stager** — this is the entire Painter-side action covered in this video.
2. **(Stager)** Stager opens and auto-imports the mesh with every exported Painter texture already wired into matching Stager materials — no manual export/reimport step.
3. Import a separate ground/environment mesh (drag-and-drop an OBJ into the viewport); rename it clearly in the Scene panel; disable the built-in "ground plane" shadow-catcher property if a real terrain mesh is being used instead.
4. Position the character by dragging its pivot point directly on the ground mesh — it snaps along the target surface's normal.
5. Apply a downloaded Substance material to the terrain via drag-and-drop; adjust its exposed parameters (Resolution, UV repeat tiling) in the object's Material tab.
6. Create a camera (toolbar Create Camera button); set output resolution and focal length (50mm used here) to taste.
7. Enable ray tracing (GPU-accelerated in this demo) for a real-time-shaded preview.
8. Adjust environment/HDRI lighting: pick a bundled Starter Assets HDRI (or import a custom one), rotate it interactively with **Shift + right-mouse-drag** (same gesture Painter itself uses for HDRI rotation), and control global intensity from the Environment entry under the Lights category in the Scene hierarchy.
9. Enable mesh Displacement on the terrain object; choose a tessellation mode (per-triangle-fixed vs. total face budget — face-budget mode used here, starting at 10,000 and later raised to ~7,000,000 for final render); in the object's Material tab, raise the Height channel's Height Scale (pushed to 6 in the demo) to make the displacement visible.
10. Add a 2D background plate to the camera (drag an image, e.g. a sky PNG, onto the camera's Background input) — note this flat plate won't correctly interact with Depth of Field later.
11. Add physical lights from Starter Assets (spotlight, directional, area light, etc.); an Area Light can be dragged directly onto a mesh face to auto-align to that face's normal — useful for quick rim/accent lighting; adjust Exposure, Intensity, and Color (temperature slider) to taste.
12. Optionally enable camera Depth of Field with a focus point on the subject — disable it if a flat 2D background plate is in use, since DoF can't correctly affect non-3D background imagery.
13. Before final render, increase the terrain's tessellation face budget for higher-quality displacement detail.
14. Render via the **Render** tab: select the target camera, set resolution, choose **PSD** as the export format specifically to get Stager's extra baked-in Photoshop layers (material-selection mask, object-selection mask, depth pass), choose bit depth (16-bit used here), click Render.
15. **(Photoshop, optional post-pass)** Open the rendered PSD; use the denoised main render layer; composite a real sky in place of the flat background plate (drag in the same sky image used in Stager, transform/scale to taste, merge down); apply Camera Raw adjustments (exposure, contrast/clarity, vignette) directly or via a Smart Object for non-destructive editing; repair the depth pass if the background reads as solid black (fill a new white layer beneath it, then select-and-delete the black area with the Magic Wand-style select tool, merge down); use the repaired depth layer as a **layer mask source** (copy the depth layer, paste into a new fog layer's mask) to drive a color-sampled atmospheric fog effect, refined with Levels on the mask; duplicate the render layer, paste the same depth data into its mask (then disable the mask so it's used only as the **Lens Blur** filter's depth-map source), apply Filter → Blur → Lens Blur with the focal point set on the subject to add physically-plausible post-render Depth of Field; fine-tune fog/DoF strength via layer opacity.

### Layers / Tools / Settings
- **Painter:** File → Send to → Send to Substance 3D Stager (the sole Painter-side step).
- **Stager:** Scene hierarchy/Environment (Lights category — HDRI selection, intensity, Shift+right-drag rotation); Object → Displacement (tessellation mode: per-triangle-fixed vs. total face budget); Material tab → Height → Height Scale; Camera (focal length, output resolution, Background image input, Depth of Field/focus point); Starter Assets → Lights (physical Area/Spot/Directional lights, face-normal snap-alignment, Exposure/Intensity/Color temperature); Render tab (camera selection, resolution, format = PSD with 16/32-bit option, additional baked layers: material selection mask, object selection mask, depth pass; built-in denoising).
- **Photoshop (post, optional):** Camera Raw filter (exposure/contrast/clarity/vignette); layer masks driven by copy-pasted depth-pass data; Lens Blur filter (depth-map-driven post DoF); Levels for fog-mask tuning.

### Difficulty
Intermediate (Stager scene-building and Photoshop compositing knowledge; the Painter-side step itself is trivial — a single menu command).

### App & Version
Substance 3D Painter (export handoff only) and Substance 3D Stager (primary subject of this video); no version number stated on screen for either app. Photoshop used for the optional post-effects pass, version not stated.

### Tags
`export`, `viewport`, `intermediate`

---

## Related Tutorials
- **Texturing an ornate sword in Substance 3D Painter** (`tutorials/texturing-an-ornate-sword-in-substance-3d-painter-adobe-substance-3d.md`) — uses the same File → Send to → Send to Stager handoff at the end of its Painter workflow, and explicitly references "the next video" (this one) for the Stager-side follow-through.
- **Hero Assets for Fashion - 06 - Asset Texturing and Presentation** (`tutorials/hero-assets-for-fashion---06---asset-texturing-and-presentation-adobe-substance-.md`) — also demonstrates the Painter-to-Stager Send-to handoff, followed by its own (more detailed, fashion-specific) Stager lighting/rendering pass.
