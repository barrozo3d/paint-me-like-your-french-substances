---
title: Creating & Reusing Smart Materials in Substance 3D Painter | Stylized Crab | Adobe Substance 3D
source: YouTube
url: https://www.youtube.com/watch?v=ZiWAe_iZ_CI
author: Adobe Substance 3D
ingested: 2026-08-13
app: "Substance 3D Painter"
version: "11.0.0+"
tags: [layers, fill-layer, masks, smart-material, generator, anchor-point, blend-mode, curvature, tri-planar, procedural, texture-set, basecolor, intermediate, advanced]
extraction_status: complete
frames_dir: tutorials/frames/creating-reusing-smart-materials-in-substance-3d-painter-stylized-crab-adobe-sub/
frame_count: 0
frame_status: pending-selection
---

# Creating & Reusing Smart Materials in Substance 3D Painter | Stylized Crab | Adobe Substance 3D

**Source:** [YouTube](https://www.youtube.com/watch?v=ZiWAe_iZ_CI)
**Author:** Adobe Substance 3D
**Duration:** 10m12s | 7 section(s)

---

## Raw Data (for Claude Code extraction)

## Ingest Safeguard Report (reviewed, resolved)

The flagged empty chapter ("Adjusting the Smart Material project for different look" [5:16]) is a real ~10-second on-screen transition with no dedicated narration of its own — not a content gap. The surrounding transcript flows continuously across it (creator says "we can definitely adjust things very easily... click on the magic wand" at [5:12], then the very next chapter "Adding Gradient effect" [5:26] picks up mid-thought with "Oh and by the way..."). No information was lost; extraction proceeded normally.

---

Frames are not captured yet. Read the timestamped transcript below, pick moments
that actually show a technique/result worth a still (not blind percentages —
even within a named chapter, verify the real moment against its timestamps), then run:
  python select_frames.py creating-reusing-smart-materials-in-substance-3d-painter-stylized-crab-adobe-sub <ts1> <ts2> ...
(seconds or mm:ss). This appends a "Captured Frames" section and updates the
frontmatter before you write the Structured Notes below.


### <Untitled Chapter 1> [0:00]
**Transcript (timestamped):**
[0:00] Hey, what's up guys, Paulo Muñoz here. In this video, I'm going to show you how I can take one of my stylized material setups and turn that into a smart material all within Adobe Substance 3D Painter so that we can reuse it in other projects.
[0:18] Alright, so here is the project of the stylized scrap and it is currently half finished, but I did spend some time setting up the shell material for the legs in this case with custom mask, with custom, you know, cool anchor points, that sort of stuff.


### Setting up the layers to reuse effects [0:22]
**Transcript (timestamped):**
[0:31] So I want to be able to reuse some of that setup in other parts of the project or, you know, even new projects. So I want to walk you through all of that.
[0:38] The first thing I like to do is make sure that my layer stack is neatly organized and named properly, specifically if I'm going to reuse this material in a brand new project, maybe in a few months from now.
[0:49] Currently, I have a yellow color as my base, a red color with a custom mask that blends into the yellow color and then a third folder that I set up with anchor points so I can do some manual painting.
[0:58] Now, since I'm planning to reuse this in other projects, I like to make sure that the effects I use are set as triplanner. This goes for any table black and white image or anything of that nature that you use to drive the effect of a mask.
[1:10] So for instance, this grunge texture is set to triplanner in my project so I can reuse it in other projects. That way I can adjust it and move it later on if I need to so that it fits better any other project in the future because I don't know what that project might be.
[1:22] Now I'm going to name this layer color variation and this layer is making things darker so let's just call it darker yellow and let's go ahead and do the same thing for the layers on the red folder.
[1:32] This layer is making things a bit lighter so let's go for lighter reds and the third one here is kind of like similar actually so maybe we can just call this one lighter reds 01 and then copy and paste this into the next layer and call it lighter reds 02.
[1:48] Not super creative but it helps me remember what these layers are used for. Now if you want to be super organized you could also look into custom mask and look for anything in the stack of filters that is not very descriptive and change it for a custom name as well.
[2:01] In my case I have this grunge concrete paint leaks on top which is a very clear name but it's not really telling me what this is doing for the mask so we can call this something like extra dirt or actually this is more like a scratch material so maybe let's call this extra scratches.
[2:17] I'm also going to rename the third folder custom spots but here is the most important part. If you have anything with custom paint layers like what we have here or you can just paint custom details like this remember that this is painting this specific UV layout so keeping this effect and reusing it in a different mesh with different UVs will look out of place.
[2:36] So what we need to do is just remove it all together or delete it and create a brand new paint layer to replace it. I like calling this layer paint here just to remind my future self that this is the layer that I need to use for custom painting.
[2:48] And the final thing would be just let me just check the anchor point and I think I want to call this fill layer something like custom spots mask reference maybe that is too long maybe just go for spot mask reference and instead let's go ahead and update the anchor point name to be spot mask.
[3:03] Okay so now the boring part is done but believe me this is a very important step so that you can make the most out of your own assets later on. Now we're going to turn all of these layers into our very own smart material.


### Converting the Asset into a Smart Material [3:10]
**Transcript (timestamped):**
[3:14] Let's go ahead and press the shift key and select all the folders and create a brand new folder by clicking on this icon of the folder right here on the top right.
[3:21] Go ahead and name the folder with whatever name you want to give to your material. I'm simply going to call mine stylized scrap and now all we have to do to create that smart material is to right click on the folder and select the create a smart material option.
[3:33] Give it a few seconds and now you'll see your brand new asset in your own library. So now I can literally delete everything in my layer stack bring back all my meshes so that we visualize this as a let's say a brand new project and I'm going to click and drag my custom material into the legs and there you go but also drag it into the body of the crap and you know the eyes as well
[3:53] and you see how this is using values from all those settings within the material layer and the mask of course but applying them to each mesh differently. What's really cool about this is that we can go to the texture set settings and let's choose something different maybe maybe like the body and it's also isolated so that we can see only this mesh for now.
[4:11] And let's go to the layers of that smart material folder and find the layer called spots manual and the empty pain that we created called pain here and now we can have some fun adding some custom details in the areas that make sense to have them for this specific mesh how cool is that.
[4:24] Alright so now let me share with you something even better about smart materials so to prove the portability of these assets basically to ensure that you know whatever works in this project can also work in other projects.


### Using the Smart Material in different Project [4:31]
**Transcript (timestamped):**
[4:35] Let's go ahead and switch to a brand new project with a completely different crap or a different asset.
[4:40] Alright so this guy right here is completely new project. It has nothing to do with the previous project other than the fact that you know it's a it's a crab but for practical purposes it has different measures it has different UVs it has a different
[4:52] bake maps. The only thing that I have done is just a couple of layers for the eyes. Now because we saved our smart material into our library I can access it from here and simply drag and drop it into the craps body.
[5:02] That's it how cool is that and we can go ahead and open up the folder you'll see that we have all the same layers and of course we can look for that pain here layer to create some custom bumps in here as well.
[5:12] Now this is cool and all but what if I want a completely different look for my project. Well the cool thing is that we can definitely adjust things very easily and we can for instance select our main folder and click on the magic one here to add an effect to the entire folder.


### Adjusting the Smart Material project for different look [5:16]

### Adding Gradient effect to quickly change colours [5:26]
**Transcript (timestamped):**
[5:26] Oh and by the way this is a bit of a tangent but since we're here in this effects section I should mention that there has been a recent update with six really really cool filters that you can mix and easily create stylized textures to achieve all sorts of really cool effects.
[5:40] So you have the anisotropic kuhara the bevel smooth which actually deals with the height information more than anything directional distance grayscale conversion quantize and stylization which are super super cool and you get really awesome effects when you combine them together.
[5:55] Anyway let's go back to edit this material. So from the effect list let's go ahead and find something called gradient. Now this effect is very cool very simple and it's going to look at the colors within the folder and simplify them to a gradient of three values.
[6:08] Now you can take the position of each value and change them to add more contrast. I want to have more of a black color in those sort of flatter areas or panels of the crab shell and the white colors more towards the crevices with maybe less of those gray mid tones.
[6:22] Now we can have some fun by changing the colors of that gradient and this is where you can be very creative and try something completely different completely new. I'm going to go for a dark blue for darker values maybe a green tone around the mid values and let's just go for a yellow or maybe like a lighter gray here for the lighter
[6:39] values. That's it. You can also play with how this entire gradient effect blends with the rest but I think I'm going to keep it simple and I'm just going to go for overlay just to add a little bit of contrast.
[6:49] But if things look a little bit too dark we can always come back and adjust the color picker and change them again. Maybe going for some more saturated maybe lighter colors will help as well and you know make things a little bit more interesting.
[7:00] And I know it's not really the color of a crab but I just want to show you how much you can change things very quickly. In fact we can create a stack of effects just to change how the original smart material looks.
[7:12] So we can for instance maybe add another filter and let's search for something like the HSL Perceptifilter. And this is a very simple filter as well but it allows you to change the hue all at once and you can explore different color palettes.
[7:25] You know play with the saturation the lightness of the entire color palette. So if I turn this effects on enough you'll see how much they affect in the original material.
[7:32] Alright so hopefully that makes sense. Now here is another awesome feature. Let's say that you're happy with the tweaks that you created in your new custom material from that original but you want to apply those to the rest of the texture sets in your project.


### Instantiate layers across multiple texture sets [7:43]
**Transcript (timestamped):**
[7:43] You could of course right click the folder and copy and paste it into the other meshes or even create a brand new smart material that includes the new effects that you did.
[7:52] However the most effective way is to right click the folder and choose the instantiate across texture sets option. This new pop up window will appear and you can leave everything checked except the source of course which is in our case the body of the crab and just click OK.
[8:06] Now what's happening is that the smart material with all the changes that we've done is being propagated through the entire texture set list. So I'm just going to go to the eyes for a second and move that instance layer below everything else that I had just because it doesn't make sense to have it on top but that's pretty much it.
[8:22] If I go back to my source which is the body of the scrap you'll be able to change anything in the effects that you added and see the changes in real time across all your meshes. This also goes for blending modes so you can now visualize the material in your entire mesh and just adjust how the effects are blending with each other.
[8:39] At this point you could refine the look of your textures by adding a new fill layer. You know let me just do that and we can basically play with how it is blending with the material. So again just my go to blending mode just to test things out is overlay.
[8:52] So let's do that and let's create a black mask at a generator and I'm going to use curvature to target those reaches and the bumpy areas of the mesh. And actually I think we can make those areas a little bit lighter so you can really see the effect.
[9:04] I'm going to first choose a bright green color which also helps and I think I can set the blending mode to screen again just to make things a little bit brighter. Let's go ahead and adjust the balance of the curvature as well and this basically adds a bit of contrast to that mask and of course we can refine the color of the layer itself so it just feels better integrated with the rest of this weird material that we're making.
[9:25] And to wrap this up I'm going to name this layer something like edge and repeat the process that I showed you before. I'm going to instantiate this layer throughout my other texture sets and that's it great.
[9:35] Now we can also have a control layer for all those ridges and bumps with a specific color all within our project.
[9:41] So that's it for this video. Hopefully you can see how quick and easy it is to create a smart material and essentially repurpose all your assets and create your own library of assets. I myself have a bunch of these smart materials in my library and it provides me a great starting point for any new project.
[10:03] So if you're going to go ahead and try this out let me know how you go and don't forget to subscribe to this channel if you want to see more of this content on Adobe Substance 3D.



---

## Structured Notes

### Core Technique
Converting a hand-built, project-specific layer setup into a portable, reusable **Smart Material** asset: clean/rename the layer stack, replace anything mesh-specific (custom paint strokes, tri-planar-set generators) with reusable equivalents, group into one folder, right-click → Create Smart Material, then drag onto entirely different meshes/projects and reskin it with folder-level filters (Gradient, HSL Perception, Curvature-driven edge highlight) propagated across a whole texture-set list via **Instantiate across Texture Sets**.

### Summary
Paulo Muñoz takes a half-finished stylized-crab shell material (custom masks, anchor points) and turns it into a reusable Smart Material asset. Part 1 is prep/hygiene: rename every layer/folder/mask/anchor-point to something self-explanatory, confirm any grayscale-driving textures (e.g. grunge) are set to **tri-planar** projection so they aren't tied to one mesh's UVs, and replace any hand-painted custom-UV paint layer with an empty placeholder paint layer (since hand-painted strokes are baked to specific UVs and won't transfer). Part 2 converts the cleaned folder stack into a Smart Material (select all folders → new folder → right-click → Create Smart Material) and demonstrates dragging it onto multiple meshes in the same project (legs/body/eyes) and then onto a completely different crab project with different UVs/bakes — same material, correctly adapted per mesh. Part 3 shows re-skinning that Smart Material for a new look without leaving the material folder: adding a **Gradient** filter (3-color remap driven by the folder's existing tones) and an **HSL Perception** filter for fast palette exploration, then adding a folder-level **Curvature**-masked edge-highlight fill layer, and propagating every tweak to the rest of the project's texture sets in one action via **Instantiate across Texture Sets**. A brief tangent name-checks Painter's then-recent "6 new filters" batch (Anisotropic Kuwahara, Bevel Smooth, Directional Distance, Grayscale Conversion, Quantize, Stylization).

### Key Steps
1. Prep: with the half-finished stylized-crab shell material open (yellow base, red color-variation folder with a custom mask, and a third "custom spots" folder built on anchor points), rename every layer/folder to something self-explanatory (e.g. "darker yellow", "lighter reds 01/02", "extra scratches") so future-you (or anyone reusing the asset) understands each layer's purpose at a glance.
2. Confirm any grayscale mask-driving texture (e.g. a grunge concrete-paint-leaks texture) is set to **tri-planar** projection rather than plain UV — this decouples the effect from any one mesh's UV layout so it transfers cleanly to new meshes/projects.
3. Identify and remove anything tied to this mesh's specific UVs — a hand-painted custom paint layer under the anchor-point-driven folder — and replace it with a brand-new **empty paint layer** (named e.g. "paint here") as a placeholder for future manual detailing on whatever mesh the material ends up on.
4. Rename the anchor point itself (e.g. "spot mask") and its source fill layer (e.g. "spot mask reference") for clarity.
5. Select all the prepped folders (Shift-click), group them into one new folder, and name that folder after the material (e.g. "Stylized Crab").
6. Right-click the folder → **Create Smart Material** — the asset now appears in the Shelf/Library, ready to reuse.
7. Test in the same project: delete the layer stack, drag the new Smart Material onto multiple different meshes (legs, body, eyes) — the material's masks/generators adapt correctly per mesh while pulling from the same shared settings.
8. Isolate a texture set (e.g. body only) via Texture Set Settings, open the Smart Material folder's layers, find the empty "paint here" layer, and hand-paint mesh-specific custom details on top of the shared base.
9. Portability test: switch to a completely different project (different crab mesh, different UVs, different bake maps). Drag the same Smart Material from the Library onto the new mesh's body — it adapts automatically; the "paint here" placeholder layer is still there for fresh custom painting on the new UVs.
10. Re-skin without leaving the material: select the Smart Material's top folder, click the **magic wand effect icon** to add a folder-level filter; search for **Gradient** — this filter reads the folder's existing color values and remaps them to a 3-color gradient (adjustable stop **Positions** for contrast, e.g. more black on flat panels, white in crevices).
11. Recolor freely by editing each gradient stop's color (e.g. dark blue → green → yellow/light gray); set the filter's blend mode (e.g. **Overlay**) to control contrast strength.
12. Stack a second folder-level filter, e.g. **HSL Perception**, to shift hue/saturation/lightness across the whole existing palette at once for fast exploration.
13. Propagate the tweaked material to the rest of the project: right-click the folder → **Instantiate across Texture Sets** → in the popup, leave all target texture sets checked except the source (the mesh you edited) → OK. All other meshes now receive linked instances of the edited material; reorder the resulting instance layer in each texture set's stack as needed (e.g. eyes needed the instance moved below existing eye layers).
14. Refine further: add a new fill layer inside the folder, black mask + **Curvature generator** to target ridges/bumps, pick a bright accent color, set blend mode to **Screen** for extra brightness, adjust the curvature Balance for contrast, name the layer (e.g. "edge"), and **Instantiate across Texture Sets** again to push this new edge-highlight layer to every other mesh too.

### Layers / Tools / Settings
- Layer/folder/mask/anchor-point renaming discipline for reusability
- Tri-planar projection (mask-driving grayscale textures, for UV-independence)
- Empty placeholder paint layer (replaces mesh-specific hand-painted strokes before converting to Smart Material)
- Smart Material creation: multi-folder select → new folder → right-click → **Create Smart Material**
- Texture Set Settings (isolate a single mesh/texture set)
- Folder-level effects/filters: **Gradient** (3-color remap, stop Position, blend mode), **HSL Perception** (hue/saturation/lightness), plus a name-check of the "6 new filters" batch (Anisotropic Kuwahara, Bevel Smooth, Directional Distance, Grayscale Conversion, Quantize, Stylization)
- **Instantiate across Texture Sets** (right-click folder; checkbox list of target texture sets, excludes source)
- Fill layer + black mask + **Curvature generator** for edge/ridge highlighting; blend mode Screen

### Difficulty
Intermediate to Advanced — the core workflow (rename, group, Create Smart Material) is approachable, but getting real reuse value out of it depends on understanding tri-planar projection, anchor points, and folder-level filter stacking.

### App & Version
**Substance 3D Painter 11.0.0+** — the creator explicitly lists "six really really cool filters" by name (Anisotropic Kuwahara, Bevel Smooth, Directional Distance, Grayscale Conversion, Quantize, Stylization) as a "recent update," and `references/release-notes-painter-11.0.md` lists exactly these six filters as new in 11.0.0. Strong, explicit version floor. Exact patch build not shown on screen.

### Tags
`layers` `fill-layer` `masks` `smart-material` `generator` `anchor-point` `blend-mode` `curvature` `tri-planar` `procedural` `texture-set` `basecolor` `intermediate` `advanced`

---

## Related Tutorials
- **"SUBSTANCE PAINTER: Building Masks Explained"** (`tutorials/substance-painter-building-masks-explained.md`, video `um3YRzqwYU4`) — shares the tri-planar-projection and anchor-point-driven masking fundamentals this video assumes are already in place before converting to a Smart Material.
- **"How to TEXTURE like a PRO with ANCHOR POINTS | Substance Painter Tutorial"** (`tutorials/how-to-texture-like-a-pro-with-anchor-points-substance-painter-tutorial.md`, video `l2W67e5MQuk`) — that video's "modular anchor point library" use case (building reusable, stacked anchor-referenced materials) is the direct conceptual sibling of this video's Smart Material conversion workflow.
- **"Texturing a Cyberpunk Building in Substance 3D Painter – Project Breakdown"** (`tutorials/texturing-a-cyberpunk-building-in-substance-3d-painter-project-breakdown-adobe-s.md`, video `gv9R6a6VPYQ`) — same Adobe-official channel; reuses the Plastic Dusty smart material across many objects the same way this video demonstrates building and reusing a custom one.
- **"Footwear Texturing from Start to Finish – Live Tutorial in Substance 3D Painter"** (`tutorials/footwear-texturing-from-start-to-finish-live-tutorial-in-substance-3d-painter-ad.md`, video `s59xbaF4Q14`) — complementary material-reuse philosophy: this video formalizes a tuned layer stack into a portable Smart Material asset, while that video achieves similar consistency more informally via repeated copy → Paste Layer as Instance.
