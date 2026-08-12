---
title: Tempering Colors in Substance Painter | Steel Heat Effects
source: YouTube
url: https://www.youtube.com/watch?v=Y3plK51emsA
author: Dolinskyi
ingested: 2026-08-12
app: "Substance 3D Painter"
version: "not specified (modern UI, post-8.3 baking-mode era; no version-pinning element visible)"
tags: [layers, fill-layer, masks, anchor-point, blend-mode, smart-material, procedural, alpha, roughness, basecolor, metal-rough, intermediate]
extraction_status: complete
frames_dir: tutorials/frames/tempering-colors-in-substance-painter-steel-heat-effects/
frame_count: 8
frame_status: complete
frame_selection: content-anchored (manual timestamps chosen from transcript, not blind percentages)
---

# Tempering Colors in Substance Painter | Steel Heat Effects

**Source:** [YouTube](https://www.youtube.com/watch?v=Y3plK51emsA)
**Author:** Dolinskyi
**Duration:** 6m42s | 1 section(s)

---

## Raw Data (for Claude Code extraction)

Frames captured — see "Captured Frames" section below.


### Full Content [0:00]
**Transcript (timestamped):**
[0:00] You have definitely seen this rainbow effect on metals and you probably know that it happens because the metal is exposed to high temperatures.
[0:08] Tempering colors appear when steel or other metals are heated. A thin oxide layer forms on the surface and depending on the temperature, it refracts light differently.
[0:18] That's why we see a gradient of colors, from light yellow to deep blue.
[0:22] Now let's try to recreate this effect in Substance Painter step by step.
[0:26] Let's recreate this effect from scratch. Add a fill layer and name it mask.
[0:34] Turn off all the channels. This layer will be used only for painting the mask. Add a paint effect and place an anchor point on top of it.
[0:44] Next, add a second fill layer that will reproduce the actual effect. You can name it, for example, color or something else.
[0:55] In the base color, add our mask. Right now, it's black.
[1:02] Let's paint a gradient by selecting paint on the previous layer. Try to make a smooth transition from black to white.
[1:12] You can use blur to make it even softer.
[1:15] In the color layer, add a gradient filter.
[1:34] According to this guide, we need to create 10 values. So set the number to 10 and pick the colors one by one.
[1:45] Then, add a fill layer.
[2:05] Done. Now we need to distribute these colors evenly along the gradient.
[2:09] Conceptually, divide our gradient into 10 parts where each tone represents a different metal color. Set their position sequentially.
[2:17] 0.1, 0.2 and so on. Make sure the first one is 0 and the last one is 1.
[2:24] Done. Now we can paint with this effect.
[2:54] You can also use a procedural texture instead of a paint layer. Just take any texture and add it through a fill into the mask layer. And you'll get this effect.
[3:25] Let's take a look at an example of using tempering colors on a suppressor. This time, I'll use my own smart material, which already has all the color variations set up, along with a few additional handy features.
[3:40] You can find the link to the material in the description below the video.
[3:45] Suppressors tend to overheat in specific areas during prolonged automatic fire, and under extreme stress, they can even get damaged or destroyed.
[3:53] So this is a great way to add some visual variety to your texture. Let's add the smart material to the scene.
[4:00] Enable custom mask, then turn on the fill layer inside the color mask. Now we can paint the mask in the layer below.
[4:30] Next, you just need to adjust the opacity to your liking or play around with the blending mode.
[4:46] Smart materials also include a blur function, so you can increase or decrease the blur to make the color transition smoother or sharper. You can also tweak the roughness. Just enable the roughness channel in the color layer and move the slider.
[5:07] Let's take a look at another example of using tempering colors.
[5:14] If we increase the contrast of a reference photo, we can notice a heat discoloration effect on the slider that remains after the manufacturing process.
[5:24] It's barely visible, but adding it can make your texture look much more realistic and interesting.
[5:30] Let's recreate this effect in Substance Painter. Add a smart material to the scene. By default, it will display the default patterns that can be switched using the grunge slider.
[5:42] I want to set it up as if we had one specific spot where the overheating started, which then gradually spread across the entire slider.
[6:12] It's more or less ready. You can still play around with opacity and blending modes. You can also add a paint layer and erase the pattern in areas where you don't want it to appear. That's it. We've briefly gone over the tempering colors effect, covered the theory and created it in practice. Thanks for watching.



---

## Captured Frames

- [0:34] tutorials/frames/tempering-colors-in-substance-painter-steel-heat-effects/frame_000.jpg
- [1:15] tutorials/frames/tempering-colors-in-substance-painter-steel-heat-effects/frame_001.jpg
- [1:45] tutorials/frames/tempering-colors-in-substance-painter-steel-heat-effects/frame_002.jpg
- [2:24] tutorials/frames/tempering-colors-in-substance-painter-steel-heat-effects/frame_003.jpg
- [3:40] tutorials/frames/tempering-colors-in-substance-painter-steel-heat-effects/frame_004.jpg
- [4:20] tutorials/frames/tempering-colors-in-substance-painter-steel-heat-effects/frame_005.jpg
- [5:50] tutorials/frames/tempering-colors-in-substance-painter-steel-heat-effects/frame_006.jpg
- [6:20] tutorials/frames/tempering-colors-in-substance-painter-steel-heat-effects/frame_007.jpg

---

## Structured Notes

### Core Technique
Building a reusable, mask-driven "tempering colors" (heat-discoloration/oxide-rainbow) effect from a 10-stop reference gradient, using a paintable anchor-point mask to drive a `Gradient Map`-style multi-color fill layer, then applying the same principle two more ways (a ready-made smart material, and a subtle reference-matched overheating spot on a slider part).

### Summary
Short, focused technique video (no chapters) that opens with the real-world physics (a thin oxide layer on heated steel refracts light differently at different temperatures, producing a yellow-to-blue color gradient) and then rebuilds that effect three times at increasing production-readiness: first from scratch with two stacked fill layers (a paintable mask layer + a gradient-filter color layer calibrated to 10 real tempering-color reference swatches with their Fahrenheit/Celsius values), then via a pre-built custom smart material with the same gradient logic baked in, applied to a suppressor to simulate localized barrel overheating, and finally a very subtle version applied to a firearm slider based on a real reference photo, tuned down in opacity so the discoloration reads as a faint manufacturing/heat artifact rather than an obvious rainbow.

### Key Steps
1. **Create the mask layer first:** add a `Fill Layer`, name it `mask`, and disable every channel on it — its only job is to hold a paintable grayscale mask, not to contribute any material properties itself.
2. **Add a `Paint` effect with an `Anchor Point`** on top of the mask layer so the painted grayscale data can be referenced by other layers downstream.
3. **Add a second `Fill Layer`** (named e.g. `color`) that will carry the actual visible tempering effect.
4. **Wire the anchor point into Base Color:** in the color layer's Base Color channel, add the mask (referenced via the anchor point) — starts fully black since nothing has been painted yet.
5. **Hand-paint a smooth black-to-white gradient** directly on the mask layer (select the paint tool on that layer), then apply `Blur` to soften the transition further — this grayscale ramp is what the color gradient will later be mapped across.
6. **Add a `Gradient` filter to the color layer's Base Color**, then build a 10-color gradient matching a real tempering-colors reference chart (350°F/176°C light straw through 730°F/388°C deep blue) — set the filter's color quantity to 10 and pick each swatch color by hand.
7. **Evenly distribute the 10 gradient stops:** treat the 0-1 gradient range as 10 equal divisions (0, 0.1, 0.2 ... 1.0) and set each color's position field to its corresponding value so the reference chart maps linearly across the painted mask.
8. **Paint with the finished effect:** because the gradient is now driven by the paintable mask, painting new grayscale values (or repainting the mask) directly controls where each tempering color appears — demonstrated live on the bracket-shaped test mesh.
9. **Alternative mask source — procedural texture:** instead of hand-painting the mask, feed any tileable/procedural grayscale texture into the mask layer via a `Fill` to get organic, non-hand-drawn tempering patterns automatically.
10. **Production example — smart material on a suppressor:** apply the creator's pre-built tempering-colors smart material (link in video description), enable its `Custom Mask`, turn on the mask layer's own paintable fill, and paint directly on the suppressor mesh to localize the heat-discoloration to where automatic fire would realistically overheat the metal.
11. **Tune the smart material's built-in controls:** adjust layer `Opacity` and `Blending Mode` to taste; the smart material also exposes a `Blur` slider (softens/sharpens the color transition) and a `Roughness` channel toggle so heat discoloration can also perturb roughness, not just color.
12. **Reference-matched subtle example — slider:** using a contrast-boosted reference photo showing a barely-visible heat-discoloration patch near the slide's ejection area, apply the smart material again, use its grunge-pattern slider to pick a pattern that reads as "one origin point that gradually spread," and finish by adding a `Paint Layer` to manually erase/break up the pattern in areas where it shouldn't appear — keeping the final result subtle rather than an obvious rainbow.

### Layers / Tools / Settings
- **From-scratch build:** `Fill Layer` "mask" (all channels off, holds only a paintable grayscale mask) -> `Paint` effect + `Anchor Point` -> second `Fill Layer` "color" with Base Color driven by the anchor-point mask
- **Filters:** `Gradient` filter (10-color-stop mode, each stop's position set manually 0.0-1.0) used to map the reference tempering-color chart onto the grayscale mask; `Blur` used both on the hand-painted mask and as a smart-material control for transition softness
- **Reference data used:** 10-step tempering-color chart with paired Fahrenheit/Celsius values (350°F/176°C through 730°F/388°C), visible on-screen as a captured diagram
- **Smart material controls (creator's own asset, link in description):** `Custom Mask` toggle, internal paintable fill layer, grunge-pattern slider (pattern selection), `Opacity`, `Blending Mode`, `Blur`, optional `Roughness` channel enable
- **Finishing tool:** `Paint Layer` used as a manual eraser/breakup pass over the smart material's automatic pattern on the slider example

### Difficulty
Beginner to Intermediate — the underlying layer/anchor-point/gradient-filter mechanics are simple and clearly explained step by step, but getting a physically-plausible result (correct color chart, believable localization, restrained opacity) requires some material-authoring judgment, especially in the final subtle-reference-matching example.

### App & Version
Not stated explicitly on screen. UI is the modern dark-theme layer-stack/fill-layer/gradient-filter layout with a `TEXTURE SET SETTINGS` tab and standard per-layer Properties panel — consistent with the post-8.3 Baking Mode era generally seen across this skill's other ingested tutorials, but nothing in-frame pins an exact version.

### Tags
layers, fill-layer, masks, anchor-point, blend-mode, smart-material, procedural, alpha, roughness, basecolor, metal-rough, intermediate

---

## Related Tutorials
- [Realistic Painted Metal in Substance Painter | M24 Grenade Texturing](realistic-painted-metal-in-substance-painter-m24-grenade-texturing.md) — same creator (Dolinskyi); part of the same multi-video M24 Grenade weapon-texturing project, and the anchor-point-driven paintable-mask + gradient-map technique taught here is directly reusable for the painted-metal wear/damage work shown there.
- See `tutorials/INDEX.md` for a possible sibling-ingested "Realistic Wood in Substance Painter | M24 Grenade Texturing" entry (same project, different material) — cross-link there too once/if present.
