---
title: Tips & Tricks in Substance 3D Painter to Make Semi-Realistic Textures | Adobe Substance 3D
source: YouTube
url: https://www.youtube.com/watch?v=ng-Wb7RaYHU
author: Adobe Substance 3D
ingested: 2026-08-13
app: "[PENDING]"
version: "[PENDING]"
tags: []
extraction_status: pending
frames_dir: tutorials/frames/tips-tricks-in-substance-3d-painter-to-make-semi-realistic-textures-adobe-substa/
frame_count: 0
frame_status: pending-selection
---

# Tips & Tricks in Substance 3D Painter to Make Semi-Realistic Textures | Adobe Substance 3D

**Source:** [YouTube](https://www.youtube.com/watch?v=ng-Wb7RaYHU)
**Author:** Adobe Substance 3D
**Duration:** 42m31s | 1 section(s)

---

## Raw Data (for Claude Code extraction)

Frames are not captured yet. Read the timestamped transcript below, pick moments
that actually show a technique/result worth a still (not blind percentages —
even within a named chapter, verify the real moment against its timestamps), then run:
  python select_frames.py tips-tricks-in-substance-3d-painter-to-make-semi-realistic-textures-adobe-substa <ts1> <ts2> ...
(seconds or mm:ss). This appends a "Captured Frames" section and updates the
frontmatter before you write the Structured Notes below.


### Full Content [0:00]
**Transcript (timestamped):**
[0:00] Hello everyone! And as I was already introduced, my name is Anna, I'm from Ukraine, and today
[0:14] we're going to talk about tips and tricks on making semi-realistic skin, and my speech
[0:20] is going to be divided in two parts. In the first part, there is going to be a presentation,
[0:26] and in the second part, I will open Substance Painter, and I will show you all the layers,
[0:31] all the masks which are used to create the semi-realistic skin. But before we start, I
[0:37] wanted to tell several words about myself, and I started being a 3D artist since 2014,
[0:45] and I specialize in creating stylized characters of full cycle pipeline. I mean, I start making
[0:52] characters in that brush from Sculpting, and I finish them rendering. Rendering is not
[0:58] like the part of a working pipeline. If we are talking about the working pipeline, I
[1:03] finish making characters in Substance Painter after texturing. I have 10 years of experience,
[1:09] and I had luck to work for such projects and for such companies as Blizzard, Riot Games,
[1:15] Starships Indicate, and others. And also right now, I'm an official streamer at the
[1:21] Brushleaf, and I have two YouTube channels. One of them is in English, which is a new
[1:27] signature art, and there you can find actually the full video of making of the cyberpongal.
[1:32] And the second channel which I have is GameDev from Girl, and it is in Ukrainian. And right
[1:40] now, about this project. That project was like quite a challenge for me. I wanted to try to do
[1:48] something what I've never did before, and this project is the first work without a concept. We
[1:55] know that to be a concept artist, it is a separate special profession, and we need to spend several
[2:01] years to learn to be a concept artist, and that's why being a 3D artist, it is very difficult to
[2:07] create something, to understand the forms, to understand the lines, and to understand the colors.
[2:14] But I decided to challenge myself. That's why it is the only character in my portfolio which is
[2:19] created without a concept. Also, I specialize in GameDev characters, but this time I wanted to try
[2:27] Xgen hair and Arnold render, which as you know, it is part of pipeline for cinematics, for ketunes,
[2:34] so that was also quite a challenge for me. And of course, I was inspired by the game cyberpong.
[2:40] I started making this character when this game was released, and I think I looked through all
[2:46] available pictures of cyberpunk on artstation and decided to do something from myself. And the most
[2:55] funny, I think, fact about this project is that previously I had cyberpunk project at work, but
[3:03] that was under NDA, and for that project we created material in Substance Painter, this glittering
[3:11] jacket, and I loved it so much, and I wanted to post it in my portfolio, but the project was under NDA.
[3:18] That's why I just promised myself that I will make a project where I will use this material,
[3:23] because I just wanted to show this material. So this is how this work was born.
[3:30] And talking about the textures,
[3:35] I'm sorry, talking about the textures, I need to say several words that
[3:42] the all the textures here I fully made in Substance Painter. I didn't use any other
[3:48] softwares on the Substance Painter except of the hair. The hair, the color of the hair was done
[3:55] straight in Arnold. It's not kind of texturing, so I did not include the texturing here. And also
[4:03] I used PBR pipeline, but that PBR pipeline was like a combination between hand paint techniques and
[4:12] generative, generate procedural techniques, and this is why I like Substance Painter, because in
[4:19] this program you can combine both hand paint and procedural techniques in one, like in one project.
[4:26] And I want to say that creating textures is easier than it seems to be. I know that every
[4:32] time when we open Substance Painter and looking at our gray material, we just don't know what to do,
[4:39] and we have chaotic thoughts in our head, but if you make a structure, what should be done first,
[4:46] then second, then third, everything will become easier and I will prove it when I will go to my
[4:53] Substance Painter file, what the textures of the skin. And the types of skin which I used here are
[5:03] like the skin texture, the makeup texture, glittering texture, and glasses. And I also had here the
[5:12] material of metal, but I decided not to speak today about the metal material, because here
[5:18] everything is pretty straightforward, just a combination of two materials, and that's it,
[5:23] that's why I don't think that I need to stop explaining the metal material which I used.
[5:30] And talking about the skin, I used the technique of three skin layers. What does it mean? That
[5:38] means that all of us know that we have a sub-dermal layer, I created the sub-dermal layer, on top of
[5:44] it I created dermal layer, and on top of dermal layer I created just like kind of fixed layer where
[5:51] we have all scars or some details which we can add to our skin. And as I said before, the skin is
[5:58] created by the combination of procedural and hand paint approaches, and you will see that
[6:05] somewhere we really need to use our hand paint approaches. About the textures, for rendering,
[6:11] of course I used displacement, but for texturing I used normal map, I baked both these maps,
[6:18] but for texturing I used only normal maps. Also here I made the base color, that's obvious, right?
[6:26] I also painted roughness, which is also obvious, but instead of metallic layer I used the specular
[6:34] layer. Why? Because our skin is not metal, that's why the metallic map would be just one color,
[6:42] and that's not interesting. But when they're using a specular layer, so we can, by using specular layer,
[6:49] we can show the areas which can be more shiny, and that's why this map would be more informative
[6:57] than the metallic layer, that's why I decided to paint the specular map. Also you can see that on
[7:04] my character we have the makeup, and this makeup was created by a separate layer.
[7:09] Makeup texture. The makeup texture, as I said, was created as a separate layer, but the thing is that
[7:20] for the makeup in Arnold I used the layer material, that means that I combined two materials,
[7:29] and they mixed through the mask, which you can see here, the black and white mask,
[7:35] and I want to say that for the makeup I used only the base color, but you can see glittery
[7:41] effect here around her eyes, and this glittery effect was achieved only by a, I think it is,
[7:48] crystal note in Arnold, but it wasn't painted, however it is possible to make even a substance
[7:55] painter, but I didn't want to make like thousands of maps, that's why I made this effect in Arnold,
[8:03] but the color itself I painted in substance painter. Glittering jacket, that material, and
[8:13] the most like the tips and the biggest secret is that this material is made of car iridescent,
[8:21] iridescent, I'm not sure how to pronounce this word in English, it's not my native language,
[8:26] so sorry, but this is the material which I used for this jacket, it is like it was the base,
[8:34] and the color was painted just like another layer, but all this glittering effect is achieved
[8:41] only by this iridescent car material, car paint, and glass textures, that was also very interesting,
[8:50] I tried several ways how to make semi-transparent glasses and textures, but I ended up by creating
[8:58] the mesh of glasses, which is absolutely transparent, and inside of these glasses I inserted just a
[9:06] plane, and here you can see the map, that's like an alpha map, which I created in substance painter,
[9:16] and you can understand that the black parts are not visible and the white parts are visible,
[9:22] and the color again I applied in the Arnold, because as I said before I didn't want to just
[9:28] create thousands of maps, and I can say that all the ornaments on the glasses except of this one,
[9:36] which is actually is not visible from the front view, all the other ornaments are created by the
[9:45] standard alphas in substance painter, first of all I was thinking to find some special alphas
[9:52] somewhere in the internet or to create a photoshop, but then I ended up by just standard alphas
[9:59] from substance painter, because they were looking much better than all the previous variants,
[10:04] and right now I think it is time for us to go to substance painter, where I will show all the
[10:17] layers of the skin material, which I was talking about, so here we are, let's go to head, and I
[10:30] think here we need only three dv, and by now I will turn off all the layers,
[10:42] and I will turn in on them later, explaining each layer,
[10:53] it takes some time,
[11:00] and here we are, I think everybody knows that when we upload something to substance painter,
[11:17] our character will look this way, and then I as you see have a folder which is called
[11:25] subdermal layer, let's turn it on, and here we have three layers, the first layer is just
[11:33] very simple, it is just a base color, and it is red, because we all know that through the skin we
[11:39] can see like red parts on our faces, so right now it's just flat color, nothing special, but the next
[11:47] next layer is called redness, and here you can see that it is very irregular, and I have a lot of
[11:57] noise here, and how this noise was created, if I look here you will see that I use the generators,
[12:05] like I mean fill layers with noise, like clouds, and here you can see the names of the noise which
[12:13] I used here, and also here I used some hand paint to make veins,
[12:21] and also some hand paint techniques which I use just to make this area on the lips darker,
[12:28] because here our lips in reality look a little bit darker, and this is how it looks, and if you
[12:35] look in the base color you can see that it is pretty irregular, and the next layer is purple layer,
[12:43] everybody knows this purple layer when we sit in front of the computer for eight hours, and then we go to the
[12:48] mirror and we see round purple circles around our eyes, so yeah when you're creating a skin texture
[12:55] you need to remember about this, not a lot, but somewhere it should be, and this is what I call
[13:02] the sub dermal layer, and the next layer, like group of layers, is sub dermis, and then we go to our
[13:12] first layer, and this is skin layer, and before I will explain how I painted it, I want you to
[13:22] look through it and see that we have areas where the skin is, through this layer we see this somewhere
[13:31] purple, somewhere red areas, and how is it made, if we go here we will see that our mask it is not
[13:41] like fully white or fully black, it like semi-transparent, and how it was created, I used noisy brushes,
[13:52] and where we have assets, and if we go here to, on my computer it looks
[14:01] differently at home, I need to find here brushes, and the most popular brush which I use is a
[14:10] smooth brush, smooth noise brush, here it is, this brush I highly recommend for you to use if you
[14:17] want to receive this irregular looking of your textures, not just flat, and also for to make this
[14:27] figure kind of flakes, I used one of these brushes, it's like dirt, and something like that, and when
[14:37] you just start painting your texture with these brushes you receive areas which are not like
[14:46] covered by the color, and that's why this is how you can receive this irregular looking of the textures,
[14:57] and of course on top I have like kind of
[15:01] correction, correction layer, I mean in the end I realized that her purple eyes are very purple
[15:08] here, that's why I created another one, like correction here, and next layer in this dermis
[15:16] group of layers is sun damage, it is not really visible, but the main point about the textures
[15:24] is that you create things which are like not really visible, but when you have like 10 such
[15:32] things, 10 such layers, they make difference, and I think if we go to the base color
[15:43] you can see the sun damage is pretty visible here, and on here, just a second,
[15:52] yeah, and the mask here is looks this way, and again I have the generators which I used them,
[16:00] I sharpened them, and I just painted some areas where I don't want to see the sun damage,
[16:08] of course we need to have freckles, because a lot of people have freckles, and again if we go to the
[16:14] base color, they look this way, and in the freckles you can see that first of all I just painted them
[16:22] with one of these brushes, the name I don't remember, but I think you will find it's just not
[16:28] difficult brush here, I blurred them a little bit, and I used this filter warp, because our freckles
[16:39] they are not like perfect circles, and we need somehow to distort them, and of course I created
[16:48] bad heads, you can see what, let's again go to the base color, and you will see without bad heads,
[16:56] and with them, but again on our face it is not visible same everywhere, that's why we need to make
[17:05] a mask, and I used the curvature generator, and on top I used just a paint, and again everywhere
[17:15] here I'm using this smooth noise brush, when I need to wipe something out, and you can see that there
[17:22] are areas where these back heads are not visible, next one is here in the dermis layer is group with
[17:31] lips, and here we have just the base color, nothing special, and I have like two layers for the lips,
[17:42] the first one is darkness, let's look here, of course we have like a mask for the lips,
[17:49] and the mask for each layers, and here that was I used the thickness map to create this darkness,
[17:58] and also I used levels to make it more visible, so here we can see without darkness with darkness,
[18:06] and the lightness, of course we need lightness, and this lightness is going to be here in the middle,
[18:14] again here we have the curvature generator, and somewhere I painted I just removed this light,
[18:23] next one is redness, and when I say redness I mean these veins, I think you remember that
[18:35] when I was, let's go to the base material here, and now you can see veins here, and I just duplicated
[18:47] the layer from the subdermal layer, and I deleted everything what I had here in the mask
[18:57] except for veins, because I wanted to make these veins a little bit visible, that also brings more
[19:05] realism to our work, and the final layer I think it's just like kind of the makeup techniques,
[19:14] understand what I am talking about, I just know that on our face when we're making the makeup
[19:21] there are the areas which we try to make darker, because these things make our face looking better,
[19:30] and this is what I used to also to make my face looking more natural without it,
[19:40] and was it I think was it, it looks much better, and this is our dermal layer, next I created
[19:47] this specular layer, to create the specular layer first of all I work like in this just standard
[19:54] PBR, PBR, yeah the standard shader, and but to create specular layer I went to, let me remember
[20:08] where because I have different interface in my computer, I created another channel
[20:16] which is okay I will not search for it right now, I think you know you understand what I'm talking
[20:21] about, but I will show that, let's take this one, you can see that here I have specular layer,
[20:30] so I can go here to look at my specular layer the way it looks, and here we are specular layer,
[20:39] so let's turn it on, so first of all it was just a simple gray color, and on top of it I added the
[20:46] noise, and this noise consists of different generators, nothing special just I need to get
[20:54] this irregularity, and on top of it I have cavities, which I don't know why I can see,
[21:02] nothing is here almost, this is the way it looks, and after the specular layer there was another
[21:10] folder which is roughness, and let's go to roughness, in roughness map we have just the base color as
[21:20] usually, and we have the roughness looks pretty simple, but here we have the first I have lips
[21:29] because our lips always look more wet, that's why you need to make them look more wet,
[21:37] next layer was oiliness, because again our skin has this like fat, and that's why we can see this
[21:46] is the area where we have, we can see this oiliness, and just the back layer I just needed to wipe out
[21:53] here, nothing special, so in general the roughness looks this way, and this is, I can say that this
[22:06] is the final version of the skin itself, if you're interested I also have here the makeup,
[22:15] and the makeup, I have a photo makeup, I have for the group the mask, which is just looking this way,
[22:24] and this is how looks the makeup, only for to see how it's going to be looking like kind of
[22:34] in Arnold, I edit here the metallic, metallic channel, but in the end I didn't export
[22:45] metallic, only the base color, so here for the makeup it was so simple to do here, because I think
[22:52] as I said before textures are more simple than it seems for you to be when you just understand
[22:58] the structure, and here we have just the base color, on top of it we have an eyeliner, and to
[23:05] make them look a little bit more interesting I edit also here one more color, so the makeup consists
[23:12] only of three layers, this is the way it is done, and I think about this demonstration in substance
[23:19] painter we are done, and we can go back to the presentation, and so I think it's right now it
[23:34] is time for your questions, and I want to say if you want to follow me on my social networks you
[23:41] can scan the QR code, but before you go I want to offer you to ask questions, and if you have any
[23:50] questions you are welcome to ask them. For questions please use the microphones in the aisle,
[23:55] and you can get up and use the microphone.
[24:09] Hello, hello, I was wondering your fine art background before you started, if you have one,
[24:16] before you started working in substance painter like painting or ceramics or anything?
[24:22] You mean my background before I became a 3D character?
[24:25] Yeah, that's what I mean. I have a major diploma in foreign languages, so I'm an interpreter in
[24:33] English and Italian, that's why I'm not connected with art, I don't know painting at all, so I draw
[24:41] as I don't know, the best what I can draw I think is heart and the star, and that's it, so it is not
[24:47] obligatory to be perfect in 2D if you want to become a 3D artist.
[24:53] I just want to say that's amazing because I have a background in painting and sculpture,
[24:57] and it looked very natural and intuitive to what I've learned in school for art, so thank you.
[25:03] Thank you, that can be a big boost for you, it will be easier for you if you know all the study
[25:09] skills, if you know sculpting, if you know drawing, but it is not obligatory, you still can become
[25:16] good artist if you don't have the talent for all this.
[25:22] I noticed that in your sculpt before you started texturing you already had the pores done,
[25:26] was that done by hand or through a generator? Oh sorry, I didn't hear you.
[25:29] The pores in your face sculpt were those done by hand or through a generator?
[25:35] The question is about the pores, and the texture of the pores were done by the curvature map,
[25:44] so I used a generator, the curvature, and through this generator I created this back head.
[25:54] Hello. Hello. So I was wondering, so I specialize in both stylists and realism,
[26:03] and I noticed that you're purely stylized, did you start off as purely stylized or did you have any
[26:09] works of realism inter-propfolio when you were looking? I don't have any works in realism,
[26:16] except of this girl, I make only stylist characters, and the reason why I decided to be
[26:21] a stylist artist is because I didn't want to spend a lot of time on creating hair with planes.
[26:26] So do you feel like artists should lock into one style if they want to enter this industry?
[26:33] Oh, a little bit louder please. Oh, do you feel like artists should choose one style if they want
[26:39] to enter in this industry? I think that if you're at the beginning of your way becoming a 3D artist,
[26:48] you need to choose one style, because you will do this style and each work will be better.
[26:54] If you at the very beginning try to work in all the possible styles, then your skill is on the
[26:59] same level, you just have the same level of works in different styles. Okay, thank you. You're welcome.
[27:09] Hello, thank you for coming and giving this presentation first. So I'm a fairly new user
[27:15] for Substance Painters, so this might be a question that everyone knows, but when you have all these
[27:20] different layers for skin, how do you get them to show in the final render? So because to my
[27:27] understanding that when you have these layers, don't they cover each other up? Is there some sort of
[27:31] like transparency or you like tone down the opacity so that they show through? The main,
[27:37] you saw when I was making this dermal layer, the first the base layer, I showed you the mask and
[27:44] that it was semi-transparent. This is how they show off, not show off, they just mix with each
[27:51] other. You just create masks which are not solid, but they are semi-transparent. Okay, I see, that
[27:58] makes sense. Thank you very much. You're welcome. Hi, I was wondering how long did the processes take
[28:05] you of sculpting and retopo and then the texturing of course? This character took I think three months,
[28:14] but in usual life it would take twice less because here I didn't have concept and
[28:22] pity fact is that I was rendering this character on my computer and Macutra is not very powerful
[28:29] for Arnold rendering and to render one shot, not one shot, one picture took about 30 hours and at
[28:37] that time I'm very sorry talking about the it, but that was time when we had the blackouts in
[28:43] Ukraine because a lot of bombs fell on my city and that's why every time I started render I didn't
[28:49] have enough time of electricity to render it, so I started it just several times, so that's why it
[28:56] took so much time. Sorry, Shandvel. Thank you. Hi, my question is you clearly know a lot about
[29:07] like how skin textures behave and I was wondering when you were building these or maybe you learned
[29:12] this in your fine art background. Did you have like a medical textbook open next to you to study
[29:20] how those layers worked and the way the veins moved and stuff? First of all I looked through a lot of
[29:27] tutorials on the internet and I just wrote down what should be on my textures. We know that we
[29:34] have freckles, I need to make freckles, so I write down that we need to, I need to make freckles,
[29:39] then I have like there was a list of freckles, veins, blackheads and so on, this is how I decided to
[29:46] make it. Just like regular old YouTube videos? Yes. Right on. Yes, well the end of also reference
[29:55] and the thing is when we are talking about experience, when you have experience, all I think in the
[30:01] word of experience we have a lot of information, that means that for 10 years you were looking at
[30:09] at 3D models and you know the 3D models so good that you have them in your head and you know
[30:17] each details of your models. This is what we have when we are talking about experience,
[30:24] this what means to have this experience, you know all the details, all the possible details,
[30:30] that's why when you start making something you know all these minor things which you need to include.
[30:37] Thank you. You're welcome. Hi, I saw on your presentation you didn't really go over anchor
[30:46] points, I was wondering what you thought about anchor points when it comes to substance painter?
[30:53] That's a big shame, I don't know how anchors work in substance painter. No, you're good.
[30:59] I was just wondering. I know that they are very powerful but I never had, well I always
[31:06] did all my textures without anchors so unfortunately I don't know how they work.
[31:12] You're good. Thank you. Oh, I see. Yeah. Hi, sorry height differences.
[31:23] So I saw that you did a lot of stylized work. On average how many layers would you say that you
[31:28] use for a stylized piece that you consider finished? So in all of your stylized pieces that went into
[31:38] games and were actually being used, about how many layers on average would you say that you wind
[31:44] up using? I think the amount of layers which you saw on my, here on the skin is the average what
[31:52] I use for texture in any other skin. If we're talking about the clothes, for clothes usually I
[31:57] use less layers because it doesn't have so much information and a lot of fabric materials which
[32:04] I use they already have a lot of information so I don't need to paint everything from the scratch.
[32:11] Okay, cool. Thank you. You're welcome.
[32:16] Hi, thank you for this page. I have a question. Do you prepare any like exports presets for the
[32:24] texture into the engines like Unity or Unreal to use subsurface scattering and everything because
[32:30] it looks different in engine and look different in Substance Painter or your pipeline just ends
[32:36] in Substance Painter? As for the presets for this work I used Arnold presets which are standard here
[32:43] and all these details like subsurface scattering I set it in Arnold, they're just Arnold settings
[32:55] and not the maps. Okay, and do you prepare shaders or something in engines or not? Do you set up textures
[33:03] when you give it to your outsource manager? It works, it works. It works, no, I don't, I don't
[33:12] check. Okay, thank you very much. You're welcome.
[33:18] Hi, thank you for the speech. So I'm more of a level designer but I've been wanting to kind of
[33:25] better collaborate with some of my artists and kind of tech artists. What would you say is like a
[33:32] really good start for kind of like learning Substance in terms of kind of collaborating with
[33:39] my other team members who are more directly working with Substance? So you're asking about the tutorials
[33:45] for Substance Painter? I guess so or like just a general good start, you know. You know, when I was
[33:53] learning Substance Painter there were like three ways, not like three ways, three sources. The first
[33:58] one were official tutorials on the YouTube from Substance Painter. Really they are very good,
[34:03] I really love them. The second one was I asked my team leaders and art directors when I didn't know
[34:10] something. And the third one, I like tutorials of Jay Hill on the YouTube and he gives a lot of
[34:15] information. Okay, thank you. You're welcome. Hi, and I'm really impressed like how you layer out
[34:25] all the layers and I'm more like environment artists but it's very impressive to see how the
[34:31] character artwork. I'm just curious to say you mentioned that it's not best on existing concept.
[34:39] So I'm just wondering like how you gather like references and how you analysis your references
[34:45] that usually how many references you gather for this kind of project. Very good reference, very good
[34:51] questions. Thank you. Unfortunately I don't have this pure file with all the references which I had
[34:58] but I had references here for everything. So I had groups like style, quality, eyes,
[35:05] eyebrows, lips, hair style, general style. So I just had a lot of structured reference
[35:12] and I was just comparing what I'm receiving to what I see on this reference.
[35:18] So you mean you have like a library you build that over the years?
[35:22] No, no, just for this project. Oh, just for this project. So you just break down to different
[35:27] section and compare your reference. Yes, all the references were in the pure file and I created
[35:33] them only for this project. So I just was just going through the art station looking for the
[35:38] picture which I need. Thank you. You're welcome.
[35:46] Hello. I like to say thank you for your presentation, very informative. Your final render it was taken
[35:55] in Arnold. So the textures that you had to take, you had to export them out from substance painter.
[36:02] Were there any particular issues regarding whenever you take those textures into Arnold
[36:10] and rendering them out? Were there issues regarding like sometimes being those textures being like
[36:16] a different shade or maybe a different shade of color or maybe there's something wrong with
[36:22] specific maps. I know there can be an issue regarding taking some of those textures out from
[36:29] painter and testing them out in different engines may cause some issues regarding,
[36:35] it'll cause them to look different in other engines and in other renderers than they would be in painter.
[36:41] Good question. And I can say that in this project I didn't have any issues. I exported this Arnold
[36:47] preset and everything worked in Arnold. I had in general problems with Arnold because it is so
[36:53] un-understandable and not intuitive software. So that usually happens when you're just looking for
[37:03] one tick which you don't have and you look through everything and finally left it two days to find
[37:08] it. So I just in general have some issues in Arnold which are not connected with the textures.
[37:15] And in my situation I think I usually just select the preset which I need. It works sometimes I have
[37:22] the presets already premade and I just import to Substance Painter the preset. Then it always works.
[37:31] So in general I didn't have any issues. Okay thank you. You're welcome.
[37:38] Hi Anna, thank you for this incredible presentation. So I have a question regarding the skin materials. So
[37:42] when you're using the skin is that a preset template that you already set up from previous
[37:46] projects or do you recreate the skin from scratching? What's your thought process of the skin materials?
[37:51] Thank you so much. Can you a little bit louder please? Sorry, let me repeat it. I'm sorry English is
[37:58] not my native language. Okay let me repeat the question sorry. So do you use a skin for your
[38:04] skin material textures? Do you have a preset template that you import prior like a base template
[38:11] prior to making the skin or are you creating the skin from scratch for every... Everything was
[38:17] done from scratch as I saw. I didn't have any preset material. Okay cool thank you. But I converted
[38:22] the skin into a preset. That's why every time when I'm textured in semi-realistic skin I'm just using
[38:28] this preset. Oh that's okay awesome that's smart thank you so much. You're welcome. Hello thank you
[38:36] for the presentation. So you mentioned about you create like stylized because of hair but in this
[38:41] project I saw your hair in action is really pretty. I wonder the color is also made from the
[38:50] Maya the action or is in the substance painter? The color of her hair. Yes. X-gen. In the X-gen when
[38:59] you're making a color it's not X-gen it is hair material and it is Arnold hair material and there
[39:08] you have an opportunity to draw on your UV map just to draw and the color and the hair which
[39:21] touches this color they're going to be this color and the other area which is the another color
[39:28] it's going to be that color it's just you're drawing on your UV map in Arnold with this
[39:33] Arnold hair material. That's amazing thank you. Thank you thank you. I think we have last question.
[39:42] Hi so whenever I'm working in substance painter and exporting it to other softwares like it looks
[39:49] really good in painter but then when I export it to other softwares maybe it looks 50% or 75%
[39:56] is good. What tricks and tips do you have to maybe make ensure that it looks as good as it can be
[40:03] in other softwares? The thing is the trick here is that you need to use the same HDR which you used
[40:09] in substance painter. If you're rendering your character then in Marmoset in Marmoset you have
[40:14] this opportunity to upload the HDR which you used in substance painter and then all your textures will
[40:21] be looking absolutely same as they look in substance painter. Thank you so much. You're welcome and
[40:28] before we finish I say that that was the last question I want to say several words and I want
[40:34] to say that the profession of 3d artist is I think it's one of the most perfect profession in the
[40:43] world because this profession it is very creative profession and besides if you're talking about
[40:51] like another part of this profession this profession can save you in any situation of your life
[40:58] whether it is covid as we had it before no matter whether it is war like in my country you still have
[41:04] an opportunity to work and I can say that I know it is very difficult at the very beginning to get a
[41:11] first job to enter the studio and to start being the artist with 3d artist but later when you become
[41:19] a middle artist and senior artist you will not have a lot of problems you will enjoy everything
[41:26] all the best things which you have in this profession because this profession pays you off
[41:32] and I want to say that it doesn't matter whether you are not good in drawing like me or finished
[41:39] art school it doesn't I mean I want to say that if you work a lot and if you really want to become
[41:47] 3d artist that will come just take your time and to all of you I wish all the senior positions I
[41:55] wish to you to become best artist to find your place to make the game which you really wanted
[42:01] because a long ago I wanted to make Heroes of the Storm for Blizzard and I never thought that
[42:08] would come true but I made skins for this game and everything what you wanted this life can happen
[42:15] to you thank you for listening and I really hope that you liked my lecture



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
