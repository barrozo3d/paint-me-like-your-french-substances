---
title: Creating environment materials and meshes in Substance 3D Painter
source: YouTube
url: https://www.youtube.com/watch?v=JMtw05Cj1gE
author: Wes McDermott
ingested: 2026-08-13
app: "[PENDING]"
version: "[PENDING]"
tags: []
extraction_status: pending
frames_dir: tutorials/frames/creating-environment-materials-and-meshes-in-substance-3d-painter/
frame_count: 0
frame_status: pending-selection
---

# Creating environment materials and meshes in Substance 3D Painter

**Source:** [YouTube](https://www.youtube.com/watch?v=JMtw05Cj1gE)
**Author:** Wes McDermott
**Duration:** 46m20s | 14 section(s)

---

## Raw Data (for Claude Code extraction)

Frames are not captured yet. Read the timestamped transcript below, pick moments
that actually show a technique/result worth a still (not blind percentages —
even within a named chapter, verify the real moment against its timestamps), then run:
  python select_frames.py creating-environment-materials-and-meshes-in-substance-3d-painter <ts1> <ts2> ...
(seconds or mm:ss). This appends a "Captured Frames" section and updates the
frontmatter before you write the Structured Notes below.


### Intro [0:00]
**Transcript (timestamped):**
[0:00] Hey, this is Wes. In this video, we're going to take a look at how we can use a Substance Painter to create some tileable environment materials.
[0:07] We're going to be blending materials, working with displacement, as well as using Painter's painting tools to fix any issues that we run into.
[0:15] Here is the result of what we're going to create in this video.
[0:18] This is the exported mesh from Painter with textures as a Nanite mesh in Unreal Engine 5.
[0:25] I will also cover the process of rendering the exported displacement map using Substance Stager.
[0:30] This is great for checking the displacement and producing some raytrace renders.
[0:36] Now, I was inspired to create this video based on a course that I recently checked out on ArtStation Learning called Environment Production by Decagon Studios.
[0:45] In that course, there is a video from Steph Velzabor that explains how to use Substance Designer to create environment meshes.
[0:52] That inspired me to check out how we can do that in Substance Painter.
[0:57] I'll put the link of the course in the description of this video.
[1:01] Now, let's jump into Substance Painter and check it out.
[1:06] Here we are in Substance Painter. I'm probably going to move through this fairly quickly.
[1:10] I'm going to assume that you already know Substance Painter.
[1:14] This is more of some advanced techniques.


### Scene setup [1:17]
**Transcript (timestamped):**
[1:17] Taking a look here, I've already created a project and I imported in a ground plane.
[1:22] This ground plane is four meters.
[1:25] Let's come over here to my display properties and I'm going to enable my mesh wireframe.
[1:32] We'll set this here to green and let's take our opacity up.
[1:35] You can see that it's already pre-subdivided, not too dense.
[1:39] Like I said, this is a four meter by four meter plane.
[1:43] You'll also notice here that the plane will slope down to basically zero on the grid.
[1:51] Here along the edge.
[1:53] If we take a look here, this is what this looks like.
[1:56] The plane is coming in and just slopes down like this.
[1:58] The reason I have this is because when I start to take this plane and kit bash it into other applications
[2:04] like where I'm going to be rendering it, I can just slide these planes together.
[2:08] What it ends up looking like is when you start to put these guys together like this,
[2:12] something like putting together flooring tiles,
[2:14] we can mash these two guys together where they slope down.
[2:18] Then some of my height information now will easily start to blend together in this area.
[2:24] Because the height information is so detailed and dense that you really makes it super hard
[2:29] to see any types of seams or anything like that.
[2:32] That's what I'm doing with the overall mesh.
[2:35] Let's go in and just turn off that mesh wireframe and let's get to texturing this guy.
[2:40] Now, to start off, I'm going to be using some substance materials that I downloaded from substance 3D assets.
[2:46] You can jump out to the website and download materials and import them into Painter.
[2:51] In this particular case, I always like to use the Creative Cloud Desktop app.
[2:56] Here I have the Creative Cloud Desktop app.
[2:58] The reason why I go this route is here under Stock and Marketplace under 3D,
[3:02] I can browse my materials, but I have this really nice ability to click a material that I like.
[3:07] I can click the Send to button and I can send this straight into Painter.
[3:11] It just saves me the process of being on the web page, downloading the material,
[3:14] re-importing it back in.
[3:16] I can just send it right into Painter.
[3:18] I have two materials that I grabbed from substance 3D assets.
[3:21] These are actually fairly new.
[3:23] I'm going to be using these two materials.
[3:26] We're going to mix and blend them together to create a nice, tileable environment material.
[3:32] I'll go ahead and close out the Creative Cloud Desktop app.
[3:34] You can see that I have these materials here in my library.
[3:38] Now, something else I did that's fairly new to Painter, I right-click.
[3:41] You can actually, I've already done it, but you can add materials to Favorites.
[3:46] Here it makes it very easy to tag assets and then reuse them.
[3:50] Here, for example, in my library, if I do a search here for Favorite,
[3:54] you can see that it just shows my Favorites.
[3:57] Then I'll click my little Folder button.
[3:59] This pops those guys out into a new tab.
[4:01] I'll set this to be a large icon.
[4:03] Now I have two tabs here.
[4:05] Let's go back to the assets.
[4:07] I'm just going to tear this off and dock it to the bottom.
[4:10] Now I have a tab that lets me look at the materials I want to work with in my project.
[4:15] Then I have my actual assets that when I want to choose different brushes and things like that.
[4:20] With that said, I'm going to grab this material.
[4:24] This is going to be this construction soil.
[4:28] We're going to drag and drop it here onto the plane to apply it.
[4:31] Within a second here, you can see that there we go.
[4:33] We have that material.
[4:35] You can see here that this material or the mesh has a texture set of just a single material.
[4:41] If I look at my texture set settings, it's set to 2K.
[4:44] Again, I can always increase this resolution or export it at a different resolution.
[4:48] I'm going to keep this at 2K for now.
[4:51] Now I'm ready to get to work.
[4:54] First things first, let's look at the material here.
[4:57] I don't need this little layer that was painted in here.
[4:59] I'm just working with the fill layer.
[5:01] First thing I'm going to do is look at my channels.
[5:04] I have color, height, rough, normal.
[5:06] I'm not going to be working with the normal information.
[5:09] I can turn off the normal.
[5:10] You can see now we don't have anything, no information.
[5:13] What I need to do is just enable the height channel itself.
[5:17] Now I'm starting to get some of this information here.
[5:19] It doesn't look great.
[5:21] Here's what it would look like with the normal.
[5:22] You can see that you get a little bit more detail.
[5:25] What we're doing here with the height information, just so you know how painter works under the hood,
[5:29] is that when you have the height channel, we take that and we convert that height to normal in the shader.
[5:35] You're actually looking at some normal information.
[5:38] With the height, I'm not doing any displacement yet.
[5:41] This is completely flat.
[5:43] That's where we're starting to get that detail.
[5:45] It's actually a normal.
[5:46] Then when I enable the normal channel, now I'm getting a normal value on top of a normal value.
[5:52] It's like a double normal and it can cause some issues sometimes.
[5:55] It may not be what I'm looking for.
[5:57] We'll actually generate our own normal a little bit later on.
[6:00] For now, let's turn this off.
[6:02] It's looking pretty weak, but we'll fix that in a second.


### Using Physical Size [6:04]
**Transcript (timestamped):**
[6:05] Let's set up our overall scale because that's the very next step we want to do.
[6:09] Now that we have our channels that we're working with enabled.
[6:12] Underneath the attributes category, you can see that I can see the size.
[6:17] This is 180 centimeters by 180 centimeters or 1.8 meters.
[6:22] As I said before, this ground here is 4 meter by 4 meter and we're almost there, right?
[6:27] 1.8.
[6:28] What I could do is under my UV projection, thinking, okay, this is close to 2 meters.
[6:33] This is 4.
[6:34] Why don't I just tile it by 2 so I get hit 2.
[6:37] That would size this material so that it appropriately matches the physical size of the actual geometry plane that I'm working with.
[6:48] That's one thing we could do.
[6:49] However, here in Painter, we have an even better way to do this.
[6:53] We can come over to projection and I can set this to triplanar and then for scale option on the UV transformations, I can set this to physical size.
[7:01] As soon as I do that, Painter is able to read the physical size information of my material and compute that so that it works and tiles correctly for the physical size of the object, even at 1.8 meters.
[7:14] This is perfect.
[7:15] This is exactly what I want to work with.
[7:18] Now we have our tiling set using physical size.
[7:21] Great feature.
[7:22] Love this.
[7:23] We need to set our actual displacement because right now we have zero displacement happening.
[7:27] So let's jump in and take a look.
[7:29] One thing we'll notice is that for the Z on this, this is 9.65 centimeters.
[7:34] So let's jump over to our shader and you have your shader settings.
[7:38] I also want to make sure first off, my quality, it's set to really low 16 samples per pixel.
[7:44] And that's really going to give me like a false sense of what my roughness looks like because the samples are so low, it's going to blur the roughness and it's just going to look more rough than it actually is.
[7:54] So what I like to do is pump this up to like very high just by default every time.
[7:58] And that's going to give me a more accurate display of what my roughness looks like.
[8:01] You can see there was a change in the viewport.


### Setting up displacement [8:03]
**Transcript (timestamped):**
[8:03] Now we're going to jump over here to displacement and tessellation.
[8:07] I can see that it's enabled, but my scale is set to zero.
[8:11] Source channel is height.
[8:13] So we need to set this up, right?
[8:15] So if I set this to like a one, well, that's crazy.
[8:17] We don't want to do that.
[8:18] And you can see it just went to 0.5.
[8:20] So I'm going to set this to a value of like, say, 0.02.
[8:24] And now you can see that, okay, well, we're starting to get some displacement here.
[8:28] That's all great, but you know, it's really low quality, right?
[8:32] So here's where we need to increase the tessellation in our shader.
[8:35] We can do that by uniform or edge length.
[8:37] I'm just going to set this subdivision count all the way up.
[8:40] And now we're starting to get some nice tessellation here.
[8:43] It looks pretty good.
[8:44] And so this is just an arbitrary setting that I'm kind of going with here in my shader.
[8:49] And it depends.
[8:51] If I'm taking this to another third-party renderer where I need to set the scale of the height,
[8:55] you need to work out what the differences would be in that scale.
[8:59] In my case here, though, I can actually export this tessellated mesh right out of Substance Painter.
[9:04] And so now it's really a matter of what I want it to be.
[9:07] So for example, if I want it to be super accurate, I could do .0965, I think.
[9:13] Nope, I need to do .20s there, I think.
[9:16] So I could do this.
[9:17] And that's a bit more accurate.
[9:19] But maybe that's not enough, right?
[9:23] So maybe I want to do something more like that.
[9:26] And again, just art-directing this a little bit.
[9:28] Just, ah, okay, that's better.
[9:29] Let's do that.
[9:30] Okay, so at this point, you can see here that we've set up our material.
[9:36] We've tiled it based on physical size.
[9:39] We've enabled our color height rough and we don't need metal.
[9:42] And we've disabled our normal.
[9:43] And now we actually have displacement.
[9:45] The normal that we see is being generated from the height information.
[9:49] We do that inside of Substance Painter via the shader.
[9:52] So now we have our base set up and I'm already looking at this from a tiling perspective.
[9:57] And I'm seeing, okay, look at this.


### Fixing repeating patterns [9:58]
**Transcript (timestamped):**
[9:58] We're getting some really recognizable patterns here.
[10:01] Let's take a look at how we can fix that.
[10:03] Okay, so let's jump in and see how we can fix this.
[10:06] And to do that, we're going to use the cloning tool in Substance Painter.
[10:10] So first thing, we'll come over to the layer and I am going to call this layer.
[10:14] I'm creating a paintable layer and we'll call this tiling fix.
[10:18] And then over on my left toolbar here, we're going to grab the clone tool.
[10:22] Now the clone tool is going to allow me to clone data across multiple channels at the same time.
[10:28] Super awesome to be able to do that.
[10:30] But to get it set up, all I need to do is come over to the layer
[10:33] and I need to explain or set the blending modes to pass through for the channels that I want to clone.
[10:39] So base color, definitely want to do that.
[10:41] So I'm going to set this to pass through.
[10:43] Then I'm going to use my channel selector to go to height.
[10:46] I'm going to set that to pass through.
[10:48] I'm going to go to my roughness information and once again set that to pass through.
[10:52] And then I'll jump this back to base color just so I can see the color icon here.
[10:56] And now that that's set up, I can easily clone across any of these channels.
[11:00] So I'll hit the V key to just sample an area.
[11:03] And then I'll come over here to this kind of really noisy detail and we'll just clone that right out.
[11:09] And what we're doing is we're cloning across all of our channels at the same time, which is pretty cool.
[11:14] And that looks great.
[11:15] So we can go in and do that.
[11:16] Not being super careful over it just for this demonstration, but here, let's just go kind of quick with it.
[11:23] And there we go.
[11:25] Just kind of clone that guy out.
[11:27] And you know, you could be a lot more careful with it.
[11:30] I don't really like what's going on there.
[11:31] So let's just do this, just kind of clone into here.
[11:34] You can see, like I said, it's cloning the height information and everything.
[11:38] So we'll just tweak that there.
[11:39] Okay, looks fine.
[11:41] Okay, next up, let's get this side here too.
[11:43] So again, just pick a cloning area and just clone into here like we want clone something like that.
[11:51] That looks too close of a detail.
[11:53] There we go.
[11:54] Okay.
[11:55] And you can also like another thing that would be really helpful for this would be instead of just using a circle brush.
[11:59] I could try to do something like, let's see here, let's just look at my alphas and go through here and just grab an alpha that's a little bit more grungy.
[12:09] Try to find something pretty quick.
[12:11] You know what's probably easier to do it over here.
[12:13] So again, we'll go to our alphas and let's see here.
[12:20] Just try to grab something.
[12:24] Let's do a dirt.
[12:26] Yeah, any of these are good.
[12:28] This dirt cloudy.
[12:29] Okay, let's do that.
[12:30] So I could throw in this as my cloning shape and I can, you know, increase or decrease the hardness, the shape of that.
[12:38] And then again, we're going to hold down the V key, sample an area, and then you could go in and paint here.
[12:43] Let's make that way less hard.
[12:46] And there we go.
[12:47] And then kind of just stamp and clone around in here.
[12:49] That makes it a little bit more organic, right?
[12:51] So any little bit of chaos that you can, you can throw into these guys, the better in here.
[12:56] That looks so much better than what I was doing a second ago.
[12:59] So here again, you know, you can, you can sit and tweak on these things all day long, right?
[13:04] So here, let's just get it pretty much into place.
[13:07] So that's the clone tool.
[13:08] It's pretty awesome.
[13:09] It's really great for this setup.
[13:11] All right.
[13:12] So now that that's in place, I have a couple other like, okay, so this dirt area is really like super visible, right?
[13:18] In my tile.
[13:19] But you know, I think it's going to be okay because I'm going to now blend another material over top of this.
[13:24] And I think that's going to really take care of most of what I want to do.
[13:27] So before I do that, there's a couple other things I'm going to set up.
[13:31] First thing, let's start working with some ambient occlusion.


### Creating Ambient Occlusion [13:34]
**Transcript (timestamped):**
[13:34] So I'm going to come over to my texture set settings and the channels.
[13:37] I'll click the plus button and let's add an ambient occlusion channel here.
[13:41] Now on my layer, I could come over and I could add ambient occlusion and it's very low quality or I mean, sorry, low intensity.
[13:48] So I could add it and then come down to the channels and tweak it and everything, but I'm not going to worry about that.
[13:53] So I'm going to include here an ambient occlusion channel that allows me to work with that data here in my layer stack.
[13:59] Then I'm going to come over to my assets and we will do a search for ambient.
[14:05] Whoops, I'm in my filters here.
[14:07] This is where I want to go.
[14:08] Sorry guys.
[14:09] There.
[14:10] All right.
[14:11] Ambient occlusion, horizon based ambient occlusion.
[14:13] That's what this stands for.
[14:14] And then I can just simply drag and drop this filter here to the top of the layer stack.
[14:19] And there we go.
[14:20] I start to get that ambient occlusion now.
[14:22] So if I turn it on and off, here's the difference we're getting.
[14:26] Now this horizon based ambient occlusion in here in Painter, it doesn't have the real world settings, which is kind of a shame.
[14:34] We can adjust this like you can't go above one, right?
[14:37] So if I type for, you're kind of stuck here.
[14:40] So it's just a matter of just trying to, I think visually just figure out where you want this to be.
[14:45] So I'm just going to play with this and then maybe increase the radius.
[14:49] So all I'm doing here is just adding in some of that ambient occlusion information and I'm generating it from all this height information that I've been working with.
[14:57] And once again, once we get this height information, something else we can do is if we take a look at our normal, we don't have any normal right now, right?
[15:06] We're just working with height.
[15:08] And you know, that's fine.
[15:10] I could, you know, do this and export out a test related mesh and it'd be great.
[15:14] Maybe I want to export out the mesh, but then also have a normal that's going to give me some detail on top of it.
[15:19] So how do we generate that based on this layer stack that we're building up for this material?


### Using Height to Normal [15:24]
**Transcript (timestamped):**
[15:24] Well, here in our filters, we have another option here called height to normal.
[15:28] This works pretty well.
[15:29] So I'm going to take this guy, drag and drop again, filter placing it here at the top.
[15:34] And now we're starting to get some height information.
[15:37] The problem is, is it's just like I had shown you before in our shader is, you know, we're seeing some normal information here that's being generated.
[15:43] You know, in the shader itself.
[15:45] And now we're generating a normal information on top of that, which you can see here now we have this normal channel.
[15:51] So we're kind of getting this double intensity value.
[15:54] So I do have real world or use world units on this.
[15:58] So here we can say, you know, do we want to overwrite the existing normal mean for these that that's inside the normal data in here?
[16:05] For example, if I had normal data enabled on this channel, we could override it.
[16:09] We turned everything off so we don't have to use worry about it.
[16:11] So here I'm going to set my centimeter signs to 400.
[16:16] And then I'm just going to play with that height depth.
[16:19] So here I could actually set this to, you know, 9.65.
[16:23] And that's going to give me a pretty accurate normal in terms of making sure that it matches the physical size of everything that I'm doing here.
[16:31] And that looks pretty good.
[16:32] I might just, you know, bring the value down slightly again, just kind of art directing this just, you know, what looks good for right now.
[16:38] I'm not having to, you know, match anything specific.
[16:41] I'm just kind of reform creating this as I go.
[16:44] So now I have that normal channel information and it's at the top of my layer stack.
[16:48] So anything I do below it is going to feed into this new normal map I'm creating.
[16:52] So we've got our, we've got our ambient occlusion and our normal data.
[16:56] Now, like I said, one of the next things I want to do is layer in another material.


### Adding additional materials [17:00]
**Transcript (timestamped):**
[17:01] So here I have this pathway debris.
[17:04] I got this from substance 3D assets, sent it in using the creative cloud desktop app, just like I did previously.
[17:10] So let's take this guy, drag and drop and place him now in the layer stack.
[17:15] And you can see that we're starting to get something happening happening here.
[17:20] It looks terrible, right?
[17:22] So the problem is, you know, a couple of things.
[17:25] First off, it's the way the blending mode is affecting everything on individual channels.
[17:31] So for example, I know we're working with height.
[17:33] So if we go to height, the blending mode is set to like this ad mode.
[17:37] So it's taking the height information that's below the layer, this stuff, and it's blending it with the height information that's in the layer.
[17:44] And this is what we get, just kind of a mess.
[17:46] Also, this material has not been set correctly in its physical size.
[17:53] So first things first, I already have the height information channel toggle set to height.
[17:58] So let's change this blending mode.
[17:59] I want to overwrite to go to normal.
[18:01] We don't see anything.
[18:02] And that is because my height information is off.
[18:05] So let's turn that on.
[18:06] Now we are overriding the information and we see these rocks.
[18:10] This is what I want.
[18:11] Let's turn off here, the AO.
[18:14] Let's turn off the normal.
[18:15] You can see it's having zero effect because my height to normal is overriding any existing normals.
[18:20] But that's okay.
[18:21] We're just turning it off.
[18:22] Now, what we want to do is you can see that we're actually getting some displacement here with this too, because of the way we set up our shader,
[18:30] which is pretty cool.
[18:31] So now what I'm going to do here is come into my Rockway debris here.
[18:38] And I'm going to start to play with the normal.
[18:41] There's lots of ways you could do this, right?
[18:43] So I could look at the material properties and there's a bunch of properties in here for height position.
[18:48] All substance materials have these technical parameters.
[18:51] So I could even come down and play with things like the height, range and position here as well.
[18:57] But I'm not going to do that.
[18:58] It's just, I don't want to dig around and all this stuff.
[19:00] So what I like to do is with the layer selected, I'll just throw levels on this and then set the affected channel here to height.
[19:07] And now I can just play with the histogram.
[19:09] So let's do this.
[19:10] Let's go in and take this input white and just push it up.
[19:14] So now you can see we're really starting to get some nice displacement in here.
[19:17] That's looking pretty good.
[19:19] Happy with that.
[19:20] Also, as you can see, because we already have our normal in place, so you can see it's generating the normal and it's generating the normal.
[19:27] And it's generating that ambient occlusion information.
[19:30] So I'm just toggling those layers on and off.
[19:33] Now what I can do is I can also play around.
[19:36] This is kind of like my height position here.
[19:39] And so I can play with this stuff here in just a bit.
[19:42] Okay, now here's what we want to do.
[19:44] We want to blend these two materials together, right?
[19:47] So, oh, you know what?
[19:48] Before we even do that, we need to set our physical size.
[19:51] I almost forgot to do that.
[19:52] So let's come over to our properties just like we did before.
[19:55] We're going to try to planar this guy and for scale, we're going to physical size and boom, it's set.
[20:00] Now, one of the things that it's way too intense right now because we've set, you know, we're basically tiling this guy.
[20:07] And now all I need to do is go back to that height information, just readjust based on that tile.
[20:13] Okay, so I'm just making some tweaks here.
[20:16] Let's do that and that.
[20:18] Okay, so that looks like that's going to work.
[20:21] So how do we blend these guys together?
[20:23] I mean, lots of things you could do.
[20:25] You could, I could keep playing around with this levels until I try to get some type of blend happening in here between these layers.
[20:31] It doesn't look good though.
[20:32] I could mask this layer and just paint it if I wanted to.
[20:35] But the best way to do this is to, with the layer selected, come over here to my masking options and I'm just going to use this add my, add mask, excuse me, add mask with height combination.


### Blending Materials using compare mask [20:41]
**Transcript (timestamped):**
[20:46] And as soon as I do that, I'm getting a really nice blend already because we're using our good old friend compare mask.
[20:53] So I covered this in a, in a earlier video when I was talking about using compare mask with anchor points.
[20:58] But here compare mask and is going to allow me to compare my channel information, which is height, and we're comparing it to this layer, which is showing in green versus the layers below it.
[21:10] And you can barely see them, but it's like this bluish purple back here.
[21:13] And where these two layers overlap based on the compare operand.
[21:17] So in my case here, it's greater than you get this time turquoise blue.
[21:21] And that is what's generating for me.
[21:23] I'll left click on the mask.
[21:25] We can see it.
[21:26] This mask.
[21:27] So that turquoise range in my histogram is what is the mask is being generated by the mask.
[21:32] And I have this little hardness value here as well that we can tweak.
[21:35] Okay.
[21:36] So now that we have this in place, what's interesting is we go back to our levels now, watch this.
[21:42] We can now come in and I can start to play around here with my, my value here.
[21:47] Let's zoom in really close.
[21:48] Look at this.
[21:49] You can make this rock.
[21:50] You can just sink it right down into the surface like this.
[21:52] This is like an interactive blending control here.
[21:55] This is really nice.
[21:56] So we can, you know, sink this guy into here.
[21:58] I can even push these guys up and down by using my input white.
[22:02] And then I can adjust the overall range by using my output black and my output white if I need to.
[22:09] So we'll do something like that.
[22:10] And now I'm getting a really nice blend all based on height information here in my layer.
[22:15] And this really helps to kind of just break up everything that I'm working with here.
[22:20] So again, we could just play with these values.
[22:23] And, you know, something I could do because I was working with physical size on this, you know, there's so many neat tweaks you could do.
[22:31] I could, you know, change the way this is actually tiling.
[22:35] So I could set this at a custom size.
[22:37] Let's unlock this and then set this to like, you know, 140.
[22:41] Whoops, hit the tab key there. 140.
[22:45] And, you know, I could just kind of play with these guys.
[22:49] Maybe I want to make this, let's do this.
[22:51] Let's make this like 200 and hit 200.
[22:55] And that just makes the rocks a little bit bigger.
[22:57] So again, like I said, I'm just kind of art directing this now, you know, maybe I'll go with this route instead.
[23:03] So it's just, you know, taking what was physically accurate and then now tweaking a little bit.
[23:08] Maybe it's not, you know, totally accurate, but it's maybe more in line of what I want to do, right?
[23:13] Just from a creative perspective.
[23:15] I like this better.
[23:16] So that takes care of the rock in this particular case.
[23:20] Now, something else I can do right now, this is all just using compare mask and levels adjustments.
[23:26] And every kind of level adjustment I do, it's being fed through the compare mask and creating the blend for me.
[23:31] So the compare mask is doing all the heavy lifting, which is really nice.
[23:35] Now we can get into maybe tweaking this a little bit more.
[23:38] So with the layer selected, come over here to our add effect and I'm going to add a paint.


### Adjusting height with Paint Effect [23:39]
**Transcript (timestamped):**
[23:42] Now for the paint on the material, I can just paint hide information, right?
[23:46] And let's say we paint some, let's increase the hide information.
[23:50] So we're above one, I have my paint brush here and I start to paint.
[23:54] Now I can go in and just fine tune and paint areas that I want to raise and lower.
[23:59] So here we could drop this guy down and I could go in and just, you know, paint this stuff out.
[24:03] And it's all depending on the height levels, right?
[24:06] So I'm painting here and look, I can't go below because of the height level.
[24:09] But if I really want to push that rock down, I have to decrease the hide information.
[24:13] I have to make sure that it is lower than or less than because our operand is greater than.
[24:18] I have to make sure it's greater than this layer.
[24:20] I'm sorry, you have to make sure that it's less than this layer.
[24:23] And that's what we're doing here with our paints.
[24:25] We go in and we paint and now look, I could actually sink that down into the surface.
[24:28] And just push it all the way into here.
[24:31] And now you can go in and really fine tune this stuff.
[24:34] This is where we can have a lot of fun and go in and just kind of paint some of this information here.
[24:38] Look, we can just sink this kind of rock away, just shape it in and, you know, do whatever we want here.
[24:43] And then again, we'll push this back out and then we can go in and paint.
[24:47] And here we can lessen that amount.
[24:50] Just keep playing with it.
[24:53] And there we go.
[24:54] So pretty cool.
[24:55] And that's how we can use a paint on top of it.
[24:57] So at this point, I'm going in and just manually painting and getting things just like I want them to be here in my scene.
[25:05] So there we go.
[25:06] That's how we can use the levels adjustment.
[25:08] We can use paint on top of it to really fine tune that overall result.
[25:12] Now I can also see that I don't think my color values are matching very well.


### Adjusting Color with Substance Parameters [25:13]
**Transcript (timestamped):**
[25:16] Let's fix that really quick because I'm using a substance material.
[25:20] It's going to be super easy.
[25:21] So we select the material and within the material I have, well, all these color values.
[25:26] So I'm just going to use the color pick tool or the sample color tool and sample the color and then just choose something from the background.
[25:35] And here we'll try this and you can see as soon as I do that, it just changes my rock color value.
[25:39] Now we're starting to get something that looks like it's matching a little bit more because we're actually sampling the information from our background and applying it to the foreground.
[25:48] So pretty, pretty fun there.
[25:50] Let's go in and select another color.
[25:52] See what that does.
[25:53] I don't really like that.
[25:55] Again, you can tweak this all day long.
[25:58] Let's see what this does.
[26:00] Okay, that's not good at all.
[26:02] So we'll undo it.
[26:03] I think just that our first color change is going to be enough for me.
[26:06] So there we go.
[26:07] Got that in place.
[26:08] And you can see we have our displacement and everything for these rocks.
[26:12] Okay, so next thing we could do, let's just to further improve this overall effect here.
[26:19] We could start to add maybe another layer on top of this, like a dirt pass that basically helps to kind of consolidate my surfaces together, really help to bring them together.
[26:30] Just so it's just something that unifies the two materials as they're kind of blending together here.
[26:36] So to do that, we are going to create a fill layer and I'm going to call this dirt.
[26:42] And for the properties, let's see here, I'm going to do something crazy.
[26:48] We're going to do like this red so you can see it.
[26:50] And then we're going to increase our roughness value.
[26:53] And of course, we need to mask this.
[26:55] So we're going to create a black mask.
[26:57] And with the mask selected, I'll grab a generator.
[27:01] And for my generator, I'm going to use this dirt generator.
[27:04] And so already you can see if we move our dirt level up and down, we're starting to get something here, right?
[27:08] Now the problem is this dirt generator works based on specific image inputs.
[27:13] And we don't have anything baked about this model.
[27:16] Like I have no curvature.
[27:17] I have no ambient inclusion.
[27:18] I don't have any of this stuff.
[27:19] So it's not really working.
[27:20] It's just throwing a noise over top of everything.
[27:22] So the question becomes, what do I do?
[27:24] How do I get my information that I've been working with and building up in this layer stack?
[27:30] How do I get it here into this dirt generator?
[27:32] And the answer to that is going to be with our amazing anchor system, which works super, super well.
[27:39] So what I'm going to do here is let me think about this.
[27:43] Where could we do this?
[27:44] Let's here, if I put my dirt on top of this guy, I think that'll work.
[27:48] Let's come into here where we have this height to normal.
[27:51] And I am going to just click my effect tool and add an anchor point in here where it says height to normal.
[27:58] And then what I can do, let's turn on the dirt.
[28:01] Let's go into the dirt generator.
[28:02] I turned on the dirt material.
[28:04] And for the image inputs, I'm going to come down to where I have this section here called micro height and micro normal.
[28:10] Well, I have normal information that I want to use.
[28:13] So I'll click the normal.
[28:15] I'll come over here to anchor points and choose height to normal.
[28:18] And then for the reference channel, I'll set this to be normal.
[28:22] Okay. So we got that set up.
[28:24] Now I can come over to the detail section itself and just enable the control.
[28:28] And so when I do that, I start to get some information here and it's now working.
[28:33] So here, if you come in and you see that if I turn this micro normal off and on, now the dirt is starting to show up in some of these kind of occluded areas.
[28:42] So for example, if I play around with this, let's take our dirt level and just increase it slightly.
[28:47] And now you can see that it's really starting to show up in some of these occluded areas in between all the rocks and everything.
[28:53] And that's precisely what I want to do.
[28:55] And I can decrease that dirt contrast or increase it, play around with that grunge amount.
[29:01] Let's decrease that down.
[29:04] And let's see here, let's increase that, you know, it's just a matter of tweaking it here and maybe even increase that grunge scale.
[29:11] See what that does.
[29:13] Maybe it might put too much of a pattern noise on what I want to do here.
[29:17] All right. So, okay, this red is not going to work anymore.
[29:20] So now we're just going to create your let's all I like to always sample something from my background and then tweak it afterwards.
[29:27] So we get something that's coming from the from the actual world itself.
[29:31] And so here, you know, let's just get a color.
[29:35] And then it's a matter of going in and just tweaking and playing around with it.
[29:39] So we can increase this guy.
[29:41] We lower that down.
[29:45] I can even change the blending mode on this. What would that do?
[29:48] So we set that to normal.
[29:51] Maybe that'll work.
[29:54] Let's do this, increase the grunge amount.
[29:57] Okay, I'm just going to leave it at normal.
[29:59] It kind of darkened things a bit.
[30:00] So now I just back it off kind of like feather it with the layer opacity here.
[30:04] We'll do something like that.
[30:05] And it's subtle, right?
[30:07] It's like not a big deal if we turn it on and off.
[30:09] I mean, can we really notice it's just enough to help unify my two materials together?
[30:13] I always like to do it like, we'll call it a unification pass of that.
[30:18] Okay, so looking at this guy, we're pretty much done.
[30:22] But you know, if I zoom out, I can, you know what, I've got some repeating stuff here, right?
[30:26] So maybe maybe I want to tweak and play around with that.
[30:29] So a couple of things I could do is maybe take my tiling fix and drag it up above my two layers.
[30:34] So if I do that, you can see that it automatically is adjusting where I did that tiling before.
[30:40] And so maybe I want to go with that route.
[30:42] But while I'm here, I'm going to grab my clone tool and, you know, some of these rocks, I'm not really liking too much.
[30:50] So I'm going to hit my V key and this guy here, I'm just going to clone that guy out.
[30:54] So we'll get ready him.
[30:56] And let's do the same thing over here.
[30:58] Let's get rid of that guy.
[31:01] And this guy's, he's giving me issues. I don't like him.
[31:04] Let's do that.
[31:05] All right.
[31:06] Oh, yep.
[31:07] Let's get rid of him too.
[31:09] There we go.
[31:10] All right.
[31:11] So, you know, we still have these four in the corner.
[31:12] So I could change them.
[31:14] I could do something like that, I guess, if I want to.
[31:17] They're kind of sticking out a bit.
[31:19] Just a matter of tweaking them slightly.
[31:22] Take that guy.
[31:24] All right.
[31:25] That should work.
[31:26] That's good enough.
[31:27] All right.
[31:28] So this, this clone layer that we did, and because we set up the past path through,
[31:32] excuse me, pass through blending modes, it's all going to work.
[31:35] We can move it up and down the layer stack.
[31:37] That works pretty good.
[31:39] All right.
[31:40] So there is my brush.
[31:41] There's everything set up.
[31:42] Let's see.
[31:43] Can I think of anything else?
[31:44] I think that is going to work for what I want to do.
[31:47] Okay.
[31:48] Awesome.
[31:49] So right here at this point, I'm kind of at a spot where, you know, I'd really like to
[31:53] check this down.
[31:54] Let's do some rendering on it.
[31:55] So this is, like I said, this is being tiled.
[31:57] So it's basically a two by two tile based on the physical size of those materials on
[32:03] a single four meter plane.
[32:05] And I could go ahead and test this in a render.
[32:08] So a really quick way to do that is to use Stager.


### Rendering with Stager [32:10]
**Transcript (timestamped):**
[32:11] So here I'm going to do file send to substance three Stager, and that's going to open up
[32:16] Stager, and it's going to bring my plane in.
[32:18] It's going to have displacements.
[32:19] It's going to have everything hooked up for me.
[32:21] I'm just going to have to do a slight little tweak to it here in a second.
[32:25] And let's see here.
[32:26] We'll see this is coming in.
[32:28] Zoom out.
[32:29] There's my plane.
[32:30] So like I said, we need to do a slight little tweak here.
[32:33] The plane selected, I'm looking at my object.
[32:36] Displacement's on, but the tessellation mode is really low, right?
[32:40] So the total face budget, it's at 10,000.
[32:43] I'm going to do like two million, I think.
[32:47] So we'll do something like this.
[32:49] And it's going to take just a second to subdivide that up, and now it's done.
[32:53] So that's going to give me a pretty good idea.
[32:55] So let's turn on, actually, before we do the ray tracing, the environment, I think,
[32:59] is just some basic studio light.
[33:01] So let's jump over here to my lighting, and let's scroll down to my environment lights.
[33:05] And there is this panoramic.
[33:07] I like to use this one.
[33:08] It's exactly what I was using in Painter.
[33:10] So I'll click it once.
[33:11] That's going to apply it.
[33:13] And let's turn on ray tracing so we can do a render preview.
[33:16] And here we go.
[33:18] So now we can start to look at what this looks like.
[33:20] And here in my environment, I have the ground is on.
[33:25] So that's kind of neat because if I sync that piece, remember, I told you how the edges kind of slope downwards to like the zero of the grid.
[33:33] Now, if I push those under the grid, that kind of shows how the object is going to be broken up around the edges like this.
[33:40] So that's really interesting.
[33:42] And then what I could do is just quickly, you know, let's create a camera.
[33:45] Let's grab this guy.
[33:46] Let's hit Control D to duplicate it.
[33:48] We'll take just a second here to duplicate that.
[33:51] Now I can grab the mesh.
[33:52] I'm doing all this, as you can see, just working as I'm doing a real time ray trace.
[33:58] Stagers render is actually pretty fast.
[34:00] Look at like, you can see this geometry where it's intersecting because the details are so intense.
[34:06] It's like impossible to see.
[34:07] It's so much noise.
[34:09] They hear, look, you can see where they're overlapping.
[34:11] I move my mouse out of the way and boom, it's really hard to see like where these guys are actually intersecting here.
[34:18] So we're going to set this up.
[34:20] Let's get a little shot in place, maybe something like this.
[34:23] I'm going to move my light.
[34:26] Okay, let's grab the environment intensity here to this guy.
[34:30] Where's my light intensity?
[34:32] Maybe set it to like, I don't know, 200.
[34:35] Let's see hit Enter.
[34:37] That's probably too much.
[34:40] I'll do 125.
[34:44] Okay.
[34:45] So like I said, just going to set up a shot really quick.
[34:47] You can see what I'm doing.
[34:49] This guy in place.
[34:51] And then I got my camera.
[34:54] Let's turn on some depth of field and a focus point here.
[34:57] Blur that guy up.
[35:01] Zoom in focus again on a certain area.
[35:04] Looks pretty cool, you know, so pretty neat, quick way to get a really neat little render of my scene just using Stager.
[35:10] You can see it's perfect for these testing for this testing that I'm doing here.
[35:14] So our focus point here.
[35:16] And there we go.
[35:18] So, oh, there's one other thing I want to show you guys here in Painter that you'll run into when we're looking at the overall kind of displacement of this.
[35:25] So we'll set our focal point here.
[35:28] Our lights.
[35:31] I'm just lighting this with just an environment light, but I could also just throw in like a directional light as well if I want to.
[35:37] But here's just just to give you an idea of some of the, of what we're looking at here.
[35:40] And that's just, you know, complete displaced geometry, but it's a little chunky over in these areas like this.
[35:45] So here's something I want to show that's pretty cool.
[35:48] So here back in Substance Painter, I'm going to show you just another technique.


### Fixing jagged edges in displacement [35:50]
**Transcript (timestamped):**
[35:52] So when we look at our rock where we're displacing everything, we just displaced everything just vertically straight up, right?
[35:57] And so what we get when we really look at this close, things start to fall apart pretty easily because we get all these jagged edges and stretching and it just isn't awesome, right?
[36:06] And, you know, that's what I would expect.
[36:08] I mean, it's not doing anything that's like, okay, yeah, you know, it's, it is what it is, right?
[36:13] It's doing what I would expect it to do.
[36:15] But there's some other kind of cool ways that we could fix this in Painter for some of these real troublesome areas.
[36:21] And let's take a look at that.
[36:22] So what I'm going to do is I am going to create another layer and we're going to call this smoothing.
[36:27] And what I'm going to do is come over here to my layers, I'm sorry, my toolbox, and I'm going to grab this smudge tool.
[36:36] And this is kind of, kind of work like a blur, right?
[36:39] But it's my smudge tool.
[36:40] I believe, unless it's been removed, let me see, we do have a blur tool in here.
[36:45] Oh, go in.
[36:46] Yep, we do have a blur brush too.
[36:48] This could work.
[36:49] I haven't tried this one.
[36:50] Let me try the smudge brush first.
[36:52] But we're going to go to smoothing, right?
[36:53] And I have the smudge.
[36:54] So what I'm going to do is I'm going to set my, my actual values that I want to pass through.
[37:01] So just like we did with the clone, I want to smudge some of the channel information.
[37:06] And really what I'm looking at here is probably just my height, right?
[37:10] So let's come over here to my material and let's try just the height information.
[37:14] And we're going to look at the height.
[37:17] We're going to grab a pass through on this so that we're pulling all that information.
[37:21] You can see that the thumbnail shows me what's being passed through to it.
[37:24] And now I can come over here with my brush and here you can see, again, we got this like real jaggedy stuff happening.
[37:31] And I can just click and drag and just smooth that guy right out.
[37:34] So again, it can get intense quick, but you're just, you know, just slight little tweak here and it really fixes this.
[37:41] Let's come over to this area right here.
[37:42] This is where this is pretty troublesome, right?
[37:44] And we're just going to click and drag, click and drag, just smooth it a little bit on the edge like that.
[37:49] There we go.
[37:50] Pretty cool.
[37:51] So again, it softens it, but it kind of helps with some of those, you know, chunky areas.
[37:57] And so this is something we can go in and use just to kind of fix some of those problems.
[38:01] So we'll just go in and just blur that slightly around on the edge, lower my brush, blur that edge a little bit like this.
[38:07] Just on some of these areas that I think are really going to stick out or going to be a problem spot.
[38:12] Some of the small ones, it really did a great job here.
[38:14] Some of these small rocks I really don't need to worry about, but I'm just showing you this just so you have the idea of the technique.
[38:20] And you can see it works pretty well.
[38:22] You just got to be careful because you can kind of really over blur things.
[38:25] But again, it works in a pinch, right?
[38:29] So we'll go in and scale this up, blur that guy down.
[38:34] It really helps to just stop that, you know, it just gives a little bit of a slope to that overall rock.
[38:41] So here I might just look at that.
[38:43] That's really nice.
[38:44] I can go in and just blur that rock out.
[38:46] Here's another example here.
[38:48] It's kind of fun using this tool.
[38:50] I mean, I'm going to stop because I'm going to keep doing it.
[38:52] But there we go.
[38:53] So we can just use the smudge tool to blur and fix that.
[38:56] Okay, so now that we've done that, something else we could do, you know, I just keep adding stuff, right?
[39:01] I keep thinking of these ideas.
[39:03] We could in our filters come over here and we do have a sharpen.
[39:07] Maybe this would help, right?
[39:09] So we can throw a sharpen in after it's going to be a little aggressive at first, and then we can just lower this down.
[39:15] So here it is without the sharpen, things are a little blurry.
[39:17] And then we can just sharpen our texture up slightly like this.
[39:20] Okay.
[39:21] Now, don't forget before you send this over to Stager, if you want to do a rendering,
[39:26] what you need to do is just come over here to your texture set settings.
[39:29] And I need to set this to 4K because remember, we're going to get more detail as soon as we set this to 4K resolution.
[39:35] And you can see this is computing now.
[39:37] And I sent everything and everything I was rendering was done in 2K.
[39:41] So I'm just going to let Painter go ahead and do this, compute this 4K image.
[39:45] And there we go.
[39:46] That's looking even more sharp and crisp.
[39:48] And that little blur that I was doing is now really not so bad.
[39:52] And let's see, I should be able to work pretty well here in this 4K mode.
[39:57] Let's see.
[39:58] Sometimes when you're painting in 4K with displacement, yeah, see, it's not really real time in a sense.
[40:04] So it takes a little bit of a tweak there, but, you know, I can kind of get it.
[40:07] But that's why you work in 2K.
[40:09] And then you pass it up to 4K when you're on render.
[40:11] But yeah, that's doing a great job now that I look at it in 4K.
[40:15] So we've talked about being able to render this with a displacement map.
[40:19] But now I'd like to export this mesh so that I could use this as a Nanite mesh inside of Unreal Engine 5.


### Export Nanite Mesh for UE5 [40:22]
**Transcript (timestamped):**
[40:25] So let's take a look at that process.
[40:27] So here I could go to File.
[40:29] I'm finished with all my texturing, right?
[40:31] I could export mesh.
[40:32] And now we have this option here to export with displacement and tessellation.
[40:38] This is awesome, especially if you're using something like Unreal Engine and you want to make this into a Nanite mesh.
[40:43] This is perfect.
[40:44] This is really good.
[40:45] So with displacement and tessellation, now I am going to turn off, uh, recompute vertex normals.
[40:52] Because what that's going to do is I'm going to export the geometry without the vertex normals.
[40:56] And I'm going to rely on the normal map.
[41:00] So again, our normal map that we've created, we're going to rely on this to give us the details.
[41:05] Now, if we had vertex normals on the mesh and applied the normal map, we would get that double normal, uh, situation that I kind of explained to you
[41:12] what's happening here inside of Painter.
[41:14] So again, we could do File, Export, Mesh, with tessellat- excuse me, with displacement and tessellation, turn off Compute Vertex Normals,
[41:22] and I'm going to export this.
[41:26] So here I'm using Unreal Engine 5.
[41:28] I have just a basic template scene open just from New Level.
[41:32] And I'm going to import that mesh that I just exported from Substance Painter.
[41:36] So here I'm going to import, and I'm going to choose this ground four meter high.
[41:41] Again, this is exactly what I just exported from Painter.
[41:44] So we'll click Open.
[41:46] And once this comes in here, we're going to make sure that Build Nanite is enabled.
[41:51] And everything else should work.
[41:53] This is already appropriately scaled.
[41:55] So you can see my import uniform scale is set to one, and I should be good to go.
[42:00] So let's go ahead and just put import, excuse me, click, Import All.
[42:05] And this is going to import the mesh and build this as a Nanite mesh.
[42:12] All right, so now I have my mesh.
[42:15] We'll just click and drag, place this here into the world.
[42:18] And I'm just going to zero out the location.
[42:21] And here's the mesh.
[42:22] And as you can see, because I did not export this mesh with Vertex Normals,
[42:28] it looks a little strange here.
[42:29] But that's OK because our normal map that we're exporting from Painter is going to take care of that normal information for me.
[42:35] And speaking of, let's jump back over to Substance Painter.
[42:38] Let me show you how I export the textures.
[42:41] So here I'm in Substance Painter.
[42:42] I just do export textures, and I'm just using a default output template.
[42:46] So if I just drop down here, you can see there's all these options.
[42:49] And what I go with here is just going to be this version called Unreal Engine 4 Packed.
[42:55] And so with that said, let me export these textures.
[42:57] We'll jump back to Unreal and let's create our material.
[43:01] So now let's import the texture maps.
[43:04] You can see that I have my base color, my normal, and that packed map.
[43:07] It's going to be RGB where red is going to be my occlusion.
[43:11] The green channel is my roughness, and the blue channel is my metallic,
[43:14] which I don't have to worry about in this case.
[43:16] So let's select these guys and click Open.
[43:18] It's going to import all the textures.
[43:20] And my normal map should be set for me automatically.
[43:23] But let's go ahead and just double click here, this packed map.
[43:26] And I'm going to make sure that the sRGB flag is disabled, and then I'll click Save.
[43:32] And that's going to take care of the setup.
[43:34] You can see that I did export these guys out at 496 or 4K.
[43:38] And so now we're going to right click, and we're going to create a material.
[43:42] And I will just call this Ground for now.
[43:46] And let's go ahead and open up the material and start playing around here with our maps.
[43:51] So I'm going to grab all three of my maps and just drag those here into my material.
[43:57] Let's plug in our base color, and let's plug in our normal.
[44:02] And see if we get our normal in here.
[44:04] And then like I said, this map here is packed with some information.
[44:08] So for example, the red channel is going to be my ambient occlusion.
[44:12] So we'll plug this guy into here.
[44:14] And the green is going to be my roughness.
[44:16] And then like I said, the blue is metallic.
[44:18] We don't need that for the ground.
[44:20] Now, something else I like to do sometimes here when it comes to specular,
[44:24] especially for like ground surfaces, is I might lower the specular value just a little bit.
[44:28] So let me try something like this.
[44:30] I'm just going to create a constant here.
[44:32] And we'll plug this into specular and then maybe give this a slightly lower value.
[44:37] So I'm going to try something like 0.35.
[44:40] And that should do it.
[44:41] We'll hit Save.
[44:42] And we'll save this material.
[44:44] And then I just need to apply it to my ground.
[44:46] So now I have my material left click, drag and drop it to the ground.
[44:52] And there we go.
[44:53] We have our material and it's looking quite awesome.
[44:56] I'm super happy with this.
[44:57] Let's just kind of look around and see what we get.
[45:00] Pretty cool.
[45:01] So now that this guy is in place, what we can do now is just start kind of playing around
[45:06] by just kind of kit bashing our asset together.
[45:09] So we'll hit Control-D. Let's just move this around.
[45:12] You can see now I can just start moving these pieces in.
[45:15] And because, again, all of this crazy amounts of detail that we're getting because of Nanite,
[45:20] you know, you don't see seams at all with this.
[45:23] So it's quite awesome.
[45:24] Let's scale this up and down and whatever we need to do.
[45:28] So here I'm just going to duplicate this a few times across the environment.
[45:32] We get something like this.
[45:34] And there we go.
[45:35] Now we have this really nice ground.
[45:37] And again, because we're duplicating and just kind of kit bashing these areas together,
[45:41] we can really also start to hide some of that, you know, noticeable tiling patterns.
[45:46] We also just play with my lighting here a little bit.
[45:49] So we'll hit Control-L and just make a slight little lighting adjustment.
[45:53] Maybe something like that.
[45:55] Yeah, that's looking pretty cool.
[45:57] And there we go.
[45:59] There is our ground.
[46:01] Here you can see an example where I have the two ground tiles that just snapped them together
[46:05] so that you can see that the texture we did create is seamless.
[46:09] So that's going to conclude this video on how we can use Substance Painter to create tileable materials and meshes.
[46:15] Thanks a lot for watching and I'll see you next time.



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
