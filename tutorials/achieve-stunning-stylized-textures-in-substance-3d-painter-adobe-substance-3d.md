---
title: Achieve Stunning Stylized Textures in Substance 3D Painter | Adobe Substance 3D
source: YouTube
url: https://www.youtube.com/watch?v=WYbp7SY-wEo
author: Adobe Substance 3D
ingested: 2026-08-13
app: "Substance 3D Painter"
version: "11.0.0"
tags: [layers, masks, generator, ambient-occlusion, curvature, procedural, basecolor, roughness, metallic, normal-map, iray-render, viewport, intermediate, advanced]
extraction_status: complete
frames_dir: tutorials/frames/achieve-stunning-stylized-textures-in-substance-3d-painter-adobe-substance-3d/
frame_count: 9
frame_status: complete
frame_selection: content-anchored (manual timestamps chosen from transcript, not blind percentages)
---

# Achieve Stunning Stylized Textures in Substance 3D Painter | Adobe Substance 3D

**Source:** [YouTube](https://www.youtube.com/watch?v=WYbp7SY-wEo)
**Author:** Adobe Substance 3D
**Duration:** 8m15s | 12 section(s)

---

## Raw Data (for Claude Code extraction)

## Ingest Safeguard Report (reviewed, resolved)

The flagged empty chapter ("Presets Showcase" [7:08]-[7:43]) is a genuine silent B-roll montage — the presenter narrates nothing while several stylization-preset examples play on screen. Resolved by capturing frames directly from that range: a 6-color-variant grid of a still-life tray (jug/cup/croissant) and a fantasy-costume hand/sword close-up credited "Art By Anastasia Kukosh" — the same artist-credit example seen in the companion "6 Powerful New Filters" video. No narrated information was lost; the chapter is visual-only by design.

---

Frames captured — see "Captured Frames" section below.


### Introduction [0:00]
**Transcript (timestamped):**
[0:00] Hello, I'm Stefan, Technical Artist at Adobe Substance 3D.
[0:04] In this video, I will showcase the new stylization filter inside Substance 3D Painter.
[0:09] This filter offers a simple solution to convert realistic models into stylized assets.
[0:15] The filter also comes with a range of custom presets that can be adjusted to your liking.
[0:20] Okay, let's jump into Painter to take a look at it.


### How to use Stylization [0:23]
**Transcript (timestamped):**
[0:24] Let's start by locating the filter in Painter's shelf.
[0:28] If you type stylization, you will find it in the filter category.
[0:32] You can drop it on a texture set via the viewport or from the layers tag.
[0:37] The filter needs a texture or at least a fill layer on the channels you want to process.
[0:42] If you want to apply the stylization effect to the entire scene, simply duplicate the layer across your texture set.
[0:59] To isolate the effect on the part of your 3D scene, you simply use a mask on the stylization layer.
[1:05] If you are getting slow feedback when tweaking the filter, decrease the resolution of the texture set.
[1:11] If you want the best result for stylization, I recommend baking the normal ambient occlusion
[1:16] and cover your maps through the baking menu.


### Overview [1:19]
**Transcript (timestamped):**
[1:19] Okay, let's start exploring the stylization filter.
[1:24] The default state of the filter will give you a natural base.
[1:27] The stylization parameter sets the overall intensity of the filter.
[1:32] The following parameters control the intensity of specific effects and are tied to the menus at the bottom.
[1:39] You can also browse a wide variety of presets to get different looks quickly.
[1:43] Let's take a quick overview at each of the specific effects and their settings.
[1:47] The brushstrokes parameter blends brushstrokes on the model surface.
[1:52] This parameter is tied to the brushstrokes menu that controls how patterns are splattered.
[1:57] And the brushstrokes effect tweaks the look.
[2:00] The smoothness parameter controls the overall style and smoothing of the filter and works with the smoothness menu.
[2:06] The color wise parameter lets you add color and grunge to the base color and is linked to the color wise menu.
[2:13] The gradient parameter lets you blend the gradient across the model and is also adjusted through the gradient menu.
[2:19] The bake lighting parameter lets you add lighting reflection on the model, but you can tweak further in the bake lighting menu.
[2:27] The edge and cavities parameter lets you reinforce the details and contouring of the model and more options are available in the edge and cavities menu.
[2:35] Finally, the helpers menu lets you display some specific masks related to the submenus.
[2:42] Now that you are starting to familiarize yourself with these effects, let's dive even further into each of the settings.


### Brush Strokes [2:48]
**Transcript (timestamped):**
[2:48] The brushstrokes amount sets the number of strokes splattered on the model.
[2:53] It's important to note that setting high values for this parameter will drastically slow down the filter.
[2:59] There are three strokes mode to choose from.
[3:01] The multiple strokes splatter different shapes on the model.
[3:05] The single strokes splatters the same shape over and over.
[3:09] You can also choose different brush patterns from the stroke select menu.
[3:13] The custom input mode lets you load your own shape to be splattered.
[3:18] You can find the image inputs at the bottom of the properties panel.
[3:22] You can further tweak it with the scale, rotation and so on.
[3:26] The strokes follow surface option will automatically orient the brushstrokes to follow the 3D surface of the model.
[3:33] Finally, the projection hardness and normal threshold parameters control all the stamps fade away across the 3D surface variations.


### Brush Stroke Effects [3:42]
**Transcript (timestamped):**
[3:42] Next, in the brushstrokes effect menu, you can control the appearance of the brushstrokes.
[3:47] Color variation blends brush patterns in the color, taking into account your base color.
[3:53] If you want to add a specific tint, you can toggle color custom and pick a color.
[3:58] You can repeat the operation for the roughness, metallic and normal.
[4:02] The normal custom displays options to fine tune the normal effect.
[4:06] And lastly, the normal random is helpful to get stronger brushstrokes effect on flat surfaces.


### Smoothness [4:16]
**Transcript (timestamped):**
[4:16] Moving on, the smoothness menu lets you smooth each material channel separately with an anisotropic couara effect.
[4:24] Lower values will result in a flatter look, and a higher values will result in a smooth look like an acrylic painting.
[4:32] This effect is particularly striking when applied to the base color or normal.


### Colorize [4:37]
**Transcript (timestamped):**
[4:39] The color rise menu lets you blend a uniform color on the base color.
[4:43] Remember to increase the color rise in the stop master parameters to see the effect.
[4:48] You can add some grunge variations by selecting a pattern in the drawdown menu.
[4:54] Then, play with the dedicated grunge parameter to fine tune the effect to your liking.
[5:03] The gradient menu lets you add a gradient on your model with one or two colors.


### Gradient [5:07]
**Transcript (timestamped):**
[5:08] You can choose the opacity and blending mode for each color.
[5:12] And you can adjust the position and contrast of the gradient at the bottom of the menu.
[5:25] To make the gradient easier to adjust, enable the gradient mask in helpers to better visualize the gradient places.
[5:31] Looking at the baked lighting parameter, you can add lighting reflection on the model.
[5:36] The brushstrokes and lighting parameter affects the lighting based on the brushstrokes,


### Baked Lighting [5:39]
**Transcript (timestamped):**
[5:41] allowing you to follow an anisotristic approach.
[5:44] You can control the intensity, color, radius and contrast of both the diffuse and specular reflection.
[5:50] And like the gradient setting, you can enable the baked lighting mask in helpers to better place the lighting effect.
[6:00] Lastly, the edges and cavities menu lets you intensify the details and contouring on the model.
[6:06] You can also adjust the color of the gradient, the color of the gradient,
[6:11] and the color of the gradient.


### Edges and Cavities [6:13]
**Transcript (timestamped):**
[6:14] Lastly, the edges and cavities menu lets you intensify the details and contouring on the model.
[6:19] You can amplify details in the texture with color sharpen or on the model surface with surface sharpen.
[6:32] To add contouring to the model, select edges, cavities or buff from the drop down menu.
[6:38] You can add a custom color to the contouring with the switch at the bottom.
[6:42] Play with the opacity, spread and contrast parameters to fine tune the mask extracted from the curvature map.
[6:49] To alter contouring with brushstrokes, you can use either the brushstrokes in edges or cavities.
[6:58] So that's all the specific effects of the stylization filter.
[7:02] But before ending this tutorial, I would like to showcase some of the presets applied on different models.


### Presets Showcase [7:08]

### Conclusion [7:43]
**Transcript (timestamped):**
[7:43] In this tutorial, you have learned how to use the new stylization filter in Substance 3D Painter.
[7:49] As a reminder, the stylization filter helps you convert your models into stylized hand-vainted assets.
[7:55] And all the assets can be exported and rendered in any standard game engine or renderer.
[8:00] Thanks for watching and stay tuned for more tutorial videos.
[8:12] Thank you for watching.



---

## Captured Frames

- [1:24] tutorials/frames/achieve-stunning-stylized-textures-in-substance-3d-painter-adobe-substance-3d/frame_000.jpg
- [2:53] tutorials/frames/achieve-stunning-stylized-textures-in-substance-3d-painter-adobe-substance-3d/frame_001.jpg
- [4:24] tutorials/frames/achieve-stunning-stylized-textures-in-substance-3d-painter-adobe-substance-3d/frame_002.jpg
- [4:48] tutorials/frames/achieve-stunning-stylized-textures-in-substance-3d-painter-adobe-substance-3d/frame_003.jpg
- [5:12] tutorials/frames/achieve-stunning-stylized-textures-in-substance-3d-painter-adobe-substance-3d/frame_004.jpg
- [5:44] tutorials/frames/achieve-stunning-stylized-textures-in-substance-3d-painter-adobe-substance-3d/frame_005.jpg
- [6:32] tutorials/frames/achieve-stunning-stylized-textures-in-substance-3d-painter-adobe-substance-3d/frame_006.jpg
- [7:15] tutorials/frames/achieve-stunning-stylized-textures-in-substance-3d-painter-adobe-substance-3d/frame_007.jpg
- [7:30] tutorials/frames/achieve-stunning-stylized-textures-in-substance-3d-painter-adobe-substance-3d/frame_008.jpg

---

## Structured Notes

### Core Technique
Dedicated deep-dive on the **Stylization filter**'s six effect sub-menus (Brush Strokes, Brush Strokes Effects, Smoothness, Colorize, Gradient, Baked Lighting, Edges and Cavities) that together convert a realistic PBR material into a hand-painted-looking stylized asset, demoed live on a still-life scene (moka pot, coffee cup, fig).

### Summary
Adobe technical artist Stefan walks through every setting of the **Stylization** filter first announced in the companion "6 Powerful New Filters" video. Applied by dragging it from the Shelf's Filter category onto a texture set (needs at least one fill layer/texture on the channels to be processed; duplicate across texture sets for a scene-wide effect, or mask the layer to isolate it to part of the scene — lower texture-set resolution first if filter feedback feels slow). Baking Normal/AO/Curvature maps first is recommended for the best stylization result. The top-level **Stylization** slider sets overall intensity; below it, seven collapsible menus each control one visual effect and share their name with a global intensity parameter: **Brush Strokes** (splatters shapes across the surface — Amount, three Strokes Modes [Multiple/Single/Custom Input], per-stroke Scale/Rotation/Hue Variation/Jitter, "follow surface" orientation, Projection Hardness and Normal Threshold fade-off); **Brush Stroke Effects** (Color Variation blending base color into strokes, optional Color/Roughness/Metallic/Normal custom tint overrides, Normal Random for stronger strokes on flat surfaces); **Smoothness** (per-channel anisotropic-Kuwahara-style smoothing — Color/Roughness-Metallic/Normal/Ambient-Occlusion Smoothness sliders — low values flatten, high values give an acrylic-painting look, most visible on Base Color/Normal); **Colorize** (blends a uniform Color Swatch onto Base Color, with a Grunge Variation pattern dropdown + Tiling for texture breakup); **Gradient** (Gradient Mode 1/2-color, Color, Color Opacity, Color Blending Mode e.g. Overlay, Horizontal/Vertical position, Gradient Contrast — a Gradient Mask helper visualizes placement); **Baked Lighting** (fake diffuse+specular light response baked into the texture — Diffuse/Specular Intensity, Color, Radius, Contrast, an anisotropic "Brush Strokes in Lighting" toggle, plus a helper mask); and **Edges and Cavities** (Color Sharpen / Surface Sharpen to intensify detail, a contour-source dropdown [Edges/Cavities/Buff] extracted from the curvature map, custom contour color, Opacity/Spread/Contrast, and brushstroke-driven contouring). A **Helpers** menu exposes each effect's isolated mask for placement tuning. The video closes with a silent B-roll of finished presets on different assets (a recolored still-life tray set, a fantasy-costume hand/sword close-up) and a reminder that stylized assets export and render normally in any standard game engine or renderer.

### Key Steps
1. Locate the filter: type "stylization" in the Shelf search (Filter category), then drag it onto a texture set — via the viewport or the Layers panel — to apply it. The filter needs at least a texture or fill layer present on the channels you want processed.
2. For a scene-wide effect, duplicate the Stylization layer across every texture set; to isolate it to part of the model, add a mask to the Stylization layer instead.
3. If filter feedback feels slow while tweaking, temporarily lower the texture set's resolution.
4. For the best stylization result, bake Normal, Ambient Occlusion, and Curvature mesh maps first via the Baking menu before applying the filter.
5. Set overall effect intensity with the top-level **Stylization** parameter; the default state gives a natural, lightly-stylized base. Browse the built-in **presets** dropdown for quick starting looks.
6. **Brush Strokes**: set the stroke **Amount** (high values slow the filter significantly); choose a **Strokes Mode** — Multiple Strokes (varied shapes), Single Strokes (repeats one shape), or Custom Input (load your own shape via the Image Inputs section at the bottom of the Properties panel); pick a pattern from **Strokes Select**; tune Scale/Rotation/Hue Variation/Position Jitter; enable **Strokes Follow Surface** to auto-orient strokes to the 3D surface; use **Projection Hardness** and **Normal Threshold** to control how stamps fade across surface-normal variation.
7. **Brush Stroke Effects**: **Color Variation** blends stroke patterns into the base color; toggle **Color Custom** to force a specific tint instead; repeat the same custom-override pattern for Roughness, Metallic, and Normal; **Normal Random** strengthens the brushstroke effect on otherwise-flat surfaces.
8. **Smoothness**: separate sliders smooth each material channel (Color, Roughness/Metallic, Normal, Ambient Occlusion) with an anisotropic-Kuwahara-style effect — low values read flatter, high values read like a smooth acrylic painting; most visually striking on Base Color or Normal.
9. **Colorize**: blend a uniform **Color** swatch onto Base Color (raise the Colorize intensity in the top-level parameters to see it); add texture via a **Grunge Variation** pattern dropdown, fine-tuned with its own grunge parameters.
10. **Gradient**: choose a 1- or 2-color **Gradient Mode**, set each color's **Opacity** and **Blending Mode** (e.g. Overlay), adjust **Horizontal Position**/**Vertical Rotation**/**Gradient Contrast**; enable the **Gradient Mask** under Helpers to visualize exactly where the gradient falls on the model.
11. **Baked Lighting**: fakes a light response baked directly into the texture — control **Diffuse** and **Specular** Intensity/Color/Radius/Contrast independently; the **Brush Strokes in Lighting** toggle applies an anisotropic look following the stroke direction; enable the Baked Lighting helper mask to place the effect precisely.
12. **Edges and Cavities**: amplify detail with **Color Sharpen** (texture-level) and **Surface Sharpen** (geometry-level); add contouring by selecting **Edges**, **Cavities**, or **Buff** from the dropdown (mask sourced from the curvature map); optionally recolor the contour with a custom-color switch; tune **Opacity**/**Spread**/**Contrast**; contouring can also be driven by the Brush Strokes system for a hand-drawn edge look.
13. Presets showcase (silent B-roll): several finished looks demonstrated on other assets — a still-life tray set recolored into 6 distinct palette variants, and a fantasy hand/sword close-up (art by Anastasia Kukosh).
14. Export: stylized assets built with this filter export and render normally through any standard game engine or renderer — the stylized look survives because it's baked into ordinary PBR texture maps, not a special shader.

### Layers / Tools / Settings
- **Stylization** filter (Shelf → Filter category), top-level Stylization intensity slider + presets dropdown
- **Brush Strokes**: Amount, Strokes Mode (Multiple/Single/Custom Input), Strokes Select, Scale, Rotation, Hue Variation, Position Jitter, Strokes Follow Surface, Projection Hardness, Normal Threshold, Image Inputs (custom stroke shape)
- **Brush Stroke Effects**: Color Variation, Color/Roughness/Metallic/Normal Custom overrides, Normal Random
- **Smoothness**: Color Smoothness, Roughness/Metallic Smoothness, Normal Smoothness, Ambient Occlusion Smoothness
- **Colorize**: Color swatch, Grunge Variation pattern + Tiling
- **Gradient**: Gradient Mode (1/2 Color), Color, Color Opacity, Color Blending Mode, Horizontal Position, Vertical Rotation, Gradient Contrast, Gradient Mask helper
- **Baked Lighting**: Brush Strokes in Lighting, Diffuse Intensity/Color/Radius/Contrast, Specular Intensity/Color/Radius/Contrast, Ambient Occlusion, Baked Lighting Mask helper
- **Edges and Cavities**: Color Sharpen, Surface Sharpen, contour source dropdown (Edges/Cavities/Buff), custom contour color, Opacity/Spread/Contrast
- **Helpers** menu (isolated mask preview per effect)
- Baking menu (Normal/Ambient Occlusion/Curvature recommended pre-bake)

### Difficulty
Intermediate to Advanced — applying the filter is a one-drag action, but the sheer number of interacting sliders across seven sub-menus requires real experimentation time to land a specific stylized look, as the presenter notes ("this filter has a lot of options... take your time").

### App & Version
**Substance 3D Painter 11.0.0** — this is the dedicated Stylization-filter deep-dive explicitly referenced by the companion "6 Powerful New Filters" video ("we have recorded a dedicated deep-dive tutorial on this specific filter"), which itself is the primary Adobe source confirming the "6 new filters" batch (including Stylization) as new in 11.0.0 per `references/release-notes-painter-11.0.md`. Same demo still-life scene (moka pot/coffee cup/fig) and same "Art By Anastasia Kukosh" B-roll credit appear in both videos, confirming they're a companion pair from the same production. Exact patch build not shown on screen.

### Tags
`layers` `masks` `generator` `ambient-occlusion` `curvature` `procedural` `basecolor` `roughness` `metallic` `normal-map` `iray-render` `viewport` `intermediate` `advanced`

---

## Related Tutorials
- **"6 Powerful New Filters in Substance 3D Painter"** (`tutorials/6-powerful-new-filters-in-substance-3d-painter-adobe-substance-3d.md`, video `aCi0RG9-9so`) — the companion feature-announcement video that introduces Stylization alongside five other new filters and explicitly defers deep coverage of Stylization to this video; shares the same demo still-life scene and the same "Art By Anastasia Kukosh" B-roll example.
