---
title: Creating Trim Sheet UVs for Substance 3D Painter | Adobe Substance 3D
source: YouTube
url: https://www.youtube.com/watch?v=Dp2ZpGIaumA
author: Adobe Substance 3D
ingested: 2026-08-12
app: "[PENDING]"
version: "[PENDING]"
tags: []
extraction_status: pending
frames_dir: tutorials/frames/creating-trim-sheet-uvs-for-substance-3d-painter-adobe-substance-3d/
frame_count: 0
frame_status: pending-selection
---

# Creating Trim Sheet UVs for Substance 3D Painter | Adobe Substance 3D

**Source:** [YouTube](https://www.youtube.com/watch?v=Dp2ZpGIaumA)
**Author:** Adobe Substance 3D
**Duration:** 15m30s | 1 section(s)

---

## Raw Data (for Claude Code extraction)

Frames are not captured yet. Read the timestamped transcript below, pick moments
that actually show a technique/result worth a still (not blind percentages —
even within a named chapter, verify the real moment against its timestamps), then run:
  python select_frames.py creating-trim-sheet-uvs-for-substance-3d-painter-adobe-substance-3d <ts1> <ts2> ...
(seconds or mm:ss). This appends a "Captured Frames" section and updates the
frontmatter before you write the Structured Notes below.


### Full Content [0:00]
**Transcript (timestamped):**
[0:00] In this video, we will go over how to UV unwrap 3 assets that will be using a trim sheet texture.
[0:15] This is a continuation of our trim sheet series, which you can find on our YouTube channel.
[0:21] We will go over on how to UV unwrap this particular large scale window asset over here from this
[0:27] sci-fi environment.
[0:29] We will not be using the same trim sheet texture that we have created in our previous videos.
[0:35] Instead, we will be using a slightly more complicated trim sheet texture to get the most out of our
[0:40] model.
[0:42] We have various details on this trim sheet.
[0:44] We have details which are tileable on a horizontal axis like you can see with this flat metal
[0:49] over here and this trim sheet over here.
[0:52] We also have some of them down here, which you can see with the lines.
[0:55] And we also have some more specific details that have specific edges and edge damages,
[1:00] which you can use for example over here to create these type of section details.
[1:06] Now next to this, we also have some more specific perfectly square details which are tileable
[1:11] on a vertical axis as you can see over here.
[1:16] And these details we can use to later on place down here and repeat them over and over again
[1:22] along this bottom section.
[1:25] Next to this, we also just have some more additional details like some floor panels, which you
[1:29] can see over here and down here some more additional floor panels and some specific
[1:35] details.
[1:36] These details actually also have a mask like you can see over here, which allows us to basically
[1:42] cut out any of the background and use them as simple text which we can place on a trim
[1:48] sheet.
[1:49] This entire environment that you see over here has actually been created using this one single
[1:55] trim sheet texture, just like we did in the previous videos.
[1:59] Down here we also have one small section which features a unique texture because in trim
[2:05] sheets you can just also place a unique texture.
[2:08] However this one we will not be using as it will just be used for these crates.
[2:12] In this video we will be focusing only on this window asset over here.
[2:18] For this tutorial, we will be using 3S Max to showcase you how to UV unwrap this asset.
[2:23] However, these techniques can easily be replicated in your favorite 3D software.
[2:28] Also, we are going to save a lot of time by mirroring our asset so I can select half
[2:34] width and delete it and later on I can mirror this in order to basically save half of our
[2:39] time.
[2:41] Now we are going to get started by an introduction with some smaller details like we have over
[2:45] here.
[2:47] These are the details that you can see down here which are located in our UV unwrap on
[2:51] the left bottom side here.
[2:55] The first thing that we want to do is we want to go ahead and we want to apply our trim
[2:59] sheet texture to this asset so that we can properly preview it.
[3:03] Now as you can see, this plane over here is a very simple plane and it has been specifically
[3:09] split up into square sections over here.
[3:13] The reason we did this is so that we can make these sections properly tileable just like
[3:18] you can see in our squares over here.
[3:21] We want to go ahead and we want to open up our UVW unwrap window so that we can get started.
[3:27] So the first thing in our window that we want to do and you can do this in whatever software
[3:30] you want is you want to go ahead and load in your trim sheet texture so that you can
[3:34] properly preview it.
[3:37] Now let's get started with the simple one which is going to be this square.
[3:41] We want to go ahead and layout this square over here and then we can decide which specific
[3:46] detail from these two that we want to use.
[3:50] I myself will go ahead and use the one that has a little bit more visual interest.
[3:54] So all I have to do is I have to go ahead and go in here and I can nicely map it to this
[4:00] specific detail.
[4:02] Because these squares have been created to be an even 512 by 512 texture, what we can
[4:09] do is we can go ahead and we can snap the grids inside of 3s Max.
[4:14] In this case I would just want to go ahead and show my grid and then what I'm going to
[4:17] do is I'm going to go up here and turn on snap toggle.
[4:21] Then I will switch to vertices and now it is as easy as simply snapping this to my grid
[4:27] vertices over here.
[4:28] This way I can be assured that it will be perfectly tileable.
[4:33] I can then move on to the next one, iron it, scale it down and once again overlay it.
[4:41] What I like to do is I like to have it a little bit more in the center over here so that I
[4:45] can then more easily select my vertices and snap this to the grid.
[4:52] Doing that what you can see is that now if I for example turn off my edge and faces we
[4:56] will have a perfect continuation.
[4:59] You might see over here like a little line but this line will not show up in Unreal Engine
[5:03] since this is just a visual bug from 3s Max.
[5:07] Now let's go ahead and go back into IEV and let's focus on this little end over here.
[5:13] Sometimes you will have sections that will not properly fit.
[5:15] In these sections you can just take some creative liberty.
[5:18] Let's go ahead and UV unwrap this one shell over here and I do want to still make it tileable
[5:24] on one side let's say down here.
[5:27] In this case I like to fit my UV shell a little bit better to make it a little bit easier
[5:32] to work with and then what I can do is I can once again just go ahead and select the vertices
[5:37] and snap them to the grid over here.
[5:41] For these sides what I'm going to do is I'm going to decide roughly where I want to basically
[5:45] end this piece.
[5:47] If I just go ahead and push this back over here you can see that we will get a little
[5:51] bit of stretching.
[5:52] Now a little bit of stretching is not the end of the world.
[5:55] This is something that can be quite easily compensated.
[5:59] However I feel like that this one might be a little bit much so what I'm going to do
[6:02] is I'm going to push this back a little bit more like this over here and then I'm just
[6:08] going to actually edit my geometry.
[6:11] Basically going in here and moving these last two sections a little bit more towards the
[6:18] right side over here.
[6:23] And this is a concept that I want you to understand when we are talking about trim sheets.
[6:28] With trim sheets you cannot always keep the same text or density and you cannot always
[6:32] keep everything at the exact perfect proportions.
[6:35] So you will have to be a little bit more flexible with it but in turn you get great optimization
[6:41] and often even a faster asset creation process.
[6:45] Now I will go ahead and I will map these details over here only on these straight details.
[6:51] On this angular detail over here we will just go ahead and use some plain metal since we
[6:55] cannot properly map a detail like this on a shape like we have over here.
[7:01] I'm now going to show you how to apply your trim sheet on a very large structural asset
[7:07] like this window over here.
[7:09] Now believe it or not but this entire window is actually using only this small metal section
[7:14] over here.
[7:15] The key goal for this is that your texture is tileable on both sides so that we can repeat
[7:25] our shapes over and over again.
[7:27] One thing that we can actually map around this entire window using only this small section.
[7:33] So if we go ahead and go to 3s max again and we will apply our trim sheet texture.
[7:38] Now as you can see this will look very bad right now.
[7:42] Please note that with this technique you simply cannot maintain text or density.
[7:47] So what you need to do is you need to find the right balance where you do not notice
[7:51] the difference in resolution while still having everything look like a proper resolution.
[7:58] As you might notice you can see that our metal over here is a long thin section.
[8:07] Now if we look at our model you can see that our model has also been split up into these
[8:11] long thin sections.
[8:13] So what we can do is we can simply unwrap all of these sections individually and like
[8:18] that we can map them onto our metal texture.
[8:22] Let's start over here at the top.
[8:24] Let's load up our UV unwrap.
[8:27] Select our trim sheet.
[8:29] Just to make things organized I'm going to temporarily move all of this away.
[8:34] And let's say that we want to go ahead and start by UV unwrapping just this top section.
[8:39] You can select your section.
[8:41] Press iron in this case and then I also always like to relax it a bit.
[8:46] And then move it to our trim sheet over here.
[8:50] Now at this point what I like to do is I like to set this into the corner as much as possible
[8:55] so that it is just touching the top so that I can get the most of my resolution out of
[9:00] this.
[9:01] And I will make the window a bit bigger for you guys.
[9:03] And then I hold CTRL and I evenly scale it all the way down or up in this case like you
[9:09] can see over here.
[9:11] I need to scale it a little bit further back over here.
[9:15] And every 3D software does also have a function where you can show the tiling of your mesh
[9:20] to make it easier to preview.
[9:22] Now you can see that instantly our texture over here has been applied.
[9:27] Luckily, because this texture is so generic we can even just select the second section
[9:33] and that is the key goal to also keep these textures very generic with very little specific
[9:37] details so that when we go ahead and place another one over here the seam that will be
[9:45] created whenever we repeat this will be barely visible.
[9:48] So we are going to nicely go ahead and go up here and scale it up again.
[9:53] And if I would go ahead and collapse this and then have a quick look up close.
[9:58] Once again these seams are a visual bug but you can see that your seam is barely visible
[10:02] over here which is great because inside of Unreal Engine it will be even less visible
[10:08] because it is so far away.
[10:10] Make sure to UV unwrap your assets based upon the context in your scene.
[10:15] If it is very close to the camera you want to be a little bit more precise with your
[10:19] UV unwrap but if it is very far away from the camera like over here you can easily be
[10:25] a little bit more relaxed with the rules.
[10:28] Now let's go ahead and kick in a quick time lapse where I will show you how to UV unwrap
[10:32] this really large section over here.
[11:15] I want to finish things off by showing you some additional techniques that you will often
[11:33] come across when UV unwrapping with trim sheets.
[11:36] The first one is that sometimes instead of deforming your trim sheet to your mesh you
[11:42] actually want to deform your mesh to your trim sheet.
[11:45] So let's go ahead and say that we have this plane.
[11:47] I want to go ahead and I want to UV unwrap this plane like normal by selecting it, UV
[11:53] unwrapping it and in this case I already have some pre-made details that I placed inside
[11:58] of my trim sheet over here.
[12:01] So I can go ahead and map this from let's say this point over here and then I want to
[12:06] just nice scale this down a little bit.
[12:11] I will tell this and maybe like manipulate the scaling a little bit until it fits.
[12:16] Now once you've done this you can just simply edit your geometry in order to make this fit
[12:21] a little bit better.
[12:22] I do this by simply adding some additional loops wherever I have placed my edges and
[12:28] luckily for me I'm able to see these edges thanks to the edge damage that I placed and
[12:34] then I select the faces that I want to edit for example these two over here.
[12:40] Push them back like this and then maybe what you can also do is you can also go ahead and
[12:46] give it a few little baffles just to add some weighted normals over here and there we go.
[12:57] So now if I go ahead and turn off my edge and faces I now instantly have created this
[13:01] interesting looking detail.
[13:03] The second one that I want to show you is that I have this really thin edge over here.
[13:08] If we go ahead and open up our UV and go into our trim you can see that this edge has been
[13:13] mapped to this very small thin detail that I have placed in my trim sheet.
[13:18] I like to call these construction lines.
[13:21] You can see that these construction lines are placed all over this mesh over here and
[13:25] they will simply add some additional visual interest to our mesh because in real life
[13:31] you would rarely have such a large metal structure that is made out of one solid piece
[13:37] of metal.
[13:38] Often it is made out of panels and that is what these construction lines are here for
[13:42] to make it seem like this large mesh has been made out of panels without actually having
[13:47] any type of unique textures.
[13:50] Next this you can also place details in your trim sheet like we have done over here and
[13:55] that is as simple as then going into your 3D modeling software creating a simple plane
[14:01] wherever you want like let's say over here and placing the plane just in front of your
[14:06] mesh.
[14:07] At this point you can UV unwrap the plane by going ahead and opening up your UV unwrap
[14:14] tool showcasing your trim sheet as always unwrapping it and then mapping it on whatever
[14:23] text or other detail that you might have created like this.
[14:27] Then I can of course go ahead and now fit everything a little bit better just to make
[14:32] this a little bit nicer.
[14:34] Once you do this and you go into a wheel as long as you have an alpha that cuts out these
[14:39] decals and you apply this to your material you can instantly place these decals all over
[14:44] your mesh to add some additional details to this.
[14:49] And finally this might be a little bit more un-wheel specific but what I did is I layered
[14:54] a grunge map on top of my details over here to just give some additional variation to
[15:00] my texture going from clean to something that looks a little bit more dirty.
[15:05] This is one additional grunge map texture that will not take up a lot of memory in your
[15:10] scene so it is a great way to just like add an extra bit of detail.
[15:14] However, I would say that clean still works very well for this asset also.
[15:20] That was about it for this small tutorial video.
[15:22] I hope it was useful and I hope to see you next time.



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
