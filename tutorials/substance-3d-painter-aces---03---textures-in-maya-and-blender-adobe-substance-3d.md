---
title: Substance 3D Painter & ACES - 03 - Textures in Maya and Blender | Adobe Substance 3D
source: YouTube
url: https://www.youtube.com/watch?v=Lksg6Fum3gw
author: Adobe Substance 3D
ingested: 2026-08-12
app: "[PENDING]"
version: "[PENDING]"
tags: []
extraction_status: pending
frames_dir: tutorials/frames/substance-3d-painter-aces---03---textures-in-maya-and-blender-adobe-substance-3d/
frame_count: 0
frame_status: pending-selection
---

# Substance 3D Painter & ACES - 03 - Textures in Maya and Blender | Adobe Substance 3D

**Source:** [YouTube](https://www.youtube.com/watch?v=Lksg6Fum3gw)
**Author:** Adobe Substance 3D
**Duration:** 9m31s | 8 section(s)

---

## Raw Data (for Claude Code extraction)

Frames are not captured yet. Read the timestamped transcript below, pick moments
that actually show a technique/result worth a still (not blind percentages —
even within a named chapter, verify the real moment against its timestamps), then run:
  python select_frames.py substance-3d-painter-aces---03---textures-in-maya-and-blender-adobe-substance-3d <ts1> <ts2> ...
(seconds or mm:ss). This appends a "Captured Frames" section and updates the
frontmatter before you write the Structured Notes below.


### Intro [0:00]
**Transcript (timestamped):**
[0:00] Hello, and welcome back to the third part of this video series covering Substance Painter and its implementation of ASUS CG.
[0:10] Once again, I'm Michael Wilde, and if you haven't watched Parts 1 and 2, then hop over to them first,
[0:14] as we've already covered the important color space terminology and how to work with OCIO and ASUS CG inside of Painter.
[0:20] In this final part, we're going to quickly look at correctly importing our textures into Maya to get an ASUS CG render matching our Substance Painter viewport.
[0:29] I'm going to be demonstrating with Maya since it's the industry standard digital content creation package for VFX,
[0:34] which most large and mid-sized studios build their pipeline around.
[0:38] Plus, 9 times out of 10, it's the software you need to know when applying for VFX jobs.
[0:43] I will also briefly cover the same thing in Blender since it's an important first step for people learning VFX,
[0:49] and getting the same result across multiple programs also demonstrates part of the reason ASUS and OCIO were created.
[0:55] To standardize, handling color data across multiple digital packages.
[1:00] In the previous video, we looked at our export settings in Substance.
[1:04] With all that good to go, I'm ready to actually export my textures.
[1:07] This is done exactly the same as it would usually be.
[1:09] You can use a Substance Preset for whichever renderer you're using, or make a preset yourself.
[1:14] I have one here that exports my textures as 8 and 16 bit tiffs,
[1:18] within naming conventions similar to the ones used in VFX studios.
[1:22] Since this doesn't affect color space, I'm not going to explain how I did that,
[1:24] but if you're unfamiliar, then check out the other videos on Substance's YouTube channel.


### ACES's OCIO config file [1:25]
**Transcript (timestamped):**
[1:28] As we discussed in part 2, ASUS Color Management can be added to a piece of software with OCIO via a config file.
[1:35] Like with Substance Painter, the latest version of Maya comes built in with ASUS as standard,
[1:40] but for older versions of the software, we can set it up ourselves.
[1:44] You can download ASUS for free from their website if you need it.
[1:47] It comes in at about 2GB, so go and make a cup of tea whilst it downloads.
[1:51] In Maya, we're going to open up our preferences and go to Color Management.


### Maya's colour management [1:52]
**Transcript (timestamped):**
[1:55] I'm in Maya 2023 here, and you can see by default we have Color Management enabled,
[2:00] ASUS CG set up as our rendering space, and SRGB as our display, just like we had in Painter.
[2:06] We also have the View setting as ASUS.
[2:09] We could change this to something else, for example, if we wanted to see our renders without any color
[2:13] management for debugging, but as it stands, this is correct.
[2:17] If you're working with an older version of Maya, for example, here I have 2019 open,
[2:21] then you need to select the ASUS 1.2 OCIO config file that we downloaded earlier as our config path.
[2:28] Doing this will give us a slightly different set of defaults.
[2:31] If we're using a downloaded config file, it will set our display to ASUS, but then add an
[2:36] SRGB view transform on top of that to show us our ASUS renders correctly.
[2:42] Regardless of if you're using the in-built ASUS setup or the downloaded ASUS config file,
[2:46] it's important to set this up at the start of your project, as altering halfway through
[2:50] may mean you need to retell Maya how to manage the color of every single file you've already imported.


### Maya shader setup [2:55]
**Transcript (timestamped):**
[2:57] I've got my model into Maya ready to apply my textures on it.
[3:00] I'm going to open up the Hypershade and create a new Arnold Standard Shader,
[3:03] and then add a File node to the color.
[3:06] I'm now able to import my substance-based color textures by finding the files on disk.
[3:12] After I've linked that up, it's time to go down to my file's color space drop-down and tell Maya
[3:18] how to handle this input. Since my base color map is color data, like we saw in part 2 of this series,


### Maya Colour Space options setup [3:20]
**Transcript (timestamped):**
[3:25] substance exported it as utility SRGB texture. We need to tell Maya that this is the color
[3:31] space of this image, and the same for any other color data maps so that it can be ingested correctly.
[3:37] Remember our Google Translate metaphor from the previous video.
[3:40] We're helping the color data be interpreted properly by telling it what's being inputted.
[3:44] If I click the drop-down of every input color space the ASUS config gives us,
[3:48] I will find utility SRGB texture eventually in this long list.
[3:54] If you're using the inbuilt Maya 2023 ASUS setup instead of a downloaded ASUS config file,
[3:59] this is a little bit more streamlined, so you actually have a lot less to select from,
[4:03] and you're looking for an option called Display SRGB instead.
[4:07] The final thing to change on this file node is the UV tiling method,
[4:11] which needs to be UDIMS so that my texture files get picked up correctly.
[4:16] Now I'm going to add my spec roughness in the same way. After creating a file node for it,
[4:21] and selecting the images on disk, I will go down to my color space options to set this up again.
[4:26] As covered in part 2, specular roughness is scalar data, so we don't want to use the same input color
[4:32] space this time. In fact, we don't want Maya to do any conversion, since we just want the pixel
[4:37] data to be read as pure data. The utility raw option tells Maya exactly that. This is raw data,
[4:44] no conversion is needed. And it's as easy as that. You just need to remember to set up UDIMS again
[4:49] if you're using them, and then use the raw setting for any other scalar data maps you might import.
[4:55] Once I've set up the map so I export from painter, I'm also going to set up the same
[4:59] HRI that we had in substance as well. To do that, I'll add an Arnold Skydome light, and under the
[5:03] color of it, I'll once again select a file. I'll locate the EXR file on my computer and add it.
[5:09] This time, however, we're going to need to set it up slightly differently. Our HRI image is color
[5:14] data, but unlike the earlier maps that we were importing, it's a linear EXR file, so we need
[5:19] to tell Maya this. For this kind of file, we need to select utility linear sRGB. Again, if you're
[5:25] using the inbuilt Maya 2023 ASUS setup, this will be named slightly different, and it's called
[5:31] scene linear, scene linear rec709 sRGB. Now you'll see it in the Maya viewport looking correct.
[5:38] And really, that's all that we need to do. If I rotate the HRI to be the same angle and set off
[5:43] a render, we can compare the Substance viewport and the Arnold render view and see that they look
[5:47] very similar. Obviously, there will be slight differences as Substances viewport and Maya use
[5:52] different render engines, for example, Arnold has shadows, but both programs are correctly using
[5:57] ASUS CG via OCIO to handle our color data correctly. I can further show this by setting up a render
[6:03] AOV in Arnold to show just my base color map at render time and view the same then in Painter.
[6:10] This way, I can bypass the slight differences of the renderers and their shaders
[6:14] to see that the imported textures are set up correctly. And what would you know? They look


### Blender ACES setup [6:18]
**Transcript (timestamped):**
[6:18] exactly the same. Now let's do the same thing in Blender. So Blender is slightly less user-friendly
[6:24] for color management and to get ASUS working. There's no way in the software to just import
[6:28] a config file like we did in Maya, so we need to set up a Windows environment variable that points to it.
[6:37] I'll create one called OCIO with a link to the ASUS config file, and now when I open Blender,
[6:42] it will pick this up automatically. It's worth mentioning that this will override other programs
[6:47] that read this variable like Maya and Substance if you are using their inbuilt ASUS setups in a file.
[6:54] If you do get errors from this, then deleting the environment variable before opening those
[6:58] files will stop the issue. As I've had to do recording this video, jumping between all these
[7:02] different programs. So in Blender, when I've got that set up, if I go to color management under
[7:07] Output Properties, you will see now that I have the ASUS settings similar to Maya. I've set up a


### Blender Colour Space options setup [7:11]
**Transcript (timestamped):**
[7:13] principled shader with my textures already hooked up. Under Color Space, I've used the same options
[7:18] as earlier. Utility, sRGB Texture for my color data maps, and Utility Raw for scalar ones.
[7:25] One thing to mention here is that since there are so many presets in the ASUS config file,
[7:30] Blender can't actually fit them all onto the screen. So it's really annoying, but to see them all,
[7:35] for example, the Utility sRGB Texture option, which kind of comes towards the end, you need to zoom
[7:40] out so that they all fit onto the screen, then get your reading glasses on to find the correct
[7:44] setting in that wall of tiny text. When all my shader inputs are set up, I can jump over to my
[7:50] HGRI settings to choose the correct color space for that. Once again, you can see here, just like Maya,
[7:56] I've used the same Utility Linear sRGB option because we're using a linear EXR file. And that's
[8:02] the beauty of OCIO, a unified pipeline across different packages. Now, if I render, you will
[8:08] see it's all working and our colors look correct. You may notice the specular is slightly brighter
[8:13] in this render engine. I'm only using a spec roughness map with this object and not a specular color
[8:18] one to control the brightness of the spec. But to debug that I haven't set up something incorrectly,
[8:23] I can create another AOV to view the base color and make sure that all my maps are coming in as
[8:29] expected. Since we set up ASUS correctly and told the input textures how to be handled,
[8:34] the color is exactly the same as our Substance Viewport and the Arnold AOV that I set up earlier.
[8:39] So it's just a case of the shader specular model working slightly differently to the others.


### Outro [8:42]
**Transcript (timestamped):**
[8:44] Once again, this is one of the most important things about ASUS and OCIO for texture artists,
[8:49] the ability to have perfect parity with our colors between different 3D packages.
[8:54] So I think that's a perfect place to wrap this video up since we've got our ASUS CG Substance
[8:58] textures imported and rendering correctly in other packages. Just remember it's really important to
[9:04] correctly set up your color space settings on all of your maps. And that also finishes out this video
[9:11] series. I know it's been a lot of information but hopefully over the last three videos I've been
[9:15] able to help you understand what color spaces are, the needs and advantages of ASUS and how to
[9:21] implement it in your Substance Texturing Pipeline and beyond. I've been Michael Wilde, thank you so
[9:27] much for sticking with me and I'll see you around the internet. Cheers.



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
