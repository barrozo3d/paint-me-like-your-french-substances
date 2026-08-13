---
title: Custom Fonts in Substance 3D Painter | Adobe Substance 3D
source: YouTube
url: https://www.youtube.com/watch?v=QSVgnyiDADc
author: Adobe Substance 3D
ingested: 2026-08-13
app: "Substance 3D Painter"
version: "10.0.0 (stated in narration: '10.0 and above'; also visible in the cache-usage readout 'Version: 10.0.0 (OpenCL)')"
tags: [layers, fill-layer, masks, alpha, texture-set, MatFX, procedural, beginner]
extraction_status: complete
frames_dir: tutorials/frames/custom-fonts-in-substance-3d-painter-adobe-substance-3d/
frame_count: 4
frame_status: complete
frame_selection: content-anchored (manual timestamps chosen from transcript, not blind percentages)
---

# Custom Fonts in Substance 3D Painter | Adobe Substance 3D

**Source:** [YouTube](https://www.youtube.com/watch?v=QSVgnyiDADc)
**Author:** Adobe Substance 3D
**Duration:** 3m30s | 7 section(s)

---

## Raw Data (for Claude Code extraction)

Frames captured — see "Captured Frames" section below.


### Introduction [0:00]
**Transcript (timestamped):**
[0:00] Hi there, and welcome to another brand new Substance 3D Painter release.
[0:06] This release is now available to you in Substance 3D Painter 10.0 and above.
[0:12] In this video, I'll be taking you through our brand new text resource feature.
[0:18] With this feature, you will now be able to create custom text easily and dynamically
[0:23] on your model.
[0:24] You will also be able to bring in your own custom fonts and effortlessly swap between
[0:29] them so it can perfectly match your vision.
[0:32] First, let's look at how to use our fonts.


### How use fonts [0:33]
**Transcript (timestamped):**
[0:35] As you can see, we have a brand new filter icon in the Assets panel.
[0:40] This is where you'll find your text resources.
[0:43] To use a font, click and drag it from the Assets panel onto either your model, the layers stack,
[0:50] or the channel slot of your choice.
[0:53] You can use it in any texture channel or as a mask.
[0:57] You can also adjust the projection settings of the text too.
[1:00] This works just the same as any other standard texture resource.


### Formatting the text [1:06]
**Transcript (timestamped):**
[1:06] You can change the styling and the content of your text resource in the Properties panel,
[1:10] just like when editing a material.
[1:14] Here, you can edit the text content, font size, alignment, and color.
[1:20] The Advanced section includes properties such as line and letter spacing, offset,
[1:26] background fill, and resolution.
[1:30] Setting the font size to auto will choose a font size so that the text fully fits inside
[1:34] the projected square image.
[1:37] This includes changing the line spacing and letter spacing, but not the offset.


### Using custom fonts [1:42]
**Transcript (timestamped):**
[1:42] If you want to try out new fonts, you can click and drag new ones into the resource box.
[1:49] The parameters you have set, like text content, font size, alignment,
[1:53] including the Advanced parameters, will not change, so you can easily swap out fonts without
[1:59] it affecting your actual text content, which really makes things a lot easier.


### Using text with other tools [2:05]
**Transcript (timestamped):**
[2:06] Text resources are ideal for image inputs of SPSAR materials,
[2:10] like the recently added Custom Spray Paint, Stickers, Stamps, Wood Carvings, Metal Engraving,
[2:18] and much more.
[2:20] All aspects of the text remain fully editable.
[2:24] Now, let's look at how we can import new fonts.


### Importing fonts [2:25]
**Transcript (timestamped):**
[2:29] All fonts installed on your operating system are automatically loaded into Painter.
[2:35] If you have additional libraries stored on your computer,
[2:38] you can add these locations in the Settings panel.
[2:42] To import a font, you can drag and drop the font files from your File Explorer to your Mesh,
[2:49] Layer Stack, or Assets panel.
[2:51] You can also manually import by going to File, then Import Resources.
[2:56] If the font has certain licensing restrictions, it will not be made available.
[3:02] You will see an error in the log the first time you try and import it,
[3:06] or if you're dragging and dropping it, you will see a red tooltip or a viewport message.
[3:11] Most fonts and characters are supported, including right-to-left script languages.
[3:16] If characters are not supported, they will display as a rectangle.


### Conclusion [3:21]
**Transcript (timestamped):**
[3:21] And that concludes our text resource tutorial for Substance 3D Painter.
[3:26] Thank you for watching.



---

## Captured Frames

- [0:40] tutorials/frames/custom-fonts-in-substance-3d-painter-adobe-substance-3d/frame_000.jpg
- [1:14] tutorials/frames/custom-fonts-in-substance-3d-painter-adobe-substance-3d/frame_001.jpg
- [1:45] tutorials/frames/custom-fonts-in-substance-3d-painter-adobe-substance-3d/frame_002.jpg
- [2:35] tutorials/frames/custom-fonts-in-substance-3d-painter-adobe-substance-3d/frame_003.jpg

---

## Structured Notes

### Core Technique
A new **Text resource** type (Painter 10.0+) that behaves exactly like any other image/grayscale resource — drag it onto the model, a layer, or a channel slot — but generates its pixel content dynamically from live-editable text properties (content, font, size, color, spacing) instead of a fixed bitmap, and can swap fonts non-destructively without losing any of those settings.

### Summary
Official Adobe feature-tour video (espresso-machine asset) introducing dynamic text resources. Text resources appear in a new dedicated **T (filter) icon** tab in the Assets panel alongside the usual resource categories. Dragging one onto a mesh, the layer stack, or any channel slot works identically to a normal texture resource — including using it as a mask. All text properties (content, font size, alignment, color, plus Advanced: line spacing, character spacing, horizontal/vertical offset, background fill/opacity, resolution) live-edit in the Properties panel exactly like editing a material parameter. Setting Font Size to **Auto** fits the text to the projected square image automatically (adjusting line/character spacing but not offset). Swapping fonts is fully non-destructive: dragging a new font onto the resource box changes only the typeface — text content, size, alignment, and all Advanced parameters are preserved. Text resources are called out as ideal grayscale/image inputs for SBSAR MatFX-style materials (Custom Spray Paint, Stickers, Stamps, Wood Carvings, Metal Engraving, and similar), remaining fully editable even after being fed into those materials. Font sourcing: every font already installed at the OS level auto-loads into Painter; additional font library folders can be added in the Settings panel; fonts can also be imported ad hoc by dragging font files onto the Mesh/Layer Stack/Assets panel, or via File > Import Resources. Fonts with licensing restrictions are silently blocked from import, surfaced via a log error (manual import) or a red tooltip/viewport message (drag-and-drop). Most fonts and character sets are supported, including right-to-left scripts; unsupported characters render as a rectangle placeholder.

### Key Steps
1. Open the Assets panel and select the new **T (text)** filter tab to browse installed Text resources.
2. Drag a text resource onto the model in the viewport, onto a layer in the Layer Stack, or directly onto a channel slot (works in any texture channel, or as a mask) — projection settings work the same as for any standard texture resource.
3. Select the resource and open the **Properties** panel to edit the text content, font size, alignment, and color, exactly like editing a material's parameters.
4. Expand **Advanced** for finer control: line spacing, character spacing, horizontal offset, vertical offset, background fill, background opacity, and resolution.
5. Set **Font Size** to **Auto** to have Painter automatically size the text (adjusting line/character spacing) to fully fit the projected square image — offset is not affected by Auto sizing.
6. To try different typefaces without losing work, drag a new font directly onto the existing text resource's box in the Assets panel/resource slot — content, size, alignment, and all Advanced parameters carry over unchanged.
7. Feed a text resource into MatFX-style SBSAR materials (Custom Spray Paint, Stickers, Stamps, Wood Carvings, Metal Engraving, etc.) as their grayscale/image input for dynamic, fully-editable stenciled text.
8. Fonts installed at the OS level are auto-detected; for additional font folders, add the library location under the **Settings** panel.
9. Import a specific font file by dragging it onto the Mesh, Layer Stack, or Assets panel, or via **File > Import Resources**.
10. If an imported font is license-restricted, Painter blocks it: check the log for the error (manual import) or watch for a red tooltip/viewport warning (drag-and-drop import).
11. Right-to-left scripts and most non-Latin character sets are supported; any unsupported glyph renders as a placeholder rectangle instead of failing the whole import.

### Layers / Tools / Settings
- **Assets panel > T (text) filter tab** — new resource category for Text resources
- **Properties panel** parameters on a Text resource: Text (content), Font size (numeric or Auto), Alignment, Color, and Advanced group (Line spacing, Character spacing, Horizontal offset, Vertical offset, Background fill, Background opacity, Resolution)
- Non-destructive **font-swap** workflow: drag new font onto the resource box, all other parameters persist
- **MatFX / SBSAR materials** compatible as text input: Custom Spray Paint, Stickers, Stamps, Wood Carvings, Metal Engraving
- **Settings panel** — add custom font library folder locations
- Import routes: drag-and-drop onto Mesh/Layer Stack/Assets, or **File > Import Resources**
- Licensing enforcement: blocked fonts surfaced via log error or red tooltip/viewport message

### Difficulty
Beginner (drag-and-drop resource workflow, no masking/generator chains involved).

### App & Version
Substance 3D Painter **10.0.0** — stated explicitly in narration ("available to you in Substance 3D Painter 10.0 and above") and confirmed on-screen via the cache-usage readout ("Version: 10.0.0 (OpenCL)").

### Tags
`layers`, `fill-layer`, `masks`, `alpha`, `texture-set`, `MatFX`, `procedural`, `beginner`

---

## Related Tutorials
- [Native Illustrator File Support in Substance 3D Painter](native-illustrator-file-support-in-substance-3d-painter.md) — same channel (Adobe), same short feature-tour format; a complementary new-resource-type addition (vector .ai import) from the same Painter version era.
- [3D Path Tool Updates in Substance 3D Painter](3d-path-tool-updates-in-substance-3d-painter.md) — same channel (Adobe), same short feature-tour format covering another 10.x-era Painter workflow addition.
- [6 Powerful New Filters in Substance 3D Painter](6-powerful-new-filters-in-substance-3d-painter.md) — same channel (Adobe); same "official new-feature tour" structure, different Painter version's headline additions.
