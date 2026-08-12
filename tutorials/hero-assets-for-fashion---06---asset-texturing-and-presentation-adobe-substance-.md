---
title: Hero Assets for Fashion - 06 - Asset Texturing and Presentation | Adobe Substance 3D
source: YouTube
url: https://www.youtube.com/watch?v=us4NAWtaRic
author: Adobe Substance 3D
ingested: 2026-08-12
app: "[PENDING]"
version: "[PENDING]"
tags: []
extraction_status: pending
frames_dir: tutorials/frames/hero-assets-for-fashion---06---asset-texturing-and-presentation-adobe-substance-/
frame_count: 0
frame_status: pending-selection
---

# Hero Assets for Fashion - 06 - Asset Texturing and Presentation | Adobe Substance 3D

**Source:** [YouTube](https://www.youtube.com/watch?v=us4NAWtaRic)
**Author:** Adobe Substance 3D
**Duration:** 19m4s | 1 section(s)

---

## Raw Data (for Claude Code extraction)

Frames are not captured yet. Read the timestamped transcript below, pick moments
that actually show a technique/result worth a still (not blind percentages —
even within a named chapter, verify the real moment against its timestamps), then run:
  python select_frames.py hero-assets-for-fashion---06---asset-texturing-and-presentation-adobe-substance- <ts1> <ts2> ...
(seconds or mm:ss). This appends a "Captured Frames" section and updates the
frontmatter before you write the Structured Notes below.


### Full Content [0:00]
**Transcript (timestamped):**
[0:00] In this tutorial, I will demonstrate how to texture a dress for hero images and render
[0:13] it with Stager.
[0:16] In previous tutorials in this series, I created a silk gazzar fabric, which I will now use
[0:22] as the base material for this dress.
[0:26] Substance Painter is a great solution for fashion asset texturing and the way I will
[0:30] use it is by layering several elements.
[0:35] First I will apply a variation of the base material, then I will use several height and
[0:40] normal layers to add folds, wrinkles and other elements that will contribute to a realistic
[0:47] result.
[0:48] I will add these up going from large to medium to small scale creases and imperfections.
[0:55] Finally, I will work on the French seams and the stitching.
[1:00] Although all of these can be painted by hand with Painter's brush tools, I will favor
[1:05] a more parametric approach based on fill layers in this tutorial.
[1:11] I will demonstrate several different techniques to that end.
[1:15] To start this off, I create a new Painter document with an Adobe Standard material and
[1:21] I load my mesh.
[1:25] I set the document to 4k, check Use UV Tile workflow as I will be using several tiles
[1:33] and turn off auto unwrap as I want to keep my existing UVs.
[1:39] My UVs are laid out over 4 tiles which are listed in the Texture Set List panel.
[1:46] Before I start texturing, I go to the Shader settings, turn off Subsurface Scattering as
[1:52] I won't be using it and enable Anisotropy which I will need to view my fabric correctly.
[2:00] Next in the Texture Set settings, I click the plus button to add anisotropy level,
[2:06] anisotropy angle and opacity to my existing channels.
[2:11] These are necessary to account for anisotropy and opacity on my fabric.
[2:18] I have to do one more thing before texturing and that is to bake some mesh maps.
[2:24] Baking converts several characteristics of the mesh to maps so that they can be used
[2:29] by filters and generators.
[2:32] They are also combined with the painted textures when exporting the final maps.
[2:38] I make sure all my tiles are selected, set the resolution to 4k and select the maps I
[2:44] want baked, in this case normal, ambient occlusion, curvature and position.
[2:51] Finally, I load my high poly mesh from which painter can calculate normal on the low poly
[2:57] mesh I use for painting.
[3:00] He can create a high poly mesh by exporting the same dress from this teacher or other
[3:05] fashion app at a higher resolution.
[3:09] Don't worry if you don't have this, it is not necessary.
[3:13] I click Bake Selected Textures with the default settings and painter bakes the selected maps.
[3:20] These maps are now applied to the mesh.
[3:24] They are visible in the Texture Set settings and can be viewed by cycling through the channels
[3:29] in the 3D viewport.
[3:32] Time to import my base material.
[3:35] From Designer I select Send to Substance 3D Painter with my package selected and the
[3:40] material appears in Painters Assets panel.
[3:44] The process is the same if you use Substance Sampler to make your materials.
[3:49] I drag and drop the material onto the mesh and it becomes a fill layer in the layer stack.
[3:56] The parameters I created and exposed while making the material are here and I will adjust
[4:02] this as well as the material styling and filtering to get the desired result.
[4:09] If you haven't already, you may want to watch the previous tutorials in this series that
[4:14] show how I created a Silk Gazare material with 4 different methods.
[4:21] I will now build several layers of large, medium and small creases to create an intricate
[4:27] realistic result while hiding all layers I am not actively working on.
[4:33] This will allow me to focus on each individual layer before I finally blend all the layers
[4:38] together.
[4:41] For large folds I will load some displacement maps I previously created in a sculpting application
[4:48] and use them here as height maps.
[4:51] Substance Painter largely eliminates the need for sculpting directly on the mesh and favors
[4:57] a non-destructive workflow fully based on parametric texture maps.
[5:03] Using displacement maps generated from sculpting on the mesh as height maps brings together
[5:08] the best of both worlds.
[5:11] Creating the first map will load all 4 maps, one for each UV tile that I am using.
[5:18] I create a fill layer, turn off all channels except height and drag and drop the height
[5:25] maps into the height input field.
[5:27] I select the height channel in the layers panel and reduce the strength of the layer
[5:33] before naming it appropriately and hiding it.
[5:37] To create more large folds I will make a second fill layer and only leave its height
[5:43] channel on as well as its color temporarily for visual clarity while editing.
[5:49] I right click on the material and add a black mask which will render the full layer invisible
[5:56] until I add brighter elements to it to reveal parts of the layer.
[6:01] I then right click on the mask and add a generator.
[6:04] I click in the generator field and select the UV border distance generator which generates
[6:11] an area along the dress's UV islands which are also its pattern seams.
[6:17] After adjusting the mask settings to start strongly at the edges of the patterns and
[6:22] taper off toward the inside of the patterns I go back to the material settings and turn
[6:29] off the color which was only there to help me visualize the result.
[6:34] I then add a 3D simplex noise to the height and adjust the settings to achieve the desired
[6:41] effect of large folds near the seams.
[6:45] It's worth spending some time testing various noises at different scales and settings to
[6:50] achieve different results for each kind of fabric and garment.
[6:54] There is a distinct line here cutting through my folds and this is caused by my mask.
[7:00] Adding a blur filter to my mask fixes this.
[7:05] After naming this layer and adjusting its opacity I will hide it and create yet another
[7:10] fill layer this time for medium creases.
[7:14] Once more I will turn off all channels but the height and this time I will add a crystal
[7:20] 2 procedural texture to it and adjust its styling size to simulate medium sized wrinkles.
[7:29] To apply the texture selectively I add a black mask to the layer, add a UV border distance
[7:36] generator to it and adjust its settings to contain the creases near the seams.
[7:43] I then add a blur at a low intensity to both the material and the mask to smooth out the
[7:49] creases a little.
[7:52] Finally I pull back the layer's opacity to make the creases more subtle.
[7:58] I then right click on the layer and select duplicate layer from the context menu.
[8:04] This will duplicate the creases layer with all its parameters, masks and filters intact
[8:10] and it will be the basis for a new layer with smaller creases.
[8:14] From the material settings I increase the tiling and reduce the scale to make the creases
[8:20] smaller and I adjust the contrast, balance and other settings of the procedural texture
[8:27] to get to more believable results.
[8:30] To finish this I go back and adjust the materials and masks blur filters to get smoother transitions.
[8:38] It's now time to turn back on all of my layers and adjust their opacity so that they all
[8:43] combine in a convincing way.
[8:46] The result has to be subtle as this is essentially a formal dress so I keep the height opacity
[8:52] numbers fairly low.
[8:55] Next I want to flatten the seams a little to give the impression of French seams, which
[9:01] are seams used with sheer fabrics that attempt to be invisible by enclosing raw edges.
[9:08] To do this I create a new fill layer with a black mask with a UV border distance generator.
[9:15] I leave the fill material to the default for now.
[9:19] I adjust the settings so that the mask affects around half a centimeter on both sides of
[9:24] the seams.
[9:26] In the layers panel and in the height channel I set the layers mode to replace and the opacity
[9:33] to 10.
[9:35] This partly overrides the height of the previous layers and flattens the selected areas.
[9:41] I also add a blur with a very low setting to smooth out the transition of the mask.
[9:47] I name the layer accordingly and turn off all of my layers once again.
[9:55] Another great way to introduce wrinkles, creases and folds is using the inflate shrink wrap
[10:00] filter on a new fill layer and adjusting its settings to imitate specific fabrics.
[10:08] There are several options here that can combine to achieve considerably varied results.
[10:14] I use it here for some medium sized folds on my silk gazzar.
[10:19] I need some additional creases for the whole dress and for this I will use a different
[10:24] technique.
[10:25] I click the plus button in the assets panel to add an image I previously downloaded from
[10:30] Adobe Stock.
[10:32] Any similar image of a flat wrinkled fabric or sheet will do as long as its monochrome
[10:38] grayscale or normal map.
[10:41] I set the type to texture and import the resource to my project.
[10:46] I then create a new fill layer with only the height channel enabled and drag and drop the
[10:52] image into the height input field.
[10:56] For normal maps you can use the normal channel input field.
[11:00] I adjust the size and position using the bounding box in the 2D view.
[11:06] Because the image is low bit depth it gives me a grainy result so I add blur to the layer
[11:13] to eliminate this.
[11:15] I lower the layers height opacity to make the result subtle and name the layer accordingly.
[11:22] Now I need some stitching and I will make it procedurally.
[11:26] To achieve this I will combine two masks with UV border distance generators and one with
[11:32] a procedural texture.
[11:35] First I add a new fill layer and adjust the settings to make a rough non-metallic with
[11:41] positive height for the stitching material.
[11:45] I then add a black mask with the UV border generator to the layer and set its parameters
[11:51] to 0.05 for balance, 1 for contrast, 0 for smoothness and 0.1 for distance.
[12:01] I then add a second UV border generator and set its parameters to the same values except
[12:07] the balance at 0.04 leaving a short distance between this and the previous mask generator.
[12:16] This will be the thickness of the stitching.
[12:18] Finally, I set the second generators mode to subtract.
[12:24] This will subtract it from the previous generator leaving just a narrow line along the seams.
[12:30] Next, I add a fill on top of the generators and the fabric diagonal thin procedural texture
[12:37] to it.
[12:39] I increase the filter's styling to 10 and the texture style parameter to 16 and set
[12:46] its mode to subtract.
[12:49] This will break up the continuous line giving me individual stitches.
[12:54] Now I can go back to the stitching material and adjust the color and height.
[12:59] To remove possible unwanted stitching areas, as this method covers all seams, I add a paint
[13:05] filter to the mask and use a black brush over them.
[13:09] In some cases, manual stitching by creating a paint layer and using a stitching tool on
[13:15] it is preferred.
[13:17] For such cases, there are several stitching tools that ship with Painter and they support
[13:22] several kinds of stitching including running, double and overlook as well as several kinds
[13:28] of thread.
[13:30] I find it more intuitive and precise to use this technique in the 2D view, holding Shift
[13:36] while clicking to create straight lines between selected points.
[13:41] One final check by rotating the light around the dress to identify potential problematic
[13:47] areas before exporting.
[13:50] Bear in mind that the seams' HDRI can be changed from the environment settings so that you
[13:56] can preview your model in several lighting scenarios.
[14:01] Shift plus right click plus drag rotates the HDRI.
[14:07] Once happy with the result, I can go to File, Export Textures, set the directory, template
[14:14] and file type and create the maps for all channels and UV tiles.
[14:19] However, in this case, I prefer to send the dress directly to Substance Stager through
[14:25] the Send to Substance Stager button.
[14:28] Over in Stager now, the model loads with all maps in place and as soon as I turn ray tracing
[14:34] on, it will render as intended.
[14:38] Rendering with the GPU tends to be faster depending on the computer specifications.
[14:44] I previously downloaded the mannequin from the Substance Asset Library and textured
[14:49] it with Painter.
[14:51] Shift plus left mouse button plus drag rotates the lights similarly to Painter.
[14:57] The creases are a little too prominent so I will delete the dress and go back to Painter
[15:03] for some tweaking.
[15:05] I balance the layers a little more and make the overall effect more subtle before sending
[15:10] the dress to Stager again.
[15:14] From the Starter Assets panel, I drag and drop a 3-point light setup into the scene.
[15:20] With the environment selected in the Scene panel and in the Light properties, I hide
[15:25] the environment light and adjust the key light settings so that it hits the dress from the
[15:31] front right and highlights the dress's features.
[15:36] I put the fill light front left and adjust it so that it partly fills the shadows created
[15:42] by the key light.
[15:44] I then play around with the backlight before deciding to take it off altogether as it does
[15:50] not contribute to my scene.
[15:52] From the Starter Assets models, I drag a plane into the scene, rotate and scale it in the
[15:58] 3D view and using the Transform panel so that it becomes my backdrop.
[16:04] I also add a gray matte standard material to it from Stager's Basic Material presets.
[16:10] I add a camera from the Camera menu and set its resolution to 2K and its focal length
[16:17] to 100 which is better for product photography.
[16:21] I select the backdrop plane and darken its color so that the dress pops a little more
[16:27] although I plan to work on the backdrop in Photoshop once the render is completed, so
[16:31] this is really a placeholder.
[16:33] I rename my scene's objects appropriately and I'm expanding the Dresses Model folder
[16:38] in the Scene panel which includes four objects representing the four UV tiles I painted in
[16:44] Painter.
[16:46] I can now select these and adjust the strength of the channel maps.
[16:50] As an example, if I want to make the fabric more sheer, I can click on the Opacity map,
[16:56] double click the preview to open it in Photoshop and add an Adjustment Layer to darken it.
[17:03] Saving the document will update the map in Stager where the dress fabric now looks more
[17:08] sheer.
[17:10] After a few more adjustments I arrived at this result which I am now ready to render by going
[17:15] to Stager's Render module.
[17:18] Here I can select the camera I wish to render along with its attached resolution, the name
[17:24] of the file to export, its format and the export directory.
[17:30] I normally use the Medium preset for everyday renders as I find it offers a good balance
[17:36] between quality and speed.
[17:38] For production I would normally use at least 1000 samples so I would probably opt for the
[17:44] high preset.
[17:46] Stager also denoises the final result to make rendering times shorter and to fix possible
[17:52] firefly artifacts on difficult scenes.
[17:55] For stales I normally use the PST format so I can do some basic post-work in Photoshop.
[18:02] PST renders include additional layers for selecting objects and background easily.
[18:09] I downloaded a few images from Adobe Stock and mixed them here to create a backdrop.
[18:15] I made a close-up shot by creating a second camera and adjusting the lights to be complementary
[18:22] to this part of the dress.
[18:25] I find Stager to be a great tool for fashion visualization as I can send design iterations
[18:31] directly from Painter and visualize styles and collections in real time.
[18:37] The latest Stager release also supports animation so 360 turntables are now possible and very
[18:44] easy to set up and render.
[18:47] This concludes this series of tutorials on Hero Assets for Fashion.
[18:51] I hope that you enjoyed it and I look forward to seeing some of your work based on these
[18:55] techniques as well as feedback on these tutorials.



---

## Structured Notes

### Core Technique
[PENDING EXTRACTION]

### Summary
[PENDING EXTRACTION]

### Key Steps
[PENDING EXTRACTION]

### Layers / Tools / Settings
[PENDING EXTRACTION]

### Difficulty
[PENDING EXTRACTION]

### App & Version
[PENDING EXTRACTION]

### Tags
[PENDING EXTRACTION]

---

## Related Tutorials
[PENDING EXTRACTION]
