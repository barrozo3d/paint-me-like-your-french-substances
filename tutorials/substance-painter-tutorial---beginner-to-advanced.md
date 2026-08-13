---
title: Substance Painter Tutorial -  Beginner To Advanced
source: YouTube
url: https://www.youtube.com/watch?v=qcQPItAXxgE
author: TriGon
ingested: 2026-08-13
app: "[PENDING]"
version: "[PENDING]"
tags: []
extraction_status: pending
frames_dir: tutorials/frames/substance-painter-tutorial---beginner-to-advanced/
frame_count: 0
frame_status: pending-selection
---

# Substance Painter Tutorial -  Beginner To Advanced

**Source:** [YouTube](https://www.youtube.com/watch?v=qcQPItAXxgE)
**Author:** TriGon
**Duration:** 81m33s | 22 section(s)

---

## Raw Data (for Claude Code extraction)

Frames are not captured yet. Read the timestamped transcript below, pick moments
that actually show a technique/result worth a still (not blind percentages —
even within a named chapter, verify the real moment against its timestamps), then run:
  python select_frames.py substance-painter-tutorial---beginner-to-advanced <ts1> <ts2> ...
(seconds or mm:ss). This appends a "Captured Frames" section and updates the
frontmatter before you write the Structured Notes below.


### Intro [0:00]
**Transcript (timestamped):**
[0:00] Hey guys, welcome to this video about Substance Painter.
[0:04] In this video we're gonna take an in-depth look at everything in Substance Painter I
[0:08] use to texture.
[0:09] I'm gonna explain all about smart materials, normal materials, masking, filters, and a lot
[0:17] more.
[0:18] And to do this we're gonna make some textures for this wooden barrel.
[0:22] I'm gonna explain at every step what I'm doing and why I'm doing it.
[0:27] So I hope you enjoy.


### Setup [0:33]
**Transcript (timestamped):**
[0:34] So we're gonna start off by setting up a project.
[0:37] Go to File, New, then here we can select our assets.
[0:42] First let's go with the mesh.
[0:44] I'm just gonna navigate to my mesh, click it.
[0:48] Then let's put the document resolution at 4k.
[0:52] Here you can choose your template.
[0:54] If you're gonna render it in Unreal Engine, I highly recommend that you put it on Unreal
[0:59] Engine obviously.
[1:01] But if you want to do something a mama said you can put it on PBR or whatever.
[1:08] Then here we can add our textures.
[1:10] This will be the bakes that we did.
[1:13] So I'm gonna navigate to them.
[1:18] Let's just add them all.
[1:21] And if you don't have UVs you can do an auto unwrap.
[1:24] But most of the times you have UVs already.
[1:27] Now we just hit OK.
[1:29] And here we have our model.
[1:34] Now we can go to Textures Settings.
[1:38] Now we can select our bakes here.
[1:40] So normal map.
[1:43] Real space.
[1:46] Our ID map.
[1:50] Ambient occlusion.
[1:53] Curvature.
[1:57] And the position map.
[2:01] Lastly the thickness.
[2:03] I'm gonna explain a bit later what all these maps do.
[2:09] But for now we have our model set up and we can start to texture.


### Custom UI [2:13]
**Transcript (timestamped):**
[2:14] I do not like the default UI.
[2:16] Let's up some spaint and nowadays comes a bit.
[2:19] So I'm gonna change it up a bit.
[2:21] Gonna drag this one down.
[2:24] Let's drag this one up.
[2:27] Drag this one up.
[2:28] And the properties spaint we're gonna drag to the left.
[2:34] Drag this one one more time to the left.
[2:37] Now it's a bit more organized in my opinion.
[2:41] We can also hit this little icon.
[2:43] And we'll get like a tab where we can navigate between all the different stuff and paint.
[2:50] So if we just hit the producerals we'll have all our producerals here.
[2:57] Materials and whatever.


### Materials vs smart materials [2:59]
**Transcript (timestamped):**
[3:00] So one of the most important things in Substance Painter obviously is the materials.
[3:05] So let's talk a bit about it.
[3:08] As you can see we have a whole bunch of materials that come with Substance Painter.
[3:13] And let's drag one in the Layers stack.
[3:16] So as you can see this is a fabric knitted sweater.
[3:21] We just get one layer in the Layers stack.
[3:24] I don't work a lot with materials as I don't really like to.
[3:29] Another thing that we can work with is smart materials.
[3:32] This is a lot better.
[3:34] So let's go to Wood.
[3:37] Let's pick up Wood.
[3:39] Let's go with this one.
[3:42] And you can see that we now have another material.
[3:48] That's Wood.
[3:49] But you can see instead of one layer we have a layer group.
[3:53] Once we open it we can see every layer that makes this material up.
[3:58] So if we just disable everything.
[4:03] You can see that this is a material like this one.
[4:06] This will be our base.
[4:09] And then it's just working with layers to break that material up and to make it more realistic.
[4:16] So it's a lot better to work with smart materials as they will have just more to add it in Substance
[4:22] Painter.


### Creating our own smart materials [4:24]
**Transcript (timestamped):**
[4:24] Personally I also don't really like to work with smart materials that Substance Painter
[4:29] gives as it's just a really limited way of working.
[4:34] The best workflow in my opinion is to go up here and we create a fill layer.
[4:41] But this is just a layer with some basic values.
[4:44] And we're going to make our own smart material.
[4:48] So instead of using this wood let's make our own wood.
[4:52] So we can pick a color.
[4:56] Pick a brown.
[4:59] Put the roughness down.
[5:01] No metallic.
[5:02] Make it a little bit lighter.
[5:05] Let's disable this one.
[5:08] Now we call this base.
[5:10] Then we can group it.
[5:12] Hit Ctrl G.
[5:15] We can call this boot material.


### Color variation [5:21]
**Transcript (timestamped):**
[5:21] The next thing that I want to do is add some color variations.
[5:27] If we hit the C key you can go to the base color.
[5:31] What ever channel you want to see.
[5:33] You can see that we have a lot of variation in the colors.
[5:36] Like here it's a light.
[5:37] Here it's more dark and saturated.
[5:41] So let's do that with our own material.
[5:45] To do this I'm just going to go to Filters.
[5:49] So let's see Filters.
[5:53] You can also go here and hit Filters.
[5:58] And we're going to use the huge saturation filter.
[6:01] It's going to work the exact same like Photoshop.
[6:04] This will allow us to change the color.
[6:06] So let's drag it into our layer stack.
[6:09] And the layer stack is just...
[6:12] Here you have your group.
[6:14] And here's your layer stack of that group.
[6:18] So let's hit on the filter.
[6:21] And here you have the channels.
[6:23] Whichever channel you pick the huge saturation filter will be applied to.
[6:27] So if we go to Lightness we turn this down.
[6:31] The color channel will get darkened.
[6:34] And any other channel it won't.
[6:37] Unless we hit the channel as well.
[6:40] But for now we're just going to keep it at the color.
[6:43] Let's call this Darken.
[6:48] Let's group it.
[6:50] Now in the base color.
[6:52] This is where the settings for each channel are.
[6:56] So let's go to base color.
[6:58] You want to set this on pass through.
[7:00] And now you can see the filter will be applied to our base.
[7:05] Anything that's under our filter layer.
[7:08] Any layer the filter will be applied to.
[7:12] But of course now it just makes everything dark.
[7:15] And we do not want that.
[7:17] So we can add a mask.
[7:19] Let's go to add black mask.
[7:22] Then we can add an effect.
[7:24] We're going to add a fill effect.
[7:28] If we alt click on the mask.
[7:31] You will see the mask is just a preview.
[7:34] So let's go to a fill.
[7:37] Now we can go to producer roles.
[7:39] We can choose our mask.
[7:42] So let's go where it's clouds to.
[7:46] Just hit it and drag it.
[7:49] Now you can see that we have a mask.
[7:51] Like Photoshop.
[7:53] The white will be shown.
[7:54] And the black won't be shown.
[7:56] Let's go to UV projection.
[7:58] And put it to try playing up projection.
[8:01] This will just make sure that any seams are hidden.
[8:05] If we put on UV projection.
[8:07] Now you can see we have a really bad scene.
[8:11] And once we go to try planar.
[8:13] It fixes itself.
[8:16] So producer role is just a tiling texture.
[8:19] With some stuff to edit.
[8:21] So we can change the balance.
[8:23] This will change the intensity.
[8:25] And the contrast.
[8:27] So let's do something like this.
[8:30] You can mess around with the scale a bit.
[8:33] Then if we hit M.
[8:35] You will go back to your material view.
[8:38] You can see now that we have some dark parts.
[8:41] And some light parts.
[8:43] So let's edit this a bit more.
[8:46] So we get something that we like.
[8:49] And I like this.
[8:52] Now we can duplicate the layer.
[8:54] Ctrl D.
[8:56] And let's call this light.
[9:00] Now we go back to our filter.
[9:02] We're gonna lighten the color instead.
[9:05] Let's also give it a bit more saturation.
[9:09] And let's go back to our mask.
[9:12] Now we wanna edit this a bit.
[9:14] So let's rotate it a bit.
[9:16] Let's give it a new producer role.
[9:19] Let's change the intensity a bit.
[9:22] Now you can see that we have some spots that are lightened.
[9:30] So I like this.
[9:31] But I think the effect overall is a bit too strong.
[9:35] So let's go to our folder.
[9:37] Let's call this color variation.
[9:43] Now we can also add a mask here.
[9:45] We're gonna add a black mask.
[9:47] This will get rid of the effect.
[9:49] Let's add a fill.
[9:51] Now we have a fill.
[9:53] Now we can edit the intensity of the whole folder.
[9:57] So I like it like this.
[10:00] Actually a little bit lower.
[10:03] Let's put the balance here a bit higher.
[10:07] So now we have some nice variation in our color.
[10:11] I also wanna get some of the variation back in the roughness.
[10:15] So I'm just gonna hit the roughness channel.
[10:19] And for this one as well.
[10:21] Hit the roughness channel.
[10:23] But it's not showing.
[10:25] As I said earlier, we need to go to our channel roughness.
[10:29] And put the folder color variation to pass through.
[10:34] Now you can see we have some variation in the roughness as well.
[10:40] So I think that's a nice start for smart material.


### Filters vs fill layers [10:46]
**Transcript (timestamped):**
[10:46] I also wanna empathize with something really important.
[10:49] You always want to be working with filters.
[10:52] Not with actual fill layers.
[10:54] This is a really destructive way to work.
[10:57] Because right now we can change our base color.
[11:01] And you can see that all our filters will update itself.
[11:05] So it won't break.
[11:07] Let's go back.
[11:09] We can even say it's blue and still works.
[11:12] But if we did the darken with a fill layer.
[11:15] It's just a darkened brown.
[11:17] As soon as we change the base to let's say green.
[11:22] Now we're gonna have a layer stack that's not working.
[11:26] As it will break.
[11:28] Because now you have the green mixed with the brown.
[11:30] With the huge saturation filter it will just update based on the base layer.


### Details [11:38]
**Transcript (timestamped):**
[11:38] Now let's compare our own material to the other one that we have.
[11:43] As you can see the wood is supposed to have some details.
[11:47] We're missing any kind of details right now.
[11:51] So we're gonna make a new group.
[11:54] Let's start off with a fill layer.
[11:56] Just so we can add control G to the group.
[11:59] We're gonna call this details.
[12:03] A stack of fill layer.
[12:05] Gonna disable everything except for the height channel.
[12:09] Let's call this layer height.
[12:12] For the details now we add black mask.
[12:17] Gonna add a fill.
[12:20] Add fill.
[12:22] Let's go to producerals.
[12:24] Type wood.
[12:27] Now you can see some paint that comes with the wood producerals.
[12:31] So let's drag it.
[12:33] Alt click to preview the mask.
[12:37] Now we wanna rotate the mask.
[12:43] I mean the producerals.
[12:45] Now you can see that's aligned with the wood.
[12:47] We hit M.
[12:50] Now in the height channel we can choose the intensity of the details.
[12:55] So let's do it a little bit inwards.
[13:01] Now you can see our wood has some details.
[13:04] But only in the height.
[13:06] Now we can add another filter.
[13:11] Let's go to filters and the HSL again.
[13:16] I don't really like to use any of the others as I just like to keep it simple.
[13:21] This filter works perfect.
[13:25] So again for a filter to work we need to change the blending mode to pass through.
[13:32] Now in the filter we're gonna drag the lightness down.
[13:36] As you can see anything where it's white.
[13:40] Now it's darkened in the color.
[13:43] Now you can see that the wood is starting to look a lot better already.
[13:48] So let's mess around a bit with how we want it to look.
[13:53] And yeah I like this.
[13:56] So let's call this layer color.
[14:01] And we can do another HSL.
[14:05] Let's call this, let's put it on the roughness channel.
[14:09] Again roughness, details pass through.
[14:13] Now it will work.
[14:16] Let's drag this.
[14:18] If you drag it down it will be more shiny.
[14:21] The more black the more shiny.
[14:23] The more white the more rough.
[14:25] So let's do it white.
[14:29] If you disable it you can just see what it does.
[14:33] Now you can see how much more detailed our wood is.
[14:37] It's starting to look a lot better already.


### Seperating details [14:45]
**Transcript (timestamped):**
[14:45] So a big problem right now that we have is that we have these wood planks.
[14:50] As you can see the details are just continuing.
[14:53] This looks really weird. This breaks any kind of realism.
[14:58] So earlier we gave one of the input maps an ID.
[15:02] If we hit B you can see the mesh maps.
[15:06] This is our ID map.
[15:09] An ID map is just used to tell substance painter.
[15:12] I want to be able to select this part of the mesh and to mask it.
[15:18] You create this in Zbrush by using polypaint and baking it as the ID map.
[15:25] So let's go to layers and to details.
[15:29] As soon as we have this whole thing done and we're happy with how it looks like.
[15:34] What we have.
[15:36] We can group this again.
[15:38] As you can see it breaks again.
[15:40] Put it on path through roughness, base color, path through.
[15:44] Now it's working again.
[15:46] Let's call this one details.
[15:49] Let's call this one 0 1.
[15:55] Let's do a duplicate.
[16:00] As you can see everything is really strong as we are duplicating the effect.
[16:05] Let's hide this one.
[16:07] Now we're going to add it a mask.
[16:09] Right now we only have the details as a mask.
[16:13] Let's hit M.
[16:15] Let's add a color selection.
[16:19] Now we can pick colors.
[16:22] Let's add this one.
[16:25] This one.
[16:26] We're just going to go one by one.
[16:38] Now you can see what we're doing.
[16:41] As we have an uneven number.
[16:43] We're going to have to do this three times but for the sake of this video I won't.
[16:49] So now we can go to this one.
[16:53] Now let's do the same here but with the other ones.
[16:58] We can also...
[17:00] Yes, the ones that are more bright.
[17:02] Let's select the ones that are more bright.
[17:17] Now you can see it's working again.
[17:20] You can see it messed up the colors.
[17:22] All we have to do is check out the mask.
[17:25] We can see that's applying it from.
[17:28] Let's change the output value to black.
[17:32] Let's do the same for the other one.
[17:38] Now you can see it's working properly again.
[17:41] The reason why is if we keep this to white.
[17:45] It will apply the effect, the HSL, to everything that's white.
[17:50] So these ones will be fully applied.
[17:53] So just change it to black.
[17:55] Now there's some mask which is good.
[17:59] Now to break this.
[18:01] We can go to our woods.
[18:03] We can just change the offset.
[18:06] Now you can see it's not continuing along anymore.
[18:11] So that's how you can break this kind of stuff up.
[18:17] I also don't like how many not stars.
[18:20] So let's just...
[18:22] ...low it at.
[18:28] So now we have a pretty nice detailed boot.


### Edge damage [18:32]
**Transcript (timestamped):**
[18:33] So now our boot has a layer.
[18:35] It has a base layer, a color variation and some details.
[18:39] So we go through it.
[18:41] You can see how with every group we're adding more detail to our material.
[18:46] One thing that's really lacking right now is some wet...
[18:50] ...let's make that.
[18:52] We're gonna do another fill layer, Ctrl G to group it.
[18:56] Let's call this edge damage.
[19:03] And there are lots of ways to make the mask for edge damage.
[19:06] But the most easy way is just to go to Smart Mask.
[19:11] And type edge damage.
[19:15] You will see some stuff.
[19:17] Let's keep that edge.
[19:19] So now we can preview.
[19:21] Kind of look at the edge dusty, edge blur.
[19:24] We're just gonna look for one that we like.
[19:30] So I like edge strong scratched.
[19:34] I like how that one looks.
[19:36] So let's drag it to our edge damage group.
[19:41] You see that we'll add some edge damage.
[19:44] The way this works is with the curvature map.
[19:48] Curvature we linked it earlier in our input maps.
[19:52] This one, let's go to curvature.
[19:55] This is just gonna make all the edges of your model bite.
[19:59] And you bake this one out.
[20:02] So now Substance Painter can make a map based from that information.
[20:07] We go here to the curvature.
[20:10] Alt-click it to see it. Curvature.
[20:13] We get some settings.
[20:16] So here we can go to global balance.
[20:19] We can decide how strong the effect is.
[20:23] Let's keep it kind of subtle.
[20:25] Here at curvature you can change more settings.
[20:30] Let's just mess around with it until we get something that we like.
[20:40] So let's say I like this.
[20:42] Now we have some damage.
[20:44] Now we can change the fill layer to height.
[20:49] Just get rid of everything except the height.
[20:54] Let's mess around with that a little bit.
[21:00] And now instead of doing a filter, I am going to use a base layer.
[21:05] The reason why I'm using a base layer instead of a filter is as you can see.
[21:12] Now it's replacing everything in the color that we had before.
[21:17] We go to filters.
[21:21] We put a filter, the HSL.
[21:25] Let's put this to the bathroom.
[21:28] You can see that it's keeping the details.
[21:33] That's something I do not like.
[21:35] As this will break the real lesson.
[21:38] As the details are supposed to disappear when we have some broken edges.
[21:42] Let's change back to normal.
[21:44] Get rid of this one.
[21:46] Let's call this base.
[21:50] For the color we can just pick here.
[21:53] Let's make it a little bit more light.
[22:02] I think the height is a little bit too strong.
[22:05] Let's turn it down a bit.
[22:10] I think that's looking pretty nice.
[22:13] I think it's too subtle.
[22:15] Let's go back to the mask.
[22:19] Let's put it up.
[22:21] Now you can see we have some real nice damage.
[22:26] The problem for me is now that all the damage is very boring.
[22:31] That's the same color.
[22:33] We can go back to our color variation.
[22:36] We can just duplicate this.
[22:38] Duplicate layers.
[22:41] We can put it in the edge damage folder.
[22:45] Let's put this on past through again to have it work.
[22:52] Color variation.
[22:54] Light and dark.
[22:56] Let's go to dark and see the mask.
[22:59] We want to make this a little bit smaller.
[23:02] So it's actually working with this.
[23:08] Let's change the contrast.
[23:12] The balance.
[23:14] You can now see that we have some break up here.
[23:18] So we can change the opacity.
[23:21] For the strength.
[23:23] Let's do the same for the light.
[23:28] Alt-click it.
[23:30] Change the scale.
[23:32] Balance.
[23:34] Contrast.
[23:36] Hit C to go to color.
[23:38] Now we can just kind of see that it's working.
[23:42] Let's make some saturated spots.
[23:51] The whole time you're just messing around with sliders.
[23:54] That's all.
[23:56] Change the opacity.
[24:00] As you can see now we have edge damage.
[24:02] It has some color variation.
[24:05] This will just help the realism.
[24:08] So I think that's looking pretty nice for edge damage.
[24:13] Now we can also say we want to have more damage.
[24:17] Let's group the edge damage.
[24:19] Now I see stuff breaks again.
[24:21] One set to past through.
[24:30] Past through.
[24:32] We only did the color.
[24:34] But we still need to do the roughness channel.
[24:36] Let's go back to edge damage.
[24:39] Let's go to base.
[24:41] Let's do the roughness here as well.
[24:44] So for damage let's just make it really rough.
[24:49] Now here we want to get rid of the roughness.
[24:53] Get rid of the roughness here.
[24:57] I'm going to do a new HSL.
[25:00] Let's call this one roughness.
[25:06] Disable color and go to roughness only.
[25:12] Now you can see we can edit the roughness as well.
[25:18] Let's edit the roughness a little bit.
[25:21] Let's say a little bit less rough.
[25:24] Let's add a quick mask.
[25:27] Add a fill.
[25:30] Go to producerals.
[25:33] Let's go with bnv spots.
[25:37] Let's view it.
[25:40] Tri-planar.
[25:41] Balance.
[25:43] Scale.
[25:44] Contrast.
[25:48] Now you can see we just have a little bit more break up.
[25:52] Make the effect a little bit stronger.
[25:57] All this break up, all it does is just going to help the material to be feeling more realistic.


### More damage [26:05]
**Transcript (timestamped):**
[26:06] Now let's go back to our folder.
[26:09] Let's continue our damage.
[26:11] Let's call damage.
[26:14] Make sure everything is passed through.
[26:16] Now first damage layer is the edge damage.
[26:22] We want to have some damage overall as well.
[26:25] Let's do a new fill layer.
[26:28] Actually we can just duplicate this whole layer stack.
[26:33] Instead of edge damage let's call it general damage.
[26:40] Let's view the mask.
[26:42] Let's get rid of it.
[26:44] Now we have no damage in the general damage.
[26:48] Let's add a fill.
[26:50] Producerals.
[26:52] Let's go to crunches.
[26:57] Now we can just pick a produceral that we like.
[27:00] I think this one looks pretty nice.
[27:05] Make some scratches or whatever.
[27:09] We can change it however we want.
[27:13] We can also invert it.
[27:17] Invert.
[27:18] Let's add some scratches.
[27:23] Let's change the name again.
[27:25] Let's go to scratches.
[27:31] Now our scratches will have everything that we did earlier.
[27:35] We'll have color variation and all that good stuff.
[27:39] For this I want to change the height.
[27:43] I want to make it a little bit more intense.
[27:47] Just a little bit.
[27:49] Now you can see we have a lot of scratch damage.
[27:52] What we can do is go to the mask.
[27:55] We don't just need to use one produceral.
[27:59] We can also add fill.
[28:01] We can put a blending mode on multiply.
[28:04] Now we can add another produceral.
[28:07] We can pick with this produceral.
[28:10] We can get rid of some of the parts of this one.
[28:13] Let's go to clouds.
[28:16] As you can see, if we disable this and let's put on normal.
[28:20] Anything that's white here will show in the background.
[28:24] We can add a new layer.
[28:27] We can add a new layer.
[28:29] We can add a new layer.
[28:31] Anything that's white here will show in the old produceral.
[28:35] Let's go multiply again.
[28:38] It will be a little bit more clear if we up the contrast.
[28:42] You can see that we are getting rid of some of the mask that we had earlier.
[28:49] We can just do what we like.
[28:51] Hit the M for your material.
[28:54] You can see how it's now more subtle effect.
[28:57] We can change how much it's shown through.
[29:00] I think like this, it looks really nice.
[29:03] We can view our channels.
[29:06] The base color is looking good now.
[29:08] And the worthiness as well.
[29:10] Pretty happy with what we have now.
[29:13] Let's do it one more time.
[29:16] Ctrl D, we can also do that to duplicate.
[29:19] Let's call this one general.
[29:21] Let's get rid of the mask again.
[29:24] Let's take a look at some smart masks.
[29:30] Type damage.
[29:32] Let's see what pops up.
[29:34] Hatch damage.
[29:36] I don't like this.
[29:38] We can just have a look by hand.
[29:40] See if we see something that we like.
[29:48] No, it's not something that I like.
[29:51] Let's go to producerals and let's build our own mask.
[29:56] So again, fill.
[29:59] It's always good to just look around.
[30:01] Maybe there's a smart mask that's going to work perfect for you in one time.
[30:05] In the other time, there's something just going to mess around.
[30:08] It produces rolls.
[30:11] Let's go to crunches.
[30:15] Noise maybe?
[30:17] Crunches.
[30:21] Let's go with this one.
[30:24] Let's change the contrast, the balance.
[30:33] Now we have a really beaten up boot and I like outlooks.
[30:40] Get rid of some of the bottom.
[30:43] Again, fill.
[30:49] Let's add another mask.
[30:53] So we did for this time.
[30:56] Multiply.
[31:01] I messed around until you got something that you like.
[31:08] So now I'm going to call our smart material done.


### Secondary details [31:13]
**Transcript (timestamped):**
[31:13] Actually, I'm going to have a little bit more details in the wood.
[31:17] As you can see, it's lacking some of the more finer detail.
[31:21] We compare.
[31:23] You can see these grains.
[31:25] We don't really have that yet.
[31:30] So in the details.
[31:36] Let's make a new fill layer.
[31:41] Let's call this height.
[31:43] Control-G. Let's name the detail.
[31:47] Fine lines.
[31:50] Let's go with wood lines.
[31:53] You want to make sure that you're as clear as possible in your layer stack.
[31:57] The more layers you keep adding, the more complicated your project is going to be.
[32:01] And especially if anyone else is going to need to work on your substance painting.
[32:06] It can be really difficult to find out later what you're doing.
[32:10] So you just want to try to be as organized as possible.
[32:16] So let's disable everything.
[32:19] Let's add a mask.
[32:22] So let's see if we can find a producer that will add some nice lines.
[32:27] So let's look.
[32:31] You can also drag this up.
[32:35] Here we have some lines.
[32:37] It's too much rounded.
[32:39] I'm going to have straight lines.
[32:49] So I think these look pretty good.
[32:59] I think the best way we can do is use this one's base.
[33:02] And then we can use this one's breakup.
[33:05] So let's start with that one.
[33:09] Add a fill. We're going to add this one.
[33:14] Actually let's add the color back so we can see what we're doing.
[33:19] Let's rotate this again.
[33:24] Now you can see we have some straight lines.
[33:27] They're a little bit too thick so let's change the scale.
[33:32] Now this is messing up. So let's keep that one.
[33:35] We're going to break this lock.
[33:37] Now we can edit the X, separate from the Y.
[33:42] In the Y we can just scale it up.
[33:45] So we'll have more horizontal lines.
[33:50] So I like this. This is looking good.
[33:53] One problem is that it's looking really, really straight.
[33:56] What we can also do is we can add filters to masks.
[34:00] So let's add a filter.
[34:03] Let's type warp.
[34:07] This is just going to warp our mask.
[34:11] As you can see. Let's edit it a bit.
[34:14] Then set the size.
[34:16] Let's edit it a bit.
[34:18] Tensity divided by 1000 is good.
[34:21] Let's change the intensity.
[34:26] Now we can disable and enable.
[34:29] You can see it's adding some nice break up.
[34:34] Now height. Let's disable the color again.
[34:37] Let's punch this down a bit.
[34:40] Now you can see we have some more lines.
[34:44] Add another filter.
[34:53] Let's call this one color.
[35:00] Let's put the lightness down.
[35:02] Again, pass through.
[35:06] Now you can see we're getting a lot of details in the wood.
[35:14] So I like how that looks.
[35:18] The height.
[35:20] We can also go to the height channel.
[35:23] You can edit it here.
[35:25] Sometimes it's a little bit more easier as you have more control.
[35:34] Let's also go to the roughness.
[35:37] Duplicate this layer.
[35:39] Call it roughness.
[35:44] And then the roughness channel.
[35:47] Let's add on pass through again.
[35:49] Now we get the details back.
[35:53] As you can see, now we have a lot more detailed wood.
[36:02] I also want to do this one more time.
[36:04] As I said, the other one looks good for break up.
[36:07] Let's duplicate the whole layer.
[36:09] Let's call it a boot.
[36:12] Let's call it boot lines.
[36:14] Break up.
[36:19] Go to a mask.
[36:21] Now all we do is disable the warp from now.
[36:25] Let's go to produce rows.
[36:29] Let's see the directional noise.
[36:32] Noise.
[36:40] Let's check our base color.
[36:46] As you can see, it's too general right now.
[36:48] Let's change the contrast.
[36:50] Let's change the scale again.
[37:00] Let's change the scale again.
[37:08] The balance needs to be lower.
[37:10] The balance needs to be lower.
[37:20] Let's put this to 3.
[37:26] No, 6.
[37:34] As you can see, now it's just adding some break up details.
[37:41] Let's do a little bit more balance.
[37:46] The more break up you have in your material, the more realistic it's going to look like.
[37:52] Of course, you can have too much break up and it's going to become a noise.
[37:56] So you want to avoid that.
[38:01] I don't know what happened to the roughness, but it's messing up a bit.
[38:06] Let's go to the roughness.
[38:09] Let's make this more light instead.
[38:16] We have a bit too much height, so it's become really noisy.
[38:21] For this one, I think we can disable the height.
[38:24] The wood lines break up.
[38:26] Let's just drag this down.
[38:29] If you have too much height, it's just going to become noisy.
[38:32] So you want to keep an eye on that.
[38:35] For this one as well, let's drag it down.
[38:39] This one, drag it down.
[38:44] And for this one.
[38:47] That's a bit better.
[38:49] I think our wood is too rough now.
[38:58] Yes, that one.
[38:59] Go to the roughness.
[39:01] Let's make the break up more white instead.
[39:09] Now what we can also do is group this.
[39:20] Base color, best true.
[39:25] Roughness, best true.
[39:28] Let's call this primary details.
[39:33] Now for the wood lines, these are secondary details.
[39:38] Put it to best true.
[39:41] Base color, best true.
[39:46] Let's call this secondary details.
[39:55] So I'm going to quickly expand my primary details and secondary details.


### Primary/secondary details explanation [39:57]
**Transcript (timestamped):**
[40:00] You also have the tritary details and micro details.
[40:05] Those are like the four layers that you build up surfaces.
[40:08] You do it in ZBrush as well all the time.
[40:12] Let's actually see if we can spot it here.
[40:19] This one doesn't have micro details, but it has all the others.
[40:23] The primary details would be these big shapes.
[40:27] These are going to add a lot.
[40:31] And then the secondary details would be like these lines that we were doing earlier.
[40:36] It's basically the more visible the details.
[40:40] It's going to depend what class they are.
[40:42] Primary, secondary, tritary, micro.
[40:47] These are still pretty visible.
[40:50] So these are still pretty visible.
[40:52] So they're the secondary.
[40:55] And then if we zoom in all the way, you see like these lines.
[40:59] They're very visible, but they're going to break up the surface.
[41:03] Those will be the tritary details.
[41:05] And then if you add some details that are like almost invisible, that'd be the micro details.
[41:12] In games, we don't really use the micro details.
[41:16] As you won't be seeing them, as will just become a noise.
[41:19] But you can use them, but don't spend too much time on them.
[41:23] They're more important when you have like really close-up renders, like in films or whatever.


### Adding final details [41:32]
**Transcript (timestamped):**
[41:36] You also just kind of define whatever what is for your own.
[41:40] Like the secondary details doesn't need to be really really small.
[41:45] If the second most visible details on your model, then they become the secondary details.
[41:54] So I do want to add one more detail pass.
[41:57] Just have like some break up, like some rounded stuff in the wood.
[42:05] So let's add another.
[42:08] Let's do a fill group.
[42:14] Let's call this height.
[42:18] We're going to leave the colon so we can actually see what we're doing.
[42:21] Add a black mask.
[42:25] Let's look for something that's going to add some rounded details, like some areas.
[42:31] I want to have some more detail.
[42:33] I think a good one would be plasma.
[42:38] Let's add fill.
[42:41] Let's put it here.
[42:43] Now you can see we have some rounded plots.
[42:47] Change the balance.
[42:53] Change the scale.
[43:02] I think something like that is pretty nice.
[43:05] Let's change the shape up a bit.
[43:08] Let's go to filter, warp.
[43:12] Now we can warp it a bit.
[43:16] Now I want to get rid of some of these.
[43:19] Let's go to fill.
[43:25] Let's actually do another plasma.
[43:30] Change the balance.
[43:36] Change the balance.
[43:40] Maybe a purlin noise.
[43:46] Change the balance.
[43:50] Now we have some spots.
[43:53] Now we can mess around with the blending mode.
[44:00] Now only on the white, the details are going to show through.
[44:04] Let's make this one a little bit bigger.
[44:23] Now we have some spots.
[44:26] I think we need a little bit more contrast.
[44:29] So we can do our levels.
[44:34] Let's see a mask.
[44:46] You just want to mess around with it.
[44:53] Now we have some spots.
[44:56] Let's go to the blue.
[45:02] I want them to be a little bit more spread.
[45:05] So we can add a filter.
[45:08] We can do a blur.
[45:11] But not a normal blur.
[45:14] You have a blur slope.
[45:17] This is just going to break the shape up in a more organic way.
[45:21] I think that's good.
[45:24] Let's go to height.
[45:26] It's disabled everything except for the height.
[45:30] Let's punch this in.
[45:34] Now you can see our wood has punched in height.
[45:44] Filter, HSL.
[45:50] Let's change the lightness.
[45:53] Best True.
[45:59] This is just going to add a little bit of a break up.
[46:06] As you can see it doesn't add a whole lot.
[46:09] It's just going to add some break up from the material.
[46:12] So it looks less repeating.
[46:19] Let's call this one spots.
[46:24] Let's move to a secondary details folder.
[46:32] That's it for our wood material.
[46:35] I think we have something that looks good now.


### Saving your smart material [46:37]
**Transcript (timestamped):**
[46:38] Now that we're done with our wood material let's compare.
[46:43] As you can see the wood looks good.
[46:46] The advantage of making your own smart materials is
[46:50] they can make it look like how you want it to look.
[46:56] If we use this material I don't like how this wood looks.
[46:59] I prefer something that looks more grime and dark.
[47:05] Now we're going to have to go in the layers stack and edit everything.
[47:08] At that point you're just kind of working against yourself.
[47:11] For me it's easier to just start off fresh and do whatever you want.
[47:14] Now I know exactly how my smart material works.
[47:20] I can easily edit anything I want later on.
[47:24] So one very important step.
[47:27] Just right click.
[47:29] Now you can click create smart material.
[47:33] Let's change the name.
[47:36] Boots let's say try for Trigon.
[47:42] Now we can right click create smart material.
[47:45] Now in our smart materials step we will get a new smart material.
[47:50] Called wood trike material.
[47:54] Now when you're working on any kind of project where you're using wood.
[47:59] Let's say I made this for this wooden barrel.
[48:02] But I also have a wooden crate.
[48:04] I can just drag the smart material.
[48:12] It's gonna load.
[48:20] Now we have a smart material.
[48:24] Now it's the same as using the painted default smart materials.
[48:28] Except for that we made this one ourselves.
[48:34] Let's get rid of the default one.


### Viewport settings [48:36]
**Transcript (timestamped):**
[48:37] Let's talk about something else that's pretty important.
[48:41] How your substance painter looks.
[48:44] It's like a small thing.
[48:46] It's just gonna make working substance painter more nicely.
[48:51] I always wanna work with the Tomoko studio.
[48:55] This one just has a little bit more accurate color.
[48:59] Like the base color will be more similar to your material color.
[49:03] I like to put the opacity all the way up.
[49:06] And the blur also all the way up.
[49:09] Now with the opacity it becomes like a slide of how dark your background should be.
[49:14] Let's say like this.
[49:17] So I wanna add some shadows.
[49:19] Let's put on average.
[49:21] If you have a really good computer you can put it on intensive.
[49:25] But average is fine.
[49:27] You can change the opacity.
[49:29] I like to put it somewhere down the middle.
[49:34] The focal length I like to work with a really big one.
[49:38] Let's put it at 80.
[49:43] And the bigger the focal length the less perspective you have.
[49:48] And the smaller the more perspective you have.
[49:55] If you're working with faces and portrait photography like 80 is the usual that people go with.
[50:03] You can post effects.
[50:06] Let's add some vignette.
[50:11] And the aliasing I like to just put it all the way on top.
[50:15] And sometimes I like to work with color profiles.
[50:19] But one thing that's like important you need to remember.
[50:23] That it's gonna distort like your color accuracy.
[50:27] Like what you see is not the actual texture at this point.
[50:31] So you can just pick one that you like.
[50:34] And you can kind of mess around with it.
[50:37] I don't like to work with this too much.
[50:41] Usually I just turn it on at the end to get a little bit nicer of a look.
[50:47] But I'll come back and turn it off a lot of times to see more accurately what my textures are looking like.
[50:55] The texture filtering we can put this one a little bit higher.
[50:59] It's just gonna give some a little bit nicer of a preview.
[51:05] You can change the AO intensity.
[51:09] You can change the quality.
[51:15] Put that high.
[51:20] Now these other settings I don't really mess around with.
[51:25] Just go back and change the opacity.
[51:28] Let's put a little bit more like this.
[51:32] And to me the viewport looks a lot nicer to look at now.


### Adding more details [51:37]
**Transcript (timestamped):**
[51:38] Now of course we're working with multiple materials.
[51:41] Not everything's gonna be wood.
[51:43] Like here we have metal parts.
[51:48] So let's go to Smart Materials.
[51:54] And now you can choose to make another Smart Material and do it all from scratch.
[51:59] But as it's just to show you our video, I'm not gonna do that.
[52:02] I'm just gonna go with a basic one.
[52:04] Style Steel.
[52:06] Go with Steel Bruined.
[52:14] So let's drag it.
[52:16] Now we're gonna have to mask out the metal parts.
[52:19] Add a black mask.
[52:22] And what you can do is you can add mask with color selection.
[52:26] Now with the ID map we can choose the parts that's gonna have the metal selected.
[52:32] But as these are separate meshes I prefer to just go here.
[52:37] But if everything is merged together you're gonna need to use your ID map.
[52:41] We can put it to object.
[52:44] And whatever object we click will have white applied.
[52:48] Or you can have black applied.
[52:52] So let's go through it.
[52:54] And now I'm gonna have to select all of these layers.
[52:58] So let's go through it.
[53:00] And now I'm gonna have to select all of these layers.
[53:03] So better way to do it is just to select everything here.
[53:07] Make it black.
[53:09] Now we make white.
[53:11] The part that we don't wanna be shown.
[53:15] And now all that we have to do is add a filter.
[53:19] Let's go to invert.
[53:23] It's gonna invert the black to white and the white to black.
[53:26] Nightlight.
[53:28] Invert.
[53:30] It's gonna invert the black to white and the white to black.
[53:32] Now you can see we have it.
[53:38] Let's also add some rust to this.
[53:44] Actually let's make it a little bit less shiny first.
[53:48] On top of smart materials the easiest way to edit them.
[53:52] Just go to filters again.
[53:55] The HSL all the way at the top.
[53:58] Let's say it's too shiny.
[54:00] Roughness.
[54:02] And we can change it all really fast and easy.
[54:07] And I think that looks a lot better right now.
[54:10] Let's call that one roughness.
[54:13] Minus.
[54:16] There's a pretty cool filter as well.
[54:19] Some filters.
[54:22] You have this rust filter.
[54:25] You can drag this on top.
[54:28] It's just gonna add some rust.
[54:38] So pick something that you like.
[54:41] I think that looks pretty cool.
[54:44] It's a bit too much though.
[54:49] So let's say this is fine.
[54:53] Now we have a steel rune.
[54:55] Let's go with metal.
[54:58] And we have a metal filter.
[55:01] Let's go with metal.
[55:04] And we have a metal filter.
[55:07] Let's call it metal.
[55:10] And we have a wood.
[55:12] I like to right click and give it colors.
[55:17] This way you can just easily see in the layer stack what's about.
[55:21] Like if you have a lot open I can easily say.
[55:24] This is red, here's green, here's a new material.


### Effects group [55:31]
**Transcript (timestamped):**
[55:31] Now we're pretty far on the textures.
[55:34] So I think that I like to do.
[55:37] I have a fill layer, Ctrl G to group it.
[55:40] And put a layer on top called FX.
[55:43] It's just gonna be effects.
[55:46] So let's call this one curve for the curvature.
[55:52] It's disabled everything except for the color and roughness.
[55:57] Let's go to project, clear project.
[56:00] Now we're gonna grab a curvature map.
[56:03] In both slots.
[56:05] This is just gonna fill that channel with the texture.
[56:10] Let's set this on path through.
[56:12] Roughness, path through.
[56:15] Let's go to the roughness.
[56:18] Now the blending mode we're gonna put this to overlay.
[56:22] Now it's gonna overlay your roughness.
[56:25] Overlay your curvature on the roughness.
[56:28] This is just gonna give your model a little bit more depth.
[56:31] And it's gonna get some of the details from your high poly back in the textures.
[56:35] You wanna keep this subtle though.
[56:38] So put that 25.
[56:41] And for the base color, gonna do the same.
[56:47] Overlay.
[56:50] 25.
[56:53] It's just gonna add some depth.
[56:57] It's a really subtle effect but it helps.
[57:00] It is gonna darken everything though.
[57:03] So we can also add another filter.
[57:09] Now I like to use the color correct filter here.
[57:14] Let's keep the name.
[57:16] It's good. Color correct.
[57:18] Now we can just correct the color.
[57:21] So let's go to color channel.
[57:24] We can mess around with these sliders.
[57:27] Just to get a better look.
[57:31] So change it however you want to.
[57:48] I think that's pretty nice.
[57:54] We can track a PBR validator on top.
[57:57] And we can check if we break it PBR values.
[58:00] Whether it's red, it's not good.
[58:03] Whether it's green, it's good.
[58:05] So you can see that we broke a little bit.
[58:08] Just track this one down a bit.
[58:11] You can break it but just be aware of it that you're breaking PBR.
[58:18] But in the end, I like to just do whatever looks better.
[58:21] But I do want to stick to the edge.
[58:24] I don't want to push the PBR values too much in the broken side.
[58:30] So I think that looks pretty nice.
[58:33] I do want to change your edge damage a bit though.
[58:36] So we can go in our layer stack.
[58:39] We can look to damage, general, scratch edge damage.
[58:44] Now instead of changing the base, we can do that.
[58:48] But we can also just track a HSL on top.
[58:54] And we can edit it this way.
[58:56] The thing with using these filters on top instead of going back in your base,
[59:00] is going to make your material take longer to generate and paint.
[59:05] So that's something that you need to be aware of.
[59:08] But it's just fast and easier and you have some more control on top.
[59:13] It's just going to be more organized.
[59:15] So I do like to use it.
[59:17] So let's call it color adjustment.
[59:22] Let's put the saturation up a bit.
[59:27] Lightness.
[59:29] Put that down a little bit.
[59:37] Too much.
[59:41] I can see it's a little bit more saturated.
[59:44] I like it a little bit more like this.
[59:48] You can also add a fill.
[59:52] Add a black mask.
[59:55] Fill.
[59:58] Project.
[60:05] Let's get our ambient occlusion.
[60:08] Actually, filters.
[60:10] We don't want to do a fill.
[60:14] HSL.
[60:16] Black mask.
[60:17] Fill.
[60:18] Project.
[60:22] Inter occlusion.
[60:25] Now we have a mask with our AO and we can bake.
[60:28] So we can make our mask.
[60:30] So we can make our mask.
[60:32] So we can make our mask.
[60:35] Now we have a mask with our AO and we can bake the AO.
[60:40] Into our texture.
[60:43] We do need to invert this though.
[60:47] Add filter.
[60:49] Invert.
[60:55] Now you can see we're baking the AO into our color map.
[60:58] Again, this is going to break some of the BBR workflow.
[61:02] This is just going to make your textures look nice in my opinion.
[61:07] When I'm doing random momma set, I like to do this.
[61:10] But if I'm doing something in Unreal Engine,
[61:13] I don't like to do the AO bake into the textures.
[61:17] As we can make a custom shader and we can control the AO intensity bake down in the color.
[61:23] In the shader itself there.
[61:26] But for now I'm just going to keep it here.
[61:30] In the roughness I don't like to edit it.


### Weathering effects [61:36]
**Transcript (timestamped):**
[61:37] So now we're pretty much done with our materials.
[61:40] We got our materials defined.
[61:42] The only thing that we're missing right now is some wear.
[61:47] Some weathering.
[61:48] This is just going to blend materials together and make your textures come alive.
[61:53] Right now we don't have any impact from our environment.
[61:58] It sounds a little bit fake, but you'll see in a bit.
[62:01] It's really easy.
[62:02] So let's go all the way to top.
[62:04] Let's put the effects at top.
[62:07] I like to have that one at the top all the time.
[62:09] Let's give it a color.
[62:11] Let's call this weathering.
[62:17] Ctrl G.
[62:18] And here we're going to do our first weathering layer.
[62:21] So let's call this one dust.
[62:24] Now in a fill layer you can choose the dust color and whatever.
[62:31] I like to use a dark blue-ish.
[62:34] Because this is really brown and a complementary color of the brown is blue.
[62:39] So that's why I like to use the blue here.
[62:43] So it's a smart mask.
[62:45] A static dust.
[62:47] Remember we can use a smart mask.
[62:49] Or we can create our own using fill and produce roles and maps.
[62:56] Let's look for one.
[63:03] The soft dust.
[63:05] I choose this subtle.
[63:09] Let's try this one.
[63:11] Let's put the balance up.
[63:24] Now you can see we're getting dust.
[63:29] This is just going to blend it in a little bit better.
[63:33] The materials.
[63:34] I think that looks nice.
[63:36] It's a little bit too dark though.
[63:40] Make the lid a bit more light.
[63:45] Put saturation down a bit.
[63:52] Yeah, I like that.
[63:54] Let's also do another one.
[63:56] Let's say...
[63:58] Blood.
[64:09] Let's just make some settings that look nice.
[64:12] Like a blood.
[64:14] I like to use blood because it's like I'm thinking of battle scene.
[64:18] The Vikings walking around for example.
[64:21] And they ended up being some blood on a barrel.
[64:24] This is how you can tell story through your textures.
[64:27] And they're going to make your objects come to life a bit more.
[64:32] For this one let's go to produce roles.
[64:35] Fill.
[64:38] And let's see if we can find a nice one.
[64:43] Like a fluid.
[64:48] Now that looks horrible.
[64:58] Just go through your trenches and see if you can find something that you like.
[65:03] Black mask.
[65:07] Fill.
[65:14] But I want to keep this really subtle.
[65:16] You don't want to have too much.
[65:18] That's going to look weird.
[65:20] Change the color.
[65:25] Because this is going on both materials.
[65:29] It's just going to blend the materials together a bit better.
[65:35] One thing that I want to do is the UV protection.
[65:39] Tri-planar.
[65:41] As you can see now it's going a bit better.
[65:45] Like you have a splatter of blood that continues on the next thing.
[65:55] So let's do a little bit less.
[66:00] For this barrel I'm imagining it standing on the ground.
[66:04] Let's add another fill layer.
[66:07] Let's get a small mask.
[66:10] We have dirt ground.
[66:16] Let's edit this a bit.
[66:18] Put the AO down all the way.
[66:22] Let's do the kerf down as well.
[66:26] Let's do the balance.
[66:29] The level up.
[66:33] Now you can see we have dirt that starts from the bottom.
[66:37] Do the crunch down.
[66:42] Let's do a fill.
[66:46] We can go to produce also.
[66:48] Let's do a simple clouds.
[66:50] And put this on multiply.
[66:52] This is just going to break our mask up a bit.
[66:58] Let's do a level up a bit again.
[67:06] This is being shown folder.
[67:08] Ctrl G.
[67:10] Actually let's make this like mud.
[67:13] It's going to add some nice break up in the roughness.
[67:17] Let's add a lot of height.
[67:32] It's not working well.
[67:38] Let's copy this mask.
[67:40] If you put it on the wrong layer you can just copy mask.
[67:43] Like a black mask.
[67:45] Let it fill.
[67:51] I mean paste into mask.
[67:53] Now we have a mask back.
[67:55] We can get rid of this mask.
[68:00] Let's see why it's not working.
[68:03] We still have to remove mask.
[68:13] And I cannot find why it's not working.
[68:15] Let's just do it again.
[68:17] Let's delete the whole layer.
[68:21] Let's copy the mask though.
[68:23] Copy mask.
[68:27] I'm going to group it.
[68:29] Add a black mask.
[68:33] Fill.
[68:35] And paste into mask.
[68:39] As you can see it's still not working.
[68:41] That means the mask is broken.
[68:45] Let's add a black mask.
[68:49] If you shift click you can disable it.
[68:55] Let's go to smart mask and let's just drag it in again.
[68:59] So ground.
[69:05] As you can see now it's working.
[69:07] I'm not sure. Maybe it was just a bug.
[69:13] Change the global balance.
[69:23] Let's put it up all the way.
[69:25] I think that looks nice.
[69:29] Let's call this one base.
[69:31] Let's put the roughness down.
[69:33] It's way too much.
[69:37] I think that's nice.
[69:39] The problem right now is we don't have any variation in the mud.
[69:41] So what we can do is we can create our variation layer again.
[69:43] We can just go in here.
[69:45] We can be really lazy.
[69:47] Just...
[69:49] We can just go in here.
[69:51] We can just go in here.
[69:53] We can just go in here.
[69:55] We can just go in here.
[69:57] We can just go in here.
[69:59] We can be really lazy.
[70:01] Just copy layers.
[70:03] Now control the duplicatum.
[70:07] We can just drag them from one smart mask.
[70:09] Smart material.
[70:11] Into another layer stack.
[70:13] As you can see now we have some variation back again.
[70:19] I think that's way too much variation though.
[70:21] So let's push that down.
[70:25] I think that's nice.
[70:29] So let's call this mud.
[70:33] Add a fill.
[70:43] Let's go with clouds again.
[70:47] Put it on multiply.
[70:53] I'm not sure why this is breaking it.
[70:55] So if it's not working we can also just group this again.
[71:03] Put on pass through.
[71:05] And on the second group now we can add another mask.
[71:09] Let's do a black mask.
[71:11] Add fill.
[71:13] Now we can track the producer all here.
[71:17] As you can see now it's working.
[71:21] Let's change the offset a little bit.
[71:25] Now we have some mud on our barrel.
[71:33] I think it's still a little bit too much though.
[71:35] We can mess around with this mask.
[71:39] Or we can go down to this mask.
[71:43] We can change the balance.
[71:49] You can basically add whatever you can think of.
[71:51] Like let's say it has some grass spots on it.
[71:53] You can add some green spots or whatever.
[71:59] That's basically all there is to texturing.
[72:03] It's just you're working with layers and you keep building your stuff up.
[72:07] So let's do a quick run through.
[72:13] As you can see first we have a base.
[72:15] It's just one solid color.
[72:17] Now we add color variation and roughness variation.
[72:19] It still doesn't look like anything.
[72:23] We add our details.
[72:25] Now it's starting to look like something.
[72:29] Then we add a damage.
[72:31] It's going to add a lot of nice break up.
[72:33] Now it's starting to look like something.
[72:37] Going to add more materials.
[72:41] Then we add some wear.
[72:43] Some weathering.
[72:45] It's going to tell some story and break a texture sub more.
[72:47] Then the effects layer.
[72:49] That's it. That's all there is to texturing.
[72:53] Like I said earlier.
[72:55] We don't have the right colors though.
[72:57] We have the color profile.
[72:59] So you do want to see how it looks without.


### Hand painting [73:02]
**Transcript (timestamped):**
[73:03] Actually there's one more thing to texturing that I forgot to talk about.
[73:07] Right now we only work with generators and produce roles.
[73:11] Doing everything with that.
[73:13] But we didn't do anything by hand.
[73:15] Like to push your text just further you do want to do some hand painting.
[73:21] So let's say in the boot we can go here.
[73:25] Create a new layer.
[73:27] Make the group.
[73:29] Let's say hand.
[73:33] Painting.
[73:35] Edge.
[73:37] Damage.
[73:39] Make it black.
[73:41] Now we can go to brushes.
[73:43] Let's search.
[73:45] Let's use a basic soft brush.
[73:53] Set up paint.
[73:57] Go to brush.
[73:59] Now we can start to paint some damage.
[74:05] This is just going to push your textures to the next level.
[74:07] It's going to look a lot more natural.
[74:09] It's going to have more break up.
[74:15] So now there we have some damage here.
[74:17] So sometimes you can like follow your textures.
[74:21] Like the generators that we added.
[74:23] They can guide you.
[74:25] Here we have like this shape.
[74:27] We can say alright let's take this shape.
[74:31] Let's just get rid of it.
[74:33] By following what you did earlier.
[74:35] It's going to make your textures look more natural.
[74:39] Let's go to color.
[74:43] So of course this looks horrible.
[74:45] So now we need to actually change the attributes.
[74:49] The color.
[74:51] Again I'm not using a fill layer.
[74:53] I'm using a fill layer because I want to get rid of the details underneath it.
[74:59] Color selected.
[75:01] Let's go with this one.
[75:03] Height roughness.
[75:05] We do need to height roughness.
[75:07] We're going to put this one really rough.
[75:11] Now in the height we're going to push this one down.
[75:19] It's looking pretty good.
[75:21] We can still also add it to our hand painted stuff.
[75:23] With filters.
[75:25] And fills.
[75:27] For this one I like to add a filter.
[75:29] Blur.
[75:33] And slope.
[75:37] Change the divider.
[75:39] And intensity.
[75:43] This is going to give a little bit more of an organic look to what we did.
[75:51] Now we can just go back to the paint.
[75:55] We can start painting our way stuff that we don't want.
[75:59] So again I'm just following the produce rules that we put in earlier.
[76:07] And it's a little bit slow.
[76:09] If you want to have it faster you can go to texture settings.
[76:15] You can change the size to 2K.
[76:19] It's just going to go through all your layers.
[76:21] It's going to generate them in 2K.
[76:23] As you can see it looks a lot worse.
[76:25] But now we can paint a lot faster.
[76:31] So my computer is pretty okay.
[76:33] So I can keep it at 4K.
[76:37] It's just going to generate everything again.
[76:39] For that 4K.
[76:53] Let's continue to paint here.
[77:03] I think that looks nice.
[77:05] I can actually add a little bit more detail.
[77:11] Make it a little bit less big.
[77:19] As you can see now our material has a lot more nice break up.
[77:23] Just turned off none.
[77:27] You can see it adds a lot.
[77:29] So you want to do this for everything here.
[77:31] You can also go to wet ring.
[77:33] Make a new folder.
[77:37] Like I said earlier you can add some grass spots.
[77:41] Let's call this grass.
[77:49] Make it green.
[77:57] Less saturated.
[78:01] Black mask.
[78:05] Add paint.
[78:13] Now with the brushes we can pick one that we like.
[78:17] I like to use this one a lot.
[78:19] The dirt one.
[78:27] Now we can just paint some spots on there.
[78:31] It's a bit too strong.
[78:37] And you need to remember that if we paint we can add it with produced rolls.
[78:43] So you can add a fill.
[78:47] Produce to multiply.
[78:51] Produce rolls.
[78:57] Let's add spots.
[79:01] Now we can change this.
[79:05] Now we can just edit your hand painted stuff a bit more.
[79:11] What you can also do is you can go to the blood one that we did.
[79:17] We can add a paint.
[79:19] Now we can hand paint some blood away.
[79:27] So let's say we paint that away.
[79:29] The one problem doing it this way.
[79:31] Now if we want to paint that back we take the white and you can see it ignores the generated.
[79:37] So let's undo that.
[79:39] We're going to add the blood.
[79:41] We're going to add a mask here on the folder on top.
[79:45] So let's add a white mask.
[79:47] Now if we get rid of this.
[79:51] We can go back to the white and we can still paint it back.
[79:55] But only where the generated generated it.
[79:59] So it's a little bit less destructive.
[80:05] That's really all there is to texturing.


### Exporting [80:08]
**Transcript (timestamped):**
[80:09] So now that we textured an asset all we have to do is control E.
[80:13] We can pick our settings and we can export it.
[80:19] I hope you enjoyed this video.
[80:21] I explained everything that is in Substance Paint to texturing.
[80:25] To what I use.
[80:27] There's a lot more techniques and different stuff that we didn't touch on.
[80:31] But those are all things that I do not use.
[80:35] Like you don't need them.
[80:37] These are the basics and with this you can text you anything you want.
[80:39] Once you get comfortable doing this workflow you can start to expand it.
[80:45] And look a bit more on other stuff that is.
[80:47] And these are the final textures that I did for this model.


### Closing words [80:49]
**Transcript (timestamped):**
[80:51] Over here you can see the final textures that I did for this model.
[80:55] But it's all using the same techniques.
[80:59] And maybe one or two days I'm going to upload a full video of doing these textures.
[81:05] But I'm not going to go into explaining what I do in the video.
[81:09] As I already did in this video.
[81:11] It will just be a two hour long video of texturing.
[81:15] So yeah. I hope you enjoyed.
[81:17] And if you want to see this video the next one.
[81:19] Make sure to subscribe.
[81:21] Bye guys.



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
