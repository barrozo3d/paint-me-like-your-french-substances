---
title: Creating a Leather Material for Footwear with Anchor Points in Substance 3D Painter | Substance 3D
source: YouTube
url: https://www.youtube.com/watch?v=xXad_mS7K9s
author: Adobe Substance 3D
ingested: 2026-08-13
app: "[PENDING]"
version: "[PENDING]"
tags: []
extraction_status: pending
frames_dir: tutorials/frames/creating-a-leather-material-for-footwear-with-anchor-points-in-substance-3d-pain/
frame_count: 0
frame_status: pending-selection
---

# Creating a Leather Material for Footwear with Anchor Points in Substance 3D Painter | Substance 3D

**Source:** [YouTube](https://www.youtube.com/watch?v=xXad_mS7K9s)
**Author:** Adobe Substance 3D
**Duration:** 20m42s | 1 section(s)

---

## Raw Data (for Claude Code extraction)

Frames are not captured yet. Read the timestamped transcript below, pick moments
that actually show a technique/result worth a still (not blind percentages —
even within a named chapter, verify the real moment against its timestamps), then run:
  python select_frames.py creating-a-leather-material-for-footwear-with-anchor-points-in-substance-3d-pain <ts1> <ts2> ...
(seconds or mm:ss). This appends a "Captured Frames" section and updates the
frontmatter before you write the Structured Notes below.


### Full Content [0:00]
**Transcript (timestamped):**
[0:00] Welcome to this multi-part tutorial series where we will go over on some more advanced
[0:12] techniques on how to use anchor points in your project.
[0:16] This series is a follow up of our basic anchor point series which you can find on our channel.
[0:22] In this video we will go over on how to create this very nice leather effect that you can
[0:26] see over here.
[0:28] We will place special focus on how to create some roughness variation, how to add some
[0:33] extra folds along with the color in these folds and also how to add some basic edge
[0:38] highlights, dirt and some other generic highlights as you can see over here all with the use of
[0:44] anchor points.
[0:45] So let's go ahead and dive right in.
[0:49] So what are anchor points?
[0:51] Anchor points are a powerful feature that lets you reuse a part of your layer stack.
[0:56] This means that you can define a mask or layer once and reference it dynamically in other
[1:03] layers.
[1:04] If you change the anchor point, all references are updated as well, letting you work smarter
[1:10] and faster.
[1:12] So let's get started.
[1:13] So what I have here is our base shoe and it just has a simple base leather material that
[1:20] is placed into a folder that has a color selection mask which will basically just control wherever
[1:25] we want to have our leather.
[1:27] Now what we're going to do is we are first going to get started by just improving the
[1:31] look of our leather a little bit because right now it does not look very good.
[1:36] So let's go ahead and let's start by adding some roughness variation.
[1:40] However this roughness variation will also double as our base anchor point.
[1:45] So let's get started and add a fill layer over here and just call this like leather
[1:53] roughness base over here and all we really need to do is we just need to go ahead and
[1:58] we need to grab only our roughness over here and let's give it a bit of a shine.
[2:05] So let's have a look.
[2:08] Yeah I quite like this.
[2:09] Let's do around 0.45.
[2:12] That seems like quite a nice shine or maybe like 0.4.
[2:17] There we go.
[2:18] Okay now what we want to do is we want to go ahead and add a mask, a simple black mask
[2:23] and then we want to add an ambient occlusion generator which will basically make sure that
[2:28] the roughness looks a little bit duller around our occlusion areas.
[2:33] So if we go in here we can go ahead and add a generator over here and then you can simply
[2:40] go ahead and grab the ambient occlusion generator like this.
[2:44] And with this one here you can see like it's a little bit duller.
[2:47] It's not perfect yet so let's go ahead and just improve it.
[2:50] The first thing that you will always notice although it might be a little bit difficult
[2:53] to see here maybe if I add my color.
[2:56] Yeah here see if I add the base color you can see ambient occlusions they always are
[3:01] a little bit dotty.
[3:03] I don't know how to say it like noisy like you can see like these small dots here.
[3:07] So let's go ahead and improve that by simply going in here adding a filter and adding a
[3:14] blur to this filter.
[3:16] And then you can see that that often gives us like a slightly nicer transition.
[3:23] And then what I want to do is I'm just going to add an extra levels on top to basically
[3:27] remove most of my occlusion around these areas to make it look a little bit duller wherever
[3:33] we have our occlusion.
[3:35] So let's go ahead and add the levels and like push the black slider of this levels down
[3:40] a little bit.
[3:41] Here we go.
[3:42] It might look very dramatic but don't forget that as soon as we turn off our color here
[3:47] see that looks quite nice because you do not get the roughness around these areas.
[3:52] Also one thing to keep in mind that is once again easier if you visualize with your color
[3:56] is that right now we have our laces over here that are also being included which is not very
[4:01] nice.
[4:04] For this what you can of course do is you can always go down here and add a custom paint
[4:08] layer so that you can do some custom painting.
[4:11] For example if we go to our brush and grab a basic soft brush simply press X to flip
[4:17] to a black color and then oh sorry press X to flip to a white color I mean and then
[4:23] you can go ahead and you can paint out this laces occlusion that you can see over here.
[4:29] If you want to go ahead and ignore the laces during the painting you can always click on
[4:33] this little box here and turn off your laces.
[4:37] When you do that it will simply ignore those and it makes it easier for you to paint around.
[4:41] So that's just something I wanted to show you over here.
[4:44] The reason that I'm showing you now is because we are going to add an anchor point and you
[4:49] always need to do this before you add your anchor point.
[4:53] So now what we can do is we can just go ahead and turn off the color and then we can go
[4:57] back into our mask and start by adding our anchor point and I'm just going to go ahead
[5:01] and leave the name the same so that I can easily reference it later on because we will
[5:06] be referencing this quite a bit.
[5:09] So the next thing that we want to do is we want to go ahead and add some extra leather
[5:13] details like some edge highlights, some dirt and just general details like that.
[5:19] For this what I like to do is I like to create a new folder just to keep things nice and
[5:23] organized and just go ahead and call this leather details over here and once we've done
[5:31] that what we can do is we can get started with some edge highlights.
[5:35] For this we just want to go ahead and grab a simple fill layer and just call this edge
[5:41] highlights over here and then in this fill layer what we want to do is just go ahead
[5:46] and turn everything off except for once again our roughness and our color.
[5:51] Now these highlights are quite easy all we need to do is just add a simple black mask
[5:56] and then if we go to our smart generators over here we can go ahead and sorry I mean
[6:02] smart masks of course we can go ahead and just find something that we like.
[6:07] Let's see for example let's say an edge is dusty over here as you can see here it gives
[6:12] us like a nice dusty effect and you can always go ahead and just play around with your balance
[6:16] to make it stronger or less strong.
[6:20] Next I want to go back into the fill layer and I'm just going to go to my base color
[6:26] and I'm just going to go ahead and play with my base color.
[6:28] If you want you can also use a color picker to get started and let's just make this like
[6:33] a little bit darker so they are edge highlights but they are not as much highlighted as being
[6:39] like just some darkening over here so I should have called it edge darkening.
[6:45] Now I would say that maybe like tone down my roughness a little bit more so that it looks
[6:49] a little bit duller and we can also go ahead and go back into our mask editor and maybe
[6:54] like push it up a little bit more like this.
[6:57] So that will just already like give us some darkening which gives us like a nice dirty look.
[7:03] Next what I'm going to do is I'm just going to add some general dirt this is always a
[7:06] good one to add.
[7:08] Let's add a fill layer and just call this dirt very easy and we are once again going
[7:13] to go for our roughness and set this to be quite dull.
[7:16] I always like to make my dirt quite dull.
[7:19] As for the color I'm already going to like set it to be like a brownish color but we
[7:23] will always just go back in and just balance it out.
[7:27] And then add a simple black mask.
[7:31] At this point I want to get started by referencing our leather roughness base because we can
[7:37] use this ambient occlusion to improve our dirt so that we have dirt specifically around
[7:43] our ambient occlusion areas.
[7:45] To do this we can just go ahead and add a fill, go to our grayscale anchor points and
[7:51] add our leather roughness base over here.
[7:54] You can already see it happening a little bit.
[7:58] Next we are simply going to press this little input button over here and that will give
[8:02] us control a little bit more over like where our dirt is.
[8:05] Now you can of course also play around a little bit more with your levels to increase or decrease
[8:09] it but I'm not going to play around with it too much.
[8:13] Now this does not look very good so what we're going to do now is we are going to go ahead
[8:18] and add a generator on top of this and this generator if we just go ahead and grab a simple
[8:25] dirt generator like this you can see that it already has like this extra dirt.
[8:30] Now I don't want to have this dirt everywhere so as soon as I set my dirt generator to multiply
[8:36] it will combine with my ambient occlusion to basically make my ambient occlusion almost
[8:42] like a dirt effect, almost like a nice dirt look over here.
[8:48] So what I mean is it will specifically add this dirt to our ambient occlusion so that
[8:52] it does not look so smooth anymore.
[8:55] Now at this point you can play around a little bit more with your levels if you want to increase
[8:59] or decrease the dirt and one thing that I do notice once again is that over here you
[9:04] can see that everything looks very noisy so let's go ahead and add an extra filter on
[9:10] top with a blur and just give it like a slight blur over here.
[9:16] It is no problem in this case because often with leather it is not like a very specific
[9:21] dirt but it's like a faded dirt.
[9:24] At this point we can just go ahead and we can play around with our base color to make
[9:28] it more or less strong, just play around and get whatever you want like a base color like
[9:34] this looks quite nice and I do like that my roughness is looking quite dull and you can
[9:38] see that we already are adding a little bit more texture to our shoe over here.
[9:45] So now that we have done this I want to go ahead and add some more highlights but these
[9:50] are going to be like overall highlights.
[9:53] So what we want to do is we want to go ahead and add another fill layer, call it overall
[10:00] highlights over here and let's go ahead and make the roughness to be probably like a little
[10:06] bit shiny still and for our base color I just set it to fill white so this is almost going
[10:12] to be like the white fade that you often see on leather.
[10:16] Then what we want to do is we want to go ahead and add once again a simple black mask but
[10:21] this time we are going to reference once again our leather roughness base anchor point.
[10:29] So let's go ahead and let's add a simple fill over here, reference our leather and what
[10:38] I want to do is I want to play around a little bit more with my levels over here to make
[10:46] this look quite strong.
[10:49] If you get this effect which might not look very nice although it will most likely not
[10:53] be that noticeable you can always go in and just paint a little bit more over here see
[11:00] just to blend it in a little bit better or make your brush a bit smoother but I will
[11:03] show you like a way that we can easily like just remove this ugly looking spot over here.
[11:11] The way that we are going to do that is we now have a fill over here that's totally fine.
[11:15] I now want to go ahead and I want to add another fill but this fill will have a grunge map
[11:21] so we can go into our textures and we can go down and just grab something that you think
[11:25] looks nice so I'm going to go because we have a lot of like smudgy looking grunge maps over
[11:31] here which I think feel like quite fitting for leather.
[11:35] So let's for example grab our grunge wipe smudgy soft over here and then what you want to
[11:41] do is you just want to go ahead and first of all set the blending mode to multiply and
[11:48] set the scale to maybe like I don't know it's 10 too much now 10 looks about fine and then
[11:54] you can also go ahead and you can play around a little bit more with like your balance and
[11:58] finally in general I would say just go ahead and tone everything in your overall highlights
[12:04] down so we got this one let's see if we can maybe like push around these areas a little
[12:10] bit more like this and let's see if I can make my smudgy effect maybe with my contrast
[12:16] like a little bit stronger just trying to get like a nice look something like this quite
[12:21] nice so you can see that it is really only around these areas over here.
[12:28] Next you might get a seam like you can see over here if you have this simply set your
[12:32] projection from UV projection to try planar projection you might need to then go ahead
[12:38] and like play around a little bit more with your scale because it has become a bit smaller
[12:42] but the type planar will not look at your UV so it will just properly project even if
[12:46] you have seams.
[12:48] So now at this point click on your overall highlights go down here into the opacity and
[12:53] just tone this way down to something like let's do something like around 10 I think
[13:00] seems fine or maybe like 15 here see and then we can also go ahead and we can play around
[13:07] a little bit more with our roughness just to see whatever looks best.
[13:12] Okay perfect so now we have quite a nice base leather now what we are going to do is we
[13:17] are just going to go ahead and add some extra creases just to make the leather feel a little
[13:22] bit more worn out so for our creases and folds let's go ahead and use this area as like an
[13:28] example what we are going to do is we are going to get started by creating the height
[13:34] part of it and then later on we will also add some extra colors and also even some extra
[13:38] dirt to our creases and folds so I'm going to get started by adding a fill layer and
[13:45] just go ahead and call this folds underscore height for example and all you will need to
[13:51] do is only turn on the height map now you can already give the height map like a little
[13:56] indent but what you will always see happening is that it will break our model and the reason
[14:00] for this because we currently have tessellation turned on so it will be in actual height so
[14:05] what I want to do is I'm just going to add a black mask and then on top of this black
[14:09] mask I want to already paint in just a shape so let's grab a basic soft brush and let's
[14:15] say that I want to paint in my creases and folds around these areas this will look very
[14:21] bad in the beginning but don't worry so let's say that I just have them here and it is just
[14:25] like an quick example of where I want to have them the first thing we need to do is we need
[14:31] to improve our outline over here and have it like really nicely fading into the rest of the shoe
[14:37] the way that we can do this is by adding a filter along with a blur and just making the blur
[14:44] quite strong like you can see over here see that will give us like a really nice transition
[14:49] for what we are going to do next which is adding our actual creases so to do that all we need to
[14:55] do is we need to add a simple fill and then in our grayscale we want to go ahead and want to select
[15:01] a creases texture so let's go into textures let's type in creases and let's grab our creases soft
[15:10] over here this one will do the trick just fine so you want to go ahead and drag it in here
[15:15] and then what we need to do is let's first of all set the scaling to something like 10
[15:21] and then finally right now the direction is all over the place like these ones are going sideways
[15:25] these ones are going up I don't like that so I'm going to go into my projection and set my
[15:31] projection from UV projection to try planar once I've done that you can go ahead and you can play
[15:36] around a little bit more with your scale let's say that I'm going to set it to like a seven or
[15:42] maybe like eight and of course what you can do is if you press E you can also play around with
[15:47] your rotation thanks to the try planar so we can give it like a little rotation to go along with
[15:53] our shoe if your shoe just think about the story telling how your shoe is often walking around and
[15:59] where the creases will happen they will often happen around these joints and around the front
[16:04] over here so now that we have done this we want to go ahead and we want to make sure that it only
[16:10] shows up wherever we have painted our mask we can simply do this by setting this from normal
[16:17] to multiply and now you can see that the creases only show up wherever I have painted my mask
[16:22] and I can also go in here and I can simply grab my basic soft and I can easily just paint in more
[16:28] or less creases wherever I want just like that now what I'm going to do is I'm just going to very
[16:34] quickly off camera paint in my creases in some nice areas and then we will just go ahead and continue
[16:41] okay so here we go now if you feel like your creases are looking a little bit too strong
[16:46] you can always go into your creases soft and just tone down the opacity a little bit like this
[16:51] so now finally what we need to do is we need to add a simple anchor point on top of this
[16:56] so that we can reference these these creases into our dirt and also into some general color
[17:02] and that is what I want to do next I want to go ahead and just give our creases or our folds
[17:07] a little bit of like a color so that we can see it a bit better so let's go ahead and add another
[17:12] fill layer and let's just call this folds underscore color and then we can just go ahead and add a
[17:19] simple black mask and now what we want to do is we want to probably use a nice mask generator for
[17:23] this so let's go into our smart masks over here and I'm just going to go ahead and just going to
[17:29] find like a nice little generator that really improves our curvature let's for example go for
[17:35] like a dust occlusion over here that one often seems to work fine and then if we go ahead and go
[17:42] into our generator what we want to do is we want to go ahead and we want to reference once again
[17:47] our folds anchor point over here once this is not the leather roughness anchor point but our actual
[17:53] folds so if you go in here you want to scroll down to your micro height and then you want to go to
[18:00] anchor points and grab your folds height once we've done that we do need to turn this on so let's go
[18:06] into our micro details and turn on our micro height and now you will see it's working now I actually
[18:12] want to go ahead and right now it is generating on top of the creases so I want to go down and I
[18:19] want to invert my micro height so that it is generating the dirt inside of my creases like this
[18:26] so here you can see that we can like add some general dirt you can of course play around with
[18:30] like your a o depth to increase or decrease everything sometimes your a o radius also gives you
[18:37] like a nice effect but this is looking pretty much fine to me now what I want to do is I want to go
[18:43] back and I want to make my color to be almost like a dark reddish color this is what you often see
[18:50] in like leather like a dark red color let's turn off everything else except for maybe also our roughness
[18:56] let's give it some roughness that is a little bit duller and then simply go back into your dirt and
[19:01] here you can go ahead and you can play around with your intensity to get like the effects that you
[19:08] want so I don't want to have this too strong so I'm just going to go ahead and play around a little
[19:13] bit more with like my intensity here we go like this and you can always go into your dirt and you
[19:19] can always like use your opacity to also increase or decrease this something like this it's just
[19:24] like a nice subtle effect as you can see over here now finally to finish things off what I want to do
[19:31] is I just want to also include my dirt in these creases and folds so if we go back into our leather
[19:37] details we can go into our dirt and let's go ahead and just add a new fill but of course what you
[19:43] want to do is you want to go ahead and just drag this fill below all of our dirt generators and our
[19:48] blur now in this fill all I need to do is I need to reference my folds with our anchor point and then
[19:56] go ahead and set the mode from normal to art so that it will also add this dirt on top of it and
[20:02] you can always here see you can kind of like play around a little bit more with your here see it's
[20:08] very subtle but it is there and that's the point of it so you can play around a little bit more
[20:12] with your levels if you want but in general once you've played around with all of that you have
[20:17] this very nice and flexible leather material that you can also use anywhere else and all you
[20:22] really need to change is you would need to change where you want to paint in your folds whenever
[20:27] you use done a different material and maybe paint in in or out some ambient occlusion
[20:33] so that was about it for this tutorial I hope that you liked it and I hope to see you next time



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
