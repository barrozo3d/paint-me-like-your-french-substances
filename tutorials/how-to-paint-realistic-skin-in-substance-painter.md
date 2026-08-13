---
title: How to Paint Realistic Skin in Substance Painter
source: YouTube
url: https://www.youtube.com/watch?v=jrDHqY96beY
author: FlippedNormals
ingested: 2026-08-13
app: "Substance 3D Painter"
version: "not stated on screen"
tags: [layers, fill-layer, paint-layer, masks, procedural, tri-planar, blend-mode, alpha, basecolor, color-management, advanced]
extraction_status: complete
frames_dir: tutorials/frames/how-to-paint-realistic-skin-in-substance-painter/
frame_count: 13
frame_status: complete
frame_selection: content-anchored (manual timestamps chosen from transcript, not blind percentages)
---

# How to Paint Realistic Skin in Substance Painter

**Source:** [YouTube](https://www.youtube.com/watch?v=jrDHqY96beY)
**Author:** FlippedNormals
**Duration:** 29m47s | 5 section(s)

---

## Raw Data (for Claude Code extraction)

Frames captured — see "Captured Frames" section below.


### <Untitled Chapter 1> [0:00]
**Transcript (timestamped):**
[0:00] Hi, this is Henning from FlickNomers and in this video we are going to go through how to create the skin texture for this character.
[0:09] This is going to be a really interesting video showing you really a solid breakdown of how you can create textures like this.
[0:14] Now, before we get into the video, I want to talk to you about our latest masterclass called Realistic Character Portrait Masterclass,
[0:21] where we show you how to create this whole character start to finish, including real time showing you how to create the textures,
[0:29] which we're covering in this video. We really cover everything from the first sculpting stroke in C-Rush to painting all the maps in Painter,
[0:37] setting up the skin shader in Blender, and then rendering the whole thing in Cycles in Blender.
[0:42] So if you're interested in that, please check out Realistic Character Portrait Masterclass.
[0:46] Skin texturing is a pretty big topic and we're breaking down basically into just a color map in this video.
[0:53] But one more thing we do want to talk about before we get into how to create a color map is that if you have a solid model beforehand,
[1:00] if your model is in a good spot with all the mid frequency and high frequency, all the kind of stuff,
[1:05] texturing this model is going to be so much easier.
[1:09] Texturing a model like this that has all the frequencies in here, you can see it has all the scars, the eyes that I find,
[1:15] it has pores and pimples and everything. Texturing this is so much easier than texturing something that's underdeveloped.
[1:22] This is not a discussion whether you should do the pores in C-Rush or Painter. This is more a discussion of
[1:28] you need to just be sure that your model is in a good spot. Please don't rush into texture painting.
[1:35] You are really going to do yourself a disservice. A model like this can usually be texture painting with some simple gradients,
[1:40] some procedures on top and a little bit of hand-pain here and a bit of projections.
[1:44] But if this model was not in an acceptable spot, you would have to open up your black book of tips for
[1:52] texturing. This is where you have to do an insane amount of projections. You'll have to do all sorts of
[1:57] hacky things in LookDev. Overall, you're really just adding complexity to something that really should be fairly straightforward.
[2:04] So one of the things I really want you to take away from this video is make sure the model is in a really good spot.
[2:10] So in Painter now, we just really have one fill layer on the bottom called Temp. And this is something I always put on the bottom
[2:16] just to have a base color. I usually actually make this quite a saturated color just so we have something crazy,
[2:23] so we can really see if something is going through. And this would also have all different
[2:28] challenges as well. So height, roughness and scattering, just so that you can make sure that
[2:32] you really have a base. There's nothing, nothing is going to surprise you later on.
[2:36] And then I make a folder called Color. And then in this folder, I just make a new fill layer and I call this
[2:42] base. And this is going to have our main skin tone. The advantage of this workflow is it's pretty procedural.
[2:48] And it means that we can change this base color later on. If you, if you're not happy with this base,
[2:53] you don't have to go in and like grade something, create crazy masks, you just go in and you just change this.
[2:57] And this is going to update everything. So the exact color we pick right now is not absolutely crazy important.
[3:04] It is important in the general range, but you can always change this later on.
[3:09] So we're going to pick something like this, which is quite desaturated, but you know, it's a little
[3:14] bit of saturation in it. And then you can just change the hue here as well. So I'm going to pick
[3:18] something about this color. And then we are just going to make sure this is only color. So just
[3:23] all click on the color, we don't want anything else. The way I'm organizing my projects is that I'm
[3:27] making one folder, one group for each channel. And then these will only contain the channels needed.
[3:34] In terms of pure performance, this is not crazy optimized, but it's very easy to read the project.
[3:38] This is not optimized for computers, it's optimized for humans. So if you open this up later on, it's
[3:43] quite easy to get into. So we just make sure this is in here, we can do that just by clicking the
[3:47] folder icon. And then we are making a new layer, or you can just duplicate this one, control D.
[3:52] And we're going to call this red. And this is called red, because it's going to be red. And we're
[3:57] just going to go through and make a few different colors here. So we're going to be having red,
[4:03] some maybe green, some yellows, and just overall bringing down a color variation through
[4:08] fill layers like this. So just make this a kind of a muted red color. And then we are going to
[4:14] right click on it, add a black mask. And in the mask, you just have to make sure to go under
[4:20] and create a paint layer. Because this now means that you can now paint in where you want everything
[4:25] to be. Make sure the symmetry is indeed enabled. And also that we go in and we just destroy this
[4:30] one show in our intersection, we don't want that. And then you can really start to paint. Now,


### Favorite Brushes [4:34]
**Transcript (timestamped):**
[4:35] before that, I'm going to show you my favorite brushes for painting skin, we are going to start
[4:38] off with a brush called dirt to dirt to is a fantastic general brush for just costing overall
[4:45] mayhem when it comes to painting skin is fantastic, because it has a lot of specificity,
[4:50] meaning like pen pressures enabled by default. So you can go and you can get really specific nice
[4:55] shapes. But it also means that you can just create a lot of variation here, you can also just disable
[5:00] pen pressure up here in the size and enable in the flow. And now you get this really nice and
[5:06] opacity driven brush. So this is super cool. So I reuse this a lot when creating just general skin.
[5:13] This is one of the brushes I use the most. And here you can see the workflow. Basically,
[5:17] the only thing you're doing is you are just creating a layer, and you're making a paint and
[5:21] then you X key, just go between these two, between black and white, where black is going to erase,
[5:26] and white is going to be adding to it. So this is really, really fast when it comes to just
[5:30] blocking in your paint. And then we have the dots brush dots is fantastic for
[5:34] adding like general pores and such and just creating a lot of variation here. You see what
[5:38] this is doing. This one is going to not just like create like a like a measles outbreak or like
[5:43] chicken pox outbreak is actually going to be really good for creating a base of skin, like all
[5:48] other freckles and such. What we can do instead of just being additive like this, you can go over
[5:52] this and remove a lot of stuff. And this just means that you get a lot of really, really lovely
[5:57] variation. And then we have dots erased, which is similar, but it's it's a little bit more subtle.
[6:03] This is one of the brushes actually used the most, because this blends a little bit nicer. You can
[6:08] see up here that these are very specific or regular dots brush. And that's a race just makes it a
[6:12] little bit more organic. It has a bit more opacity variation inherently built into it. So we use
[6:18] this actually a lot in the full masterclass as well. So it does erased fantastic. And then we have
[6:24] a brush called the cracks brush. I'm just gonna kill this layer and gonna make a new one.
[6:30] And here we go. And the cracks is really good for creating overall variation in like it looks
[6:37] like veins. So here you can just see that we just create get this like really nice,
[6:43] veiny pattern from this, you know, you don't necessarily want to do this with the red
[6:47] layer. You want to do this maybe more in blue. But it's really solid for just creating a lot of
[6:51] nice variation. And then we have the cotton brush, you want a few smooth brushes as well.
[7:00] So for that, we have cotton and we have a smoothie smooth noise. And and this is really good because
[7:06] it allows you to just create nice smooth gradients on the model like this. But you can see it has
[7:12] some texture to it. So you can very easily go in and just add stuff and subtract stuff like this.
[7:17] But with a little bit of texture, I don't prefer, at least we're going for realism,
[7:21] I don't prefer to have something be just crazy smooth. Just because you just need texture in
[7:27] what you're doing. And then we have the smooth noisy. And this is very similar to this one.
[7:31] And this allows you just to create like really, really soft brushes. This is inspired by a brush
[7:38] I used in Mari called super smooth. And this is just fantastic if you really just want some crazy,
[7:46] smooth gradients, it has a little bit of noise in it, which is awesome, because it just,
[7:51] it just makes it look a little bit more organic. But it's just really good for creating this nice,
[7:55] soft gradients. Then we have the mold brush and the mold brush is awesome for creating an overall
[8:00] base. This is something I've been using a lot when I just want to create like, not even just like
[8:05] some grunge textures, just some quick variation, because you can quick just see how fast you can
[8:09] create some nice variation with this brush. And again, the real magic really goes and go in between
[8:15] the X key or go in between black and white here in the bottom. So going in here and then
[8:22] just adding this. Also the topic of brushes is of us when there's always going to be some brush
[8:29] we haven't you haven't used before. So if you have a favorite brush, please let us know in
[8:33] comments, I would love to hear which brushes you're actually using because I'm probably going to
[8:37] integrate some of those into my own personal workflow. And then we have the last one, which is
[8:41] the dust brush. So just adding a new paint layer and the dust brush is fantastic for just creating
[8:46] a bit like subtle variation, some little splotches on top of everything like this. So this is really
[8:53] a solid brush for for just going through and just creating subtle variation like you can see here.
[8:58] And again, you can go over this with the value of enabled the black mode or you know, just
[9:04] switching the brush to black so you can use the erase stuff. So the dust brush, fantastic. So these
[9:10] are really all the brushes you need, of course, are a lot of really cool ones like there are a
[9:13] whole section here called Kydles brushes, where you just have a lot of really cool stuff. These are
[9:18] all based on like Photoshop brushes. So there's a lot of really cool variation in these ones as well.
[9:24] So that's it for the brush section of this. So let us move on to my overall workflow for this.


### The Hand Painting Workflow [9:28]
**Transcript (timestamped):**
[9:31] So I'm going to show you generally how I work. So we just have to make sure that we have a paint
[9:36] layer in here. And then that symmetry is enabled. And then I'm going to just make sure we have the
[9:41] mold brush. And then I'm just going to go through and just some quick variation here. I tend to
[9:45] work around the eyes first, basically, adding some value variation around the eyes, adding some
[9:51] value variation around the nose, and some around the mouth as well, and some around the ears,
[9:57] because these are the most obvious areas for where you want some red.
[10:01] And then we're just blocking this out. And like, don't be too shy at this stage. Like, just go a little
[10:09] crazy with this. You want some overall coverage, because this is going to be the base of a lot of
[10:14] things we are creating later on. Now, obviously, in this video, we can't create the whole thing,
[10:19] which you can obviously see from the length of this video. But we are covering the main steps.
[10:25] It's really the same thing over and over again. So there's a lot of labor involved, where you just
[10:29] have to just work up all the different parts. But the main workflow is the same, which is create
[10:35] a fill layer, make a mask for that, and then have a layer inside this. Also, this is procedural. So
[10:41] this means I cannot go in. I can change this to actually be a bit more red, because this was a bit
[10:46] too brown before. So I'm just going to make this a little bit more red, like so. And then after you
[10:52] done this, make sure you go into the paint layer again. So this is a really solid workflow. And
[10:57] it's really fast as well once you get used to it. So I'm just going to go in and just create some
[11:02] variation around the lips, just so we can get the main lips in here as well.
[11:08] Cool. And then I'm going to go over with dots erased. And I'm just going to really like add a
[11:13] lot of variation to this. Now, we're not going to take this specific layer too far, just because
[11:20] this is going to take a long time. In the chapter for the mask class, this chapter here was around
[11:25] half an hour long. So that's how long it would take to create just this one layer. Overall,
[11:29] I think the main texturing part for the whole thing for the skin maps was made by around three,
[11:34] four hours or so. So you can do it quite fast if you know the overall workflow for it. And of
[11:39] course, if you have some in reference for this as well. But you can see like how quickly you can
[11:43] just create a lot of variation with this, just with now we just use two brushes at this point.
[11:48] Just go over this and go in with the white and black. And again, you can also go in,
[11:56] you can change the base color as well. So you can very easily just change this at this point,
[11:59] which is super useful because a traditional workflow has been more
[12:04] project photos. And then you gray the photos and all that, which is of course,
[12:08] a really valid way of working. You get a lot of variation that way. But you end up with a lot of
[12:14] color selections, you have to do a lot of masks and such for this. But if you want to
[12:18] now change everything at the end of the project, meaning you want to change the whole
[12:21] color scheme of your character, you don't have to do that by grading something necessarily,
[12:26] you can of course, but you can just go in and change the color of the fill layer. And this is
[12:31] a really powerful way off of working. You can also see as well, like the Dots of Rays part is
[12:36] awesome because it means you can get big strokes like this, big color changes, but you can also
[12:41] go in like this. And you can really add a lot of subtle variation as well, more specific variation.
[12:48] So you can go in and just make sure these are a lot smaller, like so. And then you can go in with
[12:55] a little bit of like dust as well. And just right here, here's something to just add in
[13:00] painter as well recently you see here, we have favorites now, so you can just right click and
[13:03] just add to favorites. And then you're going to pop up here right on top, which is super useful.
[13:08] So just adding a little bit of dust as well to this, which we'll really just make sure this pops.
[13:16] And this is what the finished red map looks like, you see it looks quite different what we
[13:19] had before. Basically, the only difference is that we've balanced the base color and we have a
[13:25] different color for the red, and we just have a more variation and more refinement in the actual
[13:31] mask itself. You can see if we hit the Alt key, this is this is what we have for the actual mask,
[13:36] like it's just really nothing too fancy going on here. It's just a black and white mask that we
[13:41] just painted from scratch. And then we are starting to add more layers to this, this is where we are
[13:47] not going to show any more actual painting, because this would just take ages. But what we're
[13:51] doing, we're just building this up step by step. So now we have a layer called redder, where we're
[13:55] just adding a bit more variation into this. And then we're going in and we're adding yellow to this,
[14:00] then we're adding a little bit of blue to this. And you can see the approach is exactly the same
[14:04] as before. Now you can just see that the blue is just dots of rest going and going in here and just
[14:09] adding blue in certain areas. And then we have one called darker. And this is where we're just going
[14:15] in and just making this a little bit darker. It's important to add some value variation as well,
[14:20] because a color variation by itself is of course useful. But a lot of things are just brighter
[14:26] or darker. So this is really what it looks like when I'm done hand painting, meaning at this point,
[14:32] I've controlled absolutely everything myself by hand. So we've just built this up layer by layer.
[14:39] And no procedurals, no photo bashing on top, just straight up paint everything by hand.
[14:45] You can also see he has horns as well. We're not covering this in this video at all. So what
[14:49] you're going to see we just making a little bit darker around the base as well. The reason I
[14:53] like this approach is because it's it's simple. 3d is really hard as it is. You know, we were dealing
[15:00] with a bunch of different software on daily basis, bunch of different hotkeys, the software we're
[15:03] using is they're hard to use. And just keeping it as simple as possible is really going to make
[15:09] your life a lot easier. It means that you can, for instance, go into this scene, like two years
[15:13] after you made it, and you can understand what's going on. You understand that well, red is probably
[15:16] going to be the red one, the blues can be the blue one. And you can keep changing this, you can keep
[15:20] grading this up. And it just means that your workflow is nice and simple to use. It also is
[15:27] highly scalable because you can use this on any kind of character if you're doing a guy like this,
[15:32] who's some kind of like more a bit more for humanoid monster character, or if you're doing
[15:36] something straight up out of like Diablo, or if you're doing like a realistic baby human or anything,
[15:42] like you know, this this technique works for everything. Because basically, it's just breaking
[15:46] down the texture into a few different colors, where we need a basic color, what is the overall
[15:50] color, basically what kind of what's the melanin level, and what is the skin damage done to it,
[15:55] and what is the overall variation of the of the skin. And then we're just breaking down into
[16:01] some areas of red, some are redder, some are yellow, some are blue, some might be a little bit green
[16:06] as well. In terms of working based on the old color zones of the face, I am concerned about
[16:14] that, but not like 100%. Meaning that you can see here, the mouth area is a little bit more blue,
[16:19] the area areas around the bones are a little bit more blue, a little bit more yellow, the areas
[16:23] where there is a lot of blood there, but a bit more red. But it's not like I'm religiously going
[16:29] towards those. If you were to actually observe a human face, you're not going to just see crazy
[16:34] areas of blue, green, yellow, orange, all that kind of stuff. It's going to be more subdued than that.
[16:38] It's going to be more subtle. So that's my overall approach, look at general human faces and seeing
[16:44] what's there instead of just using some arcane color chart made ages ago, though it is it does
[16:50] serve some purpose. And at this point, we're done with our main hand painting, which means that


### Adding Procedurals [16:52]
**Transcript (timestamped):**
[16:56] we've controlled everything up until this point. But the problem is you can't really take it all
[17:01] the way up just by hand painting unless you're spending an insane amount of time. The pro of
[17:06] hand painting everything is you do control absolute everything. If we want this little scar to be
[17:11] perfectly red and the lips to be exactly where they are, we do control that beautifully. The
[17:16] problem is we need a lot of variation to make the skin read. So for that, we are using procedures.
[17:22] And the approach for that is exactly the same as before, we are making a fill layer, and we are
[17:28] making that a specific color, make sure it's only active in the color trial. Then we're going in.
[17:33] And the only difference now is that we are adding a fill layer into this instead of adding a paint
[17:40] layer. So this means that it's going to look like this, where we are just going in and we're just
[17:43] adding a procedural on top. And you can just see it just adds a bit more variation in this if you
[17:48] just go before and after. In this case, the color does change a little bit as well. And that's the
[17:53] liberate I can use this as color grading as well, where now it just gets a little bit warmer. The
[17:57] procedural I'm using here is called BNW spots three, which is just black and white spots three,
[18:02] which is really useful. And you can just go in, you can just set this to a triplanar as well.
[18:07] You can also use some of the other ones as well, like just UV projection, the problem with that,
[18:11] you can have UV seams by using just a triplanar, then you're going to have planes shooting from
[18:18] different sides, and this is going to blend it all together. So this is completely independent
[18:22] of your UV layout. And this just allows you to really easily just create some nice variation.
[18:27] You can see this the BNW spots or three is fantastic for this because it really just adds a lot of
[18:32] variation. But at the end of the day, it's just a mask, you could absolutely hand paint this from
[18:37] scratch. But the advantage is just the fact that you can change this so easily. So if there's
[18:41] something you don't enjoy, you can just change this around like this. If you were to hand paint
[18:45] this, obviously, you couldn't do that. And then we're just adding a few of these. But if you if
[18:51] you there are areas you don't enjoy, you can definitely like paint them out. Like if you really
[18:55] realize that one part around the eyes, for instance, it just is not working, you can go in, and you
[19:00] can just go in with like maybe like the cotton brush or like the smooth brush, and then just
[19:05] straight out just paint it out like so. And this is the advantage of having like soft brushes like
[19:10] the cotton and the smooth noise. Because here you can really just go in, you can just blend this out.
[19:16] So this is a really good way of doing this. Now you can go in here, you can see that around the
[19:20] eyes, there's nothing currently here. And then of course, you can change your opacity as well for
[19:25] this on and off. So really good approach for doing this, you kind of combine the best of both worlds,
[19:30] you have the procedural nature of the actual procedural, you know, everything is nice and
[19:36] organic, but then we can hand paint out or in details where you want it to be. And then we're
[19:41] just using another procedural top, this is just a three day Berlin noise, we just adds a bit of
[19:45] variation to the whole thing. And then we're doing the same thing with this as well. And here we're
[19:49] using not some grunge is on top as well. The grunge maps are really, really useful, because they
[19:53] will just add a lot of variation and not just in a dirty way, like it's actually going to feel
[19:57] like it's covered in dirt, it can just make it nice and organic. What's important with these as
[20:02] well is that they have a little bit of color in them, you don't want these just to be like a gray
[20:06] scale, like just black and white like so, because that's going to just make it feel dirty, you want
[20:10] to actually make it like make it have some hue and some saturation in it. Then we have a third
[20:16] projection, which is just a grunge projection. And this one is also just a triplanar, you can see
[20:22] here. And this is just using just a grunge concrete one. For this, it's not like I'm specifically
[20:28] using grunge concrete, like it's not like that's my favorite, I just generally just go through here
[20:32] and just type grunge, and we just try out a few different ones, and then you can change their
[20:36] brightness and contrast. And these are really going to help you, there are so many good grunches.
[20:43] And if you find some really good grunches as well, that works well for textures, just let us know
[20:46] in the comments, we'd love to see it as well. But just grunge concrete works really well for
[20:50] this. And it just looks like this, it's subtle. But it just means that you get a bit more variation
[20:56] in your color map like so. Again, this is just a mask, that's the only thing it's doing, it's
[21:01] nothing fancy. But it means that it's entirely procedural. So you can change this up quite a
[21:06] lot. So if you don't enjoy this, you can just move this around like so. And also, don't be overly
[21:12] concerned with what something looks like necessarily in the in the view here, just with the pure mask,
[21:17] because if you if you're overly concerned with this, you might be losing out a lot of awesome
[21:22] things happening in the actual material view. Because a lot of the mistakes you're seeing in
[21:28] the mask view, you can't really see them here. So just make sure that you're you're properly using
[21:33] this 3d view as a way to to gauge what's happening in your textures and not just the view here.
[21:41] That said, it's still good to send a check it because it can be really helpful to to see if
[21:45] there are any issues with like seams or some crazy stuff going on. Like you might just be aware
[21:50] that well, this side here has definitely a seam to it. So in that case, maybe you want to go in and
[21:54] just paint this in or out just create create this create a bit more of organic split here,
[22:01] you know, some of this as well. You can just go in and just make this a bit more organic.
[22:06] But you know, entirely up to you. And like I said, most likely aren't really going to be seeing this
[22:09] in the in the full material view anyway. And also one of the reasons for this is that we've been
[22:15] setting this to soft light for blending modes. I highly recommend using something like soft light.
[22:20] You can see here if you just set this to normal, this looks crazy, you cannot work with this at all.
[22:24] And now you're starting to see the issues. But the moment you're starting to play around with
[22:28] some blending modes like overlay, then you can see that stuff blends a little bit more.
[22:32] You can also just go in and set this to soft light, which is just down here. And this just
[22:36] blends it a little bit nicer, makes it a bit more saturated. And then you just change the
[22:40] opacity for this. So whenever you're adding a procedural, be sure to
[22:45] change the blending mode and make sure to change the opacity as well. And at this point,
[22:49] we have a pretty solid base for our colors, but it's still missing some overall variation,
[22:56] which is what we're going to jump to next. Now this is the point where I'm going more


### Finishing Touches to our Texture Maps [22:58]
**Transcript (timestamped):**
[23:00] between painter and seabush in a very direct way. I'm jumping back into seabush, I'm adding
[23:05] some more veins to it. Like there's going to be veins in the model, I'm going in and refining
[23:09] the forehead a little bit more and just overall adding more refinement to the model. Now I don't
[23:14] actually export the model back to painter, because you know, just add some bit of complexity to it.
[23:19] But what I am doing is I'm exporting out maps from seabush to painter. So in this case, we have a
[23:24] displaced map. And this is subtle, you want to be sure that this doesn't go too crazy. In this case,
[23:28] I have actually made all the pores and such in seabush. That's a discussion for another day,
[23:32] what you should do that in painter or in seabush. But at least in this case, we did do this in
[23:37] seabush. And again, like before, this is just a very simple setup where we have a just a fill
[23:42] layer with some color to it, just a dark saturated color, like, you know, pretty dark color. And
[23:48] then we are just going in and just adding a fill layer like this. This is just where the
[23:53] displaced map actually goes. And let's just change this to normal and just change the opacity to this.
[23:58] And you're not going to see anything at this point. And the reason for this is that the scale
[24:02] of the displaced map is a little crazy. So you really can't see anything. So then we have to go
[24:06] in with the levels. And I'm just straight up just like punching this in here, just really
[24:10] crunching this. And then we're adding another one, basically, I'm just duplicating this one.
[24:15] And now you can really see a lot if we go in here, you can really see a lot of stuff.
[24:19] And then we're going in and we're just flat out inverting this, you can just invert this with
[24:23] the invert button or just moving the input or the black and white points here. So now we just
[24:27] like this. And then I'm painting a lot of things. Because at this point, we have too much information
[24:32] in it. And I really don't want a lot of this stuff down here. It's just a bit too crazy.
[24:36] And a lot of the wrinkles and such, we really don't want them in there. So I'm just painting this
[24:41] out. And then I'm balancing this out a little bit as well. So what you're seeing now is that all the
[24:45] pores and everything, they are getting a bit more of a definition to them. They're getting a bit of
[24:50] darker and more saturated. Look, not too such just a little bit. And then we're just setting this whole
[24:55] thing to soft light. And then we just decrease in intensity or the opacity rather, which we look
[25:02] like this. So now you can see it's subtle, but it still adds a bit more of variation to it. I can
[25:07] just grounds the whole thing. And then as well, at this point, I've also painted more of the veins,
[25:12] like I mentioned before. And I'm just straight up just painting this in in painter now, just adds
[25:17] a bit more of variation to this. And I found this level to be where everything is really coming
[25:23] together. You know, it's still before we added this is still quite clean. And we really just want
[25:28] to break this up. So one thing that helps a ton is to add pimples as well. This is something
[25:34] that's easily all overlooked. But if you jump to seabush, you can really see a lot of these tiny
[25:39] pimples, like if you look at this forehead particularly and this chin as well, you can really
[25:43] see a lot of these pimples. And they just really look nice in a sense that, you know, they're super
[25:48] simple to make you just go over with the standard brush and like just a few, like a tiny tiny row
[25:54] size for this, you just go over and just add them. And they just break everything up because the same
[25:58] thing is happening here with the the overall pores, everything is looking nice and broken up. But we
[26:03] need something to just take our attention. So now our eyes is going to go from this pimple to this
[26:08] pimple. And this is going to add another frequency to it. So what I'm doing at this point actually
[26:12] is that I'm straight up just creating a mask and seabush. I'm going in, I'm just filling this in
[26:16] with white, you should probably do this not on 65 million polygons. But you're just going in and
[26:21] just filling in the whole thing with white by going to color and then fill object. And then
[26:26] we just set this to black. And now with the standard brush, we just enable RGB, or RGB, and then set
[26:31] the RGB intensity to 100. And then you can just go in and you can just paint in where you want
[26:36] these to be. The advantage of this is that you really control where these pimples are. You could
[26:41] of course extract these from some kind of displacement map. But honestly, that's not going to produce
[26:45] fantastic results. And it could look a little bit dirty in the end as well. And now we're just
[26:49] controlling it perfectly. So once you're done with this, you know, spend like 10 minutes or
[26:53] so on this, this does not take a whole lot of time. Once you're done with this, you're straight
[26:56] to just export this out from seabush using this multi map exporter. And the only thing you change
[27:01] now here is you set this to poly paint. And then you just export this out. Now jumping back to
[27:06] painter, what we're doing is we are adding another fill layer, same thing as before, make sure this
[27:10] is only available in the color and we have a pretty dark and slightly saturated color. Then in the mask,
[27:16] we're adding a filler. And this is where we are straight up adding our poly painted maps from
[27:22] seabush. You can see it has the number four in front and that indicates how many udems we have,
[27:25] because we are working with four udems for this character. And then we have to invert it as well.
[27:30] I just removed the inversion because what we did in seabush is that we painted with black on top of
[27:36] white. And this is simply so we can see what's going on. If you were to fill it in with black,
[27:41] and then you're painting these guys with white, you actually can't see anything. So we just have
[27:44] to do it that way. So paint with black on top and then we simply just invert it. I'm using just
[27:49] the quick levels for this. We can just invert and there you go. And then we are simply setting this
[27:54] to a soft light and then reducing the opacity of this. And you can always go and you can change this.
[28:00] You know, if you want this to be like crazy pink or something, you can always do this. This is a
[28:05] huge advantage of this workflow that you can very easily go in and you just play around with this.
[28:10] And that's really it for developing the color map. It's really important that you have an attention
[28:16] detail when it comes to add little veins and little pores and tiny little pimples and such.
[28:20] This is going to add a lot of variation to it. And also just like seeing tiny little scars here,
[28:25] adding a bit of variation turns into color. So that's really it on how I've created this whole
[28:30] skin texture from scratch. This is all done without any photo projections or anything. This is done
[28:36] using hand painting and procedural on top and then adding a bit of sea brush magic to this.
[28:42] Just to reiterate, the whole workflow is based around making fillers with masks and then just
[28:47] having simply different colors in the fiddle ears and then having different data in the mask as well,
[28:54] which you can do with just a few simple brushes. You can really paint the whole thing with just
[28:57] like the dirt to brush and like dots erased. So the workflow itself is really quite simple.
[29:03] So yeah, I hope you enjoyed this Substance Painter skin painting tutorial. If you like this video,
[29:10] please leave a comment. I would love to hear your skin painting tips as well, like specifically
[29:14] what brushes you use, what procedurals you do enjoy. And if you have just any general painting
[29:19] tips for a painter, we'd love to hear that. And then make sure to subscribe and hit the little
[29:23] notification bell as well to get notified every single time we put out a new video. And again,
[29:27] check out the new masterclass with 21 hours of real time videos showing you how to create this
[29:32] whole character from scratch from the first stroke in C brush to the last shader tweak in Blender.



---

## Captured Frames

- [2:15] tutorials/frames/how-to-paint-realistic-skin-in-substance-painter/frame_000.jpg
- [4:20] tutorials/frames/how-to-paint-realistic-skin-in-substance-painter/frame_001.jpg
- [4:45] tutorials/frames/how-to-paint-realistic-skin-in-substance-painter/frame_002.jpg
- [5:35] tutorials/frames/how-to-paint-realistic-skin-in-substance-painter/frame_003.jpg
- [6:30] tutorials/frames/how-to-paint-realistic-skin-in-substance-painter/frame_004.jpg
- [8:00] tutorials/frames/how-to-paint-realistic-skin-in-substance-painter/frame_005.jpg
- [10:05] tutorials/frames/how-to-paint-realistic-skin-in-substance-painter/frame_006.jpg
- [13:20] tutorials/frames/how-to-paint-realistic-skin-in-substance-painter/frame_007.jpg
- [17:40] tutorials/frames/how-to-paint-realistic-skin-in-substance-painter/frame_008.jpg
- [20:20] tutorials/frames/how-to-paint-realistic-skin-in-substance-painter/frame_009.jpg
- [23:50] tutorials/frames/how-to-paint-realistic-skin-in-substance-painter/frame_010.jpg
- [26:20] tutorials/frames/how-to-paint-realistic-skin-in-substance-painter/frame_011.jpg
- [27:50] tutorials/frames/how-to-paint-realistic-skin-in-substance-painter/frame_012.jpg

---

## Structured Notes

### Core Technique
Entirely hand-painted-first skin color-map workflow (no photo projection at all) built from a strict "one folder per channel, one Fill layer per color" architecture — Base + Red + Redder + Yellow + Blue + Darker layers, each a flat-color Fill layer masked by a nested Paint layer — so the whole map stays fully procedural and re-gradable (change any Fill layer's color at any time, globally, with zero re-masking), then supplemented with tri-planar procedural noise/grunge masks for variation beyond hand-painting's practical time budget, and finished with ZBrush-exported displacement and poly-painted pimple maps fed back in as Painter masks.

### Summary
Opens with a strong methodological point: texture quality is bottlenecked by sculpt quality — a model with all frequencies already present (pores, scars, wrinkles) textures far faster and better than an underdeveloped one; don't rush into texturing to compensate for a weak sculpt. **Project setup**: bottom-most **Temp** fill layer in a heavily saturated "shock" color across every channel (Color/Height/Roughness/Scattering) purely as a build-integrity check — if this color ever shows through unexpectedly, something's wrong. Above it, one **folder per channel** (starting with Color), each folder holding one flat-color Fill layer per named tone: **Base** (main desaturated skin tone, Alt-click-isolated to Color only — changing this single layer regrades the entire map later), then duplicates named **Red**, **Redder**, **Yellow**, **Blue**, **Darker** — each with a black mask containing a nested **Paint layer**, symmetry enabled. **Favorite brushes** for hand-painting skin: **Dirt2** (general-purpose, pen-pressure-enabled by default for organic shapes, or disable pressure on Size and enable it on Flow instead for an opacity-driven feel), **Dots** (freckle/pore-like base variation, used both additively and subtractively), **Dots Erase** (a softer, more organic variant of Dots — used most often, blends more naturally), **Cracks** (vein-like patterns, generally used on the Blue layer rather than Red), **Cotton** and **Smooth Noise** (soft blending/gradient brushes with a bit of inherent texture — deliberately not perfectly smooth, since realism needs some texture even in "smooth" areas; Smooth Noise is inspired by Mari's "super smooth" brush), and **Mold** (fast general base-variation brush, heavy X-key black/white toggling). **Hand-painting workflow**: work the Red layer first around the eyes, nose, mouth, and ears (the most naturally red facial zones), blocking boldly without hesitation since this becomes the foundation for everything after; the underlying Fill layer's color itself can still be adjusted at any time since the mask is separate from the color; repeat the identical fill+mask+paint-layer pattern for Redder, Yellow, Blue (mostly via Dots Erase), and Darker (value variation, not just hue — brightness/darkness variation matters as much as color variation). This full hand-painting stage on one character took roughly 3-4 hours total across all color layers in production (though a single layer's dedicated masterclass chapter ran ~30 minutes). Explicitly framed as more labor-intensive than reference-photo projection, but far more re-editable: changing an entire character's color scheme later is a one-click Fill-layer color change rather than re-grading baked photo data. Loosely follows traditional face color-zone theory (redder around blood-rich areas, more blue/yellow near bone/mouth) without treating it as a rigid chart — real faces are more subdued/subtle than classic color-zone diagrams suggest. **Adding Procedurals**: identical Fill-layer-plus-mask architecture, but the mask now holds a **Fill effect with a procedural texture** instead of a Paint layer — demonstrated with **BNW Spots 3** (black-and-white spots), set to **Tri-Planar** projection specifically to avoid UV seams (a plain UV projection would show them). Areas where a procedural doesn't read well can still be hand-painted out afterward with the Cotton or Smooth Noise brush — combining "the organic feel of a procedural with hand-painted control over where it applies." Additional procedural layers stack a **3D Berlin Noise** and a **Grunge** (e.g. Grunge Concrete, again Tri-Planar) — grunge maps specifically chosen with some inherent hue/saturation (not pure grayscale) so they read as organic variation rather than literal dirt. Critically, **every procedural mask layer's blend mode is set to Soft Light** (never left at Normal, which reads as visually broken/harsh) — and the recommendation is to judge the result in the full 3D material view, not the flat mask preview, since mask-view "problems" (seams, harsh edges) often aren't visible or relevant in the actual shaded result. **Finishing touches (ZBrush round-trip)**: rather than re-exporting the sculpted mesh, only new **maps** are exported from ZBrush back into Painter as additional mask sources on the same Fill-layer architecture — a **Displacement map** (Normal blend, opacity-adjusted, then aggressively pushed with Levels since the raw displacement range is too subtle to read, duplicated and inverted for a second variant, then hand-painted-out in unwanted areas like excess wrinkle noise, finished on Soft Light at reduced opacity) and a dedicated **pimple mask** authored directly in ZBrush (fill the whole mesh white via Color → Fill Object, switch foreground to black, enable RGB intensity 100%, then hand-paint pimple positions directly with the standard brush — full manual control beats extracting pimples from a displacement map, which tends to look dirty) exported via ZBrush's Multi Map Exporter set to **Poly Paint** (per-UDIM, 4 UDIMs for this character) and imported into Painter as yet another Fill-layer mask, inverted via Levels (painted black-on-white in ZBrush for visibility, then inverted since a white-on-black paint wouldn't have been visible while sculpting), Soft Light blend, reduced opacity.

### Key Steps
1. Sculpt-quality check first: ensure the model already has full detail-frequency coverage (pores, scars, wrinkles) before texturing — texturing a well-developed sculpt needs only gradients, light procedurals, and a bit of hand-painting; an underdeveloped sculpt forces a much harder "black book of tricks" workflow (heavy projections, LookDev hacks).
2. Bottom **Temp** Fill layer in a jarringly saturated color across every channel (Color/Height/Roughness/Scattering) as a build-integrity sanity check.
3. Organize by **one folder per channel** (starting with Color); inside, one flat-color **Fill layer per named tone** (Base, Red, Redder, Yellow, Blue, Darker), each Alt-click-isolated to only the relevant channel.
4. Base layer: a desaturated, slightly-saturated skin tone — exact color doesn't need to be final, since it's globally re-gradable later.
5. For each color layer: right-click → Add Black Mask → add a nested **Paint layer** inside the mask (enable Symmetry) — this is the repeatable unit of the entire workflow.
6. Hand-paint the Red layer first, focused around eyes/nose/mouth/ears (naturally reddest zones); block boldly, don't be shy — this is the foundation everything else builds on.
7. Use **Dirt2** for general painting (pen-pressure-driven by default; alternatively disable Size pressure and enable Flow pressure for an opacity-driven feel), **Dots**/**Dots Erase** for pore/freckle-like base variation (Dots Erase preferred for its softer, more organic blend), **Cracks** for vein-like patterns (typically on the Blue layer), **Cotton**/**Smooth Noise** for soft gradient blending (retain a little inherent texture — avoid a perfectly smooth, unrealistic result), and **Mold** for fast general-purpose base variation.
8. Repeat the fill+mask+paint pattern for Redder, Yellow, Blue, and Darker — Darker specifically for value/brightness variation, since color variation alone isn't enough; real skin varies in lightness too.
9. Loosely reference traditional face color-zone theory (more red near blood-rich areas, more blue/yellow near bone/mouth zones) without treating it as an absolute rulebook — keep the effect subtle, since real faces don't show dramatic color-zone shifts.
10. Add **procedural** variation once hand-painting reaches its practical time limit: same Fill-layer-plus-mask architecture, but the mask holds a **Fill effect with a procedural texture** (e.g. BNW Spots 3) instead of a Paint layer, set to **Tri-Planar** projection to avoid UV seams.
11. Selectively hand-paint out areas where a procedural doesn't read well (Cotton or Smooth Noise brush) — combines procedural organic variation with hand-painted placement control.
12. Layer additional procedurals (3D Berlin Noise, Grunge — e.g. Grunge Concrete, also Tri-Planar) — pick grunge textures with inherent hue/saturation, not pure grayscale, so they read as organic skin variation rather than literal dirt.
13. Set every procedural mask layer's blend mode to **Soft Light** (Normal reads as broken/too-harsh) — evaluate results in the full 3D material view, not the flat mask preview, since many mask-view "issues" (seams, hard edges) don't actually show or matter in the shaded result.
14. ZBrush round-trip for finishing: export new maps only (don't re-import the mesh) — a **Displacement map** into a Fill layer (Normal blend, opacity down initially since the raw range is too subtle), pushed hard with **Levels**, duplicated + inverted for a second pass, hand-painted-out where excessive (unwanted wrinkle noise), finished on **Soft Light** at reduced opacity.
15. Author a dedicated pimple mask directly in ZBrush: fill the mesh white (Color → Fill Object), switch to black foreground, enable RGB Intensity 100%, hand-paint pimple positions with the standard brush (full manual placement control beats extracting pimples from displacement data, which tends to look dirty) — roughly a 10-minute pass.
16. Export the pimple poly-paint via ZBrush's **Multi Map Exporter** set to **Poly Paint** (per-UDIM if multi-tile), import into Painter as another Fill-layer mask, **invert with Levels** (painted black-on-white in ZBrush for visibility while sculpting, so needs inverting on import), **Soft Light** blend, reduced opacity.

### Layers / Tools / Settings
- One **folder per channel**, one **Fill layer per named color tone** (Base/Red/Redder/Yellow/Blue/Darker), each with a nested Paint layer in its mask
- Brushes: `Dirt2`, `Dots`, `Dots Erase`, `Cracks`, `Cotton`, `Smooth Noise`, `Mold`, `Dust` — `X` to toggle paint color black/white
- Procedural masks: `BNW Spots 3`, `3D Berlin Noise`, `Grunge Concrete` (or similar) — all **Tri-Planar** projection, all **Soft Light** blend mode
- Favorites: right-click a brush → Add to Favorites (pins it to the top of the brush panel)
- ZBrush round-trip: **Displacement map** (Normal blend + Levels push + invert + hand-paint-out + Soft Light), **poly-painted pimple mask** (Color → Fill Object white, black foreground, RGB Intensity 100%, hand-painted, exported via Multi Map Exporter as Poly Paint, per-UDIM) — imported as Fill-layer masks, Levels-inverted, Soft Light blend

### Difficulty
Advanced — assumes comfort with layer/mask architecture and Painter's brush system; the value is entirely in workflow discipline (one-color-per-layer, hand-paint-then-procedural-then-ZBrush-round-trip sequencing) rather than any single complex technique.

### App & Version
Not stated on screen; paired with ZBrush (PolyPaint, Multi Map Exporter) and, per the video's intro, eventually Blender/Cycles for shading and rendering (out of this skill's scope).

### Tags
`layers` `fill-layer` `paint-layer` `masks` `procedural` `tri-planar` `blend-mode` `alpha` `basecolor` `color-management` `advanced`

---

## Related Tutorials
- [Speeding Up Character Texturing with Smart Masks - Substance Painter](speeding-up-character-texturing-with-smart-masks---substance-painter.md) — same creator (FlippedNormals); shares the same one-Fill-layer-per-facial-region architecture and reusable-mask philosophy, applied there to a Smart Mask library workflow instead of pure hand-painting.
- [Texturing a Clicker - FULL Substance 3D Painter Workflow](texturing-a-clicker---full-substance-3d-painter-workflow.md) — same creator; another full character/creature texturing project sharing the channel-separated-groups organizational philosophy and iterative render-feedback discipline.
- [10 New Features in Substance Painter You Didn't Know About](10-new-features-in-substance-painter-you-didnt-know-about.md) — same creator; the Favorites asset-browser feature demonstrated briefly in this video (right-click a brush → Add to Favorites) is one of the features that hub video covers in more depth.
