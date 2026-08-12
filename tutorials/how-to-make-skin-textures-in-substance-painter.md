---
title: How to make SKIN TEXTURES in Substance Painter
source: YouTube
url: https://www.youtube.com/watch?v=s0DhvFML7oM
author: J Hill
ingested: 2026-08-12
app: "Adobe Substance 3D Painter"
version: "not stated on screen; baking dialog UI matches the pre-8.3.0 inline 'Bake Mesh Maps' dialog (replaced by dedicated Baking Mode in 8.3.0, 2023-01-10) — likely predates 8.3.0, tentative"
tags: [layers, fill-layer, paint-layer, masks, generator, curvature, ambient-occlusion, thickness, tri-planar, procedural, blend-mode, pbr, basecolor, roughness, specular-glossiness, normal-map, height, alpha, color-management, texture-set, export, export-preset, channel-packing, intermediate]
extraction_status: complete
frames_dir: tutorials/frames/how-to-make-skin-textures-in-substance-painter/
frame_count: 14
frame_status: complete
frame_selection: content-anchored (manual timestamps chosen from transcript, not blind percentages)
---

# How to make SKIN TEXTURES in Substance Painter

**Source:** [YouTube](https://www.youtube.com/watch?v=s0DhvFML7oM)
**Author:** J Hill
**Duration:** 65m0s | 19 section(s)

---

## Raw Data (for Claude Code extraction)

Frames captured — see "Captured Frames" section below.


### Intro [0:00]
**Transcript (timestamped):**
[0:00] Hey, I'm Jay, and in today's video, we're going to be talking about texturing skin in Substance Painter.
[0:09] Starting with the model and the normal map we made in the last video, in this video, we're going to make the skin textures.
[0:16] Step 1, reference.
[0:19] Alright, cool. So what we're going to do is...
[0:21] Here's my screen. This is my reference, and we're going to talk a little bit about it.


### Reference [0:22]
**Transcript (timestamped):**
[0:26] But this is kind of a general, you can see from a bird's eye view, what's going on.
[0:29] In terms of skin tone and details, I'm kind of aiming at this area.
[0:34] I like the idea of maybe like a mixed ethnicity or one that's a little bit more difficult to pin down, a little bit more subjective.
[0:41] I think that's interesting. Love the freckles here.
[0:45] So this might be a nice addition and a fun thing to show.
[0:48] And yeah, generally, you know, a middle skin tone, not too light, not too dark.
[0:53] Alright, so that's what we're aiming at here.
[0:55] I got some makeup here, but we probably won't be doing any of this in this kind of video.
[0:59] Today we're going to be texturing in Substance Painter.
[1:01] We're going to make a base color.
[1:03] And then if time permits, maybe we'll make a quick little roughness map too.
[1:07] Two really important kinds of imagery that are extremely important as reference for base color maps in particular,
[1:15] is RBX imaging and cross polarized photographs.
[1:20] So RBX imaging actually was first tipped off about this by Magdalena or at Intervain on Twitter.
[1:28] She's another character artist.
[1:30] This was a great tip that she gave a long time ago.
[1:32] This is used in other industries.
[1:34] Both of these is actually used in CG a lot, but RBX is used in other industries for, I think, skin purposes, honestly.
[1:40] But look how cool.
[1:42] Look what's going on here. This is even crisper one.
[1:44] But look how cool. We've actually separated.
[1:47] You look here, this red channel and then this kind of brown color are different.
[1:51] These are not the same.
[1:52] So this is different details.
[1:54] And you'll see once we're in Substance Painter how this is really useful because we're going to be layering effects.
[2:00] So essentially we have two images here that we can see like separated almost channels of really crunched and sharpen detail
[2:09] that's beneath the skin we can see here on the left.
[2:11] So obviously this is with subsurface scattering and all that fancy stuff.
[2:15] So this is sun damage and stuff.
[2:17] This is like freckles and sunspots if you didn't have anything covering it.
[2:22] So you can see here the mole.
[2:24] These things would be freckles, right?
[2:26] And so when we see him, you can see here's that mole and here's some very light freckling, this light brown stuff.
[2:33] So you can actually just see it straight up.
[2:35] The reason why this is super beneficial is the patterns kind of a noise, right?
[2:38] And this is like the blood.
[2:39] So we see the splotchiness.
[2:40] We see lots of noise.
[2:42] We see kind of veiny type shapes maybe.
[2:45] Great reference.
[2:46] And then cross polarized photography, Texture XYZ actually sells packs that you can just purchase that you can use either for,
[2:56] you can actually just project textures on, which is really common.
[2:59] Or what we're doing right now, we're using it as reference.
[3:02] And what cross polarized photography is, is essentially photographs using filters to remove reflected light.
[3:09] So it's like not having a spec channel.
[3:11] So you're essentially seeing a real life base color map, which is obviously the best reference right off the top.
[3:17] Just, you know, obviously you came to this video.
[3:20] This is painting skin in substance painter.
[3:23] You might be asking the question, why would you paint skin in substance painter?
[3:27] You know, you could use Mari.
[3:29] You could use all kinds of different photogrammetry and different techniques.
[3:34] It really depends on your end goal.
[3:36] What I'm doing for this demo project is very much what I do in my personal work and even professional work.
[3:42] So we're hand making everything.
[3:43] We're kind of curating it.
[3:44] It's going to lend itself to somewhat of a style.
[3:47] We're not, we're not trying to replicate photography one to one really.
[3:51] But also it's a great exercise.
[3:53] It's a great tutorial kind of thing or a practice to do.
[3:56] If you want to get better at painting complicated organic things in substance painter,
[4:01] this kind of technique is going to help you if you were to make creatures and aliens and things that don't exist.
[4:07] It helps to kind of understand skin a little bit and making base color maps and how it mixes together.
[4:13] And ultimately I think it produces a pretty cool result.
[4:16] I don't know what it's going to look like now.
[4:17] We're going to, we're going to find our way during the process,
[4:20] but I find it generally satisfying to make the maps.
[4:24] It's kind of the old school way, I guess you might say.
[4:26] But again, I feel like it gives you also creatively and artistically,
[4:30] it gives you the most control right out of the gate because you are making every element, right?
[4:34] You're not taking a photograph and repurposing it.
[4:38] So there is some pros and cons there, but the methods do produce different results.
[4:43] So you just got to ask yourself what your end goal is for your project and then choose what's best.
[4:49] So right now we're going to be painting a base color in substance painter.
[4:52] Let's jump into substance painter now and talk about how we can set up the scene with our models we made in the previous video.
[4:59] And we can get ourselves ready to do texturing.


### Setting up Substance [5:02]
**Transcript (timestamped):**
[5:02] All right, so here we are in substance.
[5:04] Now what we need to do is we need to load in our model and set up the parameters of the scene and then get going with starting to set up our scene to do some painting.
[5:12] So first things first, we need to go file new.
[5:14] Then we're going to choose a template.
[5:18] PBR metal rough will work fine.
[5:20] This is in the starter assets.
[5:21] So everyone has this super basic and this will be fine.
[5:24] This is like the most basic template we can use.
[5:26] Next we got to choose our file.
[5:28] So we're going to choose our model.
[5:30] In our case, we exported this from Z brush.
[5:33] We used HD geometry and when we use HD geometry, we exported the normal map at 8k in our case, which got us all the deets.
[5:43] And we're going to bring that in a second.
[5:45] So it's a little bit of a different workflow than if you were baking a high to low.
[5:49] But here we are.
[5:50] I exported my subdivision level four right here in Z brush.
[5:53] So I actually just isolated the part that I'm going to do the demo on.
[5:56] You can see if we zoom in, this is the resolution that we're at.
[5:58] So this is the highest resolution I have without going into HD.
[6:01] When I did export it, I made sure smooth normals is on.
[6:04] It should be on by default.
[6:06] And that's really it.
[6:07] I just exported it as an FBX and then I can load it into substance painter.
[6:11] So here it is right here.
[6:12] And then we just got to choose the document resolution.
[6:14] We'll make it 4k.
[6:15] That's as big as it goes right now, I think.
[6:17] And then a little awkward tidbit is for me, I think I need to change the normal map format to open GL.
[6:23] You can change this later.
[6:25] Don't be too scared of this.
[6:26] This is just the green channel in the normal map direction.
[6:30] Is it up or is it down?
[6:31] And I did a test before and it seems like it was flipped.
[6:34] So it depends on your export settings from Z brush.
[6:37] If you're bringing normal map in from any other program,
[6:40] you just got to be sure what orientation the green channel is.
[6:43] All right, we'll hit OK.
[6:44] And now we are going to load our scene.
[6:47] Boom, here we go.
[6:48] She's in.
[6:49] All right, I'll just save this right off the top.
[6:51] Let's just save our scene.
[6:52] All right, let's take out the pen, start doing some artsy stuff, at least starting to prep it.
[6:57] What we'll do now is bring in our map and start to set up the scene to do our painting.
[7:04] So we can do a couple of things.
[7:06] Either when we started here in our project configuration,
[7:09] we could have loaded the normal map right when we set up the scene,
[7:12] or we can just hit plus right now and then add resources.


### Generating Maps [7:13]
**Transcript (timestamped):**
[7:16] And then we can go to wherever we have our normal map.
[7:18] So I'm just going to click the normal map and choose this.
[7:21] And then this is a texture.
[7:23] And then I can just keep it in this project.
[7:26] You have current session, which would end if I close it.
[7:29] And then library, obviously, for everything else, which we don't need.
[7:31] So just adding it to this project, there it is.
[7:34] And I can just drag it over there.
[7:36] So now we have our 8K normal map.
[7:40] This is all the detail that we sculpted in ZBrush.
[7:42] And we didn't do any baking.
[7:44] It's just right there, right?
[7:45] Because we exported it from ZBrush.
[7:47] So again, a little bit of a different workflow,
[7:49] because now we're going to generate some maps from this.
[7:52] So I'll come over here to the baking.
[7:54] Right now, why don't we just start with the curvature map,
[7:57] make sure things are working.
[7:59] We can go to 2K for now.
[8:01] Well, we can just go to 4K.
[8:02] This shouldn't take too long.
[8:03] So in the curvature settings here,
[8:06] you can see it's on generate from mesh,
[8:08] which is really nice and high quality if you're doing that.
[8:10] But we're not baking a high to a low.
[8:12] The normal workflow or the typical workflow
[8:15] would be in the common settings,
[8:17] you'd be adding meshes right here.
[8:19] You'd load the high poly.
[8:21] You'd have a bunch of meshes here, right?
[8:22] And then you would bake high to low
[8:24] using the cages and stuff like that.
[8:26] But we're not doing that.
[8:27] We already have the normal map.
[8:29] So we're going to just derive the detail from the normal map.
[8:33] So I'll show you how that works with the curvature map.
[8:35] Okay, so in the curvature settings,
[8:37] instead of generate from mesh,
[8:38] we'll go to generate from normal map.
[8:40] Details, we'll leave it at 0.5.
[8:42] So this shouldn't be on, obviously,
[8:44] it's brought in our normal map, right?
[8:46] It's loaded right here, so it shouldn't be checked.
[8:48] We'll hit bake, and then here it's going to do its thing.
[8:51] So now it's generating a curvature map from our normal map.
[8:54] So if we come in here and we just check the curvature channel,
[8:58] here it is.
[8:59] Doesn't look great, I know,
[9:02] but it'll be okay.
[9:04] We're just going to be using it for some chatter.
[9:07] Some people overvalue like cavity maps and stuff.
[9:10] I'm not too worried about it.
[9:11] We're just getting some details.
[9:12] So let's jump back out of here,
[9:15] and maybe we can generate some more things.
[9:17] Let's see what happens.
[9:19] We might not use these.
[9:21] World normal map.
[9:22] Ammy inclusion might not look that good,
[9:24] but that's okay.
[9:25] No, it looks pretty good, actually.
[9:26] It's cool that it's making this from the normal map.
[9:29] It used to always do this,
[9:30] but now you can generate ammy inclusion maps
[9:32] and curvature maps from the geo, which is better.
[9:35] And you might be asking now, why are you doing this?
[9:38] Well, it's in case we wanted to use certain generators.
[9:43] We might not be, though.
[9:45] So this could be useless, which is fine.
[9:49] It doesn't take that long to bake.
[9:51] It's almost done baking now,
[9:52] and I'll just save the scene and I'll have these maps.
[9:55] So with all these maps,
[9:56] if you wanted to do a top-down gradient,
[9:58] if you wanted to do certain dirt and whatever.
[10:01] Here we go, curvature, position map, thickness,
[10:04] which might help.
[10:05] Sometimes I use the thickness map when I'm making skin.
[10:07] You can see it kind of highlights things nicely.
[10:10] And our normal maps, obviously.
[10:11] So there you go.
[10:12] Let us save this scene,
[10:15] and then we'll start setting it up to paint.
[10:17] Okay, I'm going to do just some general,
[10:20] really quick stuff here.
[10:22] This focal length is killing me.
[10:24] So why don't we just do something like this?
[10:26] All right, so first thing,


### Making the Base [10:27]
**Transcript (timestamped):**
[10:27] we'll just delete this basic thing,
[10:29] and we'll start with a fill layer.
[10:30] And we'll just call this base color.
[10:32] Why not?
[10:33] So what we're going to do
[10:35] is we're going to have these layers in substance, right?
[10:38] And we're going to layer them from top to bottom,
[10:40] or from bottom to top in this case,
[10:42] as if we were kind of airbrushing
[10:44] or painting up layers of skin.
[10:46] And we'll jump around.
[10:47] We'll keep things non-destructive.
[10:49] That's the beauty of using substance painter
[10:51] rather than some other straightforward things.
[10:54] So if it makes sense, we can separate brush strokes.
[10:56] We can always change color,
[10:58] and we're just going to kind of layer detail as it goes.
[11:01] So the first thing we're going to do
[11:03] is we're going to start relatively warm.
[11:06] You know, we want to make that bloody layer.
[11:08] We kind of saw some of the RBX imaging might help us
[11:12] while we make the detail portion of that.
[11:14] But we'll start with a very warm color,
[11:16] and then we'll layer our detail up on top.
[11:18] I think what makes a good base color
[11:20] is a variety of subtle differences.
[11:24] Subtle differences in shape,
[11:26] subtle differences in value,
[11:29] subtle differences in color,
[11:31] and then also a mix of soft edges and sharpness.
[11:36] It's something that I think having sharp detail
[11:40] is something I think that does make renders and skin look nice
[11:44] and believable.
[11:46] Contrast really is what we're talking about, right?
[11:48] Like some things are soft, some things are sharp.
[11:50] Some things are this color, some things are that color.
[11:52] But the difference in what makes skin skin
[11:55] is that when we're done, it'll look relatively even.
[11:59] You know, you'll have these big general,
[12:01] like maybe the eyes are dark, it's those big gradients.
[12:04] But as you zoom in, there's going to be differences,
[12:06] but they're not going to have a lot of contrast
[12:08] because that would create all this busy noise.
[12:10] So it's going to be subtlety and organic shapes.
[12:13] We want to add all kinds of imperfections
[12:16] to help it feel believable.
[12:18] So let's start making colors.
[12:20] If you hold Alt and just click that,
[12:22] you can just do straight up colors.
[12:24] So why don't we just do this?
[12:26] Also, since this is the base,
[12:28] you know, we can just get a little bit of roughness here.
[12:31] Okay, so now we can continue adjusting our colors
[12:35] if we want.
[12:37] And first, what we're trying to do is make a lighter,
[12:40] red, blood kind of color as our base here.
[12:43] And then we're going to add our first fill layer,
[12:46] and that'll be our darker red color.
[12:49] And so the first thing we're going to do
[12:51] is we're going to try to create this complicated shapes
[12:54] in our base colors here that we can layer in on top.
[12:58] So once we make our fill layer,
[13:00] we'll create a black mask.
[13:03] And in that black mask, we can create a fill,
[13:05] and then in that fill,
[13:07] we can put whatever textures we want.
[13:09] So if we go down to our library
[13:11] and we search for noise in our textures,
[13:13] we can see all the different options we have.
[13:15] So we can pick one and just drag that into the channel
[13:18] on the left, and then we can start playing with the parameters.
[13:21] So this is where you should just have fun and experiment.
[13:23] What we're going to do is mix several.
[13:25] So once we get something that we generally like
[13:27] that's nice and noisy,
[13:29] I probably like to start out big and blobby first,
[13:31] get some interesting shapes.
[13:33] Then we'll get smaller and more refined over time.
[13:35] We can then add another fill layer
[13:37] and look for a different kind of noise,
[13:40] and definitely we want to have some kind of contrast
[13:42] in the scale between these two noises.
[13:44] So maybe we make smaller noise.
[13:46] And then we can start mixing these together in our mask
[13:50] by changing the blend mode of our next fill layer to screen,
[13:54] which just like in Photoshop is layering it up
[13:56] in terms of the light values.
[13:58] And then we can start to play with these things together.
[14:01] This is the beauty of Substance.
[14:02] This is the format I'm going to be doing over and over again,
[14:05] is creating masks on fill layers,
[14:07] sometimes creating masks on folders,
[14:09] and then layering up different fills
[14:12] to make these complex masks
[14:14] where as you can see, everything is live.
[14:17] We can change the colors and roughness.
[14:19] We can change the parameters in our masks.
[14:21] We can add, remove, delete at any time.
[14:23] So we want to stay organized
[14:25] because this can get messy and complicated fast.
[14:28] We want to take a step-by-step
[14:30] and control it as much as we can before we get ahead of ourselves.
[14:32] And we also want to leave ourselves
[14:34] like a few amount of tools to play with.
[14:36] We don't want a ton of things where we just get swamped.
[14:38] So after we make our base noise here
[14:40] to make the complicated shapes,
[14:42] then we can add a paint layer to our mask,
[14:45] and then we can start hand-painting stuff.
[14:47] In our case, I want to add more veins.
[14:50] You know, I want to add veins on the eyelids,
[14:52] and then on the nostril wings is a common place
[14:55] to find blood veins.
[14:58] And so I'm just choosing a brush
[15:00] and using my Sintiq, I'm using my pressure sensitivity
[15:03] to vary the line thickness, to vary the line pressure,
[15:07] and I'm trying to create these organic shapes.
[15:10] I'm doing it asymmetry also.
[15:12] And we can do this with all kinds of different effects
[15:15] by mixing hand-painted things with procedural things.
[15:19] We're going to get very unique, complex detail.
[15:23] Okay, once we have our bloody red layer done,
[15:27] we're going to add our next color,
[15:29] and in this case, it's going to be a purpler.
[15:31] So we're starting to introduce some color contrast now.
[15:34] I don't want to use the same colors
[15:36] or like a very few amount of colors.
[15:38] We want a little bit of a variety, even if it's subtle,
[15:40] so that it doesn't feel flat and it feels more alive.
[15:43] So we're going to go with purple. It's close to red.
[15:45] And one of the most common places to use this
[15:48] is kind of around the under eye,
[15:50] where the skin is thin and the blood is showing through.
[15:53] I'm also going to slightly put it around the mouth,
[15:55] like where hair follicles might be.
[15:57] And then we'll finally add our fill layer
[15:59] that's going to be our skin color.


### Adding Skin Color [16:01]
**Transcript (timestamped):**
[16:01] All right, so to make our skin color,
[16:03] we're going to create a new fill layer now to be our skin.
[16:06] And then we'll just choose a fleshy color.
[16:09] Again, we can always change this later on,
[16:11] or think this, just going to choose a fleshy kind of color.
[16:14] And then we're going to add a black mask.
[16:17] And then we're going to add a paint layer on this mask.
[16:20] So we're just going to do this all by hand to start with.
[16:23] We can always adjust it.
[16:25] So we're just going to first pick a brush that has some noise in it.
[16:28] And you can have fun with this.
[16:30] There's a bunch of different things you could do.
[16:32] Here I'm doing dirt three.
[16:34] And I'm just going to start painting and varying my pressure,
[16:36] varying my size.
[16:38] And the goal here, as with all of these layers,
[16:40] is we're just creating complexity that's subtle,
[16:44] different kinds of patterns, different kinds of sizes and opacity,
[16:47] so that when they mix together,
[16:49] they create an overall organic look.
[16:51] So you can just have fun with this and just start spraying around.
[16:55] I turned on symmetry in substance to save some time,
[16:58] because you're not going to notice the pattern.
[17:01] Might as well cut the time in half.
[17:03] And then I can turn off symmetry to spend some time
[17:05] so that there's no discernible patterns.
[17:08] Here I'm changing my brush to a different brush that has more noise.
[17:12] So there's not really like a right or wrong answer.
[17:14] I think variety is actually probably the most important thing.
[17:17] So go ahead and switch things up.
[17:19] But you can just spend time painting.
[17:22] And that's it.
[17:23] I'm just going to spend some time layering this up.
[17:25] And you'll see as you spend more and more time,
[17:27] it starts to become more and more like flesh.
[17:29] And we can always control the opacity of this paint layer.
[17:33] If we need to, you could also add a fill layer so that that can mix.
[17:36] That's just a solid value if you wanted to mix a little bit.
[17:39] So again, we really know right or wrong answer.
[17:41] We're just trying to do something other than a straight fill here
[17:44] so that it's irregular and it feels more organic
[17:48] when it's mixing with our layers below.
[17:50] Now with this setup and our skin painted nice and even,
[17:54] to add redness and warmth,
[17:56] we'll actually take away some of this skin color by painting black,
[18:00] like on the nose or in the eyes.
[18:02] You can also separate that with another paint layer in the mask
[18:05] to keep it clean and tidy.
[18:07] Speaking of organization, let's make a folder now called sub-dermis.
[18:10] We'll put everything that we made for below the surface in that folder.
[18:14] And then we're going to add another folder
[18:16] and we're going to call that dermis.
[18:18] So here we are in the dermis, right?
[18:20] The dermal layer, that would be the skin.
[18:22] It's like the top layer.
[18:24] Well, middle if you want to think of it that way
[18:26] because oil would be on top, makeup would be on top.
[18:30] So remember, we're going bottom to top here.
[18:32] We're organizing it like it would be in real life.
[18:35] So adding the folders, by the way,
[18:37] and adding more and more layers is going to make the scene heavier.
[18:40] It's going to make it more expensive.
[18:42] Things are going to be slower.
[18:43] So we might get to that point later on.
[18:45] Well, you'll see like I'll just end up turning off a lot of layers
[18:47] so that it's faster.
[18:49] But for right now, we want to add the sun damage,
[18:52] the imperfections that we can get the great reference from these RBX images.
[18:56] So let's see if we can start to make something like that.
[18:58] We're going to go really heavy hand in the beginning.
[19:00] It's kind of really dark burnt orange.
[19:04] All right.
[19:05] So now let's add some stuff.
[19:06] Why don't we first add some noise first?
[19:10] Doing nice, nice, gentle noise.
[19:15] How about this one?
[19:16] So we'll do another one.
[19:17] We do another technique here.
[19:19] So we got the noise, right?
[19:20] So now I'm going to add a fill and then we'll add,
[19:23] we could add clouds, we could use all kinds of stuff.
[19:25] And now I'm going to add this one.
[19:26] And now what I'm going to do with this is I'm going to set it to multiply.
[19:31] So what we've done now is remove some.
[19:34] So by having something and then removing and then adding,
[19:37] and then, you know, now we're creating complexity again
[19:40] by doing relatively simple things.
[19:42] So maybe clouds would be better actually for this one.
[19:45] Yeah, this would be better.
[19:47] Yeah.
[19:48] All right.
[19:49] So we got this.
[19:50] Now we're going to add smaller stuff.
[19:52] All right.
[19:53] I'm going to drag a new texture into our new fill layer.
[19:55] And I'm switching the projection mode to try planar projection.
[19:58] That just means it's not using the UVs.
[20:01] And this keeps patterns more uniform because it's not distorted by the UVs.
[20:05] I'll change this fill layer to screen mode too.
[20:07] So it starts to mix with everything below and we'll play with the size
[20:10] and adjust it there with the contrast to see it all mixed together.
[20:13] Now I really like the dirt three pattern.
[20:15] I felt like it was really organic and made for good like freckling and stuff.
[20:18] So I'm going to add another fill layer here.
[20:20] It's a little bit greedy, but we're going to try to go for four now.
[20:23] I'm going to set this to screen mode two.
[20:25] What I'm going to do with this one, the plan here is to just make it very large.
[20:29] So we're getting like splotches, like big old sunspots.
[20:33] You can always adjust like the rotation and offset and scale of these fill layers.
[20:37] So if you get like an awkward shape somewhere, you can always adjust it that way too.
[20:41] Now that I have all these layers, I have it to screen mode, I have the different blend modes.
[20:44] I can play with the opacity to kind of like adjust the mix.
[20:48] And then the ultimate control is I'll add a paint layer.
[20:51] Now you could just add a paint layer and straight up just paint, right?
[20:55] Like add and remove.
[20:57] But in this case, what I'm going to try to do is I'm going to try to just edit what we have so far.
[21:02] So I really only want to remove.
[21:04] So by changing our new paint layer to multiply, that means that it's only adding black.
[21:10] So as I paint and I switch from black and white, I'm just removing parts of the mass that I don't like,
[21:16] parts of the shapes or by painting white, I'm bringing it back.
[21:19] So it's not a straight painting.
[21:21] I'm really just editing the mass that we've built so far.
[21:23] And I can always add a paint layer on top of I want to do something custom,
[21:27] like if I want to add a spot or a mole like in an exact spot.
[21:30] So again, splitting all these things out for the mask gives you ultimate control and you can really go to town with this.
[21:36] But not trying to get too complicated.
[21:38] This is just some examples of what you can do to create complex masks.
[21:43] All right, now let's add a new fill layer freckles.
[21:46] We're going to make some freckles here.
[21:48] Not going to be applicable to every character in the world, although you could use them on a wide range of characters.


### Freckles [21:50]
**Transcript (timestamped):**
[21:53] Honestly, just make them very subtle.
[21:55] Ours though, we definitely wanted to feel like there's freckles on the upper nose, upper cheek region.
[22:00] Notice in some of our reference and I think it's a cool detail to add and show here in the video.
[22:05] So just making a new fill layer and then starting off with a paint layer on our mask and then just choosing a brush with dots.
[22:13] I just typed in dots.
[22:14] I'm using trusty old Kyle's brushes over here.
[22:17] Just so we don't have to make one of our own, but we can show that later on in the video.
[22:21] So just spraying down some dots.
[22:23] Easy peasy.
[22:24] So I can just put down some stuff if I want to erase it.
[22:27] Obviously, you know the drill now just by painting black and white.
[22:30] You're editing the mask here.
[22:31] I also try to play around with the dots brush, which is a different brush and varying my pen pressure.
[22:37] I can also play with opacity.
[22:38] So we're already getting something pretty complex, but everything is like perfect circles.
[22:42] And that's not what freckles look like.
[22:44] We're trying to be organic.
[22:46] So we're going to start using some more filters here to show you.
[22:49] So I'm using blur.
[22:51] Now is the first filter.
[22:53] That's going to help us get rid of those super sharp edges.
[22:57] Freckles are below the skin to a different depth.
[23:00] So that helps to make it feel like it is deep and we're just seeing them through the skin.
[23:04] And then another filter we're going to use is warp.
[23:07] Warp is one that you can use to break up patterns.
[23:10] You'll see once I choose it out of the gate, it's going to really like break it apart.
[23:15] But the key to using it to just subtly break up patterns that are perfect is to use the blur in the source parameters of the warp.
[23:23] This blurs the actual warp itself, so it's not so chattery.
[23:27] So by playing with intensity and the blur, you can just break it up as much as you want.
[23:32] So we're just avoiding perfect round circles and we're avoiding sharp edges.
[23:36] So it helps to make it organic and we're painting very subtle brushstrokes,
[23:40] but we're getting some more complicated results as it filters up.
[23:43] We can even paint as we have the filters on so we can add or remove, add more dots.
[23:48] Based on your machine, based on how many layers are in your scene, this could be slow if you have like a lot of layers and a lot of filters on something,
[23:55] but it is something cool that you can do to kind of see real-time feedback with real-time effects going on in your strokes.
[24:01] So this is the technique I use to achieve the freckles.
[24:04] Alright, now let's talk about another kind of detail that we can put in the base color map.


### Cavity Textures [24:05]
**Transcript (timestamped):**
[24:09] Actually, multiple maps, but it's a good channel to have in your textures and that's blackheads or clogged pores.
[24:15] Generally anything that uses cavities.
[24:18] So let's do that right now.
[24:20] We're going to create a new fill layer and we'll just name it blackheads in our case.
[24:24] And then we'll do the same drill.
[24:26] We'll make a black mask, then we'll create a generator this time, not just a fill layer, which create a generator.
[24:33] And then we'll go over to our generators and we'll choose curvature.
[24:36] This is how we can use our cavities.
[24:38] So in the curvature generator settings, you can see I can choose cavities as my input source.
[24:43] And you can even have it be unfiltered so it's straight up the cavity that we baked.
[24:47] So that's what's driving our mask now.
[24:49] Now what we want to do is only kind of bring out some blackheads, right?
[24:55] We just want to like with our brush paint here and there and some pores and have it fill.
[24:59] So we can do that similar to the techniques we did earlier.
[25:03] What we're going to do is we're going to fill a new paint layer with black, which will be on multiply.
[25:12] So that's going to take away everything because our generator is using the cavities as white.
[25:18] So by having everything black, you won't see anything at all.
[25:22] We'll also use the first time the fill tool and we can choose the selection type so we can just select the mesh.
[25:28] So in one click, we can fill the whole mesh, which is the whole mask in this case with black.
[25:34] And then now we can paint black and white on our paint channel.
[25:38] And by painting white, we can add some of the poor detail that we have from the curvature map.
[25:42] So that might sound convoluted.
[25:44] Hopefully you can follow along the steps in the visuals too.
[25:46] But I thought this is an interesting way to show the cavity generator to show the selection tool and the tricky ways that we can use blend layers to create the kinds of effects we want.
[25:57] So with the relatively simple brushstrokes now, we are bringing in complicated detail.
[26:02] And that's what you want.
[26:03] You always want to do simple input complex output.
[26:06] I didn't ultimately use a lot of the blackheads to be honest in mind.
[26:10] It's very subtle, but still I think useful techniques in here.
[26:13] Something too interesting that you should be aware of the benefit of doing things like this with fill layers is we could easily just turn on roughness in the channel of our fill layer.
[26:21] And then we could also end spec and we could also affect all those separate texture maps with the single mask that we made right now.
[26:29] And that's kind of the power of substance painter.
[26:32] So you get all that detail in all your channels.
[26:34] So even though it's subtle, it breaks up the light.
[26:36] And with very little work, you created something that feels organic and complex.
[26:41] All right, now that we have multiple elements that are making up our texture here, we have multiple fill layers and masks doing all kinds of things.
[26:49] Now to like iterate and work on the texture kind of bounce around.
[26:52] So if I want to add more redness to the nose, then I'm going to the skin color fill layer and I'm starting to remove some of it to reveal that sub dermal layer that we have below.
[27:02] If I want to increase the contrast in some of those shapes that is in the sub dermal layer, then I'll be bouncing down there and playing with the different fill colors there or increasing contrast and masks,
[27:15] adding, removing in masks, you know, just all kinds of stuff.
[27:19] If I want to remove blackheads, if I want to have the eyes be darker, all kinds of different things.
[27:26] That's why it's important to keep the scene relatively manageable and jump around.
[27:30] It's not very linear, you know, for the sake of the demo of the video, it might be focusing on topic to topic.
[27:35] But this is more typical of how I'll be working.
[27:38] You know, I really want to sketch out the scope of my scene as quickly as possible, like how many elements I need.
[27:43] And then the majority of the time, I'm going to be playing within those elements, like just balancing, changing aspects, changing parameters and values and colors and stuff like that.
[27:52] So this is really what most of the texturing looks like for me.
[27:55] All right, so texturing the lips.
[27:57] What I'm going to do is I'm going to create a new folder for the lips that I can put any new fill layers or anything I want inside the new lips folder.
[28:05] And we're just going to create a mask for the lips there so that we can play around inside the folder.
[28:10] So as with everything, I think what I'm going to do is I'm just going to block out the elements I think I need and then start playing with it based on my reference.
[28:18] So why don't we do that first by just creating a fill layer, call it base lips.
[28:23] I'm going to just mask the folder and then I can do whatever I want on the inside of it.
[28:28] So first start painting the mask.
[28:31] So I'm going to be heavy handed at first.
[28:33] But then the edge I need to feather off in some areas and some areas I'll be a little bit sharper.
[28:38] But I kind of just believe that like making even basic things by hand this way, like there's subtle variations.
[28:45] You know what I'm saying?
[28:46] By me using my own hand to make certain things that are layering and unlayering is just another variable.
[28:54] It just adds complexity using my dumb hand is actually useful here, which is part of the fun.
[29:00] I think of making organic things.
[29:02] It's like just going along for the ride and just like, you know, the mistakes and everything is all part of it.
[29:07] Okay, cool.
[29:08] So that is the lips mask for right now.
[29:11] Base lips color.
[29:12] And we also can do roughness and everything in here, which is cool, right?
[29:16] But for color lips, the good thing to do is try to check the value against your skin.
[29:22] Is it brighter?
[29:23] Is it darker?
[29:24] It's most likely darker.
[29:27] Saturation plays a role too.
[29:29] So we're going to leave this for now.
[29:31] So I want to see if I can get the edges of the lips.
[29:35] I'm just noticing there's some discoloration around the corner of the lips, edge of the lips.
[29:39] And I want to get anytime I can derive something from the model to add complexity.
[29:44] I like to do that.
[29:45] So how we're going to do that is we're going to create a new fill layer for the outer edge.
[29:49] And then we're going to create a mask.
[29:51] And then what we're going to do is we're going to search for a thickness map that we derived earlier and drag that into the mask channel.
[29:58] Then what we can do is right click and create a levels and then we can start to play with the contrast.
[30:04] So now we're using the model detail that we made to drive this.
[30:09] So we're getting a complicated shape right out of the gate that we can then edit with painting if we want.
[30:14] So here's the thickness map.
[30:15] So it has information in it and I'm using that to do the discoloring.
[30:21] So now I choose my darker value, which is less saturated too.
[30:25] So we're already getting like a two tonality.
[30:29] I mean now looking at the cross polarized stuff with lips.
[30:33] Another interesting thing we could do is add lightness to the pads of the lips.
[30:37] I think we could get even darker on the edges here actually.
[30:41] So now we got different color temperatures too.
[30:43] Again, subtle, but it's going to be doing something darkness.
[30:47] And then let's do lightness.
[30:50] Why don't we?
[30:51] And we'll do this for the pads again.
[30:54] We already have the details.
[30:55] So let's do that.
[30:56] We're going to do it again.
[30:58] Black mask fill.
[30:59] We'll do a generator and we'll do the curvature again.
[31:04] Boom.
[31:05] Already interesting.
[31:06] Unprocessed.
[31:07] Okay.
[31:08] Boom.
[31:09] So let's turn all this off.
[31:10] This can be confusing.
[31:11] Fine.
[31:12] Okay.
[31:13] There we go.
[31:14] Boom.
[31:15] Already interesting.
[31:16] Maybe we do this a little bit and then maybe the sharp ones too a little bit.
[31:20] Again, I can always paint this out, right?
[31:22] So can we do any fancy blending modes?
[31:25] What about lightness or lighten?
[31:27] Okay.
[31:28] Cool.
[31:29] Cool.
[31:30] And then we make it really subtle.
[31:34] Can even do a global contrast and a global blur, which is pretty cool.
[31:40] Add paint, multiply.
[31:42] And let's just get rid of some of this.
[31:44] So now just lightly remove it everywhere around the edges especially and just maybe leave
[31:48] it towards the center.
[31:50] Pretty subtle off and on.
[31:52] We've got detail in there.
[31:53] I think that's what matters.
[31:54] All right.
[31:55] So I'm going to try to darken and up the saturation of the lips.
[31:58] You can always rebalance the fill layers.
[32:00] That's what's good about it.
[32:01] And then what I'm going to do is on our new lightness layer, I'll add a new paint layer
[32:06] and then I'll start to lighten the bottom inner lip.
[32:08] I noticed it in some of my reference and I think it's a nice added bit of variety.
[32:13] All right.
[32:14] Now the lips are done.
[32:15] Let's do another final pass on our base color painting before we export this and take a look
[32:21] at it in a render.
[32:23] So a couple more things I want to do now to add a little bit more detail in the base color
[32:29] is I want to first paint around the orbital bone here that you can see around the eye.
[32:36] I want this to be more even and a little bit of a brighter yellow or tone.
[32:40] You can see this in some of the references.
[32:43] But this happens because of the different layers underneath.
[32:46] It's less blood here.
[32:47] It's more bone or muscle.
[32:49] And it's just a way to add more contrast in our base color that help it feel a little
[32:53] bit more natural.
[32:54] So we're doing it on the eyebrows here in a little bit over the edge of the...
[33:01] So we're doing it over the eyebrows here, kind of around the whole orbital bone in general.
[33:04] You might want to do it on the bottom of the chin as well or the skull.
[33:08] So it's just a way again to add some contrast here so that it's not an even texture throughout
[33:14] the entire head but that we're showing that there is difference, that there is different
[33:20] underlying tissue here and it helps to make it feel more believable.
[33:24] Also going to paint a little bit more detail around the eyelid itself.
[33:30] Could darken the upper eyelid but also have a little bit more sharp and strong along the
[33:36] edge of the eyelid as if it's discolored red or pink where the eyelids actually are ending
[33:42] where they're meeting up.
[33:43] And also on the inside where the tear duct is that would be a different color and material
[33:48] as well.
[33:49] I want to just account for that and again bring some more stronger contrast in these
[33:54] values and colors.
[33:55] So by doing all this by the way I'm really just adding and removing in the mask of the
[34:01] skin color fill layer and if I need to go farther, if I need something different, I
[34:05] can always add another fill layer to change the color or add some element that I don't
[34:10] have.
[34:11] But I'm trying to play with the elements that I do have as much as possible to keep the
[34:15] scene simple.
[34:16] So really trying to stretch the complexity with what I'm doing rather than adding more
[34:19] and more things.
[34:22] So continually jumping around between my elements of freckles and blackheads and sun damaged
[34:29] layers and just painting in my paint layers to continue refining the base color now before
[34:35] we take a look.
[34:36] So I've spent some time now, you know, I'm generally happy with how it's looking but
[34:41] really to get a sense of like what next steps to take.
[34:44] We need to export this and take a look at our renderer.
[34:46] So let's talk about exporting these textures now so we can take a look.


### Exporting Textures [34:51]
**Transcript (timestamped):**
[34:51] Okay, so to actually export the textures, we need to go to file, export textures or shift
[34:57] command E and bring up the export options.
[35:00] First thing we're going to do is select the output directory where the maps are going
[35:04] to go.
[35:05] So do this and keep it there.
[35:06] So put it in my case the project directory, then the output template.
[35:10] That's what we started with.
[35:11] So you can see in the list of exports.
[35:13] This is what it's going to export.
[35:15] So we can make changes by going to output templates and then we'll select the template
[35:19] we're using, which is PBR metal roughness.
[35:21] I'm just going to delete the mesh name.
[35:23] I don't need that.
[35:24] And you can see it's going to export everything.
[35:25] So I don't need all those things too.
[35:28] By going back to the settings and reselecting my output template, it'll apply the changes
[35:32] I made.
[35:34] Then we'll come over here to settings and we'll just uncheck everything except base color.
[35:38] You can see it's 4k, which is the texture set size right now in my project.
[35:41] So that's what we want.
[35:43] And now you can just hit save settings or export and we'll hit export.
[35:47] And now it's going to save out this map.
[35:49] You can see right here in green, that means it saved out the map.
[35:51] All right.


### Checking Renders [35:52]
**Transcript (timestamped):**
[35:52] So we spent some time making the base color so far.
[35:55] So now I'm just going to open up Marmoset to apply it to the model we made in the last
[36:00] video so we can see our texture so far with like a proper ray chase render just to take
[36:06] a look and see where we're at and then make a game plan going forward.
[36:09] So let's open up Marmoset tool bag now and we'll load it up and take a look.
[36:15] This is something that I'm doing all the time by the way when I'm texturing both professionally
[36:20] and for projects is I try to get the connection between the intended renderer and my texture
[36:28] scene or substance in this case.
[36:29] So the directory is pointing to the place.
[36:32] It's exporting the right textures in the right kind of format so that for the majority of
[36:37] the time afterwards I'm updating the textures and it just overwrites them and substance
[36:43] I can just keep exporting it.
[36:44] So when I'm doing projects and like I say for work and everything I'll be exporting
[36:48] you know a few dozen times a day.
[36:51] Something to keep in mind is something that you should probably be doing.
[36:54] So we're not going to like try to make a super nice pretty renderer for presentation.
[36:58] It's the only place where you can actually see your texture like what you're working
[37:01] on.
[37:02] So here we are in the scene now.
[37:04] So we'll go over to the head material and we will choose our texture that we made.
[37:10] So in this case it's going to be the Albedo.
[37:12] So I'm going to go here and I will select from the directory our image that we exported
[37:19] right here girl demo base color PNG that we just exported.
[37:23] And there we go.
[37:24] That's a little dark because I have this gray swatch because that's what I was using to
[37:27] render.
[37:28] So yeah we just need to make this white right here.
[37:31] And there you go.
[37:32] Now this is the correct value of our base color in here.
[37:36] Also because it was just a gray model before there was no color in the scatter depth scatter
[37:40] depth.
[37:41] This parameter is in all kinds of renders when you're doing subsurface which we're doing
[37:44] for skin right right now we're using volume scattering Marmosa there's a couple again
[37:49] we'll go into rendering later don't want to overdo this but let's give it some color
[37:53] basically give it a pretty good.
[37:56] It's kind of a peachy color for color bleed and skin because it's not just red that's
[38:01] bleeding but red is bleeding the farther so there you go now it looks a little bit more
[38:04] like skin and then let's take a look and form a game plan for texturing moving forward.
[38:10] This is just the quality of my viewport I'm going to render out a couple images so we
[38:14] can see with fine detail but already I can tell we're definitely going to need to author
[38:19] a quick spec map and glossiness map for it to feel more like skin right now the glossiness
[38:24] is getting in the way kind of but already I can tell I might want to redo the freckles
[38:30] not really feeling it doesn't feel that natural I like some of the small dark moles and also
[38:36] I want to add some more gradient like some more dark values in particular to like maybe
[38:42] the eyelids maybe underneath the cheekbone and maybe some lighter values around the face
[38:49] mask right now it's a pretty even skin tone I think we could have some general value break
[38:53] up we can see a little bit of that in some of our reference I think we could probably
[38:57] even bring some sharpness so let's take a look at a couple renders here is a render of the
[39:04] model with no texture and here it is with some color yeah like I say I kind of like
[39:10] these moles like a couple of these but the actual freckles I'm not feeling it they're
[39:14] actually very faint too I kind of like the shapes but maybe they're too numerous and
[39:18] close together blackheads aren't feeling that great either I think I might just want to
[39:23] keep a couple and that's it but yeah there's like an evenness so I think we could kind
[39:27] of vary it ears I'm pretty happy with simple but I'm down with that so that's what we're
[39:32] going to do we're going to make a quick spec map and we're going to make a quick glossiness
[39:36] map and then we're going to update our base color a little bit and then do a couple more
[39:40] renders and see where we're at so let's jump back over to substance right now and start
[39:45] making those changes alright back in substance let's update our base color so first thing


### Updating Textures [39:46]
**Transcript (timestamped):**
[39:50] I think I'm going to do is update the freckles I'm going to disable warp and blur here so
[39:55] I can just focus on the paint layer warp and blur actually moving things around and it
[40:00] could be a little slow to work with so just disabling is is the way to go then I'm going
[40:05] to wash out this and just kind of do a retake I might spend some time keeping some of the
[40:10] shapes I like but honestly I think because of the brush I used it was spraying the dots
[40:14] too close together I think that's kind of the main thing I want to fix is I want to
[40:19] have more opaque dots and I want to get rid of the ones that are so crowded together because
[40:24] I think it was just making it look dirty more than freckles I also felt like it was kind
[40:31] of flat the skin feeling in marmoset so I want to increase the contrast play around
[40:38] the patterns of my sub dermal layers there and also I think what I'm going to do is I'm
[40:42] going to bring the veins or at least one of the veiny layers up on top of my dermis layer
[40:48] that way I've got more control separated out and I can make sure that it's visible I can
[40:53] just mix that on its own.
[40:55] Alright so doing another pass of the freckles here with the Kyle's brush again because
[41:00] it sprays the dots so far apart so I'm trying to I'm adding on a separate paint layer now
[41:05] making it larger too so I can spread it out and try to get some of these opaque dots that
[41:10] aren't so close together.
[41:12] We can even make our own brush so if I just select the basic brush in spacing I can just
[41:18] max it out I can make sure that the pressure is related to size I can up the size jitter
[41:25] and the position jitter of this brush and just spray the circle that comes with it so
[41:32] it's a way for us to make our own kind of ghetto freckle brush you know you could duplicate
[41:36] this I guess and save it as your own but I mean it's pretty basic stuff but just showing
[41:40] like you can change brush parameters too to make like scatter type brushes and if you
[41:45] had a custom alpha you might want to use that to do something like veins or any kind
[41:49] of pattern but this lets us control how close the dots are together.
[41:53] Another thing that I think is going to help bring some more interest and contrast to this
[41:59] is to add a couple more values you know like again I was feeling flat so I'm going to add
[42:03] a fill layer just call it dark use a little bit of a different color temperature slightly
[42:09] and I'll be a darker value so we're doing a little bit more contrast that way and then
[42:13] I can just put a black mask on this and feather it in not just in value but also in color
[42:19] again subtle but this lets me add a little bit more depth to it to push it avoid that
[42:25] flat kind of dead feeling and try to bring a little bit more life to this so I'm going
[42:30] to add some of the darkness like beneath her cheekbones I'm also adding a blur filter on
[42:35] this dark thing because I want to be very feathery like very air brushy I'll darken
[42:40] the eyes as well because before I was just removing the skin color from the fill layer
[42:45] right which is revealing the redness from below but now with this more brown dark color
[42:52] I'm able to add darkness to the eyelids now that looks more like a discoloration along
[42:58] with dotting it in some other areas here like you see lips and nose and stuff just to bring
[43:02] more of an organic feel.
[43:05] I also noticed a little bit of strangeness in the lips like the seal between them so
[43:09] I'm just coming in here to double check in my base color mode and it is confirmed here
[43:12] that like it's not fully colored in there so I think the easiest way to solve this problem
[43:17] make sure that our lip mask is covering everything and there's no like leaking through is to
[43:23] jump over into the flat UV mode here and then switch my alignment mode to UV so that I know
[43:29] I'm just painting in this UV mode there's no 3D whatsoever and then I can just take
[43:34] a brush and make sure I'm filling all these UVs to like get that seal on the lips so we
[43:40] don't see any like bright values in between the lips when our mouth is closed this is
[43:44] just a good way to get into the nooks and crannies so switching over to that view is
[43:47] always really handy and you can do that by pressing F3.
[43:51] Alright so we've made our adjustments and our updates to our base color based on what
[43:55] we saw in our renders now we got to adjust the reflectivity we got to do the spec and
[43:59] the roughness map so let's talk about doing a specular map.


### Specular [44:03]
**Transcript (timestamped):**
[44:03] Okay so now let's author a spec map.
[44:06] Generally when you're making PBR assets though you don't need to make a spec map.
[44:10] Again this is going to layer up right because we've got the normal map detail that we did
[44:14] in the previous video while we're sculpting we've got base color detail of various levels
[44:20] of sharpness and shapes right.
[44:22] Those two things don't match up so they're mixing together and then we're going to have
[44:25] some more organic detail in the spec.
[44:28] What we're trying to do here is add this subtle complexity when we're looking at the final result.
[44:32] PBR metal rough template doesn't have a spec map.
[44:35] You really don't need a spec map most of the time for most 3D assets.
[44:40] You generally set it to like 0.45 or 0.4.
[44:44] Pretty much everything in the real world reflects light the same.
[44:47] We're kind of cheating a little bit because we're going to try to add complexity to the
[44:51] spec so we want to have a texture in there.
[44:53] We don't just want to have a solid value.
[44:56] To do that we need to change our template and our export settings because the PBR workflow
[45:02] template that we use to start our scene does not have a specular level channel.
[45:06] So we'll add that then we'll make a custom export preset so we can export that map.
[45:11] To do that though and painter since we don't have it we need to go to the texture set settings
[45:15] and then add a specular level.
[45:18] So now we have it you can see over here spec level.
[45:20] So I'll just isolate that and we can come over here in our specular level.
[45:24] So this is the specular level and right now it's set to 0.5 again like 0.4 probably a
[45:29] good place to start.
[45:31] To be able to export this new channel as a texture though we have to make sure it's in
[45:36] our export preset and to do that let's make our own.
[45:39] Let's duplicate this point.
[45:42] So now we have a copy.
[45:43] I'm going to change this.
[45:45] So we go PBR metal rough J H don't need that.
[45:50] I don't need a missive most of the time so I guess I'll just get rid of it and if I need
[45:55] it I'll add it back.
[45:56] Then we're going to create a gray map and we're going to do specular level from specular
[46:05] level.
[46:06] There we go and we'll just copy this spec.
[46:09] Boom.
[46:10] There.
[46:11] So now we have our output template.
[46:12] It's going to come in.
[46:14] You can see it matches the roughness and that is an 8 bit because it's just grayscale.
[46:18] That's all we need is grayscale.
[46:19] So we're good to go and then we need to choose it from here.
[46:22] There you go.
[46:23] So we're good.
[46:24] Save settings.
[46:25] Now that we have the channel and we can export it, it's pretty straightforward.
[46:28] We're just going to make a new fill layer with some noise as a mask and we can play
[46:33] around with the scale and the value to get some fine detail breakup.
[46:37] We can stack another fill layer on top of that with different noise, different shapes
[46:41] and with screen mode we can add them together and then we can create something that's a
[46:46] little bit more complex.
[46:48] For now just something generic and noise like this is going to get the job done.
[46:51] We just want to make the light a little uneven so that it will help feel organic.


### Nostrils [46:56]
**Transcript (timestamped):**
[46:56] For game characters I always paint out the nostrils with black on the inside if you can
[47:02] see in here.
[47:03] So I'll just show you what I would do.
[47:07] So I would just come in here with actual black and then full roughness and then spec
[47:13] level totally dark and then I would just come in here and I would paint the nostrils.
[47:20] So I do this when I'm making game characters because the shadow resolutions are not enough
[47:26] to make believable shadows in small things like this nostril.
[47:30] So I'm faking it.
[47:32] It's kind of hacky.
[47:35] If your renderer can do cavity maps it would be more accurate to author a cavity map because
[47:42] that gets to tell a renderer light doesn't go here.
[47:46] So a classic example would be a sewer grate if you're just doing it in a texture you'd
[47:50] want to black out the holes so nothing would ever show up.
[47:54] Without having a cavity map this is how you do it.
[47:57] So there you go.
[47:58] And then you could come down even more but you can see the difference.
[48:02] Just we're programmed to map faces and the nostrils being black is crucial to that.
[48:09] So I don't need this to be such with mine but I will just darken it a little bit.
[48:16] Something else we could do if we wanted to is a cavity.
[48:20] So we'll do that.
[48:21] We'll do black mask.
[48:23] We'll do generator.
[48:25] We'll get our curvature cavities.
[48:29] The sharp ones.
[48:31] Good.
[48:33] There you go.
[48:34] So now we're going to have a breakup like that.
[48:36] All right.
[48:37] So now pretty quickly we've got a really detailed spec map.
[48:40] So this should look nice.
[48:41] We can see what it looks like once we export it but now let's make our roughness.
[48:45] Okay so the roughness map we're going to make a new folder as we do and we're going to call


### Roughness [48:48]
**Transcript (timestamped):**
[48:50] it roughness.
[48:51] Everything can live in this folder.
[48:53] I like doing this not only to keep it organized but you can always just mask the folder so
[48:57] you're controlling one mask.
[48:59] With the roughness map really what we're simulating here is oiliness like the variety of glossiness
[49:05] that's on skin.
[49:07] Like the lips for instance which are wet or may have some lip gloss.
[49:11] So we're making something that controls how rough or how smooth something is.
[49:15] So the first thing we're going to do is create a base roughness.
[49:18] That's just a fill layer with a roughness.
[49:20] We can set that to 0.8 something like that.
[49:23] We can always change this stuff.
[49:25] Once we export it and we can dial it in roughness is something that kind of varies engine to
[49:29] engine but getting it started with a base is the first thing to do.
[49:33] And then the next thing is we're just going to create a fill layer that's meant to be
[49:36] the oiliness.
[49:37] The glossier parts of the face.
[49:40] And what I'm going to do to help myself visualize this rather than just paint straight rough
[49:44] right now is when I make my new fill layer I'm actually just going to use color so I
[49:49] can paint the oiliness right on the skin that just helps me in the way I'm thinking and
[49:52] visualizing it and then we can just switch this to roughness when we're done.
[49:56] So the basics of this is just the lips obviously going to be glossy especially the most glossy
[50:01] area probably is going to be where the lips touch together in my case because I wanted
[50:05] to feel like it's wet.
[50:07] And then I'm going to make the lips in general a little bit glossier so this is going to
[50:10] vary character to character.
[50:12] But that's what we're going to do for this.
[50:13] This T zone area it's called of the nose the nostril wing sometimes and a little bit of
[50:19] the upper nose like forehead.
[50:21] Once we have that maybe the eyes definitely if you can see more of the tear ducts too
[50:25] that would be very glossy and wet the eyes in general would be wet around where the eyelid
[50:29] meets the eye and then the ears sometimes people forget like the inside of the bowl
[50:34] of the ear be a little bit glossy.
[50:37] And those are kind of the basic parts I mean we can add to this forever but we're just
[50:42] going to get this going here and so we can adjust our values and maybe the size of these
[50:47] sections but getting a little bit glossier in the cheeks and the nose the lips really
[50:51] as long as there is a variety and a contrast in your roughness it's going to make it feel
[50:58] more believable and alive.
[51:00] It's the flatness that really kills it.
[51:02] So you can see here we're not being very detailed we're just painting down some splotchyness
[51:06] to try to convey something.
[51:08] Everyone's different every character is different and throughout the day throughout different
[51:11] environments can be different so it's kind of fun making a roughness map because it doesn't
[51:15] have to be very detailed you can make this really fast and it really makes a big impact
[51:20] on the look.
[51:21] Alright let's get these textures out of Substance Painter.


### Custom Export Presets [51:22]
**Transcript (timestamped):**
[51:24] Real quick what we have to do is make sure that we're exporting all the maps that we
[51:27] need so if we open up the export settings again we go to the list of exports you can
[51:32] see we've only been exporting base color so we just need to check roughness and spec
[51:36] too so we know it's coming out.
[51:38] Also double check the size of your textures if you change the texture size in the scene
[51:43] I made my scene 2k which dropped the resolution so I need to reselect 4k so I can be sure
[51:47] to export the high res maps.
[51:49] So once our maps are exported we'll move over to Marmoset and we'll hook them up so we can
[51:53] take another look.
[51:54] But before we do that let's take a look at this video's sponsor.


### Skillshare [51:58]
**Transcript (timestamped):**
[51:59] Hello from the future I have less hair here in this timeline and I've traveled back to
[52:07] you about Skillshare.
[52:10] So Skillshare if you don't know already is a website I've been a member of for several
[52:14] years where it's got tons of stuff like you can even type in 3D art if you wanted to and
[52:19] you can look at all kinds of stuff made for 3D.
[52:22] Game art learn to create 3D art for video games.
[52:25] Wow I just came across this actually I didn't know Gary V had one that was my head right
[52:29] there that was my expression when I found it that was my expression when I found this
[52:32] video.
[52:33] I didn't know that Gary V had a video on here about a course about social media strategy
[52:37] and stuff so kind of interesting I'll probably listen to this.
[52:41] There's a lot of really talented people that are tapped to make these originals which I
[52:44] really like.
[52:45] In the past I've mentioned like MKBHD for instance and like Final Cut Pro editing.
[52:49] I also noticed a video about making better YouTube thumbnails so maybe I'll step up my
[52:54] YouTube thumbnail game while I'm at it.
[52:57] But yeah anything that you're interested in really you could find some premium content
[53:00] here on Skillshare to learn from and go deeper in so if you haven't already check it out.
[53:06] The first thousand people to click the link down below in my description will get a free
[53:10] trial of Skillshare and see if you like it.
[53:14] So now back to the video let's see if those textures got any better.
[53:19] Okay so we exported the textures there they are now we're hot back over to Momma set.
[53:27] The base color is already going to refresh if it doesn't I guess you can just hit this
[53:31] refresh button but it should refresh and then we'll add a couple of our other maps right
[53:37] we have the roughness map.
[53:39] So let's load that and remember I can drop down but I can't go up.
[53:44] We also have a clear coat roughness which I think I'll point to the same one again we'll
[53:49] talk about this when we talk about rendering back map.
[53:52] Boom spec map.
[53:55] This one we can actually drop the intensity which is cool.
[53:57] So we're on draft quality let's just take a quick gander here.
[54:01] So I'm going to do a couple high res renders and we'll take a look and we can just compare
[54:05] the previous renders to where we're at.
[54:07] So we've done a couple more renders now let's take a look.
[54:12] This is what we had before and here's our update.
[54:16] So you can tell obviously a big difference in the specular and roughness and we've cleaned
[54:22] up the freckles.
[54:24] The veins in the eyelid I think right here are working that's kind of cool.
[54:29] Here's the new one here's the old one really the biggest difference is in our roughness
[54:34] feeling it is feeling a bit more like skin.
[54:37] Lips I'm pretty happy with freckles still don't feel that organic and we're also not
[54:42] even though we added it we're not getting a ton of contrast in the base color.
[54:47] So let's try to fix that.
[54:48] So I'm going to show you how you can create an adjustment layer in substance painter which


### Adjustment Layers [54:50]
**Transcript (timestamped):**
[54:54] you know we used to do all the time in Photoshop but people aren't too used to doing it in
[54:59] substance painter so why don't we hop back in the substance painter and we'll end with
[55:03] those little updates.
[55:05] Okay so here we are back in painter what we want to do is kind of just crunch up what
[55:10] we've already got.
[55:11] Let's go to the base color so yeah I think there's some kind of cool stuff in here but
[55:16] maybe we're losing a little bit.
[55:19] So we can do global tweaks so we'll just add a layer here and we'll call this color correction.
[55:27] So I did a paint layer right as opposed to a fill layer this is just an empty layer now
[55:33] and what I can do is I can add filters to this and I'll have to make it pass through
[55:38] and then it'll apply everything below it so you'll see what I mean.
[55:42] So why don't we just add a hue level saturation you're going to choose what it's filtering
[55:47] right now we're just going to do color and I'll choose hue saturation levels and so you
[55:53] can see I can change something about it if this is set to pass through but to do that
[55:58] I have to go back to base color because that's where we are there we go now we say pass through
[56:04] all right so we're in base color it's affecting base color right here right it's affecting
[56:08] color right here and I have it set to pass through and now everything below it is getting
[56:14] affected and you can see this because it's above it is not so let's reset these all right so what
[56:21] we can do with this is we can kind of play with the levels and everything and the saturation
[56:26] bring that up a little bit we can also do things like levels again base color and we can like crank
[56:36] it get a little bit more redness and stuff so we're doing global tweaks now even further I
[56:43] could add a filter and I could say base color sharpen right and now we're sharpening it again
[56:51] everything below it right so now without the color correction with the color correction so I can
[56:56] make global changes like that all right so that's adjustment layers now let's get into our final


### Final Updates [57:01]
**Transcript (timestamped):**
[57:02] round of updates on our texture so one of the things I noticed was not a lot of contrast or
[57:07] breakup so I want to add some breakup I like the cellular noise actually that I was using in the
[57:12] subdermal layer so I'm just gonna steal that fill layer and recycle it to make my new layer and
[57:17] then I'll just keep the cells so you can see here the tiny circles it's a very organic pattern it
[57:24] works well for skin and we can make it really tiny we zoom in here so we can see you see it it brings
[57:29] kind of a sharpness and resolution you know to everything too like a chatter you can see when
[57:33] we're really zoomed in here what it's doing breaking up something and the way it mixes with
[57:38] gradients you can see when I turn it off helps to unify everything too with an organic pattern
[57:43] for me too I just want to use a couple blackheads I think this blackheads layer in my scene just
[57:48] got out of control and it's like creating like kind of a noise really like I want the pores to
[57:54] blend away a little bit in the lighting I don't want to like clog every pore so I'm really just
[57:58] gonna wipe away all this stuff and I'm just gonna leave a couple little black dots here and there
[58:02] on the nose and on the chin and that's it so making it real real simple alright so another thing I
[58:08] wanted to do I mentioned the roughness just kind of making everything more rough because in Marmoset
[58:16] I can always lower roughness which would make it glossier right so what I'm gonna do is I'm just
[58:23] gonna do like we did with the base color layer I'm gonna do an adjustment layer here and I'm
[58:28] gonna add a levels to it and I'm gonna make everything brighter by making everything brighter
[58:34] closer to white I'm making it more rough right which is good I'm bringing up the value that's
[58:40] what I want to do I want to bring up the value of the roughness layer and then which is gonna
[58:44] make her feel less glossy which is good but then in Marmoset because of the way it works I can
[58:49] always drag that slider down and bring back some glossiness if I want so it brings me more control
[58:54] and right now I think it's just a little bit too glossy also want to spend some time on my freckles
[59:00] layer I kind of like some of it but I'd like there to be some more I even kind of miss some of the
[59:06] subtle stuff that was going on in our first pass here so I'm breaking up the edges so that it's not
[59:11] uniform you can see I turned off the warp and blur here too so I can just work on these individual
[59:16] dots I'm just gonna add dots here and there with different brushes we're just like a basic brush
[59:21] and add some like moles and freckles just more frequent I'm kind of like hand doing them now to
[59:28] fill in the gaps to make as many as I want always doing another pass too on that skin color fill
[59:33] layer filling in the gaps making it feel like it's a little bit more red on the nose and maybe
[59:39] the cheeks and forehead and tweaking the color correction so I've got all the elements I need
[59:44] now really you can iterate forever and you should but for the sake of this demonstration I think
[59:50] we're in pretty good shape to export what we have now and take another look in Marmoset and now
[59:55] back over Marmoset these will update and then we get a look at our new textures let's render out
[60:02] some high res images again so we can compare A and B and see where we ended up with our textures
[60:06] and we can see where our skin textures ended up here we go this is the before and here's the
[60:14] after so you see we like generally darkened her I really think removing the blackhead layer is good
[60:23] I mean I think just in a couple spots like right here you see I mean like it's interesting I think
[60:27] by removing the darkness from the pores making a little bit more rough this feels more like skin
[60:31] to me if we go back and forth you know it's a little bit reflective before a little bit too
[60:36] much contrast in the details so I think it's softening up nice I think the freckles look a
[60:40] little bit more believable I like the vein detail in the color differences on the eyelids you can
[60:46] see our evolution from when we started without a spec or roughness map really shiny and then here
[60:53] we are making some improvements and then here we are now so a little bit more subtle darker
[60:57] skin tone I feel like this feels more natural so we do another update and now we've added a lot
[61:03] more just hand placed dots and moles and things taking care to actually just put it and like


### Outro [61:04]
**Transcript (timestamped):**
[61:09] just make sure that it's not too noisy and stuff so this is obviously really close up under scrutiny
[61:13] with the lighting and things but I think like having the extra vaniness in the cheeks things
[61:19] like that is helping to make it feel more naturalistic so I took it a step further and I worked on
[61:25] it for a few more minutes and I actually had some of these moles come out in the height you can see
[61:31] here so it's actually like coming out of the height and the light is catching it so I exported the
[61:35] normal map now mixed with this height it combines it so even though the normal map came from z brush
[61:41] we add the height channels in substance and I can export that even at ak and so we get the merged
[61:47] new height that I've painted with the normal map that I baked so this is where we ended up with the
[61:51] final textures of our skin you can see it here in the various different angles under this kind of
[61:56] neutral lighting scenario I'm generally happy where we ended up and that's where I'll end for now
[62:03] for texturing you could go on forever I really believe the more time you spend texturing like
[62:10] the better it gets there's definitely a point of diminishing returns as it as there is with everything
[62:15] but with texturing I think uh not as much as other things honestly because you know imagine if it's
[62:21] a full costume just adding little bits of detail little bits of wear and tear little bits of different
[62:27] subtle contrast in these different ways and value color material definition you know just
[62:33] bringing more and more life to it as much as you can I think that's what creates such a rich
[62:38] first impression when someone's looking at your work for the first time all that extra time that
[62:43] you've spent making all these little decisions you know just kind of hits someone at once so
[62:48] because there's so much subtle complexity it makes something feel a lot more interesting or
[62:54] believable or tactile and rich so I you know obviously enjoy texturing I think spending a
[63:00] lot of time with it is important in making your work stand out and my main tip is to stay organized
[63:09] work as non-destructively as possible and iterate hook it up as soon as you can to whatever
[63:14] render you're doing and make that choice early on stick to it and then just set up the paths
[63:19] and then just be iterating just export export export and that's where you're going to spend the most
[63:24] time that's it I could talk forever about texturing so I'm going to stop right there
[63:28] thank you very much for watching the video I hope you learned something I hope you got something
[63:33] that you could add to your own texturing game on your own projects if you do please let me know
[63:38] and tag me I'd love to see that sort of thing thank you so much for making it this far in the video
[63:42] I appreciate that the full version of this video is going to be up on my patreon I'm just going to
[63:47] try putting up unedited real time I'm even here talking a little bit we're recording it right now
[63:53] what's up patrons thank you for your support so we'll see how that goes I can't do that with
[63:57] everything but this is going to be a real-time demo I'm also putting together some goodies for
[64:01] the patrons this month a little pack of like head assets like this female base mesh I used for this
[64:07] demo actually I'm also going to include like some other files like the teeth and some textures like
[64:12] the normal map that I used and a displacement map which we'll talk about in an upcoming video
[64:17] but just some assets you guys can use to make your own heads and stuff also made this little
[64:21] cheeky like ear brush a while ago that you guys can have so like so when you make like head
[64:25] studies and sketches you know you don't have to like make an ear every time you know I'm saying so
[64:30] just some of the stuff this first kind of downloadable pack that I'm putting up there on the patreon
[64:34] lots more goodies coming up with the patreon if you're interested please consider checking it out
[64:38] and yeah that's it this is how I texture skin and substance painter thank you for watching
[64:44] I'll see you in the next video peace out



---

## Captured Frames

- [1:42] tutorials/frames/how-to-make-skin-textures-in-substance-painter/frame_000.jpg
- [8:37] tutorials/frames/how-to-make-skin-textures-in-substance-painter/frame_001.jpg
- [13:50] tutorials/frames/how-to-make-skin-textures-in-substance-painter/frame_002.jpg
- [16:34] tutorials/frames/how-to-make-skin-textures-in-substance-painter/frame_003.jpg
- [23:07] tutorials/frames/how-to-make-skin-textures-in-substance-painter/frame_004.jpg
- [24:47] tutorials/frames/how-to-make-skin-textures-in-substance-painter/frame_005.jpg
- [29:53] tutorials/frames/how-to-make-skin-textures-in-substance-painter/frame_006.jpg
- [39:04] tutorials/frames/how-to-make-skin-textures-in-substance-painter/frame_007.jpg
- [45:18] tutorials/frames/how-to-make-skin-textures-in-substance-painter/frame_008.jpg
- [47:13] tutorials/frames/how-to-make-skin-textures-in-substance-painter/frame_009.jpg
- [50:01] tutorials/frames/how-to-make-skin-textures-in-substance-painter/frame_010.jpg
- [55:53] tutorials/frames/how-to-make-skin-textures-in-substance-painter/frame_011.jpg
- [60:07] tutorials/frames/how-to-make-skin-textures-in-substance-painter/frame_012.jpg
- [61:31] tutorials/frames/how-to-make-skin-textures-in-substance-painter/frame_013.jpg

---

## Structured Notes

### Core Technique
A fully hand-authored, reference-driven PBR skin texturing workflow (BaseColor built from layered procedural-noise masks + freehand painting simulating sub-dermal blood/tissue layers, plus custom Specular Level and Roughness channels for oiliness variation) validated through a tight iterate-export-render loop against Marmoset Toolbag rather than judged inside Painter's own viewport.

### Summary
Companion/sequel to J Hill's earlier skin-sculpting video — starts from an already-sculpted ZBrush head (HD geometry, 8K normal map exported directly, no high-to-low bake needed) and focuses purely on the BaseColor/Specular/Roughness maps. Two reference categories anchor the whole approach: **RBX (cross-spectrum) imaging**, which visually separates sub-surface blood/pigment detail from surface detail into distinct "channels" the artist can see with the naked eye, and **cross-polarized photography** (e.g. Texture XYZ packs), which shows a real BaseColor with reflections removed. The core method is literally "airbrushing layers of skin" bottom-to-top inside Painter's layer stack, organized into a `Sub-Dermis` folder (blood/vein/warmth layers) and a `Dermis` folder (visible skin color, freckles, blackheads) — exactly mirroring real skin anatomy. Nearly every mask is built by layering 2-3 different-scale procedural noises together with varied blend modes (Screen to add, Multiply to subtract) before ever touching a brush, and a paint layer is then added *on top* to hand-edit/refine the procedural result rather than painting from scratch — the recurring principle stated outright is "simple input, complex output." The video ends with the same lesson repeated three times: export to Marmoset Toolbag, render, look critically, go back and adjust — the workflow assumes the artist cannot correctly judge skin color/roughness while looking only at Painter's own viewport.

### Key Steps

**1. Reference (0:00–5:02)**
1. Two reference categories called out as specifically valuable for BaseColor authoring: **RBX imaging** (a cross-spectrum photography technique tipped off by character artist Magdalena/Intervain) visually separates sub-dermal blood/pigment detail from surface detail into distinct color "channels" you can literally see side-by-side (frame_000 — reference board comparing a plain photo, an RBX-red/pink sub-surface pass, and an RBX-brown pigment/freckle pass of the same face); **cross-polarized photography** (e.g. Texture XYZ packs) removes reflected light, giving a "real" spec-free BaseColor reference.
2. Explicit rationale for hand-painting skin in Painter instead of photogrammetry/Mari-style texture projection: full creative control, a curated/stylized (not 1:1 photographic) result, and — as a training exercise — it builds the organic-painting skill needed for creatures/aliens that have no photo reference at all.

**2. Scene & map setup (5:02–10:27)**
3. New project: `PBR Metal Rough` starter template, mesh = the ZBrush export (HD subdivision level, FBX), texture set resolution 4K. **Normal Map Format must be set to OpenGL vs. DirectX at project creation** — described as commonly flipped/wrong depending on the DCC's export settings (green channel up-vs-down); easy to fix later if missed.
4. Import the externally-baked 8K ZBrush normal map as a project resource (Add Resources → Texture → "This Project" scope), drag onto the Normal channel slot.
5. **Because there's no high-to-low bake in this workflow** (the normal map came straight from ZBrush), auxiliary mesh maps (Curvature, Ambient Occlusion) are instead **derived from the already-imported normal map** rather than from mesh geometry: in the Curvature baker's settings, switch **Method from "Generate from Mesh" to "Generate from Normal Map"**, Details ≈0.5, uncheck "Normal" as an input since it's what's driving the bake (frame_001 — Baking dialog: Method dropdown, Secondary Rays 32, Sampling Radius 0.001, Relative to Bounding Box, Self Intersection: Always, Auto Tonemapping; Mesh Maps checklist showing Normal/World Space Normal/ID/Ambient Occlusion/Curvature/Position/Thickness). Ambient Occlusion likewise generates from the normal map. A Thickness map is also baked and called out as specifically useful for skin work later. Bakes done at 4K.

**3. Base Color — Sub-Dermis (10:27–16:01)**
6. Delete the default layer. New `Base Color` fill layer, warm/bloody base color (Alt-click the color swatch to pick a raw color), a touch of Roughness set on the base too.
7. Organizing principle stated explicitly: layer skin **bottom-to-top mirroring real anatomy** — deepest/bloodiest layers first, then dermis/visible-skin-color layers, then surface detail — and jump between finished layers constantly rather than working linearly.
8. Complex sub-dermal color-variation mask built from **layered noise, not a single texture**: first fill layer's mask gets a big/blobby noise (from the built-in noise library) for large interesting shapes; a second fill layer with smaller/finer noise is added and its **blend mode set to Screen** so it lightens/adds onto the first, building visual complexity from two simple inputs (frame_002 — Fill layer Properties on a grayscale "Cell 1" noise generator, layer stack showing a "Redness" folder with "Cells 1" / "small shapes 2" / "big Perlin noise 2" sub-layers).
9. On top of the procedural noise mask, **add a Paint layer and hand-paint** targeted detail the noise can't produce — specifically veins on eyelids and around the nostril wings, using pen-pressure-varied stroke width and deliberately asymmetric placement for organic believability (frame_003 — Paint brush active over an all-red sub-dermal preview, mirrored brush cursor dots visible near the cheek).
10. A second, purpler fill layer is added the same way (noise mask + hand-painted veins) for under-eye/mouth-corner discoloration, introducing color *variety* (not just value variety) as a deliberate anti-flatness measure.
11. Folder organization introduced at this point: `Sub-Dermis` folder holds everything below the visible skin; a separate `Dermis` folder (added next) holds the visible skin-color layer and everything above it — folders are noted as making the scene heavier/slower, with the tradeoff accepted for organization.

**4. Adding Skin Color (16:01–21:50)**
12. New `Skin Color` fill layer, fleshy base color, black mask, **Paint layer added on the mask and hand-painted entirely from scratch** using a noisy/textured brush (author uses a "Dirt 3" brush specifically), varying size/pressure while spraying — the stated goal is subtle overlapping complexity from *variety*, not precision. **Symmetry toggled on for the first painting pass to halve the work, then off for a second pass** so the mirrored pattern isn't visually obvious.
13. To reveal warmth/redness from the sub-dermal layers below, **paint black directly into the Skin Color mask** (removing skin-color coverage) rather than adding a new red layer — e.g. on the nose and around the eyes — optionally split into a second paint layer within the same mask to keep edits organized/reversible.

**5. Sun Damage / Discoloration (part of Dermis, ~18:49–21:50)**
14. New fill layer, dark burnt-orange, built the same layered-noise way: first noise fill (gentle/nice), a second fill using **Clouds** set to **Multiply** to remove/break up the first pattern, then a third, smaller-scale fill set to **Triplanar projection** (keeps the pattern uniform, ignoring UV distortion) at **Screen** blend to reintroduce fine detail, then a fourth even-larger-scale fill (also Screen) for big "sunspot" blotches — rotation/offset/scale on any of these fill layers can be nudged if a shape lands awkwardly.
15. Final control layer on this mask: a **Paint layer set to Multiply**, used exclusively to *subtract* — painting black removes unwanted procedural shapes, painting white restores them — described as "editing the mask we've built, not painting from scratch." A separate paint layer on top is used for fully custom additions (e.g. one exact mole/spot placed by hand).

**6. Freckles (21:50–24:05)**
16. New fill layer, paint layer on its mask, a dots-shaped brush (Kyle's brushes referenced) sprayed on with varied pressure/opacity for organic scatter — described honestly as looking too much like "perfect circles" at this stage.
17. Two filters fix the "too perfect" look: **`Blur`** first (softens hard edges, sells the idea that freckles sit at a different depth beneath the skin), then **`Warp`** (breaks up the now-uniform dot pattern) — the key tuning tip: **use the Blur parameter inside the Warp filter's own Source settings**, not just Warp's Intensity, so the warp distortion itself isn't jittery/chattery (frame_004 — Filter panel with a filter-picker popup open over a heavily-freckled nose close-up, small icon grid including Blur/Warp-type filters).
18. Filters stay live while painting, so additional dots can be added/removed with the warp/blur already applied and visible in real time (author notes this can get slow on heavier scenes/more filters).

**7. Cavity Textures / Blackheads (24:05–26:49)**
19. New `Blackheads` fill layer, black mask, then (first time in the video) a **Generator instead of a fill** is added to the mask: **Curvature** generator set to use **Cavities** as its input mode, unfiltered/unprocessed straight off the baked cavity data (frame_005 — Curvature generator Parameters panel: Global Blur/Balance False/0, Curvature Invert/Mode=Cavities, Sharp/Fine/Medium/Big/Vague/Coverage/Brightness sliders, Use Texture False, Image Inputs = Curvature/World Space Normals/World Space Normals(2)/Position Gradient; layer stack shows a "Cavities" folder containing "Blackheads").
20. **Trick to selectively reveal only some of the generator's output**: fill the whole mask black first (Paint layer, blend mode Multiply, then use the **Fill tool with Selection Type = Mesh** to flood-fill the entire mask black in one click) — this hides the cavity-generator output everywhere. Then hand-paint white in that same paint layer only where blackheads/visible pores should appear, letting the underlying curvature-cavity detail show through exactly there. Framed as "simple input, complex output": one brushstroke reveals a procedurally-complex pore pattern rather than hand-drawing pore shapes.
21. Called out explicitly: because this is a **fill layer with a mask** (not a flat paint), the same mask can simultaneously drive Roughness and Specular/Spec-level channels too, breaking up light in all of them from one authored mask — "that's the power of Substance Painter."
22. Working philosophy stated here generally: keep bouncing between already-built elements (redness, sub-dermal shapes, blackheads, eye darkness) rather than working strictly linearly, to keep the whole scene's element count small and manageable.

**8. Lips (26:49–34:51)**
23. New `Lips` folder with its own mask, hand-painted heavy-handed in the middle and feathered at the edges — the imprecision of hand-painting even a "basic" shape is treated as a feature (adds organic variation) not a flaw.
24. `Base Lips` fill layer inside — check the lip color's Value and Saturation *against* the skin (usually darker, more saturated).
25. **Thickness-map-driven edge discoloration**: new fill layer, mask = the previously-baked **Thickness map** dragged directly onto the mask channel, then a **`Levels`** node to push contrast — the model's own geometric thin-ness data (thin skin around the lip edge reads differently in the thickness bake) becomes a ready-made complex mask shape with zero painting, which can then be hand-edited on top if desired.
26. A second pass repeats the same idea with the **Curvature** generator (Unprocessed mode explored, then switched to more filtered settings) blended with **Lighten**, global contrast/blur tuned, then hand-erased with a Multiply paint layer in specific areas (mostly kept centered, removed from edges) to lighten the lip pads specifically.
27. Finish: darken and boost saturation on the base lips layer overall via rebalancing the fill's own color/value, then a final paint layer lightens just the inner lower lip based on reference.

**9. Base Color final pass (34:51 area, folded into Lips section)**
28. Extra hand-painted contrast added directly into the Skin Color mask: brighter/yellower tone around the **orbital bone** (less blood, more bone/muscle showing through) extending along the eyebrows and optionally the chin/skull; more saturated red/pink right at the eyelid margin where the lids meet, plus a distinct color at the tear duct — all framed as breaking up an otherwise-too-even base color to read as different underlying tissue types.

**10. Exporting Textures (34:51–35:52) & Checking Renders (35:52–39:46)**
29. `Ctrl/Cmd+Shift+E` → Export Textures. Confirm output directory, select/edit the output template (`PBR Metal Roughness` here — mesh-name token removed from the naming convention), then in Settings uncheck every map except BaseColor for this first pass, confirm the resolution matches the project's texture-set size (4K), Export.
30. **Render-driven iteration loop (repeated 3 times across the video) is the video's central working method**: load the exported PNG into **Marmoset Toolbag** as the head material's Albedo, set the environment/base color swatch to white (a gray swatch was darkening the preview), dial in **Scatter Depth** (subsurface-scattering color-bleed parameter — set to a peachy tone since skin bleeds more than pure red) for a first "does this even read as skin" check (frame_012 — Marmoset Toolbag UI, material channel slots visible: Normal Map, Detail Normal Map, Albedo Map, Scatter Map). Explicit stated habit: **always keep the export directory pointed at the same location as the render engine's texture folder** so re-exporting from Painter just overwrites in place — "exporting a few dozen times a day" on real projects.
31. First-pass render critique (verbatim decisions, useful as a worked example of self-critique): freckles too dense/not organic, keep the moles, blackheads too strong/should be sparser, overall skin reads too shiny/even because there's no Specular or Roughness map yet.

**11. Specular (44:03–46:56)**
32. PBR Metal/Rough templates don't ship a Specular Level channel and most assets don't need one (real-world materials mostly reflect similarly, ~0.4–0.45 default) — but a textured spec map is used here deliberately to add extra organic complexity that doesn't line up 1:1 with the BaseColor or normal-map detail (layering mismatched detail scales/sources is called out as a way to avoid a "flat" combined look).
33. **Add the channel**: Texture Set Settings → add **Specular Level** channel (default 0.5, dialed toward ~0.4) (frame_008 — Texture Set Settings General Properties/Channels list: BaseColor/Height/Roughness/Metallic/Normal already present, About to add Specular Level).
34. **Make a custom export preset so the new channel actually exports**: duplicate the closest stock template, rename (e.g. "PBR Metal Rough JH"), remove unneeded outputs (Emissive), add a new grayscale (8-bit) output map sourced from the Specular Level channel, select this new preset as the active output template, Save Settings.
35. Author the spec detail itself the same layered-noise way as everything else: one noise fill for fine breakup, a second noise fill on Screen to add complexity — "just something generic and noise-like" is enough to make the spec feel organically uneven rather than flat.

**12. Nostrils (46:56–48:48)**
36. Game-character-specific practical hack, explicitly framed as *not* physically accurate: **paint the interior of the nostrils fully black across BaseColor, Roughness (full), and Specular Level (fully dark)** by hand, because real-time shadow map resolution usually can't resolve believable self-shadowing in a cavity that small — "we're programmed to map faces and the nostrils being black is crucial to that" (frame_009 — a near-black, low-exposure viewport preview mid-edit). Notes the *correct*, non-hacky alternative where the target renderer supports it: **author a real cavity/AO map so the renderer itself knows not to light that area** (the sewer-grate analogy: black out the holes so nothing can ever show through). A cavities-mode Curvature generator (Sharp) is also layered in on the same mask for extra breakup.

**13. Roughness (48:48–51:22)**
37. New `Roughness` folder (folder-level mask again, for the same one-mask-many-uses reason as before). `Base Roughness` fill ≈0.8 as a starting point (roughness numbers are engine-dependent — expect to dial in per-renderer).
38. **Visualization trick**: build the oiliness/gloss variation mask *in a Color fill layer first* (easier to see/reason about than raw grayscale roughness values), hand-paint the glossy zones — lips (especially where they touch/seal, read as "wet"), the T-zone (nose bridge/nostril wings/forehead), eyes (tear ducts, eyelid margins), and the inner bowl of the ear (frame_010 — Paint brush stroke visible at the lip corner on a skin-toned preview, layer stack showing "Base color"/"Roughness"/"Spec"/"Paint" entries) — then **switch the fill layer's channel target from Color to Roughness** once the shapes read correctly. Explicitly low-precision/fast work — "it doesn't have to be very detailed... it really makes a big impact on the look."

**14. Custom Export Presets / second render pass (51:22–54:50, Skillshare sponsor segment skipped)**
39. Re-open Export Textures, check Roughness and Specular in the list of exports (previously only BaseColor was checked), re-confirm texture-set resolution wasn't accidentally left at a lower size from earlier testing (author had dropped to 2K to test, had to reselect 4K). Re-export, reload in Marmoset (load Roughness map, point Clear Coat Roughness at the same map for now, load the Specular map with its intensity slider droppable). Second render comparison: spec+roughness make the single biggest visible improvement toward "reads as skin"; freckles/blackheads still read as too dense/noisy.

**15. Adjustment Layers (54:50–57:01)**
40. Introduces Photoshop-style non-destructive global color grading inside Painter, explicitly noting most Painter users don't realize this is possible: add a **plain (empty) Paint layer** (not a fill layer) named e.g. "Color Correction" at the top of BaseColor, set its blend mode to **Pass Through** (critical — without Pass Through it doesn't composite the layers below, it just sits inert), then **add filters directly to this empty layer**: **Hue/Saturation/Levels** (raise saturation, push levels for more redness) and **Sharpen**, each affecting everything below simultaneously (frame_011 — Filter panel on an "HSL Parametric" filter: Mode=Parametric, Hue/Saturation/Lightness sliders; layer stack shows "Roughness"/"Skin"/"HSL Parametric"/"Sub Dermis" entries). This single global-adjustment layer becomes the fast dial for "crunch up" late-stage color/contrast tweaks without hunting through individual material layers.

**16. Final Updates (57:01–61:04)**
41. Reused/recycled an existing cellular-noise fill layer (originally built for the sub-dermal layer) at a much smaller scale as a final unifying micro-detail/chatter pass across the whole face — noted as visually "unifying" disparate gradients when zoomed in, barely visible zoomed out.
42. Blackheads layer judged as having gotten out of hand — most of it removed, leaving just a couple of hand-placed dots (nose, chin) rather than a dense procedural field.
43. Roughness raised globally via a second **adjustment-layer Levels** node (pushing values brighter/toward white = rougher) specifically because it's *easier to add glossiness back in the renderer* (Marmoset's roughness slider can be dragged down) than to fix an over-glossy bake — bias the authored map rough, fine-tune per-engine at render time.
44. Freckles redone again: original warp/blur filters temporarily disabled to work on raw dot placement without lag, a second brush pass used specifically because the previous brush's dot spacing read as "dirty" rather than freckled; **custom scatter-brush trick**: select the basic round brush, max out Spacing, link Pressure to Size, raise Size Jitter and Position Jitter — turns a plain round alpha into an ad-hoc scatter/freckle brush without needing a custom alpha (could be duplicated/saved as a reusable brush preset; a real custom alpha would be the next step up, e.g. for vein-shaped scatter).
45. Lip-seam bug fix demonstrating a general debugging technique: noticed a color leak where the lips meet — switched to the **flat UV view (F3)** with brush **Alignment set to UV** (paints purely in 2D UV space, no 3D distortion) specifically to guarantee full, gap-free mask coverage in tight geometry seams like the closed lip line.
46. Final base-color pass adds more nose/cheek/forehead redness by hand and further tunes the color-correction adjustment layer; third and final render comparison in Marmoset shows the cumulative before/after (frame_013 — high-resolution final render, raised mole/freckle detail visibly catching specular highlight on the cheek).
47. **Height-driven raised detail (mentioned in Outro, not shown step-by-step)**: some moles were additionally given actual raised **Height** channel detail (not just BaseColor), which Painter merges with the imported ZBrush normal map on export — "even though the normal map came from ZBrush, we add the height channels in Substance" — exported together at 4K so the final normal map reflects both the sculpted detail and the newly hand-painted height bumps.

