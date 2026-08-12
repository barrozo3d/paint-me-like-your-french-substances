---
title: Substance 3D Painter & ACES - 03 - Textures in Maya and Blender | Adobe Substance 3D
source: YouTube
url: https://www.youtube.com/watch?v=Lksg6Fum3gw
author: Adobe Substance 3D
ingested: 2026-08-12
app: "Substance 3D Painter (export side) + Maya + Blender (import/render side)"
version: "Maya 2023 and Maya 2019 both demonstrated (built-in ACES vs. downloaded OCIO config); Blender version not stated on screen; Substance Painter build not shown (continuation of Part 2's project)"
tags: [color-management, export, export-preset, udim, basecolor, roughness]
extraction_status: complete
frames_dir: tutorials/frames/substance-3d-painter-aces---03---textures-in-maya-and-blender-adobe-substance-3d/
frame_count: 6
frame_status: complete
frame_selection: content-anchored (manual timestamps chosen from transcript, not blind percentages)
---

# Substance 3D Painter & ACES - 03 - Textures in Maya and Blender | Adobe Substance 3D

**Source:** [YouTube](https://www.youtube.com/watch?v=Lksg6Fum3gw)
**Author:** Adobe Substance 3D
**Duration:** 9m31s | 8 section(s)

---

## Raw Data (for Claude Code extraction)

Frames captured — see "Captured Frames" section below.


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

## Captured Frames

- [1:58] tutorials/frames/substance-3d-painter-aces---03---textures-in-maya-and-blender-adobe-substance-3d/frame_000.jpg
- [3:25] tutorials/frames/substance-3d-painter-aces---03---textures-in-maya-and-blender-adobe-substance-3d/frame_001.jpg
- [4:37] tutorials/frames/substance-3d-painter-aces---03---textures-in-maya-and-blender-adobe-substance-3d/frame_002.jpg
- [5:40] tutorials/frames/substance-3d-painter-aces---03---textures-in-maya-and-blender-adobe-substance-3d/frame_003.jpg
- [7:13] tutorials/frames/substance-3d-painter-aces---03---textures-in-maya-and-blender-adobe-substance-3d/frame_004.jpg
- [7:56] tutorials/frames/substance-3d-painter-aces---03---textures-in-maya-and-blender-adobe-substance-3d/frame_005.jpg

---

## Structured Notes

### Core Technique
Closing out the ACES/OCIO series by carrying Substance Painter's ACEScg-authored textures into Maya and Blender and getting each renderer's viewport to match the Substance Painter viewport — the pay-off of the color-managed pipeline set up in Parts 1-2.

### Summary
Part 3/3 of Michael Wilde's (ILM London) ACES series. Exports textures from Painter using a normal export preset (8/16-bit TIFFs, VFX-style naming — export mechanics not covered here, just color space). Sets up Maya's OCIO: Maya 2023 ships ACES built in (Color Management enabled, ACEScg render space, sRGB display, ACES view by default); Maya 2019 needs the ACES 1.2 OCIO config file downloaded manually and pointed to in Preferences → Color Management, which produces slightly different default role names. Builds an Arnold Standard Surface shader in Hypershade, wires a File node to Base Color, and sets that file's Color Space to Utility sRGB Texture (matching Painter's export role) — or "Display sRGB" if using Maya's inbuilt streamlined ACES setup — plus sets the file node's UV tiling method to UDIMs. Repeats for Spec Roughness but with Color Space set to Utility Raw (no conversion — scalar data must stay pure numeric). Sets up an Arnold Skydome light using the same HDRI as Painter's environment, with the HDRI file's Color Space set to Utility Linear sRGB (or "scene-linear Rec.709/sRGB" on the inbuilt setup) since it's a linear EXR. Confirms parity by comparing the Arnold render to the Substance viewport, and further isolates variables with an Arnold AOV that shows only the raw Base Color pass (bypassing shader/render-engine differences like Arnold's shadows) — confirms exact color match. Repeats the same setup in Blender: since Blender has no config-file import UI, points an OS-level `OCIO` environment variable at the ACES config (which will also override any other OCIO-reading program open at the same time, including Maya and Substance, and must be deleted to stop cross-contamination); once set, Blender's Output Properties → Color Management shows the same ACES options as Maya. Wires up a Principled BSDF with Utility sRGB Texture for color-data maps and Utility Raw for scalar maps (warns that Blender's OCIO preset dropdown is so long you must zoom the UI out to find "Utility sRGB Texture" near the bottom of the list), sets the HDRI to Utility Linear sRGB, renders, and again confirms with an AOV that the base color matches — noting a slightly brighter specular highlight is just Blender's spec-shading-model difference, not a color-space setup error, once base color is isolated and confirmed correct.

