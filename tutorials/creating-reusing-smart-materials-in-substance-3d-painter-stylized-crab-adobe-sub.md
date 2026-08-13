---
title: Creating & Reusing Smart Materials in Substance 3D Painter | Stylized Crab | Adobe Substance 3D
source: YouTube
url: https://www.youtube.com/watch?v=ZiWAe_iZ_CI
author: Adobe Substance 3D
ingested: 2026-08-13
app: "[PENDING]"
version: "[PENDING]"
tags: []
extraction_status: needs-review
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

## Ingest Safeguard Report

_Auto-generated at ingest/frame-capture time — explains why `extraction_status` may be `needs-review`. Safe to delete once reviewed._

- **CRITICAL:** Empty transcript in chapter 'Adjusting the Smart Material project for different look'

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
