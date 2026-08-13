---
title: Preparing a 3D Asset in Substance 3D Painter | 3D in After Effects Part 1 | Adobe Substance 3D
source: YouTube
url: https://www.youtube.com/watch?v=aZ8bzxuZ-pM
author: Adobe Substance 3D
ingested: 2026-08-13
app: "Substance 3D Painter"
version: "not clearly legible on screen in captured frames; no version number stated in narration"
tags: [layers, fill-layer, paint-layer, masks, blend-mode, texture-set, pbr, metal-rough, basecolor, roughness, metallic, height, normal-map, opacity, viewport, alpha, beginner]
extraction_status: complete
frames_dir: tutorials/frames/preparing-a-3d-asset-in-substance-3d-painter-3d-in-after-effects-part-1-adobe-su/
frame_count: 10
frame_status: complete
frame_selection: content-anchored (manual timestamps chosen from transcript, not blind percentages)
---

# Preparing a 3D Asset in Substance 3D Painter | 3D in After Effects Part 1 | Adobe Substance 3D

**Source:** [YouTube](https://www.youtube.com/watch?v=aZ8bzxuZ-pM)
**Author:** Adobe Substance 3D
**Duration:** 15m30s | 12 section(s)

---

## Raw Data (for Claude Code extraction)

Frames captured — see "Captured Frames" section below.


### Getting Started [0:00]
**Transcript (timestamped):**
[0:00] In this video, we take a look at using Substance Painter to texture a 3D asset for use in After Effects.
[0:06] To get started, you can download 3D models and materials from Substance 3D assets using the Creative Cloud Desktop app.
[0:13] Here you can see I'm browsing for a 3D watch and can download as an FBX file for texturing in Substance Painter.
[0:20] I'm going to create a new project. I go to File, New, and here I have my template.
[0:26] I'm going to use the default ASM PBR metallic roughness, and then I need to select the file that I want to use.
[0:32] This is going to be my FBX or OBJ 3D model.
[0:38] Now I will set my document resolution, and I'll leave all the other settings at default.
[0:44] If your 3D model doesn't have UVs, Substance Painter can take care of that for you here in the import settings.
[0:51] So now I'll click OK, and my Substance Painter project is created.


### UI Overview [0:55]
**Transcript (timestamped):**
[0:55] For the UI, we have our assets. This is libraries that contain materials, brushes, and filters and different textures you can use in the texturing process.
[1:05] Here in the middle we have our 3D and our 2D view.
[1:09] Over here on the far right we have our Texture Set List, which is a list of the materials associated with the model.
[1:15] Then we have our Layer Stack, which is where we do all of the texturing work.
[1:19] Finally we have our Properties panel, which is context sensitive to change based on if we're using a brush or maybe adjusting filter settings.
[1:27] So for navigating the 3D view, first thing I'm going to come over to this top bar and I'm going to set this to 3D only.


### Navigating the 3D View [1:33]
**Transcript (timestamped):**
[1:33] For the navigation, I can hold down the Alt or Option key and then left click and drag to orbit around the viewport.
[1:43] Now using the Alt or Option key, I can use my right mouse button to zoom in and out and Alt or Option once more with the middle mouse click to pan the 3D view.
[1:53] And this is how I can navigate my 3D view.
[1:56] Let's talk about layers. Here in the Layer Stack, there are two types of layers I can create.


### Paint Layers [2:01]
**Transcript (timestamped):**
[2:01] The first is this paintable layer, and I can create that by just clicking this Add Layer button.
[2:05] This is going to allow me to paint on the 3D model.
[2:08] So quickly I'll come over to my Assets, let's grab a brush. I'll just grab any brush.
[2:13] And then if I jump over to my Properties, you can see I have all of my brush settings available to me.
[2:19] I now need to come over to my Material Settings and I need to set my Material Values.
[2:24] So now I'm just going to quickly create a material. I'll choose this red color.
[2:28] Let's make the roughness kind of low, which is going to make this more shiny and reflective.
[2:32] I will increase the Metallic value to 1 to make this a metallic material.
[2:37] Now if I come over to my 3D model, I can start to paint directly on the 3D model, as you can see here, with this full material.
[2:46] It's important to understand that you can't paint across materials. Each material has its own dedicated Layer Stack.
[2:54] Here you can see that I can't paint on the glass when the body material is selected.
[2:59] I will select the glass material to activate its dedicated Layer Stack, and now I can paint on it.


### Fill Layers [3:05]
**Transcript (timestamped):**
[3:05] The other type of layer I can create is called a Fill Layer. Let's go back and select the body material, and I will delete that paint layer.
[3:13] I will click the paint bucket icon to create a fill layer. This type of layer is not paintable.
[3:18] I can then go to the Properties panel for the material and set material values, such as setting my roughness closer to 0 to create a reflective surface and metallic to 1.
[3:27] These values fill the model with the material.


### Lighting [3:30]
**Transcript (timestamped):**
[3:30] Let's talk about lighting. I will go to the Display Settings to configure the environment.
[3:35] I'll set the Opacity to 1 and the Blur to 0, and you can see an environment encompasses the 3D view.
[3:42] This environment map provides the lighting, and by changing the rotation value, I can change the lighting direction.
[3:49] Changing the environment map will change my lighting.
[3:54] I will set the Opacity back to 0 and I can hold down the Shift key and use my right mouse button to rotate my environment to change the lighting direction.
[4:05] Now that we've covered some fundamentals, I'm going to start with a blank version of the watch and start adding some materials.


### Adding Materials [4:06]
**Transcript (timestamped):**
[4:12] I'll start over in the Assets. I'm going to make sure that the Materials filter is enabled.
[4:18] In the Search field, I'll type in Metal.
[4:21] Now I have a few Metal Materials that I can use.
[4:24] If I want to get some additional materials, I can jump over to the Creative Cloud Desktop app.
[4:29] Here in Substance 3D Assets, which is under Stock and Marketplace, the 3D category, I'll do a search for Metal.
[4:35] Now I have more materials that I can use.
[4:38] For example, if I wanted to use something like this Metal Galvanized, I can come over here to this option, which allows me to Send To.
[4:45] Here I'll click and I have an option to Send To Substance Painter.
[4:49] If I click this, it's going to download the material and then it's going to send it right into Substance Painter.
[4:54] Now if I take a look here at my project, here is this additional material that I can use.
[4:59] I'm going to quickly just refilter my Assets. I'm going to remove this Base Material tag.
[5:04] I'll do a search for Metal.
[5:06] Now I'm going to re-enable my Material tag and I want to use this Metal Sandblasted material.
[5:11] Next, I'm just going to drag and drop this Material right onto the body of the watch.
[5:16] Now I have this Metal Material applied.
[5:20] If I take a look here at the Layer Stack, I can see that underneath the Body Material, I've applied this Metal Sandblasted material as a fill layer.
[5:30] What I'm going to do next is jump over here to my Properties and under the Fill Properties, I have things like my projection I can set,
[5:37] but what I want to change here is the Tiling Options.
[5:40] I'm going to set this to Repeat. I'm going to use a value of 6 and now that Metal Material is repeated across the surface.
[5:47] Now with this Substance Material within the Properties, I have some additional Material Properties I can set.
[5:54] For example, for the Metal Type, I'm going to click the drop-down and I'm going to choose Aluminum.
[5:58] Then I'm also going to make an Adjustment here to the Roughness.
[6:01] It's a little bit too reflective, so I'm going to drag the slider towards the right which is going to increase the Roughness.
[6:07] You see that makes that a little less reflective.
[6:10] Now I've applied this Metal Sandblasted material, but it's been applied to everything in the Body Material for this watch.
[6:17] What I want to do now is mask this material to specific parts of the watch.


### Layer Masking [6:18]
**Transcript (timestamped):**
[6:22] I can do that here in my Layer Stack, very similar to how you would work in Photoshop by creating a Layer Mask.
[6:28] With the layer selected, I'm going to click this Mask option and choose to add a black mask.
[6:33] The mask is black, so that means transparent, and now I cannot see the material anymore.
[6:39] It's been fully masked.
[6:41] With the mask selected on the layer, I'm going to move over to my Toolbar and I'm going to choose this tool which is my Object Fill.
[6:49] With this tool enabled and in the Properties for the tool, I'm going to make sure that I set this to Mesh Fill with a value of white.
[6:57] Now I can simply click on Areas of the 3D Model where I want to apply this mask.
[7:03] Here I'm rotating around the model and selecting areas where I want to apply this material by filling the mask with a white value.
[7:13] I'll grab these buttons and then rotating and looking underneath the watch, I can see that it's a little hard to see what's going on.
[7:20] I'll jump over here to my Display Properties and here I have an option for my Environment Alignment.


### Environment [7:24]
**Transcript (timestamped):**
[7:27] By default, it's set to World. I'm going to set this to Camera and then close this Display Settings.
[7:33] Now you can see that the environment light is now attached to my camera.
[7:37] As I rotate and look underneath the watch, I can more clearly see what I'm doing.
[7:43] Now I'll continue creating my masks here for the base of this watch.
[7:48] With that step completed, I've now applied a metal material by using a layer mask.


### Applying 2D [7:53]
**Transcript (timestamped):**
[7:53] Now I would like to apply a 2D Texture to the watch band.
[7:57] Here I have this watch pattern that was created in Illustrator.
[8:01] I can take that Texture file and simply drag and drop that from its file location and place it right here inside of my Layer Stack.
[8:09] When I let go of my mouse, I will get an option here to apply as a mask or one of the material channels.
[8:16] Because this is color, I want to choose Base Color.
[8:19] Now it's applied another fill layer with that Texture map to the 3D model.
[8:24] Oftentimes when applying a 2D Texture, as I'm doing here, it's a bit easier to come over here to the top of the toolbar and switch my view to my 3D 2D Split View.
[8:35] This allows me to see the 3D model and the UV coordinates.
[8:39] With the layer selected, I have a Transform Tool, similar to a Transform Tool that you would have inside a Photoshop.
[8:46] I'm just going to grab the right side of the Transform Tool and move it towards the left to align the aspect ratio of that Texture so that it more closely matches the width ratio of the watch band.
[8:59] Here you can see that this Texture is now looking pretty good here on the watch band.
[9:04] Let's jump back to just our 3D only view and then here in my Layer Stack, once again, I'm going to apply a Layer Mask.
[9:11] So now we will jump up to our Mask Options.
[9:14] Let's add a black mask.
[9:16] The mask is selected as indicated by this blue outline.
[9:19] We'll jump over to our toolbar and once again, we are going to grab the Object Fill tool.
[9:25] I have the Mesh Fill option and the value is set to 1 or white.
[9:32] Now I just need to left-click on the object to fill the mask with this white value, which essentially masks this material or this Texture map so that it fills just the watch band.
[9:44] And just like that, I've applied a Texture coming from Illustrator to this 3D model here in Substance Painter.
[9:50] Now the last two things I want to do is I want to work with my glass material and then I also want to apply a watch face to this LED material.
[9:58] Now the glass is going to be a little bit more involved so we're going to handle that last.
[10:02] So what I'm going to do right now is just jump over to this Texture Set List and just disable the glass material by clicking the I icon, which will turn off the material.
[10:10] Now let's select the LED and just as I've shown previously with the pattern for the watch band, I can drag and drop a Texture right here into Substance Painter.


### Using Vectors [10:19]
**Transcript (timestamped):**
[10:19] However, this time I'm going to use a vector graphic that is an SVG file so Substance Painter can work with SVG.
[10:25] So I'm just going to left click, drag and drop and instead of dropping that here into my layer stack, this time I'm going to mix it up a bit and I'm just going to drag and drop it right here onto the 3D model itself.
[10:34] And so once I let go of my mouse, I can see here that this applies my watch face and now I have this Transform tool that allows me to move, rotate and I can even scale and position this graphic right where I want it to be.
[10:47] So for example, if I take a look here at the top of the toolbar, I have some tools here for my Translate, my Rotate and my Scale tool.
[10:54] Let's enable the Scale tool and let's scale up the graphic and I'll grab my Translate tool and then just grab hold of these axis handles and then just position the graphic right here in the center of the watch face.
[11:06] Now if I take a look at my properties, I have a few options such as Outline. I can stroke the vector graphic so here I'm just choosing a color and setting a thickness.
[11:16] Now I'm not going to do that in this particular case. I also have the capabilities to apply some basic material options such as Roughness, Metallic and Height.
[11:25] In this case, again, I'm not doing that. This is just going to be my watch face, but you do have these options available to you.
[11:31] Okay, so that takes care of the watch face. It's now been applied. Now let's jump back over here to our Texture Set List for my materials and let's re-enable that glass.
[11:40] As you can see, the glass is now covering the watch face because it's not transparent. We need to actually make this into glass.
[11:48] Let me show you how that would work. We're going to select the glass material and now we need to make some changes to the actual Texture Set itself.


### Working with Opacity [11:49]
**Transcript (timestamped):**
[11:56] For that, I will come over here to my Texture Set Settings and I'm going to select this tab.
[12:01] There's a couple options here. As I scroll down, you can see that there is a Channels List and these are the channels that are available to me.
[12:08] However, I can add additional channels and that's what I want to do right here.
[12:12] If I just move over a little bit so you can see this, I'm going to click this plus button and I'm going to choose to add this Opacity Channel, which you see here.
[12:21] As soon as I add the Opacity Channel, it shows up here in the Texture Set List. Now we can start working with Opacity Information.
[12:28] Let's jump over here to our layers and once again, I'm going to click this button, my paint bucket to add a fill layer and we're going to rename this.
[12:38] Double-click and I'll call this Opacity. Now, if I scroll down here all the way toward the bottom, I now have this slider that's going to let me control Opacity.
[12:49] However, as you're noticing as I make changes, nothing is happening here in my viewport.
[12:54] One other step that we need to do is make some adjustments to the shader or how this material is rendered here in my 3D view.
[13:02] To do that, I'm going to come over here to my Shader Settings. I'm going to click this option and now I have Shader Parameters.
[13:09] All that I need to worry about in this particular case is I scroll down, you're going to see way down here towards the bottom.
[13:15] There's a section here for Opacity and I'm going to click the second option, which is to enable this Alpha Blending.
[13:23] I'll turn this on, we'll close the shader, let's jump back to our layer, make sure the Opacity Fill layer is selected and then come down here in the Properties Fill
[13:35] and change our slider from 1 to 0. Now, I'm starting to see that transparency.
[13:41] I don't want this to be completely transparent so I'm going to grab this slider, move it towards the right so that it's not 0.
[13:49] Then what I'll do is come over here to my Roughness and drag this here towards the left, closer to 0 to make this a reflective shiny surface like glass.
[13:59] That's going to take care of how glass is going to work once I get this over here into After Effects.
[14:03] I'm just holding down Shift using my right mouse button so I can rotate my light around just to get an idea of how things are working.
[14:09] This is going to take care of the glass material.
[14:11] Looking at the finished project here, I want to make one final change.
[14:16] I'm going to jump back here to that LED screen where I have my watch face and I don't like this create background.
[14:23] Let's add a color to this. Here I'll go to my layers.
[14:27] Once again, you can see you're constantly doing this in Substance Painter.
[14:30] I'm going to jump over here and add a Fill layer. We'll click our Paint Bucket icon. Let's just call this Color.
[14:36] Then what we're going to do is just come down here to our Properties Fill and you'll notice that I have this little Eyedropper tool.
[14:43] Let's select the Eyedropper and then we're just going to mouse over here into our 3D view.
[14:47] I can just choose one of these blue color values. I think I'll just sample this value right here.
[14:52] Now you'll notice that this color is overriding my watch face graphic.
[14:57] Just like in Photoshop, layers are processed from the bottom up.
[15:01] All I need to do is just reorder this.
[15:03] With the layer selected, I can left click, drag and drop that Fill layer below the graphic to Material.
[15:09] Now I have my watch face with my blue color underneath.
[15:13] I'm ready to send this 3D model into After Effects for animation.
[15:17] Take a break or spend some time checking out Substance Painter.
[15:21] When you're ready, join me for part two where we will send this watch into After Effects.



---

## Captured Frames

- [0:20] tutorials/frames/preparing-a-3d-asset-in-substance-3d-painter-3d-in-after-effects-part-1-adobe-su/frame_000.jpg
- [2:37] tutorials/frames/preparing-a-3d-asset-in-substance-3d-painter-3d-in-after-effects-part-1-adobe-su/frame_001.jpg
- [3:18] tutorials/frames/preparing-a-3d-asset-in-substance-3d-painter-3d-in-after-effects-part-1-adobe-su/frame_002.jpg
- [5:40] tutorials/frames/preparing-a-3d-asset-in-substance-3d-painter-3d-in-after-effects-part-1-adobe-su/frame_003.jpg
- [6:33] tutorials/frames/preparing-a-3d-asset-in-substance-3d-painter-3d-in-after-effects-part-1-adobe-su/frame_004.jpg
- [7:27] tutorials/frames/preparing-a-3d-asset-in-substance-3d-painter-3d-in-after-effects-part-1-adobe-su/frame_005.jpg
- [8:46] tutorials/frames/preparing-a-3d-asset-in-substance-3d-painter-3d-in-after-effects-part-1-adobe-su/frame_006.jpg
- [10:34] tutorials/frames/preparing-a-3d-asset-in-substance-3d-painter-3d-in-after-effects-part-1-adobe-su/frame_007.jpg
- [13:15] tutorials/frames/preparing-a-3d-asset-in-substance-3d-painter-3d-in-after-effects-part-1-adobe-su/frame_008.jpg
- [15:03] tutorials/frames/preparing-a-3d-asset-in-substance-3d-painter-3d-in-after-effects-part-1-adobe-su/frame_009.jpg

---

## Structured Notes

### Core Technique
A ground-up beginner walkthrough of Painter's core texturing fundamentals — paint vs. fill layers, layer masking with the Object Fill (Mesh Fill) tool, applying flat 2D/vector textures (Illustrator raster + SVG vector) as their own fill layers, and building a working glass material via a custom Opacity channel plus shader-level Alpha Blending — using a smartwatch asset that will be exported to After Effects in Part 2 (out of scope for this Painter-only skill).

### Summary
Official Adobe beginner video (Part 1 of a 2-part "3D in After Effects" series). Sources a smartwatch FBX from Substance 3D Assets (Creative Cloud Desktop app), creates a new Painter project from the default **ASM PBR Metallic Roughness** template, and lets Painter auto-generate UVs on import if the model lacks them. Tours the core UI (Assets, 3D/2D view, Texture Set List, Layer Stack, Properties) and 3D navigation (Alt/Option+LMB orbit, Alt/Option+RMB zoom, Alt/Option+MMB pan). Explains the two fundamental layer types: a **paint layer** (paintable directly on the model, material values set first — color/roughness/metallic — each Texture Set/material has its own independent Layer Stack, so painting cannot cross material boundaries) versus a **fill layer** (non-paintable, fills the whole active Texture Set with set material values). Covers environment/lighting basics in **Display Settings** (Opacity, Blur, Rotation of the HDRI environment map; Shift+RMB-drag to rotate lighting interactively) and **Environment Alignment** (World vs. **Camera** — Camera-attached lighting stays consistent while orbiting, useful for seeing detail on the underside of a model). Demonstrates sourcing additional materials from Substance 3D Assets via Creative Cloud's "Send to Substance Painter" action, applying a **Metal Sandblasted** smart material to the watch body as a fill layer, adjusting **Tiling** (UV transformations, Repeat mode, scale value 6) and per-material parameters (Metal Type dropdown → Aluminum, Roughness slider), then confining that material to specific mesh areas with a **black mask + Object Fill tool** (Mesh Fill mode, value 1/white) painted on by clicking mesh regions directly (Photoshop-style masking). Applies a 2D Illustrator-made pattern to the watch band by dragging the image file into the Layer Stack (choosing **Base Color** as the target channel from the drop prompt), using the **3D/2D Split View** and the layer's **Transform Tool** to align the texture's aspect ratio, then masking it to the band with the same black-mask + Object-Fill workflow. Applies a second graphic — this time an **SVG vector** — by dragging it directly onto the 3D model itself (rather than into the Layer Stack), which auto-creates a positionable decal with its own Translate/Rotate/Scale gizmo tools and Properties options for Outline (stroke color + thickness) and material channels (Roughness/Metallic/Height), used here for the watch-face graphic. Builds a working glass material for the watch crystal: temporarily disables the Glass Texture Set (eye icon) to work underneath it, then re-enables it and, with Glass selected, adds a custom **Opacity** channel via Texture Set Settings' channel-add (+) button, creates an "Opacity" fill layer to control the opacity slider — which has no visible viewport effect until **Shader Settings > Opacity > Enable Alpha Blending** is turned on for the active shader instance. Once alpha blending is enabled, lowering the Opacity fill layer's value from 1 toward 0 makes the glass genuinely transparent (kept slightly above 0 rather than fully transparent), paired with a low Roughness value for a shiny glass look. Finishes with a background color fix for the LED watch-face graphic: adds a new "Color" fill layer, samples a blue tone directly from the viewport with the **Eyedropper** tool, then reorders it beneath the graphic layer in the stack (Painter composites bottom-up, same as Photoshop) so the sampled color shows through as the graphic's background instead of overriding it.

### Key Steps
1. **Source a 3D asset:** browse/download a model (FBX) from Substance 3D Assets via the Creative Cloud Desktop app.
2. **Create a new project:** File > New, choose the **ASM PBR Metallic Roughness** template, select the FBX/OBJ mesh, set document resolution, leave other settings default; Painter auto-generates UVs on import if the mesh lacks them.
3. **Learn 3D navigation:** Alt/Option+Left-drag to orbit, Alt/Option+Right-drag to zoom, Alt/Option+Middle-drag to pan; switch the top-bar view mode to "3D only" while working.
4. **Create a paint layer** (Add Layer button) to paint directly on the model: pick a brush from Assets, set Material Values (color/roughness/metallic) in the Properties panel, then paint — remember each Texture Set/material has its own independent Layer Stack, so you must select the correct material (e.g. body vs. glass) before painting on it.
5. **Create a fill layer** (paint-bucket icon) as a non-paintable alternative that fills the whole active Texture Set with set material values (roughness, metallic, etc.).
6. **Configure environment lighting** in Display Settings: set Environment Opacity/Blur/Rotation to preview and adjust the HDRI backdrop and its lighting direction; Shift+Right-drag in the viewport also rotates the environment interactively.
7. **Source additional materials** from Substance 3D Assets (Creative Cloud, Stock and Marketplace > 3D) and use **Send to Substance Painter** to download and import them directly into the open project's asset shelf.
8. **Apply a smart material as a fill layer** by dragging it onto the model; adjust **Tiling** (UV transformations > Scale/Tiling, set to Repeat with a chosen value) and material-specific parameters (e.g. Metal Type dropdown, Roughness slider) in the Properties panel.
9. **Mask a material to specific mesh areas:** select the fill layer, add a black mask (fully transparent/hidden), select the **Object Fill** tool with **Mesh Fill** mode and value **1 (white)**, then click mesh regions in the viewport to paint the mask in per-mesh-part (not freehand) — exactly like a Photoshop layer mask workflow.
10. **Switch Environment Alignment from World to Camera** (in Display Settings) when working on hard-to-light areas (e.g. the underside of a model) so the lighting rotates with the camera instead of staying fixed.
11. **Apply a flat 2D texture (e.g. an Illustrator-made pattern):** drag the image file directly into the Layer Stack, choose the target channel (e.g. Base Color) from the drop prompt, switch to **3D/2D Split View** to see UV placement, and use the layer's **Transform Tool** to correct aspect ratio/scale so it matches the target surface.
12. **Mask the 2D texture to its intended area** using the same black-mask + Object-Fill (Mesh Fill, white) technique as step 9.
13. **Apply a vector (SVG) graphic as a positioned decal:** drag the SVG file directly onto the **3D model** (not the Layer Stack) to auto-create a decal with its own Translate/Rotate/Scale transform gizmo; Properties expose an **Outline** option (stroke color + thickness) and optional material channels (Roughness, Metallic, Height) for the decal.
14. **Build a working glass material:** with the Glass Texture Set selected, open **Texture Set Settings**, use the **+** button to add a custom **Opacity** channel (not present by default).
15. **Create an Opacity-purpose fill layer** and use its Opacity slider — note it has zero visible effect until the shader itself is configured to respect it.
16. **Enable Alpha Blending:** open **Shader Settings**, scroll to the Opacity section, check **Enable Alpha Blending** on the active shader instance (Main shader / `asm-metal-rough` in this project) — only then does lowering the Opacity fill layer's value produce visible transparency.
17. **Tune the glass look:** lower the Opacity layer's value from 1 toward (but not fully to) 0 for believable glass transparency, and lower Roughness toward 0 for a shiny/reflective glass finish.
18. **Fix a graphic's background color:** add a new fill layer, use the **Eyedropper** tool to sample a color directly from the viewport, then **drag-reorder that fill layer below** the graphic layer in the Layer Stack (Painter composites bottom-to-top, same convention as Photoshop) so the sampled color reads as the graphic's background instead of covering it.

### Layers / Tools / Settings
- **Layer types:** Paint layer (paintable, per-material-independent Layer Stack) vs. Fill layer (non-paintable, whole-Texture-Set material fill)
- **Display Settings:** Environment Opacity/Blur/Rotation, **Environment Alignment** (World vs. Camera)
- **Masking:** black mask + **Object Fill** tool (Mesh Fill mode, value 1/white) for per-mesh-part masking by clicking
- **Fill layer Properties:** Projection (UV projection), Filtering, UV Wrap, UV transformations (Scale, Tiling/Repeat, Rotation, Offset), Material tabs (color/height/rough/metal), per-material dropdown parameters (e.g. Metal Type)
- **2D texture import:** drag into Layer Stack (choose target channel: e.g. Base Color) + **Transform Tool** + **3D/2D Split View**
- **Vector (SVG) decal import:** drag directly onto the 3D model; Translate/Rotate/Scale gizmo tools; Properties: Outline (color + thickness), optional Roughness/Metallic/Height channels
- **Texture Set Settings:** add custom channels via the **+** button (used here to add **Opacity**)
- **Shader Settings > Opacity:** Enable alpha test, **Enable alpha blending** (required for any Opacity-channel value to actually render as transparency)
- **Eyedropper tool** (in Fill layer Properties) to sample viewport colors directly
- **Layer reordering** by drag-and-drop — bottom-to-top compositing, same as Photoshop
- Source assets: Substance 3D Assets (Creative Cloud Desktop, Stock and Marketplace > 3D), "Send to Substance Painter" action

### Difficulty
Beginner (explicitly a fundamentals video — paint/fill layers, basic masking, texture import, and one intermediate topic: Opacity channel + shader Alpha Blending for glass).

### App & Version
Substance 3D Painter. No version number is stated in narration or clearly legible in the captured frames; project template used is "ASM - PBR Metallic Roughness."

### Tags
`layers`, `fill-layer`, `paint-layer`, `masks`, `blend-mode`, `texture-set`, `pbr`, `metal-rough`, `basecolor`, `roughness`, `metallic`, `height`, `normal-map`, `opacity`, `viewport`, `alpha`, `beginner`

---

## Related Tutorials
- [Native Illustrator File Support in Substance 3D Painter](native-illustrator-file-support-in-substance-3d-painter-adobe-substance-3d.md) — same channel (Adobe); a much deeper dive into the same "drag a 2D/vector graphic in as a texture" theme this video only touches briefly for the watch-band pattern and watch-face SVG.
- [Custom Fonts in Substance 3D Painter](custom-fonts-in-substance-3d-painter-adobe-substance-3d.md) — same channel (Adobe); another dynamic-resource-as-texture feature from the same 10.x-era, complementary to this video's SVG-decal-as-fill-layer workflow.
- [Preparing Models for Substance 3D Painter in Blender / Maya / 3DS Max](preparing-models-for-substance-3d-painter-in-blender-adobe-substance-3d.md) — same channel (Adobe); shares this video's "asset preparation before texturing" framing, though for DCC-side mesh prep rather than downstream-app (After Effects) export prep.