### Key Steps
1. Export textures from Substance Painter using a normal export preset (color-space handling was already configured in Part 2's project settings; export mechanics themselves aren't re-covered).
2. In Maya 2023+: Preferences → Color Management is ACES-enabled by default (ACEScg rendering space, sRGB display, ACES view) — no extra setup needed.
3. In older Maya (e.g. 2019): download the free ACES OCIO config (~2GB) from the official ACES site, then in Preferences → Color Management set the Config Path to the downloaded ACES 1.2 config file; this produces a display=ACES + separate sRGB view-transform-on-top default instead of Maya 2023's more direct default.
4. Set up color management at the very start of a project — changing it mid-project means re-telling Maya how to interpret every already-imported file.
5. Build a shader: open Hypershade, create an Arnold Standard Surface (aiStandardSurface), add a File node, connect it to Base Color.
6. On the Base Color File node, set Color Space to **Utility sRGB Texture** (matches how Painter exported it) — or **Display sRGB** if using Maya 2023's inbuilt streamlined ACES config (fewer, renamed options).
7. Set the File node's UV tiling mode to **UDIM** so multi-tile texture files resolve correctly.
8. Add a second File node for Spec Roughness; set its Color Space to **Utility Raw** — no color conversion, because scalar data (Roughness) must be read as pure numeric values, not color.
9. Add an Arnold Skydome light, connect the same HDRI/environment used in Painter to its Color input via a File node; set that file's Color Space to **Utility Linear sRGB** (or "scene-linear Rec.709/sRGB" under Maya's inbuilt setup) because the HDRI is a linear EXR, not an sRGB-gamma texture.
10. Rotate the HDRI to match Painter's environment angle, render, and visually compare the Arnold render view to the Substance Painter viewport.
11. For a rigorous check that bypasses shader/render-engine differences (e.g. Arnold's shadow calculation), add an Arnold AOV that isolates just the raw Base Color pass and compare that directly against Painter's Base Color channel view.
12. In Blender: since there's no in-app OCIO config-file picker, create an OS-level environment variable named `OCIO` pointing at the ACES config file path; Blender picks it up automatically on next launch. Note this env var globally overrides any other OCIO-reading program (Maya, Substance) opened afterward if they use their own inbuilt setup — delete the variable before opening those to avoid conflicts.
13. In Blender, check Output Properties → Color Management — it now shows ACES settings matching Maya's.
14. Build a Principled BSDF shader, wire up textures; set Color Space to **Utility sRGB Texture** for color-data maps (Base Color) and **Utility Raw** for scalar maps (Roughness) — same role names as Maya's downloaded-config path.
15. Blender-specific gotcha: the ACES config's color-space dropdown list is too long to fit on screen at default UI scale — zoom the interface out to find options like "Utility sRGB Texture" near the bottom of the list.
16. Set the HDRI's Color Space to **Utility Linear sRGB** (same reasoning as Maya), render, and verify with another AOV isolating Base Color that the result matches both Maya's and Painter's.
17. If specular brightness looks slightly different from other renderers once base color is confirmed identical, that's a shading-model/spec-calculation difference between engines, not a color-space misconfiguration — don't chase it as a bug.

### Layers / Tools / Settings
**Maya:** Preferences → Color Management (Rendering Space = ACEScg, Display = sRGB, View = ACES); Hypershade Arnold Standard Surface shader; File node Color Space dropdown (`Utility sRGB Texture` for color data / `Utility Raw` for scalar data / `Utility Linear sRGB` for linear EXR HDRIs; renamed to `Display sRGB` / `scene-linear Rec.709/sRGB` under Maya 2023's inbuilt condensed ACES config); File node UV Tiling Mode = UDIM; Arnold Skydome light; Arnold AOV for isolated Base Color comparison.
**Blender:** OS-level `OCIO` environment variable pointing at the ACES config; Output Properties → Color Management panel; Principled BSDF shader; per-texture-node Color Space dropdown (same `Utility sRGB Texture` / `Utility Raw` / `Utility Linear sRGB` roles as Maya's downloaded-config path); AOV for isolated Base Color comparison.
**Substance Painter side:** standard export preset (8/16-bit TIFF, VFX-style naming) — color-space correctness inherited from Part 2's project Color Management settings, not reconfigured here.

### Difficulty
Intermediate/Advanced (requires comfort with Maya Hypershade and Blender's Shader Editor in addition to Painter's export settings).

### App & Version
Substance 3D Painter (export side, build not shown — continuation of Part 2's project). Maya 2023 (inbuilt ACES) and Maya 2019 (manual ACES 1.2 OCIO config) both demonstrated side by side. Blender version not stated on screen. Renderer: Arnold (Maya side).

### Tags
`color-management`, `export`, `export-preset`, `udim`, `basecolor`, `roughness`

---

## Related Tutorials
- **Substance 3D Painter & ACES - 01 - Color Space Fundamentals** (`tutorials/substance-3d-painter-aces---01---color-space-fundamentals-adobe-substance-3d.md`) — Part 1/3, the color-theory foundation (color space, gamut, gamma/transfer function, ACES/ACEScg) this video assumes.
- **Substance 3D Painter & ACES - 02 - OCIO & ACEScg in Painter** (`tutorials/substance-3d-painter-aces---02---ocio-acescg-in-painter.md`) — Part 2/3, where the Painter-side project Color Management, OCIO roles (Utility sRGB Texture / Utility Linear sRGB / Utility Raw), and Color-vs-Scalar Data distinction used throughout this video are originally set up and explained.
