---
title: Anchor Point Magic 03 - Paint Peel Effect in Substance 3D Painter | Adobe Substance 3D
source: YouTube
url: https://www.youtube.com/watch?v=0V_81uje7d8
author: Adobe Substance 3D
ingested: 2026-08-13
app: "[PENDING]"
version: "[PENDING]"
tags: []
extraction_status: pending
frames_dir: tutorials/frames/anchor-point-magic-03---paint-peel-effect-in-substance-3d-painter-adobe-substanc/
frame_count: 0
frame_status: pending-selection
---

# Anchor Point Magic 03 - Paint Peel Effect in Substance 3D Painter | Adobe Substance 3D

**Source:** [YouTube](https://www.youtube.com/watch?v=0V_81uje7d8)
**Author:** Adobe Substance 3D
**Duration:** 5m58s | 1 section(s)

---

## Raw Data (for Claude Code extraction)

Frames are not captured yet. Read the timestamped transcript below, pick moments
that actually show a technique/result worth a still (not blind percentages —
even within a named chapter, verify the real moment against its timestamps), then run:
  python select_frames.py anchor-point-magic-03---paint-peel-effect-in-substance-3d-painter-adobe-substanc <ts1> <ts2> ...
(seconds or mm:ss). This appends a "Captured Frames" section and updates the
frontmatter before you write the Structured Notes below.


### Full Content [0:00]
**Transcript (timestamped):**
[0:00] In deze video van onze multipart tutorial serie op hoe we gebruiken anchor points in verschillende manieren, we gaan over een wat meer advanced techniek te gebruiken voor anchor points en creëer deze peeling paint effect dat je kunt zien over hier.
[0:19] Veel met de normaap details dat je kunt zien hier en alle van deze kleine bumpen en alles dat weerlijk de idee van deze paint starten te peelen van ons originele model.
[0:30] Dus, wat zijn anchor points?
[0:32] Anker points zijn een prachtige feature dat laat je rekenen een deel van je layer stack.
[0:38] Dit betekent dat je een mask of layer kunt defineren en het referent dynamisch in andere layers.
[0:46] Als je de anchor point veranderen, zijn alle referenties ook geïnterregend, laat je je werken smarter en sneller.
[0:52] Oké, dus laten we gaan over onze base scene gaan over hier.
[0:56] Dus dit is een heel simpel base scene.
[0:59] Eerst hebben we onze base bronze material over hier.
[1:02] En dan op de top van dit hebben we een simpel fill layer, wat je hier kunt zien.
[1:06] Dat is gewoon niet helemaal wight, dus slecht wightig.
[1:11] En het heeft gewoon een rafne dat gaat een beetje meer om het een mooie shine te geven dat je hier over kunt zien.
[1:17] En dat is alles.
[1:19] Dus wat we gaan doen is, eerst willen we een mask voor deze genereren, dus een smaakmask,
[1:25] om ons als de actuale paint peeling effect te geven.
[1:28] We kunnen dit gewoon doen door hier te gaan en laten we beginnen met een zwarte mask.
[1:33] En dan als we hier naar boven gaan en naar onze assets en naar onze smaakmask,
[1:37] we willen gaan en we willen een mooie paint-zame mask vinden.
[1:41] Nu, dit is vaak het makkelijker als ik gewoon naar de search ga en op de paint te typen.
[1:46] Dus er zijn een paar van die over hier.
[1:48] Deze die we willen gebruiken is de paint, oude, kleine crack over hier.
[1:54] En we willen gewoon naar boven gaan en dragen dit in.
[1:56] Nu, de eerste ding dat je ziet is dat het niet heel impressief ziet.
[2:00] Dit is omdat we moeten klikken op onze mask en in de invert tab,
[2:04] we moeten gewoon naar boven gaan en pressen door zodat we dit inverten.
[2:08] Op dat punt kun je een beetje meer spelen met je levels hier,
[2:11] wat je kunt zien als een grote impact en je kunt ook spelen met je contrast als je wilt.
[2:16] Dus je kunt zien dat dit al een beetje beter werkt en het meer van de scene of feel
[2:22] dat we hebben op het begin.
[2:24] Dus nu dat we dit gedaan hebben, de volgende scene dat we willen doen is,
[2:28] we willen gewoon alweer onze anchor point te halen.
[2:30] Dus we willen gewoon naar boven gaan, gaan hier naar boven en aantrekken een simpel anchor point.
[2:35] En dan kan je weer de manier die het is nu.
[2:39] Ok, dus nu dat we dit setup hebben, dit gaat echt cool zijn.
[2:43] Dus wat we willen doen is, we willen een veel lager gaan.
[2:46] En laten we gewoon naar boven gaan en het is een paint peeling.
[2:50] Waarom niet?
[2:51] Juste iets zoals dat.
[2:52] Het is niet echt matter.
[2:53] Dan wat ik wil doen is, ik wil alleen mijn height map turnen.
[2:57] Want de paint peeling, het alleen een height nodig.
[3:00] En ik ga gewoon naar boven gaan en mijn height naar boven gaan.
[3:03] Ik weet niet hoe sterk ik het wil, want dat is iets dat we later kunnen controleren.
[3:08] Ok, wat moeten we doen?
[3:10] We moeten naar boven gaan en we moeten een zwarte mask opdelen.
[3:14] En dan, eerst moeten we naar boven gaan en we moeten onze anchor point refereren.
[3:19] Dus er zal er een paar stappen zijn die het een beetje meer moeilijk maken.
[3:22] Dus we gaan eerst een fiel lager opdelen naar deze zwarte mask.
[3:27] En dan weer, we gaan gewoon naar anchor point en we willen onze anchor point grap over hier.
[3:33] Wat je ook wilt doen is, je wilt gewoon naar boven gaan en in de anchor point,
[3:37] ga naar je lage en ga gewoon invoeren.
[3:40] Want we willen de height op de buitenlaten van onze mask.
[3:44] Ok, de volgende stop waar we moeten doen is, we moeten nu naar boven gaan en we moeten een filter aantrekken.
[3:51] Want we willen onze mask die we nu hebben bluren.
[3:54] Dus het is gewoon reedenslager als een simpel mask,
[3:57] wanneer het even referent als de anchor point.
[3:59] En dan kunnen we gewoon deze mask manipuleren, hoeveel we willen op de top van deze.
[4:04] Dus we gaan naar onze filter, grap een bluur en we geven het hier een beetje bluer.
[4:09] En je kunt het al zien gebeuren.
[4:11] Je kunt het zien nu, het geeft ons een beetje van dit peeling effect hierover.
[4:17] Hoeveel is het ook bluren in de binnenkant van onze mask,
[4:20] die er brandt en we willen niet dat.
[4:23] Dus de manier waarin dit werkt is we gewoon naar hier en dan gaat er een andere filter layer op de top van deze.
[4:30] En voor deze filter layer gaan we dezelfde anchor point van onze witte pein vervenen.
[4:35] En dan de laatste wat we moeten doen is we moeten naar en we moeten dit zetten om een multiplie te zijn.
[4:41] Wat je kunt zien is eigenlijk wat we gedaan hebben,
[4:44] is dat we de pein over hier vervenen en dan hebben we het invoerd,
[4:49] zodat het alleen vervening van de pein rond onze hoogte over hier.
[4:55] Dan hebben we dit geblurten zodat het een klein verhaal geeft.
[5:00] En dan hebben we het gedaan, is we gezegd oké,
[5:03] nu wat ik wil doen is ik wil gewoon uitdelen, dus maak het zwart,
[5:07] waarom we onze bronzen willen hebben over hier,
[5:10] die geeft ons dit effect.
[5:12] Nu, de coolste ding over dit effect is dat we altijd terug naar onze filter layer kunnen gaan.
[5:16] En we kunnen controleren hoe sterk we willen hebben de pein beelden te zien, zoals dit.
[5:21] En op de top van dat kunnen we onze geblurten over hier in onze mask
[5:25] om te controleren hoe groot een verhaal geeft dat we willen geven,
[5:28] zodat we het een heel klein verhaal geeft,
[5:31] of gewoon een echt mooi, soft verhaal geeft zoals dit.
[5:35] En net zoals dat, heb je dit echt coole schilderde effect
[5:38] dat het alles anders zal voelen als een beetje eenbampie,
[5:40] en gewoon in general, het maakt het veel meer als een dikke laag van de pein.
[5:46] En dat is eigenlijk hoe we kunnen gaan en zetten op dit
[5:50] peeling-painter effect met anchor points in Substance 3D Painter.



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
