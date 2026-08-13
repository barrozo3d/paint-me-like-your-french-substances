---
title: How to texture a realistic slipper model
source: YouTube
url: https://www.youtube.com/watch?v=U5CZJAKU47s
author: 3DRedBox
ingested: 2026-08-12
app: "Substance 3D Painter"
version: "not stated on screen, but the stroke/stitching panel is explicitly titled 'PAINT ALONG PATH' (confirmed in captured frames) — per references/version-tracker.md this tool was named Paint along Path only from 9.0.0 until it was renamed Filled Path in 11.0.0 (then Ribbon in 11.1.0), which pins this video to the Painter 9.x-10.x window"
tags: [layers, fill-layer, paint-layer, masks, smart-material, generator, curvature, anchor-point, blend-mode, ambient-occlusion, mesh-maps, baking, texture-set, uv, pbr, metal-rough, basecolor, roughness, metallic, height, normal-map, alpha, procedural, export-preset, advanced]
extraction_status: complete
frames_dir: tutorials/frames/how-to-texture-a-realistic-slipper-model/
frame_count: 9
frame_status: complete
frame_selection: content-anchored (manual timestamps chosen from transcript, not blind percentages)
---

# How to texture a realistic slipper model

**Source:** [YouTube](https://www.youtube.com/watch?v=U5CZJAKU47s)
**Author:** 3DRedBox
**Duration:** 22m17s | 1 section(s)

---

## Raw Data (for Claude Code extraction)

Frames captured — see "Captured Frames" section below.


### Full Content [0:00]
**Transcript (timestamped):**
[0:00] Hello guys, my name is Meti from T-Dreadbox Channel and today we are going to talk about
[0:14] how to texture this slipper inside the Substance Painter and create all the details directly
[0:19] inside the Painter. So let's start the process but before that let me introduce you the brand
[0:24] new course that we released for Substance Painter. Learning Substance Painter is easier than ever.
[0:30] Hey all Substance lovers, tech change seekers and awesome future artists, welcome to ultimate
[0:36] course for learning Substance Painter from zero to hero. Ready to learn how to texture with different
[0:48] projects? Substance Master released a brand new course for those who want to learn to texture
[0:55] with Substance Painter. In this course we cover from preparing the model to rendering different
[1:01] project, different challenges. If you want to level up your skill in texturing come and check
[1:06] the Substance Master ultimate course for learning Substance Painter. Okay let's start the process
[1:11] but before jumping to the Painter I want to explain this. We have this model and we want to work on
[1:17] this but because we have the back face or the bottom part and we need to work on this and we
[1:23] couldn't turn the geometry inside the Painter directly we need to export this model for the
[1:29] baking process and the rendering phase but for the texturing process we should add another variation
[1:36] from this model with duplicating and rotating the model and making upside down to have access or
[1:43] we should say the better access to the bottom part. Okay so we have two effects one for baking and
[1:50] the rendering and the other one with two different variations with different rotation for the texturing
[1:56] process. Okay so let's jump back to the Painter. Okay let's start the process and I just want to
[2:02] have the model inside the Painter so we can just drag and drop it to the viewport. In the new project
[2:07] window we set everything that we need for example document resolution to 2k and the normal map format
[2:14] should be on dial x for the template we stick to the pbr metallic roughness and the rest of the
[2:19] option should be default one. Okay so let's press okay we just import the model into the Painter
[2:25] let's go to the baking mesh maps window and in here let's choose the output size 4k change the
[2:31] anti-aliasing to 64x and the rest of the option is good for us and we just need to click on the
[2:38] bake selected textures and wait for the process going to done. Okay and now the baking process is done
[2:44] and we can change the model inside the Painter so I just import the second fix with the two variation
[2:51] model position and just press okay and as you can see we have the other variation and we can work
[2:57] on this part very easy so let's go for the texturing process. Okay so let's create two
[3:02] folder for the first step and let's rename that into plastic and fabric and I'm going to create
[3:09] mask for each folder okay let's add paint go to the mask view mode select everything here with
[3:15] the polygon field mode and right now I'm going to deselect this area the inner part and this section
[3:21] okay so the white area should be the plastic surface and the black should be the fabric okay
[3:27] so I'm going to add the anchor point here at the field load this anchor point and just invert it so
[3:33] I create a dynamic mask here and I can control it anytime that's what okay so for the plastic part
[3:40] I'm going to use the plastic smart material collection from our store that you can find a link
[3:46] of this product inside the description and having the smart material library can increase your speed
[3:51] and quality during the texturing with a little modification to fit your project okay and I want
[3:57] to add some smart material to the folder to check which one is better for us okay let's turn off
[4:04] all these folders this one is good but let's check the others no I don't like this it could be good
[4:11] for this slipper we can keep that but uh yeah I really like this material okay so this one is good
[4:18] too but yeah I prefer to use this one okay so let's delete all of them okay that's great let's
[4:23] and modify the material for this project so basically I'm going to turn off all the layers
[4:28] we have the base color that's gray we can create the second color and make it white or maybe like
[4:35] gray this and add a black mask okay and add the paint and we go here and just paint the area that we
[4:42] want to add the white okay so I'm going to create two different color for the base okay but we can
[4:47] keep this off for now and we have color variation number one it's good but we can turn down opacity
[4:55] a little we have the second color variation and we can make it lighter okay that's great we don't
[5:01] want to have something like old and dirty and rusty plastic here we just want to have some
[5:06] variation on the surface okay so we have surface noise it's good kind of yeah as you can see it's
[5:13] great and we have another surface noise which is kind of good yeah and we have the dirt variation
[5:20] let's bring down the opacity yeah and we have the edge damage we can delete this one because we
[5:26] don't want it here actually and for the dirt variation number two you're in a good position yeah
[5:31] I think this is good okay maybe we can go to the mask and just decrease the opacity for the mask okay
[5:38] and we have the roughness okay that's great and as you can see we have a lot of surface variation
[5:44] here let's go and make a rough surface here yeah and now we can see the difference in the roughness
[5:51] maybe we can bring up the value of the base color or base layer okay that's great that's fine
[5:57] can make it rough and we have the scratch okay so the scratch is good I think we should keep that
[6:03] and for the triple s we can remove this and I want to add another fill layer and let's call it edge
[6:10] roughness okay for the edge roughness I want to add a black mask add a generator go here and choose
[6:16] the curvature okay that's great and in the white area I want to have more reflective value yeah
[6:24] that's great in this way we can have better visual at the end because we have the highlight on the
[6:29] edge and it could add more interesting point to the render okay so that's it and we just need to
[6:36] paint for the second color okay let's go here and we can just paint here let's change the alignment
[6:43] to the UV and size to the texture okay right now I'm going to paint the area that I want and need
[6:49] for the white and after painting this area I'm going back and continue the process okay now the
[6:55] masking phase is done and as you can see we have this style for the plastic part and we are going
[7:01] to work on that in the next steps but right now that's enough okay so let's go back to the fabric
[7:07] okay and I want to create the fabric in here let's create two different fill layer first let's
[7:14] create the material for the top pieces okay and I'm going to use the fabric wool which is a default
[7:21] material from the library okay that's great let's add a black mask add a paint go to the polygon
[7:27] field choose this part as a top piece and let's increase the size into three yeah and I'm going
[7:33] to rotate I think 110 is great okay that's for the top piece and let's go for the inside pieces
[7:42] and for inside pieces let's add anchor point go here add a mask use a field choose this mask and
[7:49] use the invert option okay and let's go to the material mold and search a file with fill okay
[7:54] and as you can see we have this material for inside part and let's increase the size into four yeah
[8:00] I think it's good and for the color let's pick a little dark gray this one okay and we can play
[8:06] with this parameter to achieve the result that we're looking for for example I need to have more
[8:12] fiber density like this and yeah that's perfect okay and we are done for the fabric face and let's
[8:18] add the details that we need for this sleeper okay now let's add the first layer stitches number one
[8:24] and let's use the pass tool and the top stitching let's create the pass that we want okay so I'm going
[8:31] to create pass here like this okay that's great we create the path and let's go to the stitches type
[8:38] I'm going to choose slat and pin stitches like this but we need to invert the path and change the size
[8:45] from five to three okay and we need to refine the location the path like this okay we are done with
[8:52] the first pass and we need to set a mask because sometimes we have leaking data from this pass to
[8:59] this area so let's add the black mask add the paint go to the polygon field choose this section and
[9:05] yeah it's good okay and after that we need to work on this side too so I just select this section
[9:11] for the stitches one and let's create another path okay it's great but we need to change some setting
[9:17] here for example change size to two go to the stitches type and choose straight stitches okay and
[9:24] go to the stitching parameter and change the size of the stitches from one to zero point seven and
[9:31] for puckering let's change the type from thick fabric to the leather okay that's great and we can play
[9:38] with the intensity to achieve more realistic result and I'm going to duplicate this stitch
[9:43] in this side too okay that's fine and we have these stitches and right now we can create another
[9:50] paint layer and name it stitches number two add the black mask and add the paint and let's select
[9:56] this area okay so I'm going to create stitches for this section that's great so let's pause the video
[10:02] and do all the repetitive stuff and after that we come back and continue the process okay now we are
[10:08] done with these details and now we can add the effect paint layer here change the blending mode
[10:14] to pass through and apply to all channel and right now we can add different filter here for example
[10:21] let's bring the sharpen okay and keep it as the zero point five value okay that's great now we have
[10:27] so much detail in the surface okay let's duplicate it and change it to contrast and we can increase
[10:34] the contrast the color for example and let's add another filter fight to normal okay and turn off
[10:39] the use word unit and we can control the normal intensity here with this slider I think tree is
[10:46] good and it's enough okay and I think that's enough and we can go back to the detail creation and
[10:53] add some detail in here in here and for this part okay now let's create a fill layer and I'm going to
[11:01] call this l1 detail and let's add a black mask go to the fill layer keep just height and give a
[11:07] negative zero point one for the height and I want to add some small detail here like lines and a text
[11:14] over here and maybe update the color depending on the detail that we work here and at the end
[11:20] some detail in here okay so let's add a fill layer okay and in here let's search about the gradient
[11:27] linear number two okay that's great let's change the uv up to none and let's go to the 2d mode okay
[11:33] and right now I'm going to increase the scale and put it here okay we can change the rotation and
[11:39] make it as a line this and let's add filter like blur okay that's great so we have this kind of detail
[11:46] here and let's keep this detail like this and I'm going to freeze it here and let's make it smaller
[11:52] okay let's change the blending mode to linear dodge and duplicate it okay so tree line here
[11:59] and let's increase the length these lines okay that's great and I'm going to duplicate these
[12:05] details to the other side okay this one okay that's great so we add the detail we want very easy
[12:12] and fast yeah that's great okay let's add the other details like text in here okay let's add another
[12:18] fill layer l2 details keep height put it as negative point two okay add the black mask and right now
[12:26] I'm going to search about the comic songs bold okay let's type 3d wordpipes okay change the uv up to
[12:33] none make it small bring it down yeah put it here it's great you can choose the character spacing
[12:39] with the higher amount okay that's great so maybe we can decrease it yeah I think this number is great
[12:46] and let's change the blending mode to linear I'm going to duplicate it and let's keep r okay and put
[12:52] this r here and mirror this text like this okay let's duplicate this fill layer okay and search
[12:59] about the square inside the asset library and put the square board at coordinate cut and let's decrease
[13:05] the square scale like this value okay I think it's good it's fixed the position may change the size
[13:11] okay so we have this detail here and for this text I'm going to use the band half rounded okay so
[13:18] let's go to the mask oh this this hey that's great we have the borderline and right now we can change
[13:25] the blending mode of the text to subtract and as you can see we can control it with the opacity okay
[13:31] that's great yeah we have this detail okay that's fine and I think this is enough for the l2 detail
[13:38] and we need to jump the l3 for this section okay so let's create l3 detail add a black mask and choose
[13:45] this section okay and right now we need to go back to the layer turn off all the layers except the
[13:51] height change the height value to negative 0.1 okay for the l3 or the bottom part I'm going to
[13:58] create some help layer in the help layer which is a paint layer without any data and we just create
[14:05] the part of the mask on that layer and use the anchor point and load it into l3 detail okay so
[14:12] let's call it l3 placeholder mask number one okay and change the color to red and just add the black
[14:19] mask okay so I'm going to add a field okay put it as white change the uv up to none okay and
[14:26] create this line this and I want to create some region for adding the street pattern okay so let's
[14:33] add another one I'm going to change all the blending mode to clean dodge okay you have this one too
[14:38] let's duplicate it we have another one like this okay let's call this one as the strip region number
[14:45] one and whenever we want we can load this and invert this to have access to other part okay that's
[14:51] great so I'm going to create another placeholder mask in here let's call it number two change the
[14:58] color to red add a black mask add a field load the strip region number one and just invert it okay
[15:04] but right now when we invert this mask we select all the other uv island okay so we need to modify
[15:12] this just add a paint change the blending mode to subtract choose all the area press x on the
[15:18] keyboard and deselect this part okay so in this way we just invert the area that we want okay so
[15:24] this is the first mask this is the second mask and let's add another field layer and load strips okay
[15:31] and change the blending mode to multiply and change tiling to 15 that's great and let's add a rotation
[15:39] like 120 okay and in the pattern area we can increase the strip we can change the length or
[15:46] weed can play with the softness and play with the shift okay so this one is great for me right now
[15:52] okay and I'm going to duplicate this this in here okay and let's change the rotation to something like
[15:59] 116 that's great okay let's add the anchor point for placeholder mask two and rename it to
[16:06] s3 2 and in here let's add another one let's call it strip one and in the l3 we can add
[16:14] three layer and load strip one and strip two okay and change the blending mode from normal to linear
[16:21] okay we need to reset the mask for the l3 detail add a paint choose this one add the field choose
[16:26] strip number two okay duplicate the fill layer okay and now as you can see we have the detail
[16:32] that we want but we need to control it so first of all we need to create the border okay so the
[16:37] border and the line in here is very important so we can create this kind of detail with the paint
[16:44] or we can just use the pass and now I need to add a paint and choose the pass and create the
[16:51] detail with the pastel okay so let's bring down the spacing okay and now I'm going to create a paint
[16:57] here that's fine let's decrease the size to something like three I think it's good and we can add the
[17:03] border okay like this okay that's fine so I just create the divider detail and we can decrease the
[17:10] size and make it smaller okay I think this one is much better and we need to create the border so
[17:16] for creating border I'm going to create another place holder okay and add a black mask so let's
[17:22] add a paint go to the mask choose the UV Chong just like this one and let's add a filter and I'm
[17:28] going to use the bevel okay so we are going to choose a pure white area and I want to add another
[17:35] filter and let's call the histogram scan okay let's bring up the contrast and play the position
[17:41] and I think this one is great let's add another filter and going to recall blur okay that's great
[17:48] so this is the area that we want to have the details on that so let's go to the L tree and add feel
[17:55] recall the original region invert it and just the blending mode to subtract okay so we just remove
[18:01] everything that we don't want okay that's great and we can control it with the bevel and the
[18:06] histogram scan right okay that's great and we need to have the border cut right so let's go back to
[18:12] the place holder mask tree and after the original I'm going to add another filter and let's recall
[18:19] the mask outline okay so for the mask outline we have these options for example let's have this one
[18:25] okay and I'm going to add another anchor point let's call a border cut okay and we need to add
[18:32] another fill layer choose the border cut and change the blending mode to linear dodge okay and play with
[18:37] the level in here okay so we have this effect this and let's go to the mask outline and we can change
[18:44] the position this cut let's call the region okay and yeah we have what we want right and we can add
[18:50] a filter like Blair okay and put it to this value and as you can see we have all the details that we
[18:57] want but we need to remove this area so let's add a paint layer change the blending mode to
[19:03] subtract okay and let's paint and remove this area because we want to have some label text and
[19:09] shoe data in here okay so we just create the detail that we want and that's it and right now I want to
[19:14] add a fill and load a shape capsule in the fill layer change the uvrap to none come back here to
[19:21] the 2d view change the size okay and change a little bit blending mode to linear dodge okay so we have
[19:27] this one in here let's bring up the hardness okay as you can see we have the space for adding the
[19:33] detail let's add fill layer or we can just duplicate the shape capsule rename it to size and just load
[19:39] the comic son maybe 41 42 okay that's great so let's decrease the size and I'm going to change the
[19:47] blending mode from these text to subtract that's great okay that's fine so we have the detail that
[19:53] we want here but it's wrong so we need to mirror it like this okay that's great and we need to go back
[20:00] to the plastic in here in the second color and just update the mask that we create before okay so
[20:06] let's go to the mask and choose the paint and let's go to the polygon fill select this section
[20:12] this one as you can see and let's add another paint change the blending mode to subtract go to the
[20:17] paint and for this one I just need to have the 3d art box text as a white value so we can just
[20:24] remove anything else here okay that's great and let's go this section because we have the white
[20:30] value here I want to have the white in the bottom part but we need to subtract some area like this
[20:37] so let's have a more interesting point here so let's keep this section as a second color okay now
[20:43] we are done as you can see we just create the color mask for the bottom part that's fine and yeah for
[20:49] the last step we need to add the AO and ambient occlusion to the material so let's create it in
[20:56] old way so I'm going to create paint layer let's call it edge collection or edge plus change the
[21:02] blending mode to pass through and apply to all channel add an anchor point create a fill layer
[21:07] let's call it AO and keep just AO make it black and just add the black mask add the generator choose
[21:13] the ambient occlusion generator and choose the macro detail okay and let's go and choose the edge
[21:19] plus and change the reference channel to height that's great and I'm going to load the edge plus
[21:25] and change the reference channel to the normal for the normal section okay and right now I can play
[21:31] with the AO radius and just press on the google bar it's great and if you don't want to have the AO
[21:38] for this fabric part you can just place the edge plus before the fabric okay like this yeah okay
[21:43] that's great maybe in the l2 detail I just turn off this deep because it's not great so we can turn
[21:50] it off and yeah that's great so this is the end of the tutorial I hope you learned something new
[21:55] and if it's so please hit the like button don't forget to share your mind in the comment section
[22:01] and if you want to have access to the project file you can go to the patreon page and just access to
[22:07] the project file of this model and the substance painter file okay be creative be safe buy and
[22:13] don't forget to read the description because all the information is over there



---

## Captured Frames

- [3:15] tutorials/frames/how-to-texture-a-realistic-slipper-model/frame_000.jpg
- [6:16] tutorials/frames/how-to-texture-a-realistic-slipper-model/frame_001.jpg
- [7:33] tutorials/frames/how-to-texture-a-realistic-slipper-model/frame_002.jpg
- [8:31] tutorials/frames/how-to-texture-a-realistic-slipper-model/frame_003.jpg
- [9:17] tutorials/frames/how-to-texture-a-realistic-slipper-model/frame_004.jpg
- [11:07] tutorials/frames/how-to-texture-a-realistic-slipper-model/frame_005.jpg
- [15:31] tutorials/frames/how-to-texture-a-realistic-slipper-model/frame_006.jpg
- [17:22] tutorials/frames/how-to-texture-a-realistic-slipper-model/frame_007.jpg
- [21:07] tutorials/frames/how-to-texture-a-realistic-slipper-model/frame_008.jpg

---

## Structured Notes

### Core Technique
Full slipper texturing (plastic sole + herringbone fabric upper) built entirely inside Painter, with all fine detail — stitching, sole tread pattern, embossed logo/text, borders — generated from stacked anchor-point-referenced placeholder masks and the Paint Along Path stitching tool, rather than baked-in or hand-modeled geometry.

### Summary
Starts with a DCC-side prep note (duplicate + rotate the model upside-down to get workable access to the sole for texturing, separate from the baking/rendering-orientation mesh), then bakes 4K mesh maps at 64x AA. In Painter, the mesh is split into `Plastic`/`Fabric` folders via a Polygon-Fill mask, immediately backed by an inverted Anchor Point copy for reuse. The plastic sole is built by trialing several purchased smart materials, picking one, then gutting and rebuilding its layer stack (dual base colors, two color-variation passes, two surface-noise passes, dirt variation, roughness, scratch) plus a dedicated curvature-generator "edge roughness" layer for reflective highlights on edges. The fabric upper uses the built-in `Fabric Wool Herringbone` material for the top panel and a `Fabric TrapStitching`-driven Paint-Along-Path stitch line (Slant and Pin Stitches, then Straight Stitches with Leather-type puckering) for the visible seam around the shoe opening. The back half of the video is a deep-dive into building fine sole/branding detail without touching geometry: height-only "L1/L2/L3 Detail" fill layers combine gradient-linear fills, 3D word-pipe text meshlets, capsule shapes, strip patterns, anchor-point-referenced "placeholder mask" layers (used purely as reusable, invertible mask sources — never rendered directly) to lay out a tread pattern on the sole, a Bevel + Histogram Scan + Mask Outline filter chain to cut a clean border/divider line, and a final Ambient Occlusion generator (fed by two Edge Plus reference layers, one referencing Height and one referencing Normal) layered via a Pass-Through "edge collection" paint layer to unify the whole material.

### Key Steps
1. **Prep the mesh outside Painter first:** because Painter's viewport can't be freely rotated onto the mesh's own backface/underside for comfortable painting, duplicate and rotate the model upside-down into a second variant used purely for texturing access; keep the original orientation for baking/rendering.
2. **New Project setup:** 2K document resolution, Normal Map Format set to `DirectX`, template `PBR Metallic Roughness`.
3. **Bake mesh maps** at 4K output size, 64x anti-aliasing, then switch to the upside-down texturing variant of the mesh once baking completes.
4. **Split the mesh into two base folders (`Plastic`, `Fabric`)** using a black mask + `Paint` + `Polygon Fill` mode to select/deselect UV islands (white = plastic sole, black = fabric upper); immediately add an `Anchor Point` to this split mask and load-and-invert it elsewhere for a free complementary mask.
5. **Trial several purchased smart materials on the plastic sole** by toggling folders on/off to compare, pick the best base, then delete the rest and manually rebuild the layer stack rather than keeping the smart material as-is: two base colors (grey + lighter grey, second one paint-masked), two color-variation fills (opacity-tuned), two surface-noise fills, a dirt-variation fill, roughness, and a scratch layer — explicitly pruning "edge damage" and "triple-S" sub-layers that didn't suit this asset.
6. **Add a dedicated `Edge Roughness` fill layer:** black mask + `Curvature` generator, tuned so the white (high-curvature/edge) areas get a higher reflective/roughness value — called out as adding "the highlight on the edge" for a more interesting render.
7. **Build the fabric upper from two material passes:** a `Fabric Wool Herringbone` fill for the top panel (mask via Polygon Fill, pattern scaled ~3x, rotated ~110°), and a separate, darker fill for the inside lining driven by an inverted Anchor Point mask, with fiber-density parameters increased for a denser look.
8. **Add stitching with the Paint Along Path tool:** draw a path along the top opening seam, set stitch type to `Slant and Pin Stitches` (invert path, size 5→3, refine path placement), add a black mask + Polygon Fill to prevent stitch data "leaking" past the seam boundary; for a second seam, switch stitch type to `Straight Stitches`, reduce stitch size (1→0.7), and change `Puckering` type from Thick Fabric to `Leather` for a tighter, more realistic pucker; duplicate the finished stitch line to the mirrored side.
9. **Composite a "final polish" Pass-Through effect paint layer** (applied to all channels) stacking a `Sharpen` filter (~0.5) and duplicating it into a separate `Contrast` pass (color only) plus a `High to Normal` filter with `Use World Unit` off and intensity ~3, to punch up overall surface micro-detail before moving to fine hand-placed detail.
10. **Build height-only "Detail" fill layers (L1/L2/L3) for hand-placed branding/graphic elements:** each is a black-masked fill with only the `Height` channel enabled (small negative offsets like -0.1/-0.2) so detail reads purely as embossed/debossed geometry, not color — built from a `Gradient Linear #2` fill (2D mode, scaled/rotated/duplicated into multiple short lines, blend mode `Linear Dodge`) for line accents, a `Comic Sans Bold` 3D-word-pipes text fill (UV wrap none, small scale, adjustable character spacing, mirrored copy for the opposite side) with a `Square` shape fill behind it as a border box (blend mode `Subtract` for the outline), and a capsule `Shape` fill for a separate size-label detail (also mirrored).
11. **Build the sole tread pattern from reusable anchor-point "placeholder mask" layers:** create paint layers with no visible data purely to hold mask geometry (named e.g. `L3 Placeholder Mask 1/2`, colored red for visibility in the stack), fill them with white + Linear-Dodge-blended line fills to rough in tread "regions," anchor-point them, then reference/invert those anchor points from downstream `Strip` pattern fills (tiling 15, rotation ~120° and a duplicate at ~116°, blend mode `Multiply`) to lay repeating tread grooves only inside the defined regions — using a `Paint` layer with `Subtract` blend and manual polygon deselection (press X to deselect) to correct an over-broad inverted-mask selection along the way.
12. **Refine the tread border/divider with a filter chain:** a placeholder mask built from a Polygon-Fill UV-island selection, run through `Bevel` → `Histogram Scan` (contrast + position tuning) → `Blur` filters to produce a clean, softened border line; combine with an inverted, `Subtract`-blended copy of the original region to knock out unwanted areas; use `Mask Outline` on another placeholder to derive a border-cut line, then a `Linear Dodge`-blended `Border Cut` anchor-point fill plus another `Blur` pass to finalize the divider groove around the tread pattern, before subtracting out the reserved label/text area.
13. **Return to the plastic sole's second-color mask to add the logo/brand text as a final color detail:** re-select the relevant UV island in Polygon Fill mode, then paint-subtract everything except a `3D Art Box` text shape so only the brand text reads in the second (white) plastic color.
14. **Finish with a unified Ambient Occlusion pass:** a Pass-Through "Edge Collection"/"Edge Plus" paint layer (applied to all channels) holds an Anchor Point; a new `AO`-only fill layer (black mask) uses the `Ambient Occlusion` generator set to `Macro Detail`, loading the Edge Plus anchor point twice — once with its Reference Channel set to `Height`, once set to `Normal` — then tuning the AO radius; noted that reordering this Edge Plus layer to sit before the fabric layers removes unwanted AO on the fabric if not desired, and that some detail layers (e.g. part of L2 Detail) may need to be toggled off if they read poorly once AO is applied.

### Layers / Tools / Settings
- **Smart materials trialed/used:** multiple purchased plastic smart materials (trialed, then discarded in favor of a hand-rebuilt stack), `Fabric Wool Herringbone` (top panel), an unnamed darker fabric material (inside lining, fiber-density increased), `Fabric TrapStitching` material used by the stitch brush
- **Generators used:** `Curvature` (edge roughness/reflectivity), `Ambient Occlusion` (Macro Detail mode, dual Edge-Plus-anchor references for Height and Normal)
- **Stitching (Paint Along Path) settings:** stitch types `Slant and Pin Stitches` and `Straight Stitches`; `Puckering` type switched Thick Fabric → `Leather`; stitch size tuned 5→3 and 1→0.7 across the two seams
- **Fills/patterns used:** `Gradient Linear #2`, `Strip` (tread grooves, tiling 15, rotation ~116-120°), `Square` (text border box), `Shape — Capsule` (size-label detail), `Comic Sans Bold` (3D word-pipes text, two placements incl. mirrored)
- **Filters used:** `Sharpen` (~0.5), `Contrast` (color-only pass), `High to Normal` (World Unit off, intensity ~3), `Bevel`, `Histogram Scan`, `Blur` (used at multiple stages), `Mask Outline`
- **Blend modes used:** `Soft Light` not used here (unlike the black-suit video) — this one leans on `Linear Dodge` (line/tread accents, border cut), `Multiply` (tread grooves), `Subtract` (mask corrections, border-text isolation, text-outline box)
- **Anchor Point usage (heavy, this video's throughline):** one for the initial Plastic/Fabric mask split, one for the fabric inside-lining mask, several `Placeholder Mask` anchor points purpose-built purely to drive downstream tread/border fills (never rendered directly themselves), one `Border Cut` anchor point, one `Edge Plus` anchor point referenced twice with different Reference Channels (Height, Normal) for the AO pass
- **Baking settings:** 4K output size, 64x anti-aliasing
- **New Project settings:** 2K document resolution, DirectX normal format, PBR Metallic Roughness template

### Difficulty
Advanced — while the base plastic/fabric material building is approachable, the sole-tread and border detail work (Key Steps 10-12) is a genuinely advanced technique: multiple layers of anchor-point-referenced, never-rendered "placeholder mask" layers driving pattern generation, plus a multi-filter (Bevel/Histogram Scan/Mask Outline/Blur) border-cutting chain. Requires solid prior comfort with anchor points and generators to follow.

### App & Version
Substance 3D Painter — version not stated on screen. The stitching tool's panel is explicitly titled `PAINT ALONG PATH` in multiple captured frames. Per `references/version-tracker.md`, this exact tool name was only in use from Painter 9.0.0 until it was renamed `Filled Path` in 11.0.0 (and later `Ribbon` in 11.1.0) — this pins the tutorial to the Painter 9.x-10.x window, consistent with the companion "Black Suit" video's separate 10.0.0+ dating from the same creator.

### Tags
layers, fill-layer, paint-layer, masks, smart-material, generator, curvature, anchor-point, blend-mode, ambient-occlusion, mesh-maps, baking, texture-set, uv, pbr, metal-rough, basecolor, roughness, metallic, height, normal-map, alpha, procedural, export-preset, advanced

---

## Related Tutorials
- [Texturing a Black Suit in Substance Painter](texturing-a-black-suit-in-substance-painter.md) — same creator (3DRedBox); shares the same overall production recipe (DCC-side mesh prep, 4K/64x-AA baking, layered smart-material-plus-hand-built-fill-layer construction) and both videos independently date to the same pre-11.0.0 tool-naming era.
- [Texturing a Worn Wooden Stool in Substance Painter](texturing-a-worn-wooden-stool-in-substance-painter.md) — same creator; shares heavy anchor-point usage for building reusable, non-rendered mask sources (placeholder masks there, gradient/damage masks here) and the same Pass-Through "Effect" layer pattern for stacking AO/Height-to-Normal filters.
- [Texturing Women's Shorts with Lace Trim in Substance Painter](texturing-womens-shorts-with-lace-trim-in-substance-painter.md) — same creator; shares the anchor-point-as-reusable-mask-source philosophy (placeholder masks there, the multi-strap lace duplication here) and a Pass-Through "Effect" layer used to stack finishing filters at the top of the stack.
- [How to Create a Realistic Poison Bottles Material Using Substance Painter](how-to-create-a-realistic-poison-bottles-material-using-substance-painter.md) — same creator; both confirmed via the "PAINT ALONG PATH" panel to date from the same Painter 9.x-10.x window, and both use anchor-point-referenced placeholder/collector layers as reusable mask sources.
- [Speed Up Your Substance Painter Workflow with This Easy Trick!](speed-up-your-substance-painter-workflow-with-this-easy-trick.md) — same creator; both confirmed via the "PAINT ALONG PATH" panel, and both rely on the Pass tool for hand-drawn stitching detail.
