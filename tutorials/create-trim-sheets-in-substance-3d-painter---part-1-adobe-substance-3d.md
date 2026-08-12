---
title: Create Trim Sheets in Substance 3D Painter - Part 1 | Adobe Substance 3D
source: YouTube
url: https://www.youtube.com/watch?v=dE4LWGMwypc
author: Adobe Substance 3D
ingested: 2026-08-12
app: "[PENDING]"
version: "[PENDING]"
tags: []
extraction_status: pending
frames_dir: tutorials/frames/create-trim-sheets-in-substance-3d-painter---part-1-adobe-substance-3d/
frame_count: 0
frame_status: pending-selection
---

# Create Trim Sheets in Substance 3D Painter - Part 1 | Adobe Substance 3D

**Source:** [YouTube](https://www.youtube.com/watch?v=dE4LWGMwypc)
**Author:** Adobe Substance 3D
**Duration:** 18m38s | 13 section(s)

---

## Raw Data (for Claude Code extraction)

Frames are not captured yet. Read the timestamped transcript below, pick moments
that actually show a technique/result worth a still (not blind percentages —
even within a named chapter, verify the real moment against its timestamps), then run:
  python select_frames.py create-trim-sheets-in-substance-3d-painter---part-1-adobe-substance-3d <ts1> <ts2> ...
(seconds or mm:ss). This appends a "Captured Frames" section and updates the
frontmatter before you write the Structured Notes below.


### <Untitled Chapter 1> [0:00]
**Transcript (timestamped):**
[0:00] Hello everyone, in this small tutorial series we will go over on how to create trimsheet textures directly inside of Substance 3D Painter and on how they would be used in the production of 3D assets.


### What Actually Are Trim Sheets [0:21]
**Transcript (timestamped):**
[0:21] Dus, eerst wat eigenlijk trimsheets zijn. Trimsheets zijn een manier om verschillende texture elementen in een single texture te verbinden zodat je ze op je 3D models kunt gebruiken.
[0:34] Dit is een geweldig manier om te savee het tijd en texture memorie te hebben, zoals je alleen moet creëren en een single texture te loaden.
[0:41] Trimsheets zijn vaak gebruikt in video games, maar kunnen gebruikt voor verschillende situaties over alle industrie's.
[0:49] In deze tutorial gaan we je een van de situaties laten zien, waarin we een hele sci-fi-corridor scene ontwikkeld, met één single trimsheet texture.
[0:59] Oké, dus hier zijn we in het sub-painter.
[1:01] Ik heb nu een simpel PBR-metal grafne scene met een plane geloaden, maar dit is niet helemaal een normaal plane.
[1:09] Als we bijvoorbeeld naar een polygon filter gaan, zie je dat deze plane in verschillende segmenten is bevindeld.
[1:18] Dit is gewoon een geometrie die in je 3D software is geïnteresseerd.
[1:21] Je kunt dit in welke 3D software gewoon door je plane te subdermijnen.
[1:26] Dus waarom moeten we dit?
[1:27] We moeten dit, want voor een trimsheet gaan we onze trimsheet in verschillende secties brengen.
[1:33] Bijvoorbeeld een die met metal is, een die wat details is, een die wat details is.
[1:37] En het is heel makkelijk om dat in het sub-painter te doen, waar we gewoon onze kleuren selecten,
[1:43] met een littelijk klik en dragen, zoals dit bijvoorbeeld.
[1:47] Dus als we een look hebben op onze referenties hierover,
[1:50] wil je er wat referenties aan te krijgen zodat je weet wat details je wilt.
[1:54] Dit is de referentie die we gebruiken.
[1:57] Voor het eind, zie ik dat we hier wat metal details hebben.
[2:00] We hebben hier wat kleine paneling details.
[2:03] We hebben hier wat kabels, over hier hebben we een andere kleine strip van detail.
[2:07] En als we naar de andere referenties gaan, kunnen we ook zien dat we wat panel details hebben.
[2:13] En dat we wat floor details hebben.
[2:16] Dus we gaan naar de koeien en creëer een trimsheet die
[2:19] van ons floor, de pilers, onze vleugels, onze wals met wikken en alles in de between kan handelen.
[2:28] Dus wat we nu gaan doen is, gaan we een soort van een kleur ID map creëren.


### Color Id Map [2:30]
**Transcript (timestamped):**
[2:32] We moeten dit doen, want we gaan onze trimsheet in verschillende secties brengen.
[2:36] En we willen de secties later op selecten, zodat we eigenlijk de verkeerdheid kunnen maken.
[2:42] Dus ik ben heel erg goed aan het werken, dus ik wil hier een folder creëren.
[2:47] En ik ga hier gewoon deze folder color underscore ID.
[2:50] Nou, dit is eigenlijk heel makkelijk.
[2:52] Alles wat je moet doen is creëren een simpele fil layer.


### Create a Simple Fill Layer [2:53]
**Transcript (timestamped):**
[2:56] Je wilt gewoon naar buiten en alles opzetten, maar voor je kleur.
[2:59] En laten we gewoon beginnen met een red kleur.
[3:01] We gaan veel verschillende kleuren creëren.
[3:04] We gaan gewoon naar buiten en we willen dit namen geven.
[3:07] Dus laten we zeggen dat deze kleur de base metal wordt.
[3:12] Zoals je kan meestal van mijn referentie, moeten we veel base metal over hier.
[3:16] En dat is hoe je wilt denken over dit.
[3:18] Eerst wil je hier een go-up en een zwarte mask maken.


### Black Mask [3:22]
**Transcript (timestamped):**
[3:23] En nu wil je voor jezelf denken hoeveel metal je moet.
[3:28] Want we moeten veel metal.
[3:30] We willen dit sectie waarschijnlijk een beetje groter maken
[3:33] dan andere secties, zodat we een beetje meer spas hebben
[3:36] als we onze 3D model creëren.
[3:39] Dus wat we kunnen doen is we kunnen naar onze Polygon Fil Tool.
[3:43] Zet het naar onze face selectie en maak er zeker dat de kleur is wijn.
[3:47] En je kunt choose hoe groot van een sectie je wilt.
[3:51] Ik ga naar boven en ik ga creëren een sectie
[3:53] waarschijnlijk rond dit groot, misschien een beetje groter.
[3:56] En wat ik wil doen is dat ik ervoor wil maken dat het
[3:58] verstandiging van de link naar de rechts gaat.
[4:01] Dit betekent dat als ik de UV-unwapping begin,
[4:03] kan ik gewoon naar boven en blijven uit mijn 1x1 spas.
[4:08] Nu, de volgende die ik leuk vind om te doen met een trim sheet is een


### Construction Line [4:11]
**Transcript (timestamped):**
[4:12] constructie-lijn.
[4:13] Zoals je kunt zien over hier, heb ik een paar verschillende constructie-lijnen
[4:17] en ze zijn gewoon een geweldige manier om eigenlijk
[4:19] de wide-up-servies te maken, speciaal als je trim sheets creert
[4:23] omdat ze ervan kunnen horen.
[4:25] Dus wat we willen doen is gewoon duplikeren
[4:29] onze laag.
[4:30] Komen dit bijvoorbeeld een lijn en ik wil dan snel gewoon uit
[4:34] een zwarte mask maken, die we op de maas op zwarte zaken gaan resetten.
[4:38] Dan in onze kleur, we willen gewoon een verschillende kleur geven.
[4:40] Dit maakt het natuurlijk een beetje makkelijk om te zien.
[4:43] En onze constructie-lijn moet niet heel groot zijn,
[4:45] dus laten we alleen twee van hier te wide maken.
[4:49] En zo kan we het gewoon uit mijn trim sheet divijten
[4:51] tot we er geen ruimte hebben.
[4:53] Dus ik zal gewoon snel in een timelapse kicken
[4:56] waar ik het op te divijten en dan zal ik het uitleggen
[4:58] naar je de divisions die ik heb gemaakt en waarom ik ze heb gemaakt.
[5:01] Dus laten we even een snel timelapse kicken.
[5:05] Dus hier zie je dat ik in de timelapse kregen en ik ben
[5:07] nu gecreëerd, zoals wat vloerventen hierover.
[5:11] Ik ga ze gewoon venten kopen en dan naast dit
[5:13] ga ik een paar van die geren maken die ik ook in mijn referentie heb gezien.
[5:17] Nu, op dit moment heb ik meestal de lange stukken uit de manier,
[5:20] dus ik wil gewoon naar beneden en creëer een kleine sectie
[5:23] die er eigenlijk random details zal zijn, dus random
[5:26] decals, random normen, net details, dingen zoals dat.
[5:29] Dan een andere sectie die voor random teksten, decals
[5:33] en teksten en dingen zoals dat.
[5:35] En dan heb ik gewoon wat speciaal consul en natuurlijk
[5:38] laten we niet vergeten dat we ook onze eigen wouw moeten creëer.
[5:42] Dus deze zal voor onze wouw zijn.
[5:44] We gaan een simetrie op een wouw gebruiken,
[5:46] wat betekent dat we alleen een half van het creëer moeten creëer.
[5:49] Hetzelfde gebeurt voor onze vloer. We gaan een simetrie op een vloer
[5:52] in 3D, wat betekent dat we alleen een half van onze vloer nodig hebben.
[5:59] Nu dat we een Color ID map hebben, de volgende wat we gaan doen
[6:03] is dat we een art enkerpoint gaan doen naar onze masken
[6:06] door hier te gaan en een art enkerpoint.
[6:09] Dit manier kunnen we later op de referentie deze masken
[6:12] wanneer we eigenlijk willen starten teksten.
[6:14] Ik wil een individuele art enkerpoint op elk masken
[6:17] zodat ik veel controle heb om later op de referentie te maken.
[6:20] Dit is geweldig, want dit betekent dat als we deze masken nog steeds veranderen,
[6:23] het zal gewoon op de graf opneden worden geïnterreden.
[6:27] Dus ik kan gewoon gewoon hier naar beneden gaan en op alle van die
[6:30] kun je art enkerpoint.
[6:32] En dit is ook waarom het heel belangrijk was om je
[6:35] vloerleiders te namen, omdat de enkerpoints
[6:37] worden namelijk door de naam van je laag,
[6:40] waarom je het gewoon extra handig maakt.
[6:42] Dus onze Color ID's zijn nu klaar.
[6:44] De volgende wat we kunnen doen is dat we deze folder minimiseren,
[6:47] creëer een nieuwe folder en we kunnen dit normaal
[6:51] details kopen en we kunnen beginnen door de non-map details te aandelen
[6:55] naar onze trimsheet.
[6:57] Dus voor onze normaal mappen, ik ga je twee verschillende technieken laten zien.
[7:01] Een van die is de hightmap-based normaal mappen en de tweede is de normaal mappen
[7:06] based normaal mappen.
[7:08] Dus de eerste is een heel commone dat ik zeker veel van je al weet
[7:12] en het is ook de het meest makkelijkste te gebruiken.
[7:16] Wat je wilt doen is dat je wilt naar een art en field laag.


### Fill Layer [7:17]
**Transcript (timestamped):**
[7:19] Doe het naam, laten we dit een lijn,
[7:21] bijvoorbeeld omdat het onze constructie lijn is dat ik je over hier heb gegeven.
[7:26] En dan kan we alles doen, excepte voor onze hight.
[7:31] Als je de slijder van je hight maakt, zal het normaal mappen in de deur
[7:34] verdendigd worden. Als je het opgaat, zal het normaal mappen uit.
[7:38] Dus we willen gewoon het doen, want we willen de normaal mappen in verdendigd worden.
[7:43] Dan, als we een zwarte mask uitdelen,
[7:45] wat we in deze zwarte mask in de deur hebben,
[7:46] bijvoorbeeld hier kun je me zien,
[7:48] zal we in een hightmap-detail veranderen.
[7:51] Dus zoals je kunt ooit denken, kunnen we hier naar beneden gaan,
[7:54] bijvoorbeeld naar onze 2D view alleen.
[7:57] En we kunnen dan gewoon de zijkant van onze brush
[8:00] naar de zicht van onze constructie lijn die we willen.
[8:04] En dan om in onze constructie lijn te schijven,
[8:06] ik wil gewoon uit de zijkant van mijn square canvas klikken.
[8:10] Houd de schijf en dan ga je helemaal naar de andere kant.
[8:13] En als je schijft, maak er gewoon zeker dat de lijn
[8:16] geen enteialisering is, dus het ziet perfecte straat.
[8:19] En dan kan je clicken eens weer.
[8:22] Dus wat we doen is, over hier zal het lijn perfect veranderen,
[8:26] maar dan over hier, het doet niet altijd dit.
[8:28] Dus je kunt het schijven om je handen te manuële,
[8:31] te zetten, maar soms is dat heel moeilijk te doen.
[8:35] Over hier, zoals dat is, is het decent.
[8:37] Maar een andere manier waar we het snel kunnen zetten
[8:39] en ook de controle over het later hebben,
[8:42] is gewoon om een filter te aansluiten naar onze mask.
[8:46] In deze filter, als we het gewoon opschijven en een transforme aantrekken,
[8:49] ga ik mijn scaling zetten, bijvoorbeeld naar 105,
[8:53] dus 105.
[8:55] En dan kan ik in en gebruiken mijn offset
[8:57] om het opstuk te pushen naar de locatie die ik wil.
[9:01] Bijvoorbeeld minus 0.015.
[9:05] En nu zal het altijd perfect veranderen op beide zaken.
[9:09] Dat betekent dat we dit over en over kunnen repeteren.
[9:13] Nu kunnen we een soort van techniek gebruiken
[9:14] om eigenlijk ook een deel uit te hebben,
[9:17] zonder onze non-map details.
[9:19] Bijvoorbeeld willen we dit doen
[9:20] als we deze eventen over hier willen creëren.
[9:23] Wat we willen doen is gaan we naar de shader settings
[9:28] en zetten ze van PBR Metallic Rav
[9:30] naar een PBR Metallic Rav met Alpha Test,
[9:34] waarin we een aantal kutouten gaan.
[9:37] Dan gaan we naar de texture set settings.
[9:41] Je wilt gewoon naar je channels
[9:43] en dan wil je een opacity channel.
[9:45] Zoals dat.
[9:47] Nu voor onze normen maps,
[9:48] laten we naar de dupliceid en dupliceid
[9:50] onze normaal lijn.
[9:52] Moet de transformer en een nieuwe black mask uitdelen.
[9:56] We gaan deze eventen effect creëren.
[10:00] Voor deze effect,
[10:01] laten we naar deze eventen gaan.
[10:03] Het is makkelijker als we een generatoren gebruiken.
[10:06] Dus we willen de textuur te navigeren
[10:08] en de tile in typen.


### Tile Generator [10:10]
**Transcript (timestamped):**
[10:10] En dan gaan we een tile generator gebruiken.
[10:12] Je kunt niet de tile generator gebruiken
[10:14] op je mask zoals dit.
[10:15] Je moet gewoon hier naar de Magic One Tool gaan.
[10:18] Dan wil je naar de art,
[10:21] een fill layer,
[10:22] waarom het een grayscale map heeft
[10:25] waar je in de tile generator gebruikt.
[10:30] Het mooiste is dat we een soort
[10:33] capsules moeten creëren
[10:34] en we hebben een pattern type
[10:36] die is called capsule in hier.
[10:39] Zo.
[10:41] Nu, er zijn er wat specifieke
[10:44] opties die je wilt zetten.
[10:45] Ik heb natuurlijk al behoorlijk
[10:46] aangekomen welke opties die er zijn.
[10:48] Een van die is de aanglijst op 90
[10:51] zodat we hier een 90-degree aanglijst hebben.
[10:55] Een ander is onze pattern transformatie
[10:57] en de aandacht van de aandacht,
[10:59] waarin ik uitvond dat als we de aandacht
[11:01] op 38 en 33 zet,
[11:03] het geeft een mooi effect.
[11:06] En dan wil ik de rest mijn scale een beetje meer
[11:09] op 1.6 of misschien 1.5 over hier.
[11:15] Dus je kunt heel makkelijk
[11:16] alle zettings veranderen.
[11:19] Naastal willen we het wel een beetje afzetten.


### Offset [11:20]
**Transcript (timestamped):**
[11:21] Dus laten we naar onze afzetten
[11:23] en dan in onze afzetten zet dit op 0.5
[11:26] die zal ons deze mooie pattern geven.
[11:29] Het remind me van een vloer, voorbeeld.
[11:32] Naastal wil ik de balans er een beetje uit.
[11:35] Voorbeeld ga ik mijn wiremountain
[11:37] een beetje lager
[11:38] want ik wil er zeker voor dat ik
[11:40] in dit geval drie van deze binnen de spas krijg.
[11:44] En dan kan je naar je afzetten
[11:45] en je kunt voorbeeld spelen
[11:47] met je globale afzetten in...
[11:49] Oh, daar gaan we.
[11:50] Als ik dit op 0.01 heb gezet,
[11:53] dan kan je even...
[11:54] Je kunt zien dat je niet met een x-deck
[11:57] het niet bemoet, zoals ik het gewoon heb.
[11:59] Je kunt zien dat nu we het perfecte
[12:00] zitten binnen deze spas.
[12:03] En het zal ook perfecter worden
[12:04] als we van de een kant naar de andere.
[12:07] Dan finally, als je wilt, kunt je naar boven gaan.
[12:10] En laten we zeggen dat we gewoon
[12:11] naar de speciaalbehandeling gaan
[12:12] om een beetje te laten zien
[12:13] om het een beetje meer van een vleugdgebied te geven.
[12:16] En dan kan we eigenlijk
[12:17] kopen uit deze vleugdgebied hierover.
[12:20] Nu, eerst gaan we onze enkelpoint
[12:23] te maken sure dat dit pattern
[12:25] alleen zal gebeuren binnen deze spas.
[12:28] We kunnen dit doen
[12:29] door een heel simpele vleugdbehandeling op de top te aandrijven.
[12:32] Ga naar onze graze schijf,
[12:34] enkelpointen en vind je event, mask.
[12:39] En dan wil je alles doen
[12:39] als je hier gewoon wilt gaan en je wilt
[12:41] dit zetten om te multiplijten,
[12:43] wat betekent dat het deze mask gebruikt
[12:45] en alles andere zal worden behoorlijk
[12:47] removed, zonder wat is wijn.
[12:50] Finally, we kunnen terug naar de base
[12:53] van een vleugdbehandeling.
[12:54] Turnen op de opestigde slijder.
[12:57] En als je de slijder opnieuw stopt,
[12:59] kan je zien dat het uit de vleugdbehandeling
[13:00] zal kopen.
[13:02] En daar gaan we.
[13:03] Dus nu hebben we de eventen.
[13:05] Nu wat ik wil laten zien is
[13:06] ik wil je ook laten zien
[13:07] hoe je een actuale normabbehandeling
[13:09] kan maken zoals je hierover kunt zien.


### Norm Map Details [13:12]
**Transcript (timestamped):**
[13:12] Dus creëren deze normabbehandeling
[13:13] is ook heel makkelijk te doen.
[13:15] Dit keer wat je wilt doen
[13:16] is dat je een normaal laag wilt creëren
[13:18] en dat is dit normaal
[13:21] deatel.
[13:22] Dan, als we gewoon naar de library gaan
[13:25] en de deel van de taal
[13:27] elke normabbehandeling die je hier ziet
[13:29] waar je de kleur van de base kan
[13:30] is een normabbehandeling die je kunt schijven.
[13:33] Dus we kunnen zien,
[13:34] zeker hieronder veel van ze.
[13:37] Laten we naar de schoenen
[13:38] en zeggen dat we willen schijven


### Paint in a Panel [13:39]
**Transcript (timestamped):**
[13:39] in een panel.
[13:40] Wat ik leuk doe
[13:41] is ik wil de projectie gebruiken
[13:43] voor dit.
[13:43] Dus ik wil hier naar de projectie gaan.
[13:47] En dan ga ik gewoon
[13:48] op alles aangeparen
[13:49] zonder de normaal
[13:51] en dit keer ook de opestigde.
[13:53] Dus ik ga een panel dragen
[13:55] dat ik wil in de normaal en
[13:57] de opestigde slijder.
[13:59] Dan als ik S en R klik
[14:00] kan ik de projectie
[14:02] mijn projectie
[14:03] en ik kan natuurlijk zoeken hier in.
[14:06] Ik ga het op en ik kan het in een
[14:08] locatie plaatsen wat ik wil.
[14:10] Laten we zeggen dat ik het hier
[14:11] wil plaatsen.
[14:13] Als je wilt, kan je je hartstikke
[14:15] hierover, op de broek,
[14:17] wat het een beetje makkelijk
[14:18] te schijven in.
[14:19] En dan is het gewoon een simpel
[14:21] beeld van schijven dit in.
[14:23] De reden waarom we ook willen
[14:24] deze in onze opestigde hebben
[14:26] is omdat als we hier naar de materiale
[14:29] en naar onze opestigde slot gaan.
[14:31] Wat je kunt zien nu is
[14:32] dat we in het eindelijk kunnen
[14:33] een mask generen.
[14:35] Maar in order deze mask te genereren,
[14:37] er is één lastigheid die we willen doen.
[14:39] We willen hier naar beneden
[14:41] en uit een levels.
[14:43] En dan wil je de effecte channel
[14:45] opzetten om je opestigde te zijn.
[14:48] En dan gewoon move je witte slijder
[14:50] naar de linker.
[14:51] En nu heb je automatisch ook
[14:53] een mask generen
[14:54] voor elke normaal beeld die je hebt.
[14:57] En dat is het.
[14:58] Op dit punt kan je aan de kant
[14:59] om de m te voeren om naar beneden
[15:02] terug te gaan naar je projectie
[15:03] en wanneer je een ander normaal beeld wilt
[15:06] kun je het gewoon in hier dragen.
[15:09] En dan kun je bijvoorbeeld
[15:10] het hier naar beneden
[15:13] en gewoon het in zo schijven.
[15:16] Dus nu dat ik je deze technieken heb
[15:17] gezien, gaan we nu
[15:18] naar een timelapse
[15:20] waar we in een bunch van deze
[15:22] verschillende details
[15:23] op verschillende panelen zoals je hier ziet.
[15:27] Dus ik ging gewoon naar dat
[15:28] en kreeg ik in de timelapse
[15:29] en we gaan dit deel van
[15:31] gewoon om wat van de normaal beeld
[15:33] details te placen.
[15:34] Bordelijk hierover
[15:35] ben ik gewoon op verschillende
[15:36] details die ik denk dat ik
[15:38] handig kan komen
[15:38] wanneer ik mijn sci-fi-corridor
[15:40] gecreëerd ben.
[15:41] Dit zijn gewoon verschillende
[15:42] dingen zoals vans,
[15:43] wat handels,
[15:44] gewoon zoals wat kleinstof.
[15:45] En het mooiste is omdat we een
[15:47] kut uit hebben op dit.
[15:49] We kunnen eigenlijk de background
[15:51] uitkijken, wat betekent dat we
[15:51] deze details op plane
[15:53] en ze gebruiken als deels
[15:55] in onze zin in een reale engine.
[15:57] Nu over hier.
[15:58] Naast dit ik ook gewoon
[16:00] dus gewoon een variant
[16:02] van de hoge details
[16:03] en normaal details.
[16:05] Nu ga ik gewoon
[16:06] over naar een hoge detail
[16:07] switchen omdat ik mijn strijpen
[16:09] wil gebruiken,
[16:09] wat is simpel
[16:10] van de taalgenerator
[16:11] om eigenlijk wat ridden te creëren.
[16:13] Nu naast dit kan ik ook een
[16:15] blend creëren.
[16:16] Voor eerst begin ik met een base
[16:18] met mijn hoge map details
[16:20] en dan kan ik die blend
[16:21] met norme map details.
[16:23] Op deze blend
[16:24] ga ik gewoon een simpel filter
[16:26] gehuilderden
[16:27] met een blur
[16:28] en dan ga ik over naar
[16:29] een normaal map details
[16:30] waar je me kunt zien
[16:31] plaatsen.
[16:31] Gewoon een random normaal map
[16:33] details die een beetje
[16:34] meer interessant zijn.
[16:35] En dit is zoals een
[16:37] kleine console voorbeeld.
[16:39] Soms weer ga ik nu
[16:40] naar de kruis en ga ik


### Wall Panels [16:41]
**Transcript (timestamped):**
[16:41] mijn wawpennels creëren
[16:42] en deze wawpennels
[16:43] gebruiken simmetrie
[16:44] wat betekent dat we alleen
[16:45] het half van het
[16:46] en dan in 3D
[16:48] we het gewoon
[16:49] om het rond te kregen
[16:49] om de tweede half te creëren.
[16:51] Ik ben gewoon door te creëren
[16:52] om een meer simplifiek versie
[16:54] van deze wawpennels
[16:56] en ook de wawpennels
[16:57] om dingen een beetje
[16:58] meer makkelijk
[16:59] en minder voor dit tutorial.
[17:01] Over hier wat ik doe
[17:02] is ik een schilderde
[17:03] laagdraad
[17:03] dat ik het gezet om te lichten
[17:05] om eigenlijk te aandelen
[17:06] van welke details op de top.
[17:08] De reden waarom ik moet doen
[17:09] is omdat de blend
[17:10] niet werkt.
[17:12] Dus als je nog
[17:12] welke blendproblemen hebt
[17:14] dan probeer je te aandelen
[17:14] naar een schilderde
[17:16] en dan spelen je
[17:16] rond met je blendmode.
[17:19] Nu over hier
[17:19] ik ga gewoon
[17:20] duplicatie mijn ritsen
[17:22] en ik ben eigenlijk gewoon
[17:23] aandelen,
[17:24] aandelen een blur
[17:25] en dan kunnen we dit
[17:26] in bijvoorbeeld
[17:27] zoals een kabel
[17:28] dus het is een
[17:29] rubberkabel.
[17:31] En finnie
[17:31] we kunnen werken op onze


### Floor Panel [17:32]
**Transcript (timestamped):**
[17:32] vloerpanel.
[17:33] De vloerpanel
[17:34] zal gewoon een geweldige
[17:35] huidmapschapen gebruiken
[17:37] en we gaan de invert function
[17:38] van deze huidmapschapen
[17:40] te eigenlijk
[17:41] creëren een verschillende
[17:42] pattern
[17:43] dus hier kun je me
[17:43] op de inwerking zien.
[17:45] En dan heb ik
[17:45] eens een keer
[17:46] uitgepakt
[17:46] omdat je niet kan
[17:47] gebruiken zoals een racer
[17:49] of iets zoals dat.
[17:50] Je moet in de huidmode
[17:51] in de vorm
[17:51] in order die detail te schijven.
[17:54] Dan op de top van dit
[17:55] ga ik gewoon
[17:56] aandelen
[17:56] wat meer kleinere details
[17:58] voor die ga ik een
[17:59] schijflaar gebruiken
[18:00] dat ik zet
[18:00] om te veranderen
[18:02] om het eigenlijk
[18:02] properlijk alle
[18:04] van deze schapen te blenden.
[18:05] Dus soms wil je
[18:06] gewoon deze in combinatie
[18:07] met schijflaar
[18:08] gewoon voor de blenden.
[18:10] Je kunt natuurlijk
[18:11] gebruiken simmetrie
[18:12] als je wilt
[18:13] maar ik bedoel
[18:14] omdat ik dit
[18:14] heel snel was
[18:15] dat ik niet ga
[18:16] gaan gaan
[18:17] en gebruiken simmetrie.
[18:18] En nu
[18:19] ik ga gewoon
[18:19] een paar kleinere details.
[18:21] En dat was het voor dit
[18:22] deel van dit tutorial serie.
[18:24] De volgende
[18:24] deel gaan we over
[18:25] hoe we onze base color
[18:26] creëren
[18:27] en ik zal je ook
[18:28] laten zien hoe ik ze gebruik
[18:30] binnen een real engine 5.



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
