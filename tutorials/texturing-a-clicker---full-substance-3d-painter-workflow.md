---
title: Texturing a Clicker - FULL Substance 3D Painter Workflow
source: YouTube
url: https://www.youtube.com/watch?v=RTvgwZj-5Rw
author: FlippedNormals
ingested: 2026-08-13
app: "Substance 3D Painter"
version: "not stated numerically on screen; creator calls the baking-panel baker \"the new baker they're adding\" as a then-recent addition, and the brush-favoriting right-click feature as \"fairly new\" — both relative-version markers without a specific number; UDIM/UV Tiles workflow (multiple texture sets per UDIM tile) visible throughout, tentative"
tags: [layers, fill-layer, paint-layer, masks, generator, curvature, ambient-occlusion, mesh-maps, world-space-normal, position-map, high-to-low-poly, baking, cage, udim, texture-set, uv, pbr, basecolor, roughness, height, alpha, procedural, tri-planar, blend-mode, iray-render, viewport, color-management, advanced]
extraction_status: complete
frames_dir: tutorials/frames/texturing-a-clicker---full-substance-3d-painter-workflow/
frame_count: 12
frame_status: complete
frame_selection: content-anchored (manual timestamps chosen from transcript, not blind percentages)
---

# Texturing a Clicker - FULL Substance 3D Painter Workflow

