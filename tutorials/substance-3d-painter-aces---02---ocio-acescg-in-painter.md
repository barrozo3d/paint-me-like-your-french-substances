---
title: Substance 3D Painter & ACES - 02 - OCIO & ACEScg in Painter
source: YouTube
url: https://www.youtube.com/watch?v=WrFqBNI6Tx4
author: Adobe Substance 3D
ingested: 2026-08-12
app: "[PENDING]"
version: "[PENDING]"
tags: []
extraction_status: pending
frames_dir: tutorials/frames/substance-3d-painter-aces---02---ocio-acescg-in-painter/
frame_count: 0
frame_status: pending-selection
---

# Substance 3D Painter & ACES - 02 - OCIO & ACEScg in Painter

**Source:** [YouTube](https://www.youtube.com/watch?v=WrFqBNI6Tx4)
**Author:** Adobe Substance 3D
**Duration:** 10m26s | 11 section(s)

---

## Raw Data (for Claude Code extraction)

Frames are not captured yet. Read the timestamped transcript below, pick moments
that actually show a technique/result worth a still (not blind percentages —
even within a named chapter, verify the real moment against its timestamps), then run:
  python select_frames.py substance-3d-painter-aces---02---ocio-acescg-in-painter <ts1> <ts2> ...
(seconds or mm:ss). This appends a "Captured Frames" section and updates the
frontmatter before you write the Structured Notes below.


### Part 2 [0:00]
**Transcript (timestamped):**
[0:00] Hello, and welcome back to this 3-part video series covering Substance Painter's implementation
[0:08] of the ASUS CG Colour Space with OCIO. Once again, I'm Michael Wilde, a Senior VFX artist,
[0:14] and if you haven't watched the primary in Part 1, where I covered the basics of Colour
[0:17] Space, I recommend giving that a watch first, as this video will assume you understand those
[0:21] terms. In late 2001, Substance Painter V7.4 added Open Colour I.O., which is how we are


### OCIO [0:22]
**Transcript (timestamped):**
[0:28] able to work with the ASUS CG Colour Space inside of Painter. Open Colour I.O., which
[0:33] I will be abbreviating to OCIO going forward, is an open source system that Substance and
[0:37] other VFX packages use for Colour Management. It requires an OCIO config file, which defines
[0:43] the colour universe which you'll be working in, basically defining your colour management
[0:47] options. ASUS CG is one such config. Because the same setup is used across different
[0:52] programmes, whether it's Substance for Texturing, Maya for Rendering, or Nuke for Compositing,
[0:57] it means unified pipeline from start to finish, and that every step of the way, artists see


### Setting up ACES with OCIO in Substance [1:01]
**Transcript (timestamped):**
[1:02] exactly the same thing. This is incredibly important in VFX.
[1:06] So how do we use OCIO in Substance? When you set up a project in Painter, there's
[1:11] this new option at the bottom called Colour Management. Opening that up presents you
[1:14] with a number of settings. If you select Open Colour I.O. as your colour management system,
[1:20] you will see we get a dropdown asking us which configuration we want to use. Substance, ASUS
[1:25] 1.0.3, ASUS 1.2, or Custom. As you can see, ASUS comes pre-installed with Painter, but
[1:33] if you want to use another system, you can select Custom and add your own OCIO config
[1:37] file. For this video, we'll be using the most up-to-date version of ASUS, ASUS 1.2.
[1:42] You will now see it create some default settings, including making our working colour space ASUS
[1:47] CG. A working colour space is the one in which the background calculations of our scene are
[1:51] worked out in. We're going to leave everything else as default, but before we move on, I
[1:55] want to touch on what these options mean. It may look a little bit complicated at first,
[1:59] but don't worry, let's use our knowledge from the last video to go through it all.
[2:03] To put it really simply, Substance is asking us, when I import or export text to data,
[2:08] how should I interpret that data? Think about it like this. If I have a sentence I want
[2:13] to translate in Google, I need to tell it what language I'm inputting. Knowing that,
[2:18] Google can then correctly interpret the words and turn them into binary in the background
[2:21] and do its calculations. Then, by telling it how I want it to be outputted, it can spit
[2:26] them out correctly in that language. It's all about the correct flow and conversion
[2:30] of data. Computers aren't the smartest after all, and neither are 3D packages. We need
[2:34] to tell it what realm the colour data we are inputting exists within, so that it can take


### OCIO Roles [2:38]
**Transcript (timestamped):**
[2:39] all that info and display it correctly. You may be looking at your settings and finding
[2:43] yourself a little confused by the terms like utility linear sRGB and utility sRGB texture.
[2:50] These are called roles, and they are defined by our OCIO config file. Roles are basically
[2:54] just shorthand for different types of colour space transforms to tell Substance how to
[2:59] interpret or transform the data so that it can do its background calculations correctly.
[3:05] If we go back to our Google translate metaphor, this is us telling Google which language we
[3:09] are inputting. These are all set by the colour space's config file, and thankfully, we only
[3:13] need to concern ourselves with 2 or 3, so don't feel too overwhelmed by this list.
[3:18] To correctly import references and images, Substance wants to know what colour gamut they
[3:22] have and if they have a linear or non-linear transfer function. 8-bit and 16-bit images
[3:27] that you use to texture with are often sRGB jpegs and tiffs from the internet. The utility
[3:32] sRGB texture role is what Substance needs to correctly interpret these sRGB imports
[3:38] with a 2.2 gamma curve. Whereas floating point images like 32-bit EXRs for displacement
[3:44] details or HDRIs to use as lighting environments still have the sRGB gamut but need to be treated
[3:50] as linear. The utility linear sRGB role is what Substance needs to correctly interpret
[3:55] those.
[3:58] For exporting, you will notice the default settings are the same, except with one exception


### Display Transform [4:01]
**Transcript (timestamped):**
[4:02] which we'll talk about later in this video. So, I've opened up this fantastic Dragon project
[4:07] created by the Substance team at Adobe. Now that we're using Asus in Substance, you will
[4:11] see a couple of new options at the top of your viewport. This is our viewport colour management.
[4:16] This is just a display transform that converts the working Asus CG colours to our display colour
[4:21] space, which here is sRGB like most computer monitors. We can click the little monitor button
[4:27] to turn it off and on, which as we see makes it all a bit darker as it removes the sRGB gamma curve.
[4:34] There are a lot of options there, so say for example you knew your display used the Rec 709
[4:38] colour space, you would choose that one instead. You may notice that if you change from viewing
[4:43] your material to just viewing a single channel that isn't your base colour, like spec roughness,
[4:48] this gets disabled automatically and you're unable to turn it back on. Why is that? Well,


### Colour & Scalar Data [4:50]
**Transcript (timestamped):**
[4:54] to answer that, I have to explain our final and quite fundamental colour space terms,
[4:58] colour data and scalar data. In texturing, there are two types of data we can paint,
[5:04] colour and scalar data. The easiest way to think about them is colour data is data which you see,
[5:10] whereas scalar data is calculated. Let me explain that in a little bit more detail.
[5:15] In texturing, you have a number of channels which contribute to the shader we add to our
[5:19] object. Those channels will either be seen directly on the mesh or used to drive some
[5:23] attribute of the shader. For example, when we paint our base colour channel, we are defining
[5:28] the colour of parts of the mesh, this is colour data. But our black and white spec roughness map
[5:33] that dictates how shiny or rough parts of our mesh are is never shown directly at render time,
[5:38] it's just calculators to drive the roughness attribute of the shader, this is scalar data.
[5:44] Colour vs Scalar Data, actually seen vs calculated. I'll put a list on screen of the
[5:50] common colour and scalar channels. In substance, you can tell if a channel is colour or scalar data
[5:57] by going to your texture set settings. If a channel has three little spheres, it's colour data.
[6:02] If not, it's scalar. You cannot change the default channels, but if you create your own custom
[6:07] channels, you're able to change them by clicking this button here. So why does colour vs scalar
[6:12] data matter for our viewport colour transform? Well, since our scalar data will never be seen at
[6:18] render time, it won't have a colour space applied to it. It's just purely value data to be calculated.
[6:24] Remember how we saw in part one that the sRGB gamma curve means it gives less space for lighter
[6:29] values? Well, rather than display our scalar data values with an sRGB transform scrunching up the
[6:34] data incorrectly, we want to display it linearly. So that's why the display transform is disabled on


### ACES when texturing [6:38]
**Transcript (timestamped):**
[6:40] scalar channels. So now we've got the project configured to work with ASUS, what do we need
[6:45] to know about actually texturing with ASUS? Well, regarding the actual texturing process,
[6:50] not that much really changes. You may notice that the viewport is slightly darker and more
[6:54] contrasted, but that's just the realities of ASUS CG vs sRGB. Substance will also apply a colour
[7:01] space to your colour picker when choosing colours for a colour data channel, but we'll remove it
[7:05] when picking colours for a scalar data channel, like the normal map, for example. The places we


### Importing colour spaces [7:06]
**Transcript (timestamped):**
[7:10] need to be careful are when we're importing textures to use to make sure they handle correctly and
[7:15] come into painter looking like they should. Well, the settings we chose will give 1816 bit resources,
[7:20] the 2.2 gamma curve, and floating point images will be interpreted linearly.
[7:25] But what if you're importing lots of different resources and one happens to be different from
[7:29] our project settings? Well, substance does allow you to change how you interpret resources,
[7:34] but only on a per use basis. When using a resource in a layer, say for example this fill layer that
[7:39] I've made here, I can click this drop down to see my colour space options. This allows me to make
[7:45] changes to the colour space of any resource used, but only in this one instance, not every time you've


### Importing HDRIs [7:50]
**Transcript (timestamped):**
[7:50] used it in your project. Similar to importing textures, let's quickly talk about HDRIs or a
[7:55] substance calls them environments. As another type of resource you can import, they also have colour
[8:00] space options. Often HDRIs you use for your substance environment are linear images within
[8:06] the sRGB colour gamut, but they are floating point images due to the nature of values going over one
[8:11] in an HDRI map. As we saw in our settings earlier, floating point images will be imported as linear
[8:18] sRGB images. If you need to make a change to the colour space options of your environment map,
[8:23] as it's not displaying correctly, simply click on this option box here and use the drop down to
[8:27] change it. This is useful if for example you are handed an HDRI which has already been converted to
[8:32] ASUS CG. I'll go ahead and bring in a custom linear HDRI image from HDRI Haven as a resource and use
[8:39] that to light my scene. As I already discussed, the texturing process is mostly the same once we


### Exporting colour spaces [8:43]
**Transcript (timestamped):**
[8:43] have our project set up for ASUS, but what about when we want to export our ASUS textures? Well,
[8:49] like imported resources, all of that is handled in the project settings. The only difference between
[8:54] our import and export settings is that floating point images get encoded in the ASUS colour space.
[9:00] This is the default settings as defined by the OCIO config file and since the floating point data
[9:05] we may be exporting, like our height data as a displacement map, is scalar anyway,
[9:10] exporting in the linear ASUS CG colour space is fine for us. We'll leave everything as it is
[9:15] because these defaults work for us, so why even mention it? Well, because as I hope I've over
[9:21] explained at this point, colour management is all about the correct handling of data along our
[9:25] pipeline. That means we need to know exactly how we're exporting everything so that when we get
[9:30] into different programs it can all be handled correctly, but more on that in the next video.


### Recap [9:33]
**Transcript (timestamped):**
[9:35] Before we finish up here, let's quickly recap the most important points we've covered. OCIO is an
[9:40] open source colour management system which allows different 3D packages to use a matching config
[9:45] file that defines the colour universe we work in. Substance Painters Project Configuration UI is
[9:51] where we set ASUS CG up and decide how to interpret different types of incoming and exported data.
[9:58] The display transform converts the working colour space ASUS CG into the colour space of our monitors.
[10:03] It is disabled for scalar data channels. Colour data is texture information which is seen on our
[10:09] shader. Scalar data is texture information which is used as a value to calculate a property of our
[10:15] shader. Great, so join me in part 3 and we'll take a look at using OCIO in Maya and Blender to
[10:21] render our textures exactly as we see them in Substance Painter. Cheers.



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