### Layers / Tools / Settings
**Folders (bottom to top):** `Sub-Dermis` (blood/vein/warmth noise+paint layers) → `Dermis` (containing `Skin Color`, sun-damage, `Freckles`, `Blackheads`/Cavities, `Lips` folder) → `Roughness` folder → top-level `Color Correction` / roughness adjustment paint layers.
**Recurring mask-building pattern:** 2-3 fill layers of different-scale procedural noise, mixed via **Screen** (add) and **Multiply** (subtract) blend modes, topped with a **Paint layer** used either to hand-add unique detail or (set to Multiply) to *edit/subtract* from the procedural result rather than paint from scratch — the video's single most-repeated technique, applied to sub-dermal color, sun damage, freckles, and spec/roughness alike.
**Generators used:** `Curvature` — Cavities mode (unprocessed/unfiltered, driven by the Curvature mesh map baked from the imported normal map) for blackheads/pores; also explored Unprocessed and filtered Sharp/Fine settings on the lips.
**Baking (no high-to-low bake in this project):** Curvature baker Method = **Generate from Normal Map** (not Generate from Mesh) since the normal map was authored externally in ZBrush; Ambient Occlusion likewise generated from the normal map; Thickness map also baked and used later to drive the lip-edge discoloration mask.
**Selection/fill tools:** Fill tool with **Selection Type = Mesh** to flood an entire mask black in one click (used as the reset step before hand-revealing blackhead pores).
**Filters:** `Blur` (softens freckle-dot edges to sell sub-surface depth), `Warp` (breaks up repetitive dot/noise patterns — tune via the Warp's own **Source Blur**, not just Intensity, to avoid a jittery result), `Levels` (contrast push on thickness-map and curvature-driven masks, and on the final roughness adjustment layer), `HSL`/Hue-Saturation-Levels + `Sharpen` (global color-correction adjustment layer).
**Adjustment-layer pattern:** empty **Paint layer** (not Fill), blend mode **Pass Through**, filters added directly to the empty layer so they affect everything beneath it as a single global control point — used for both a BaseColor "Color Correction" layer and a separate Roughness-boosting Levels layer.
**Channels:** Texture Set Settings used to add a **Specular Level** channel (not present in the default PBR Metal Rough template) — requires also building a custom **export preset** (duplicate the stock template, remove unneeded channels like Emissive, add a new 8-bit grayscale output sourced from Specular Level) before the channel will actually export.
**Brush tricks:** custom "ghetto freckle" scatter brush built from the stock round brush by maxing Spacing, linking Pressure→Size, and raising Size/Position Jitter; **flat UV view (F3) + brush Alignment = UV** for guaranteed full-coverage painting in tight seams (e.g. the closed lip line) without 3D-projection distortion.
**Export:** `Ctrl/Cmd+Shift+E`; custom `PBR Metal Rough JH` output template; iterative small-checklist exports (BaseColor only, then + Roughness + Specular) rather than one final export; always re-verify texture-set resolution before exporting after testing at a lower size.
**External render-check loop:** Marmoset Toolbag used as the actual judgment tool throughout — Albedo/Roughness/Specular/Normal map slots, Scatter Depth (subsurface color-bleed) parameter tuned for a believable skin-tone read, environment/base-color swatch reset to white so it doesn't tint the imported texture.

### Difficulty
Intermediate. The individual techniques (fill layers, masks, generators, blend-mode stacking, adjustment layers) are each explained from a fairly accessible starting point, but successfully executing the video's actual craft — organic hand-painting judgment, reading/critiquing your own renders, building believable anatomical color variation — takes real practice; this is as much an art-direction/observation lesson as a button-by-button tutorial.

### App & Version
Not stated on screen or in narration, and unlike the companion "TEXTURE EVERYTHING" video, no filter/tool here pins a version lower bound directly. However, frame_001 (the baking step) shows a small **floating modal dialog titled "Baking"** with Cancel / Save Settings / "Bake Git_Demo" / "Bake selected textures" buttons and an inline Mesh Maps checklist — this matches this skill's version-history research (`references/release-notes-painter-8.3.md`) describing the **old inline "Bake Mesh Maps" dialog that Painter 8.3.0 (2023-01-10) replaced** with a dedicated full-workspace Baking Mode (F8, Start/Cancel buttons, breadcrumb navigation, no floating modal window). That UI match suggests this video **predates Painter 8.3.0** — i.e. it was very likely made several years before the companion "TEXTURE EVERYTHING" video (which uses the `Bevel Smooth` filter, pinning it to 11.0.0+). This is inferred from one screenshot rather than an on-screen version string, so treat it as a reasonable estimate, not a confirmed fact — but it is a useful example of exactly the kind of UI-generation-gap this skill's version-tracker exists to flag: **any viewer following this video's baking steps in a current Painter install (8.3.0+) will not find the dialog described/shown here — they need Baking Mode (F8) instead**, though the underlying baker parameters (Method: Generate from Mesh/Normal Map, Secondary Rays, Sampling Radius, etc.) are unchanged.

### Tags
layers, fill-layer, paint-layer, masks, generator, curvature, ambient-occlusion, thickness, tri-planar, procedural, blend-mode, pbr, basecolor, roughness, specular-glossiness, normal-map, height, alpha, color-management, texture-set, export, export-preset, channel-packing, intermediate

---

## Related Tutorials
None yet cross-linked — [How to TEXTURE EVERYTHING in Substance Painter](how-to-texture-everything-in-substance-painter.md) (same creator, same skill/library) is the natural companion: that video explicitly opens by referencing this one as its prequel ("four years ago I made this video about texturing skin... this is the sequel"), and shares this video's core layered-noise-mask + hand-paint-on-top pattern, folder-per-material organization, and per-channel blend-mode/opacity discipline, extended there with anchor points and the Bevel Smooth filter. Future ingests covering skin/creature texturing (Jared Chavez's "REALISTIC CREATURES: HAND PAINTED TEXTURES," "How to TEXTURE in SUBSTANCE PAINTER | Creature TEXTURING") or Marmoset Toolbag render-check pipelines should cross-link back here.