**Source:** [YouTube](https://www.youtube.com/watch?v=RTvgwZj-5Rw)
**Author:** FlippedNormals
**Duration:** 33m43s | 1 section(s)

---

## Raw Data (for Claude Code extraction)

Frames captured — see "Captured Frames" section below.


### Full Content [0:00]
**Transcript (timestamped):**
[0:00] Hi, this is Henning from FlukeNomers.com and in this video I'm going to show you how I
[0:06] textured my fan sculpt of the clicker from The Last of Us based on the TV series.
[0:12] We have another video as well covering the sculpting of this character and now we are
[0:16] proceeding with the texturing.
[0:18] The first step of texturing for me is always good sculpting.
[0:23] I really can't stress how important the step here actually is.
[0:27] If you have a good sculpt in this case, we have a model like this in C brush which has
[0:32] really solid mid frequency, has some nice high frequency and generally it's just a
[0:36] quite refined model.
[0:38] Texturing becomes so much easier.
[0:41] For instance, you can get away with a lot of things when it comes to tileable maps.
[0:45] If you were to tile something across here, you probably wouldn't even see the tiling
[0:48] just due to the mid frequency.
[0:50] The baked maps you would be generating would be of much higher quality and also if you are
[0:56] sculpting in a more physically plausible way in terms of the thickness of various things,
[1:02] the SSS is also going to be much more accurate so you would need to do a lot less work when
[1:07] it comes to the subsurface maps and if you are doing high frequency as well in a proper
[1:12] way, this doesn't necessarily have to be in the sculpting because this can also be done
[1:16] in painter as well when it comes to just using the height of normal maps there.
[1:20] But if that's done properly as well, doing the roughness map is also so much easier.
[1:25] Doing a proper sculpt like this in Seabrush is really important.
[1:29] I really keep coming back to this time and time again that a good sculpt is really the
[1:34] foundation for everything going forward, particularly texturing.
[1:38] So this is what it currently looks like.
[1:39] You can see here that we have a lot of details here when it comes to the mouth.
[1:44] We have some pores around.
[1:46] Overall, this is around almost 12 million polygons for this as well for the mushroom
[1:52] bits on top of his head.
[1:53] We have quite a lot of polygons.
[1:54] We have 25 million polygons for this.
[1:57] And it was important for me that this here was properly refined because this here is,
[2:02] this is quite an evolved model and the better the sculpt of details here is the better the
[2:06] bake maps are going to be.
[2:07] And also if you check on the back, this is very much sculpted from a single angle.
[2:11] So this is more of a quicker project for me.
[2:13] This was never intended to be anything fancy like in terms of like a full turntable or
[2:18] portfolio piece.
[2:19] This was just something I'd fun with.
[2:20] So you can still see like rush, rushed strokes or rough strokes.
[2:24] The back here, there is literally nothing.
[2:26] So sculpt based on the angle that you are working with.
[2:30] And then once I'm done with the seabird's model, then I'm decimating it out, which you
[2:34] can do with C plugin and then decimation master.
[2:36] And I'm decimating it to different resolutions.
[2:38] So each texture set, which we'll get to in a sec, is decimated at both a high and a
[2:43] low rest resolution.
[2:45] And the lowest will be brought directly into painter and the high rest will be brought in
[2:50] as a high risk map.
[2:52] So these are exported to blender.
[2:55] You can do this in any software.
[2:56] You don't technically even have to do a 3D software.
[2:59] You can export this directly from seabirds as well.
[3:02] As long as you're using polygroups instead of materials, you can, you can change that
[3:06] under the FBX export settings.
[3:08] But I find it to be a bit easier to export this out from a 3D software.
[3:12] If you have Maya or Max available as well, that that's totally fine.
[3:16] The only thing you need is where you really just need to combine the objects in the texture
[3:20] sets you want.
[3:21] And you have to just assign materials.
[3:23] So in this case here, the low rest here has just a material called head and it has the
[3:29] underscore low on them.
[3:31] And then we had the exact same model under high, same hierarchy as well, just with the
[3:37] underscore high.
[3:38] This is a default naming from painter.
[3:41] You can name this whatever you want to, as long as you are naming, as long as you're
[3:44] changing this in the baker in painter as well.
[3:47] The important thing at least is that you have the material on the low rest here.
[3:51] This doesn't really matter if it's on a high rest or not, because this is just going to
[3:53] be baked down.
[3:56] So that's it for for this.
[3:58] Then we are going to be importing this, the low rest directly into painter as an FBX.
[4:05] Now painter, of course, already set this whole thing up and already texture this.
[4:10] But this is set up using the legacy color space.
[4:12] So this uses this as such a B. I'm not using ASUS or anything fancy for this.
[4:16] This is very, very simple stuff in terms of color space.
[4:20] Now we are starting off with just baking.
[4:24] We just click this nice little croissant icon up here.
[4:26] Really like the new baker they're adding.
[4:28] This is a fantastic new baker.
[4:30] This is a real solid one.
[4:31] Then I'm just adding the high rest one.
[4:33] We just export from blender and where all the naming is correct.
[4:37] Then we are setting the match to by name or by mesh name.
[4:43] And then we don't have to do anything here because this is higher and low, which is exactly
[4:46] the same.
[4:47] This is what I said before.
[4:48] If you did change this in blender, for instance, to high rest or low rest, you just have to
[4:52] change these here.
[4:54] For maps, I'm using normal, world space, normal, ID, AO, curvature, position and thickness.
[5:00] The ones I'm using the most at the end of this would actually be curvature and mid-occlusion.
[5:04] The reason you want all these is not because you're going to be using them directly.
[5:07] It's not going to be using position directly.
[5:09] It's because a lot of the generators and such would require them.
[5:13] So just do these ones by default.
[5:16] One K is enough for now.
[5:18] If you need more than that, then you can just rebake these at a higher resolution.
[5:21] Then we go back to painting mode and just a quick discussion on the texture sets as
[5:26] well.
[5:27] For the head, this is where we have the head and we have the tongue.
[5:32] Then we have the nothing else is really combined like that.
[5:35] We have the head shrubs, then we have the neck shrubs, and then we have the teeth as
[5:40] well.
[5:41] These have been even mapped accordingly to the texture sets so that there's no overlap
[5:46] between these two.
[5:48] This is what it looks like when we just look at the UVs real quick.
[5:50] This is nothing fancy with us.
[5:52] To be perfectly honest, the UVs here are dead simple and there's nothing fancy for topology
[5:58] or the UVs.
[5:59] This is again supposed to be a quicker project.
[6:01] So the topology and UVs are not optimized for anything in particular here.
[6:05] It's just supposed to be a quick way for me to get started with this.
[6:08] This is a legit way of doing it as well.
[6:10] The end result looks fine.
[6:11] There are no problems with topology or UVs in the end result.
[6:15] All pieces have straight up been searourmashed.
[6:19] For UV mapping, I straight up selected a seams and blender and I used UV Master to do the
[6:23] unfolding because I find that unfolding to be a bit better than the default blender one.
[6:28] Then I brought it all back to blender and I just did the unfolding in blender.
[6:32] It is really important to think about your texture sets before you get started because
[6:35] if these are not set up correctly, you're just going to be in a world of pain because
[6:40] now you have to start to merge maps later on and you have to assign materials later
[6:45] on so it's really painful.
[6:47] So the way I think about it is set up the texture set in the same way that you would
[6:50] apply materials.
[6:52] So in blender, for instance, the head texture set that would just be a head material.
[6:57] This is just another way of thinking about that.
[7:00] So let's get started with the actual breakdown of this.
[7:02] Now I'm mostly going to be going through the head, but we do have additional textures as
[7:06] well.
[7:07] So we'll go through those a little bit later when we're starting off with the head because
[7:11] this is the most interesting one.
[7:13] The way I'm breaking this down as well inside the layer palette is that I have two groups.
[7:18] One is the tongue and one is the head.
[7:20] So for the tongue one, this is very simple.
[7:22] This is just a group that has masked out the tongue.
[7:25] So anything inside this can only affect tongue.
[7:28] So nice and simple.
[7:29] And then for the head, we are just going to go through this one by one.
[7:33] Now the way I do this as well is that I have one group for color and one group for roughness.
[7:39] This means that all my color maps are in here and all the roughness maps are in here.
[7:43] Now this is not particularly effective in terms of computer optimization.
[7:48] If you want to, you could run this probably quite a lot smoother than what I'm currently
[7:52] doing.
[7:53] But this is a fantastic way of working from a human point of view.
[7:57] It means that I can open up this scene at any point in the future and it's easy to understand
[8:01] what's going on and it's easy for other people to pick it up.
[8:05] And also it's just easy to texture it this way.
[8:06] So this is always my preferred way of working.
[8:09] You could technically have like fill layers like this that have roughness, normal height
[8:14] and color and all that and just optimize this in as few layers as possible.
[8:18] But I find it definitely to be worth it to work in single channels and single groups
[8:25] like this just to develop this.
[8:27] So with that said, let's get into it.
[8:30] The first thing I have for really everything, for all of these ones, for all the different
[8:34] texture sets is that I have just a fill layer, which is just a base.
[8:39] And this is just a color.
[8:41] In this case it has height and roughness.
[8:43] Well, just we have some values there.
[8:44] But in general, this is just to get a base color down.
[8:48] I think it's really important to do this because it's really easy to overcomplicate
[8:53] the texture.
[8:54] You want to start off in a methodical way.
[8:56] You want to figure out what is the local color of the actual object you are painting.
[9:01] And then we're adding another fill layer.
[9:03] Literally every single layer in this entire texture and project is just a set of fill
[9:07] layers.
[9:08] Now it's not just a set of fill layers that are being painted on.
[9:11] Some are being painted on and you can see here there's red and paint and you can see
[9:14] this one that has a curvature.
[9:16] So the first thing I do is I enable this layer, which is just a fill layer.
[9:21] Very simple.
[9:22] Just has color, darker color than the other one.
[9:25] And then in the mask, I just go right click, add the black mask.
[9:31] And then in here I'm adding a fill layer.
[9:33] And then in the fill layer, I'm straight up just adding a curvature.
[9:37] So under generator, I'm just adding a curvature.
[9:40] And this has very simple settings for it.
[9:42] And this is why we needed to bake maps before because now you can see this uses the curvature
[9:46] uses the world space normal and the gradient or position grade.
[9:50] So without these maps, this wouldn't actually work properly.
[9:53] So what this does, it simply just looks at the curvature and just makes certain things
[9:56] darker.
[9:57] So if we look at this now, you can just see there is it just pops a bit more.
[10:00] This just adds a fair bit of variety to it.
[10:04] And just to reiterate a point from before, you can see that all of this just comes from
[10:09] the scope.
[10:10] And nothing here like procedurally in terms of we're not using triplanar or anything.
[10:15] All this data comes from the scope.
[10:18] So the better your scope, this the better this is going to be.
[10:21] Then I'm adding a series of fill layers that are hand painted as opposed to this one, which
[10:25] is entirely procedural.
[10:27] So the first one is just a red layer.
[10:30] And this is just hand painting with one of my favorite brushes over here.
[10:33] We'll talk about those in a second.
[10:35] And this is simply just straight up red, just hand painting and doesn't look very fancy
[10:39] at all.
[10:40] It's very simple.
[10:41] I believe this is painted with the mold brush.
[10:43] So very simple, very nice and easy.
[10:45] And this is just something you can add and remove like this.
[10:48] And I do the same thing for the for yellow.
[10:51] And you can see I'm adding red come to some of the darker areas like where it goes, where
[10:57] it goes in like in deep for crevices like this and also where he's been bitten here
[11:01] and he has a scar.
[11:02] So just adding a bit of that, but also adding it around the mouth as well.
[11:06] And then I'm adding yellow and yellow goes over the bones.
[11:09] Now this is more just like our direction.
[11:12] It doesn't necessarily have to be exactly like this, but I think this can look quite
[11:15] nice.
[11:16] Then we have blue and just adding blue to certain areas to make him feel a bit more dead.
[11:20] But also adding blue to it can add a lot more variety to it as well.
[11:23] So highly recommend adding blue to it, even if you're doing a fairly realistic human as
[11:28] well.
[11:29] Then we're adding green as well.
[11:30] This is more subtle, but a bit darker as well.
[11:34] This is set to soft light as well.
[11:37] And this can give you like this nice breakup.
[11:39] In terms of the brushes I'm actually using, there's a cool trick in painter that just
[11:44] added, which is you can right click on it and then you can add two favorites.
[11:47] So this is a new fairly new thing.
[11:49] And the ones I'm using would be basic soft just for general, general painting.
[11:53] The cotton brush just for a soft brush with, which has some general texture dirt to for
[11:59] general grunge.
[12:00] This is just overall good brush dots for doing like general pores and pimples.
[12:05] Dots erased.
[12:06] This is the brush I used the majority of the time.
[12:08] This is the clay buildup of painter for me.
[12:11] This is fantastic.
[12:12] And it's really good for adding this like nice mottled result.
[12:16] You can see this like it's nice and broken up.
[12:18] All this here is all just dots erased.
[12:22] Dust is great for adding like very subtle breakup on top.
[12:25] This is really good for adding like textures.
[12:27] And then the smooth noisy is really good as a good soft brush as well.
[12:33] So next up, we have just a layer that's dark.
[12:36] This is a layer that just generally adds some darkness throughout the whole thing.
[12:40] This is just something that just adds a bit of contrast to the whole thing.
[12:43] This is all just hand painted as well.
[12:44] Like there's nothing fancy here.
[12:45] In this case, I actually forgot to add a layer to it.
[12:48] So I painted directly into the mask, which you should never do because now you started
[12:52] to edit this.
[12:53] You can't change your opacity off of the such.
[12:54] So make sure to paint this into a paint layer and not directly into the mask.
[12:59] You can see how nicely this integrates.
[13:02] You could probably do something with this with the procedures as well, like with an
[13:05] ambient occlusion as well.
[13:06] But I find this to be quite handy just to do this by hand because I can really control
[13:09] it.
[13:10] And you can see here as well, when it's doing dark things like this, it's not just black.
[13:16] It's not desaturated.
[13:17] Like if you're just working to do this, you see how like how boring this looks compared
[13:21] to this, like add saturation to your maps.
[13:24] It's really important to do that.
[13:26] Like it's really important to use saturation for darkness instead of just making it darker
[13:32] in value.
[13:33] Then we do a little bit more hand painting where we're just adding a bit more like value
[13:36] play with this.
[13:37] This is where we are just making a lot darker.
[13:38] The thing is you have to make the texture map a lot more contrasted than you actually
[13:43] think because when you start to look at this in the material view and you start to look
[13:47] around here, you can't really see this that well.
[13:50] Like the darkness here.
[13:51] Yeah, sure, you can see it a little bit, but like it's not as prominent as you think.
[13:56] This is this is a night and day.
[13:57] I'm gonna look at it in the material view.
[13:59] Yeah, it's prominent, but it's far less.
[14:03] So it's really important to keep this high contrast.
[14:08] And speaking of that, something we have to discuss as well is that you need to test render
[14:13] throughout the project.
[14:15] Before you are getting too far with the textures, you really have to do test renders.
[14:20] If you're not test rendering, you're flying blind and you really don't know what's what's
[14:24] going on.
[14:25] You really don't know what's going to work or not.
[14:28] So this here was the first test render I did.
[14:31] And I thought it looked decent, but it's it's you can really tell where it's lacking specifically
[14:37] what's lacking would be sculpting.
[14:40] And it's interesting because this is not a texturing note per se.
[14:43] This is a sculpting note.
[14:44] This is a model note.
[14:46] And by improving that, like you can see between these two, the really only thing here apart
[14:49] from a little bit of rim light on the back, the only difference is that the scope is much
[14:55] better.
[14:56] I spent probably around two, three hours additionally, the whole thing took like three hours to
[15:00] scope that I spent like three hours more on only these ones here.
[15:03] But you can really see the difference.
[15:04] It's not just a difference in terms of of sculpting, though, in terms of pure shape is
[15:10] also in the sense that if you looked at different areas here and here as well, you can tell
[15:15] that these areas are much more interesting because of the big maps that will improve.
[15:21] So I took this one out of Seabrook and a baked maps again.
[15:25] And then I keep doing additional renders as well.
[15:28] This is where I just keep playing around the lighting.
[15:30] It's hard to see if the texture actually changed here, but at least the the lighting did.
[15:35] And it's really important to play around with that.
[15:38] It's essential to do these test renders throughout because otherwise you just genuinely don't
[15:44] know what you need to focus on.
[15:46] For instance, some of the areas here, like the the mushrooms here on his like on his
[15:52] on his face and his neck, they're barely seen in the final version.
[15:57] So why spend time on that?
[15:59] Well, these ones here are very much seen in the final.
[16:01] So I had to spend time on that.
[16:03] So this is a way of of really focusing on that.
[16:08] So here we are developing the look a little bit further and playing around with lighting
[16:14] playing around with the camera angle as well, but also just refining textures just a little
[16:19] bit. And then we are playing again a bit more with depth of field and just just getting
[16:24] ideas for the final one.
[16:25] I end up changing the lighting from this like completely, but the depth of field stays and
[16:31] the camera angle is like most of the same.
[16:34] And then the difference between these two, like from a technical point of view, is that
[16:38] simple, but this looks so much more interesting.
[16:40] The only difference between these two is that the edges of the head mushrooms just are much,
[16:47] much smoother.
[16:48] So I changed the roughness amount on them.
[16:51] And this is from like showing it to my flip normal scheme and they had notes on this.
[16:56] So it's really beneficial to do this because you you will not be able to see this kind of
[17:00] stuff unless you're like working in an iterative way.
[17:03] Then I'm changed the lighting completely.
[17:05] I didn't really like this.
[17:06] This was a bit too.
[17:07] I just didn't enjoy it.
[17:08] And then I tried this out and texturing wise, it should be pretty similar.
[17:13] And you can see how much it changes, how much the lighting actually changes or the
[17:17] textures change between these two.
[17:19] So now I had a new new light set up.
[17:21] I really liked and this is in cycles as well.
[17:23] And we'll do another video on that as well on the actual looked at and lighting there.
[17:29] And then I'm just playing around with some with some lights with some different colors,
[17:34] but also just updating the textures, subtle changes at this point.
[17:38] And then doing more changes with this change in the color quite a lot.
[17:42] You can see the color of these ones here change quite drastically.
[17:46] And this straight up comes from from doing test renders and taking this render into
[17:50] Photoshop and then doing a huge shift on it, realizing that I thought this was much,
[17:55] much cooler.
[17:56] I thought it was I needed a lot like I need these needed to be a lot more orange
[18:01] and did a huge shift on this in Photoshop on a final render realized that's cool.
[18:05] So I did the same huge shift in in painter, like on the actual maps.
[18:10] I didn't actually do an adjustment layer.
[18:11] I just straight up changed the the color of the of like the of the fill layers.
[18:17] That's an advantage of doing this with fillers.
[18:19] You can always change the colors without grading.
[18:23] And then just going in here and then adding more refinement to it.
[18:26] And now I'm doing some more color variation, a few different areas and also adding
[18:30] blood to it as well, which I think is pretty cool.
[18:33] But the blood is is quite primitive here.
[18:35] This is more just a quick test to see if it works because you don't know if the blood
[18:39] is going to work until you put her into into blender into a render engine of choice.
[18:45] Simply because it's a complicated thing.
[18:46] You generally don't know what it works, what it looks like, because you only have
[18:50] like half the data if you're actually painting in painter.
[18:54] And then here is the final one.
[18:55] And you can see the difference between these two that the blood is a lot better now.
[19:00] It's darker, it's more spread out.
[19:01] And I've also added some like pimples around here.
[19:04] So this is just a quick discussion on like on actually look at them and shading.
[19:10] We'll get more into this in the actual shading video.
[19:13] But the point about this whole section is just it's important to know that
[19:16] you have to do look at tests along the way.
[19:21] It's really important.
[19:22] You can see here, for instance, that these ones here, the the neck mushrooms
[19:26] are barely prominent at all.
[19:27] There's barely anything on them, which means
[19:30] that the textures can be really simple.
[19:32] Well, if you were to look in the actual painter scene, the texture is kind of
[19:35] lacking, but it works here.
[19:36] So let's jump back into painter.
[19:38] Now we have to add additional layers on top of this.
[19:42] What I find to be really useful for organic textures is actually using marble textures.
[19:48] So adding a fill layer and adding marble on top of this.
[19:50] Like this is not a smart material or anything.
[19:53] This is just a fill layer with just a marble texture.
[19:55] And this is set to try planar and just been scaled down a bit.
[19:58] This is really cool because it really gives you this like nice organic look like this.
[20:03] It almost looks like like meat as well.
[20:05] So marble textures is awesome.
[20:07] You can just Google marble textures and I have just two layers of this as well.
[20:11] Add some cool color variation to it as well.
[20:14] And then I'm doing the pimple pass.
[20:17] This is just this is just straight up hand painting.
[20:20] Now you could, of course, just make a new layer like a regular paint layer and paint
[20:23] and add, but find to be really helpful to do this because now we can change
[20:26] the color of the of this quite fast.
[20:30] So without having to grade things, I'm just straight up changing the color of this here.
[20:35] So this is really useful.
[20:37] Now, if you want to do the same thing, but you want different colors on them,
[20:40] what you could do, you can make another group and you could paint this as
[20:45] as the mask for the group and have different fill layers inside that have different colors
[20:50] or just paint layers inside that can work quite well as well.
[20:53] And then we have curvature.
[20:54] Same thing as before, just adding another curvature to it.
[20:57] Pretty standard settings for this and just playing around with this.
[21:01] And you can see this like integrates it quite nicely.
[21:05] And then the last thing we're doing here is just an additional curvature
[21:09] in terms of the proceduralness.
[21:10] And then we're doing some color variation on top of this.
[21:14] And then just just changes the whole look quite a lot.
[21:17] Maybe this is a bit too strong, but you can always change this down.
[21:20] So I think I might actually know it's actually done here.
[21:23] You can see the whole thing is just a bit down.
[21:27] So this is just a bit of color variation to it.
[21:29] And then on top of this, now I did say that I usually keep my color and my
[21:34] roughness as separate channels, but I've actually broken this rule a little bit up
[21:40] here and I have blood.
[21:41] So here I have a rough layer of this like orange crustive blood.
[21:45] Then I have the more vibrant blood here.
[21:47] And then I have the roughness streaks.
[21:49] And the reason I'm doing these here combined is because now I can combine,
[21:53] like I can have roughness in both of them at the same time.
[21:56] So I can, this one for here, for instance, has both, actually this one here has
[22:00] both color and roughness.
[22:01] So if I paint on one, it affects the other one.
[22:04] So it's quite useful that you can change, like now I'm painting both color
[22:08] and roughness for this.
[22:10] So that's really useful.
[22:11] You can't really do this if you do the other way.
[22:13] You could probably do it with anchor points or something, but honestly,
[22:15] anchor points, confusing as hell.
[22:17] So let's just stick to these ones here.
[22:20] So now we have, now we have all the texture maps for the head, at least
[22:25] the main head here, that we need to just do the tongue real quick.
[22:28] And the tongue pretty simple.
[22:30] This one here is just a base color, then another curvature on it, then
[22:35] some grunge on top of this, just to break it up.
[22:37] When it comes to the specific grunge I'm using, I honestly just search for grunge
[22:41] and then I just find something that looks cool.
[22:42] I try a few different ones of them, but it's not like I have a favorite grunge.
[22:47] And then I do another one here, another grunge.
[22:48] And that's really for the tongue.
[22:51] Now it looks simple, but coming up with this took quite a lot of time.
[22:54] Really coming up with a color of the tongue that took quite a lot of time.
[22:58] It's one of these, the end result can be quite simple, but getting to
[23:01] something simple isn't easy.
[23:03] And then we have roughness.
[23:05] Roughness is quite simple.
[23:07] I'm just going to go to the head and then we're just going to look at roughness.
[23:10] Since the model is quite well developed, roughness can be really quite simple.
[23:15] Like people over complicated roughness all the time because the model is
[23:19] underdeveloped.
[23:20] So here we just have a general base.
[23:21] We had this before as well in the color, but here I'm just adding another one
[23:24] just to be sure that I'm adding the cavity map.
[23:27] This is the same thing as before.
[23:29] This is straight up a duplicate of the one before.
[23:32] And then instead of using color, I'm using roughness.
[23:35] So now we get a little bit of, uh, it's a little bit smoother in the creases,
[23:40] not a crazy amount, but just enough to give me a bit more contrast.
[23:43] Then I'm doing the lips as well.
[23:45] Just adding a bit more, uh, adding a bit more variety to the lips as well.
[23:49] Like that.
[23:50] And then we're doing the, a little bit more smoothing off the lips.
[23:55] Like so.
[23:56] And that's really it for the entire head.
[23:58] Now let's talk about the approach for doing the head mushrooms.
[24:04] So same thing as for the other one.
[24:06] We are starting off with, um, with a curvature.
[24:10] And it was really important to me that this was done as procedurally as possible,
[24:13] because honestly, hard to get into it, a lot of these spots.
[24:17] So this was, this had to be as procedural as possible.
[24:20] And then, uh, we have a bit of a, um, I really like this one, B and W spots,
[24:25] zero one.
[24:26] The thesis, this is one of my favorite procedurals, cause this really
[24:29] adds a lot of variety to it.
[24:30] This just looks like this and makes it a little bit darker now, but also adds
[24:33] bit of texture.
[24:34] Then I'm doing a bit of a blend between the, um, this area and the white area.
[24:41] Just so it looks like this.
[24:42] So this just adds a bit more variety to it.
[24:45] And then I have another group here, actually the hat that is just for the
[24:48] orange edge that just has a, a mask like this.
[24:52] And this allows me to have more variety within this.
[24:55] And this was a really important mask to create.
[24:58] And this is made from ambient occlusion.
[25:00] So here I'm in occlusion and I'm painting out certain areas that were too,
[25:04] too extreme.
[25:05] And then I'm using a fill layer on top with a procedural just to, actually,
[25:09] this is with the curvature, just to break it up a little bit.
[25:11] Then we're using levels to, um, you see here, like just what does it really
[25:15] just breaks it up in between.
[25:17] And this is all based on the sculpting.
[25:19] And then there's a little bit of a fading here, which again, again, is just
[25:22] hand painted on top.
[25:24] So this just makes it a bit more comfortable to work with.
[25:27] And then inside this, like specifically the layers here, they're quite simple.
[25:31] Like there's nothing fancy.
[25:32] This is literally just a color that will now be inside the mask.
[25:36] Then there is a yellow layer, which is just hand painted inside here.
[25:40] So this just looks like this.
[25:41] This is just, this is just straight up hand paint.
[25:44] Uh, again, inside a filler.
[25:45] And then we have another one, which is just some darker spots around it.
[25:49] And all, all this comes from the render feedback, what you can, what you can
[25:53] see, what you can't see.
[25:54] And then we're going over with the curvature on top of the whole thing.
[25:57] This adds quite a lot.
[25:59] This makes it darker, but also adds a lot of nice breakup to it.
[26:01] And then I'm going in again, feedback from the render that I need a bit more
[26:06] like focus on the center here.
[26:07] So I'm, and I'm doing that.
[26:09] And then there is another one, which is more like a dark blue center.
[26:12] Like here.
[26:13] And then we have another like B and W spots.
[26:16] This is spots, oh three instead of the other one.
[26:19] And this just makes it a bit more interesting.
[26:20] And then some subtle color variation, probably not very subtle, but some
[26:24] general color variation as well.
[26:26] The thing is you need to be more extreme in the colors because so much
[26:31] disappears when it comes, when it gets into the render engine.
[26:34] And then we have the same thing for the rough, very, very simple stuff.
[26:37] The roughness is actually all enabled right now.
[26:39] So there's not a whole lot new here.
[26:42] It's, um, we still have the edge, the, the, um, the red edge around it, like so,
[26:47] which is this needed to be darker because I really wanted this to be smoother.
[26:51] I really wanted this to be like super shiny.
[26:53] So it looks really wet.
[26:55] And then we just have another curvature on top.
[26:57] And, um, and this is really it for the, uh, for the roughness.
[27:01] So it looks like this.
[27:03] Nice and simple.
[27:05] Then we have the teeth and the teeth are split into two sections.
[27:09] It's split into the actual teeth themselves and split into the gums.
[27:13] So the top one just has the mask.
[27:15] There was no reason to have the mask for the teeth because this is just on top
[27:19] and it's just masked off like this.
[27:20] So this is very nice and simple.
[27:22] The way I'm actually doing this in terms of the masking, this is quite, quite
[27:25] interesting is that I'm, I just saw a paint layer and then I'm using the, um,
[27:30] the fill tool or the polygon fill tool.
[27:32] And then I'm just setting this to UV and then I'm just selecting this.
[27:36] I'm just selecting various chunks.
[27:37] So whatever you click now is just going to be part of this mask.
[27:41] So this is something we're going to be using in a bit, but this is how I'm
[27:43] selecting masks for this.
[27:45] So two groups, teeth and gums.
[27:47] And let's just build this up.
[27:49] The first one is I'm going to just going to enable actually the color of the
[27:51] gum because it looks really weird without.
[27:53] So we're just going to get the gum color.
[27:56] And then we're just going to get in some curvature.
[27:59] The teeth, they are not particularly well developed in terms of sculpting.
[28:02] They probably should have been more.
[28:03] And if the more developed these are, the better the teeth are going to be.
[28:08] Then we're just doing some hand painting on it.
[28:11] And it was really important to me that the edges here, the one connecting,
[28:14] we're really dark, like this person here has, so this zombie here is not
[28:18] brushed her teeth in a very long time.
[28:20] And then we're adding a bit like a muddiness to it as well.
[28:22] And then some teeth variation.
[28:24] What I'm doing here is quite cool.
[28:26] This is where I'm, I'm straight up going in and I have a filler, which has
[28:30] a specific value to it.
[28:32] And then in the teeth variation, I'm using the exact same approach I did before
[28:37] where I have a paint layer and then we use in the polygons fill.
[28:41] And then what I'm doing, the only difference is that I'm just choosing
[28:43] a random amount here.
[28:44] So if this, this, this tooth here should be dark or bright, I'm just going in
[28:47] and being like, yeah, this should be a hundred percent not masked.
[28:51] This year should be a hundred percent masked.
[28:52] And I can just see what happens if we go into this.
[28:55] Now you can see that this here is going to be affected and this is not going
[28:59] to be affected.
[28:59] So this is a really cool approach for getting just like level variety or a
[29:04] value variety.
[29:06] Then I'm painting on the teeth as well, just hand painting.
[29:08] And that's the teeth.
[29:10] Then we do the same thing for the gums.
[29:13] And we're just adding a bit of, um, adding a bit of variety here.
[29:16] This is just using a fill layer with a grunge procedural.
[29:21] And then we're doing another one, just some, some pretty saturated pink.
[29:24] Then we're doing a bit of brighter here, integrating the teeth a bit more.
[29:27] This is all based on reference as well.
[29:29] Then adding cavity to it.
[29:31] Uh, this is just a curvature to it.
[29:33] So all the cavities are just a bit more pronounced.
[29:35] And then we are going over and just making this darker.
[29:38] Again, this all comes from render feedback.
[29:41] It's really hard to make texturing videos, which are just purely linear
[29:45] because you literally need feedback from the render along the way.
[29:49] And then we have these little guys, which are very, very simple.
[29:52] There's a curvature to it.
[29:54] And then there is a procedural and then there is a brighter edges, which is
[29:57] just, uh, just painted like very simple.
[30:00] This took like just a few minutes.
[30:01] Don't be afraid to do hand painting though.
[30:03] Don't be afraid to do manual labor like this.
[30:06] Sometimes just have to do manual labor.
[30:09] I got about this far.
[30:11] And then I did the first test render, which was this one.
[30:13] And I realized you really can't see them a lot.
[30:15] So I just kind of stopped.
[30:16] And even at the end render, same apps, you really can't see them a lot.
[30:21] So keep it simple.
[30:22] Don't over-texture something.
[30:24] Don't texture something that you're never going to see.
[30:27] Now, obviously, if this was a hero character for a game or a TV series,
[30:31] you would absolutely do that because then it doesn't just need to work
[30:34] from one shot and needs to work from multiple shots.
[30:36] So for that, in that case, you would actually have to work a little
[30:39] bit on the back as well.
[30:40] Like here you can see, like there's nothing here.
[30:42] And this was because when I UV mapped it, this, this little piece here is
[30:46] straight up just like chucked away.
[30:48] This has no texture density whatsoever.
[30:50] Now, once the textures are level like this, I highly recommend you try out
[30:53] IRA, just click the little camera icon up here.
[30:56] And you're just going to get a preview as well of what this is going to look like.
[31:00] Now, the advantage of using IRA is that you don't actually have to
[31:03] export out the maps and set this up in, in something like Blender or Arnold
[31:08] or anything like this, because here you can see it directly.
[31:11] So I used this quite a lot early on and also just to test different things.
[31:15] Now, just be aware that this is not going to be exactly the same as render.
[31:18] For one, we're using a low risk model here and we're using a high risk model
[31:21] for the render and towards the decimation.
[31:24] And then the shader model is also probably a little bit different, but in
[31:27] general, pretty good approximation.
[31:30] Like this, this is a good way to, to get an idea of, of it's, if it's working or not.
[31:35] And if you think it's working, then you can export this out.
[31:38] But once you have set up the pipeline for the character, then it's really easy.
[31:43] Then you just set control shift E to export, then you just hit like
[31:47] whatever thing you want to export here, hit export.
[31:49] I'm just overwriting the maps constantly here.
[31:51] So I'm not picking new maps.
[31:53] So I'm just overwriting, then I'm refreshing the maps in Blender.
[31:57] And then I just get a new render.
[31:58] So iterating on the maps here is just click export, refresh and Blender.
[32:05] And then you see the render.
[32:07] The render is so fast, the blender, it cycles the CPU based really, really fast.
[32:12] So it's not as fast as this, but it's correct.
[32:15] At least, you know, I get older depth of field and I get older correct shaders,
[32:18] the correct subsurface amount.
[32:19] So it's that's definitely something I'm doing at the end as well.
[32:22] And towards the end, the iteration becomes tiny.
[32:26] It's like you're dealing with like, oh, this dot here needs to move from here to here.
[32:30] So it's not necessarily something you have to keep re-rendering all the time.
[32:35] You can just keep changing it here as well.
[32:37] But I do recommend actually straight up overwriting the maps, at least when
[32:41] you're working for yourself like this and you're just iterating, because it's so much faster.
[32:46] What you can also do, you can just export out the maps in different folders,
[32:49] but then you have to re-link them all the time, which is just annoying.
[32:52] This is a note at the end.
[32:53] I'm using Blender for the UV mapping and the assignment of shaders and the rendering at the end.
[32:59] But you can do this in any software.
[33:01] Like cycles is pretty neat when it comes to the GPU rendering, but you can use
[33:05] MyRMAX, Cinema 4D or anything like there's nothing spectacular about Blender for
[33:10] this kind of work.
[33:12] It's just, it just happens to be the software that I'm currently using.
[33:16] And it works really well, but feel free to use whatever you want to.
[33:20] So that's it for this tutorial.
[33:22] I hope this here was useful.
[33:24] We'll see you in the next one, where we are working on lighting and shading this guy in Blender directly.
[33:31] Make sure to check out Flicknomes.com, which has a lot of amazing training focused on character art,
[33:36] but also a lot of general CG topics.
[33:38] So we'll see you in the next video.



---

## Captured Frames

- [4:24] tutorials/frames/texturing-a-clicker---full-substance-3d-painter-workflow/frame_000.jpg
- [8:30] tutorials/frames/texturing-a-clicker---full-substance-3d-painter-workflow/frame_001.jpg
- [9:37] tutorials/frames/texturing-a-clicker---full-substance-3d-painter-workflow/frame_002.jpg
- [10:33] tutorials/frames/texturing-a-clicker---full-substance-3d-painter-workflow/frame_003.jpg
- [13:37] tutorials/frames/texturing-a-clicker---full-substance-3d-painter-workflow/frame_004.jpg
- [19:48] tutorials/frames/texturing-a-clicker---full-substance-3d-painter-workflow/frame_005.jpg
- [20:17] tutorials/frames/texturing-a-clicker---full-substance-3d-painter-workflow/frame_006.jpg
- [21:41] tutorials/frames/texturing-a-clicker---full-substance-3d-painter-workflow/frame_007.jpg
- [24:20] tutorials/frames/texturing-a-clicker---full-substance-3d-painter-workflow/frame_008.jpg
- [25:00] tutorials/frames/texturing-a-clicker---full-substance-3d-painter-workflow/frame_009.jpg
- [28:26] tutorials/frames/texturing-a-clicker---full-substance-3d-painter-workflow/frame_010.jpg
- [30:53] tutorials/frames/texturing-a-clicker---full-substance-3d-painter-workflow/frame_011.jpg

---

## Structured Notes

### Core Technique
A professional creature-texturing workflow philosophy demonstrated end-to-end on a fan-sculpted "Clicker" (The Last of Us) bust: organize the layer stack into per-channel groups (a Color group and a separate Roughness group, per texture set) rather than combined multi-channel Fill layers, build every material as a hybrid of procedural generators (curvature, AO-driven masks, B&W spots, marble noise) plus deliberately hand-painted color-variation passes, and treat iterative Iray/external-renderer test-renders as a mandatory checkpoint throughout — because texture decisions that look right in Painter's viewport frequently read as too subtle (or entirely wrong) once actually rendered.

### Summary
Henning (FlippedNormals; Whisper mis-transcribed the site name as "FlukeNomers.com") walks through texturing his own fan-sculpt creature bust, framing good sculpting as the real foundation of good texturing (bake quality, SSS accuracy, and roughness-map ease all trace back to sculpt quality) before ever opening Painter. **Baking:** decimates the ZBrush sculpt to per-texture-set high/low pairs via ZPlugin > Decimation Master, exports through Blender with consistent `_low`/`_high` naming and one material per texture set (texture sets are planned to mirror how materials would be assigned in a DCC), imports the low-poly FBX into a Legacy-color-space project, and bakes Normal/World Space Normal/ID/AO/Curvature/Position/Thickness at 1K using Painter's newer baker (matched by mesh name) — explicitly baking maps that aren't used directly, because many generators depend on them internally. **Organizational philosophy:** one group per texture-set part (e.g. tongue, head) with the mask isolating that part; inside, a Color group and a separate Roughness group (not combined per-material Fill layers) — acknowledged as less GPU-optimal but far easier for a human (including a future self or collaborator) to read and edit. **Core head material build:** starts with a plain base Fill layer (Color+Height+Roughness) to establish local color before any complexity; a darker Fill layer masked by a black mask + Fill sub-layer using a `Curvature` generator (which depends on the earlier-baked World Space Normal + Position/gradient maps) adds instant procedural "pop"; then a series of explicitly hand-painted color layers (red into deep crevices/scar tissue, yellow over bone areas, blue for a "dead" feel, green set to `Soft Light` for subtle breakup) using a small set of favorited brushes (Basic Soft, Cotton, Dots/Dots Erased for pores-and-pimples and the creator's primary sculpting-like brush, Dust for subtle top breakup, Smooth Noisy). A hand-painted dark-contrast layer follows, with an explicit warning against painting directly into a mask (locks out later opacity control — always paint into a Paint sub-layer instead) and a strong recommendation to push saturation rather than pure value-darkening for shadow areas, since desaturated darkness reads as flat/boring once rendered. **Iterative render-testing** is treated as a first-class step, not an afterthought — Henning shows a sequence of his own Iray/Blender-Cycles test renders across the project, each surfacing a different actionable note (sculpt needed more mid-frequency detail; head-mushroom edge roughness needed smoothing per feedback from colleagues; a large Photoshop-graded color shift on a test render got reproduced directly on the actual Fill-layer colors in Painter, rather than as a non-destructive grade, specifically because flat-color Fill layers make that trivial to do live). **Organic-skin detail:** two layers of Tri-Planar-projected, scaled-down `Marble` texture (chosen deliberately — "marble textures is awesome... almost looks like meat") add believable mottled organic variation; a hand-painted pimple pass uses a Paint layer specifically so its color can be changed instantly without regrading (and notes a variant technique for multi-colored pimples: mask a group with the paint pattern, then vary Fill-layer colors inside). **Combined-channel exception:** for blood specifically, Henning deliberately breaks his own Color/Roughness-separation rule and combines both channels on the same Fill layers (rough crusted blood, vibrant fresh blood, roughness streaks) so that painting once affects both Color and Roughness simultaneously — flagged as something anchor points could technically also achieve, but dismissed as "confusing as hell" in favor of this simpler combined-layer approach. **Roughness for the head** is built mostly by duplicating the same curvature/cavity setup used for color and re-targeting it at the Roughness channel instead, since a well-developed sculpt needs comparatively little separate roughness work. **Head-mushroom material:** curvature + a favorite `B&W Spots 01` procedural for organic-looking variety, plus a dedicated sub-group for the mushroom's orange edge whose own mask is built by hand-painting corrections onto the baked **Ambient Occlusion** map (removing overly extreme AO in specific spots) then layering a Curvature-generator Fill and a `Levels` filter on top to break the AO-based mask up further — described as "a really important mask." **Teeth/gums:** split into two groups; a reusable masking trick is introduced here — add a Paint layer, switch its brush to the **Polygon Fill Tool** in **UV** mode, then click individual UV shells/tooth-chunks to instantly assign each one 100%-masked or 0%-masked, producing fast per-tooth value/brightness variation without hand-painting each tooth's silhouette. **Preview and export loop:** Iray viewport preview (camera icon) is used constantly for a fast, in-Painter approximation (acknowledged as imperfect versus the real low-vs-high-poly/shader differences of a full external render) before committing to `Ctrl+Shift+E` export; for iterative work, Henning recommends overwriting the same export path every time (not incrementing filenames) so a Blender-side "refresh textures" plus re-render becomes the entire iteration loop.

### Key Steps
1. **Prioritize sculpt quality before texturing** — mid/high-frequency sculpted detail directly improves tileable-map disguise, bake quality, SSS plausibility, and roughness-map ease; texture work cannot fully compensate for an underdeveloped sculpt.
2. **Decimate per texture set at both high and low resolutions** (ZPlugin > Decimation Master in ZBrush), export through a DCC (Blender used here, but any 3D software or even direct ZBrush FBX export with polygroups works) with consistent `_low`/`_high` suffixes and one material per texture set — plan texture sets exactly as you would plan material assignment.
3. **Import the low-poly FBX into a new Painter project** (Legacy color space used here, nothing exotic) and bake via the newer built-in baker: load the high-poly, set Match to "By Mesh Name," and bake Normal/World Space Normal/ID/AO/Curvature/Position/Thickness at a modest resolution (1K here) even for maps not used directly, since many generators consume them internally; rebake at higher resolution later only if needed.
4. **Organize the layer stack per texture-set part, then per channel:** one group per model part (masked to that part only), and inside each, a separate Color group and Roughness group rather than combined-channel Fill layers — a deliberate trade against pure performance, favoring long-term editability and readability.
5. **Start every material with a plain base Fill layer** (flat Color/Height/Roughness values) to lock down local color before adding any complexity.
6. **Add instant procedural variation with a Curvature generator:** on a darker Fill layer's black mask, add a Fill sub-layer with a `Curvature` generator (depends on the baked World Space Normal + Position maps) — purely bake-driven, no Tri-Planar or other proceduralism involved, so bake quality directly limits this step's ceiling.
7. **Layer in deliberately hand-painted color variation:** red into crevices/scars, yellow over bone-like high points, blue for a "dead" undertone, green set to blend mode `Soft Light` for subtle breakup — using a small favorited brush set (Basic Soft, Cotton, Dots/Dots Erased, Dust, Smooth Noisy; favoriting via right-click, a then-fairly-new Painter feature).
8. **Add a hand-painted dark-contrast layer, painted into a Paint sub-layer (never directly into the mask)** — painting straight into a mask permanently destroys later opacity control over that edit; push color saturation for shadow areas rather than just lowering value, since desaturated darkness reads as flat once actually rendered.
9. **Test-render early and often** (Iray in-Painter preview and/or an external renderer like Blender Cycles) — use each render to identify concretely what's working/not working (sculpting gaps, unconvincing roughness, colors that read differently once lit) rather than judging purely from Painter's viewport.
10. **Reproduce large color grading decisions directly on the source Fill-layer colors**, not as a non-destructive adjustment layer, when a Photoshop-graded test render reveals a big color shift you want to keep — flat-color Fill layers make this a fast, direct edit.
11. **Add organic surface variation with Tri-Planar Marble noise:** two layers of a `Marble` texture, projection set to Tri-Planar, scale reduced, for believable mottled/meat-like organic detail without hand-painting every pore.
12. **Build a fast-iterating pimple pass:** hand-paint pimples/pores into a Paint layer specifically so the layer's color can be changed instantly afterward without regrading; for multi-colored pimple variation, mask a group with the same paint pattern and vary Fill-layer colors inside that group instead of painting each color separately.
13. **Deliberately combine Color+Roughness on the same layers for effects that must move together** (blood, here): break the earlier Color/Roughness-separation rule specifically so one paint stroke affects both channels simultaneously — considered simpler and more direct than the anchor-point alternative for this particular need.
14. **Reuse the color-layer curvature/cavity setup for roughness** by duplicating it and switching the target channel — a well-developed sculpt needs comparatively little dedicated roughness complexity.
15. **Build a bake-corrected mask from Ambient Occlusion:** for the head-mushroom "orange edge" sub-group, hand-paint corrections directly onto the baked AO map (removing overly extreme dark spots), then add a Curvature-generator Fill layer and a `Levels` filter on top of that same mask to break it up further — flagged explicitly as "a really important mask" for that material's believability.
16. **Split teeth and gums into separate masked groups**, and use a `B&W Spots` procedural + hand-painted darker edges (grime buildup at the gumline) for the teeth base.
17. **Assign per-tooth value variation via the Polygon Fill Tool trick:** add a Paint layer, switch its tool to Polygon Fill mode set to `UV`, then click individual UV shells (e.g. one tooth each) to instantly set each one to a chosen mask value (e.g. fully masked or fully unmasked) — fast, precise per-chunk variation without manual painting.
18. **Use the Iray viewport preview (camera icon) for fast in-Painter iteration**, understanding its limits (uses the low-poly model and an approximate shader, unlike a true external high-poly/shader-accurate render) — good for quick go/no-go checks, not a substitute for final external rendering.
19. **Set up an overwrite-based export/refresh loop for external rendering:** export via `Ctrl+Shift+E` to the same file path every iteration (don't create new filenames), then simply refresh textures in the external DCC/renderer (Blender shown here) and re-render — keeps the iteration loop to two clicks once the pipeline is set up once.

### Layers / Tools / Settings
- **Baking:** Normal, World Space Normal, ID, Ambient Occlusion, Curvature, Position, Thickness — 1K, Match by Mesh Name, newer built-in baker
- **Organization:** per-part groups (masked), Color group + separate Roughness group per part, one texture set per logical material
- **Base:** flat Fill layer (Color/Height/Roughness)
- **Procedural pop:** black mask + Fill sub-layer with `Curvature` generator (consumes baked World Space Normal + Position)
- **Hand-painted color variation:** red/yellow/blue/green Paint layers (green at blend mode `Soft Light`); brush set: Basic Soft, Cotton, Dots, Dots Erased, Dust, Smooth Noisy (favorited via right-click)
- **Dark contrast:** Paint sub-layer (never directly on the mask), saturation pushed over pure value-darkening
- **Organic detail:** `Marble` texture, Tri-Planar projection, scaled down, x2 layers
- **Pimples:** Paint layer for instant recolor; group-mask + varied Fill-layer colors for multi-color variants
- **Blood (combined-channel exception):** Fill layers carrying both Color and Roughness simultaneously (rough crusted blood, vibrant blood, roughness streaks)
- **Roughness:** duplicated curvature/cavity Fill setup retargeted to the Roughness channel
- **Head-mushroom edge mask:** hand-painted corrections on the baked AO map + Curvature-generator Fill + `Levels` filter
- **Teeth variation:** Paint layer + Polygon Fill Tool set to `UV` mode, click-to-assign per-UV-shell mask value
- **Preview/export:** Iray viewport (camera icon) for fast preview; `Ctrl+Shift+E` export to a fixed overwritten path for a refresh-and-rerender iteration loop with an external DCC/renderer

### Difficulty
Advanced — not because any single tool is exotic, but because the video is fundamentally about professional judgment: organizational discipline (channel-separated groups) that trades performance for maintainability, the hand-painting-vs-procedural balance for organic creature skin, reading render feedback to prioritize where detail actually matters, and several efficiency tricks (Polygon Fill UV masking, combined-channel exception for coupled effects, fixed-path export/refresh loop) that assume comfort with the fundamentals already.

### App & Version
Not stated numerically on screen. Two relative-version markers are called out by the creator: the baking-panel baker is referred to as "the new baker they're adding" (a then-recent addition, implying this was recorded shortly after a baker update), and brush right-click favoriting is called "fairly new." The project uses multiple UDIM/UV Tiles per texture set (visible in the Texture Set List panel across several captured frames) and Painter's Legacy color space (not ACES/OCIO). Neither marker pins an exact version number, but both are consistent with this skill's modern-era ingested tutorials.

### Tags
layers, fill-layer, paint-layer, masks, generator, curvature, ambient-occlusion, mesh-maps, world-space-normal, position-map, high-to-low-poly, baking, cage, udim, texture-set, uv, pbr, basecolor, roughness, height, alpha, procedural, tri-planar, blend-mode, iray-render, viewport, color-management, advanced

---

## Related Tutorials
- [Shading & Lighting a Character - Blender and Substance 3D Painter Workflow](shading-lighting-a-character---blender-and-substance-3d-painter-workflow.md) — same creator (FlippedNormals), same character/project, direct sequel — covers what happens to this video's finished Painter maps once brought into Blender for shading/lighting/rendering, including the "reproduce any downstream color correction back in Painter" discipline that extends this video's live Fill-layer color-editing workflow.
- [10 New Features in Substance Painter You Didn't Know About](10-new-features-in-substance-painter-you-didnt-know-about.md) — same creator (FlippedNormals); this Clicker video's UDIM/UV Tiles texture-set organization and baking step are a direct real-world application of that feature-tour video's UDIM-support and new-bake-types entries.
- [Texturing Creatures for Games in Substance Painter | Full Process](texturing-creatures-for-games-in-substance-painter-full-process.md) — different creator (Logan Wiesen); shares the same creature-texturing philosophy of combining procedural generators with deliberate hand-painted color-variation passes, and the same emphasis on verifying bakes/results against real shading before committing to further detail.
- [REALISTIC CREATURES: HAND PAINTED TEXTURES in SUSTANCE PAINTER](realistic-creatures-hand-painted-textures-in-sustance-painter.md) — different creator (Jared Chavez); shares the anatomy-driven hand-painted color-zone-blocking approach (red/yellow/blue-style directional color coding) applied here to a different creature.
- [SUBSTANCE PAINTER: Building Masks Explained](substance-painter-building-masks-explained.md) — different creator (Jared Chavez); this Clicker video's AO-map-hand-correction-then-Curvature-then-Levels mask-building chain for the head-mushroom edge is a direct real-world application of that video's core "mask effect stack" teaching.
