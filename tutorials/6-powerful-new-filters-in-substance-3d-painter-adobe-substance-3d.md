---
title: 6 Powerful New Filters in Substance 3D Painter | Adobe Substance 3D
source: YouTube
url: https://www.youtube.com/watch?v=aCi0RG9-9so
author: Adobe Substance 3D
ingested: 2026-08-13
app: "[PENDING]"
version: "[PENDING]"
tags: []
extraction_status: pending
frames_dir: tutorials/frames/6-powerful-new-filters-in-substance-3d-painter-adobe-substance-3d/
frame_count: 0
frame_status: pending-selection
---

# 6 Powerful New Filters in Substance 3D Painter | Adobe Substance 3D

**Source:** [YouTube](https://www.youtube.com/watch?v=aCi0RG9-9so)
**Author:** Adobe Substance 3D
**Duration:** 9m52s | 9 section(s)

---

## Raw Data (for Claude Code extraction)

Frames are not captured yet. Read the timestamped transcript below, pick moments
that actually show a technique/result worth a still (not blind percentages —
even within a named chapter, verify the real moment against its timestamps), then run:
  python select_frames.py 6-powerful-new-filters-in-substance-3d-painter-adobe-substance-3d <ts1> <ts2> ...
(seconds or mm:ss). This appends a "Captured Frames" section and updates the
frontmatter before you write the Structured Notes below.


### Introduction [0:00]
**Transcript (timestamped):**
[0:00] Bonjour, je m'appelle Guillaume Meier, je suis un artiste technique à Adobe Substance 3D.
[0:04] Aujourd'hui, je voudrais présenter les nouveaux filtres que nous avons ajoutés
[0:08] dans la dernière version de Substance 3D Painter.
[0:11] Ces filtres vont vous aider à atteindre des effets matériaux
[0:14] comme un masque avec des mousses de bevel,
[0:17] ajouter des fluides pour vos modèles avec la distance directionale
[0:21] ou donner un look stylisé et pinté pour vos modèles avec le filtre de stylisation.
[0:27] Alors, venez à l'étard et explorez les filtres en plus détaillé.


### Find the new filters [0:32]
**Transcript (timestamped):**
[0:32] Premièrement, pour trouver ces nouveaux filtres dans le Painter Substance 3D,
[0:35] setz les palettes à tous les libraries et cliquez sur le filtre icon.
[0:40] Ici, on trouve le nouveau filtre anisotropique Quara.
[0:44] Le bevel de mousses, la distance directionale, la conversion gré-scale,
[0:49] les quantités et la stylisation.
[0:52] Toutes ces filtres, exécutant la stylisation ou des filtres génériques
[0:56] qui peuvent être appliqués sur les layers de texture ou des mousses,
[1:00] vont travailler n'importe quel point dans votre stack de layer pour mieux améliorer votre fonctionnement.
[1:06] C'est vraiment facile d'appliquer ces filtres.
[1:08] Donc, venez à regarder plus près sur comment utiliser chaque filtre.


### Anisotropic Kuwahara [1:11]
**Transcript (timestamped):**
[1:12] Nous allons commencer avec le filtre anisotropique Quara
[1:15] par le droiter sur un set de texture.
[1:17] Le filtre anisotropique Quara est un effet de mousses qui tente de préserver
[1:21] les égages de couleur de votre texture.
[1:24] Ce filtre est commonly utilisé pour créer des effets de painting stylés.
[1:28] D'autant que la base couleur soit procédée.
[1:32] Mais vous pouvez aussi activer autres canaux.
[1:34] Le paramètre radio contrôle l'intensité du effet de mousses.
[1:40] Si vous avez besoin d'un valeur plus haut que 10,
[1:42] simplement ajoutez le numéro des désir.
[1:44] Le paramètre de mousses intensifie la diffusion des couleurs pour atteindre un look moussé.
[1:50] Le paramètre de mousses augmente le contraste entre les couleurs à atteindre un look flatté.
[1:56] Le smooth-tensor se brise le flow de direction extracté du texture original,
[2:02] qui réveille les résultats noisés.
[2:04] Et le paramètre de l'anisotropique
[2:06] s'étend à comment le effet se fait suivre le flow des égages de couleur.
[2:10] Pour une customisation additionnelle,
[2:12] vous pouvez localement contrôler l'intensité du filtre en utilisant l'input de la base de la base radio.
[2:17] Plus, pour contrôler la direction de la mousses avec une customisation,
[2:21] vous pouvez sélectionner l'input custom de la direction extractée dans le menu.
[2:26] Pour dédouer la direction de la mousses sur une chaîne spécifique,
[2:29] ajoutez un point anchor au lait avant le filtre.
[2:33] Laissez-le comme l'input custom et choisissez le canal que vous voulez utiliser.
[2:37] En utilisant cet appareil, l'anisotropique Quara
[2:40] va nettoyer toutes les canules uniformement en utilisant la même map de direction.
[2:45] Transformant vos matériaux de réalité dans des textures de penteurles
[2:50] est maintenant super facile avec l'anisotropique Quara filtre.


### Bevel Smooth [2:54]
**Transcript (timestamped):**
[2:54] Maintenant, let's look at the bevel smooth filter.
[2:57] Le bevel smooth est une évolution du filtre bevel.
[3:00] Il crée des bevels smooths sans artefacts pixel.
[3:05] Vous pouvez appliquer le bevel smooth directement sur une léaure avec une haine ou sur une mousse.
[3:10] J'ai créé une léaure filtre avec une haine de chanel à 1.
[3:15] Cette léaure est masque par un texte projeté sur mon modèle.
[3:19] Laissez appliquer le filtre bevel smooth sur le masque pour ajouter le bevel.
[3:24] La direction de la mousses drop-down laissez-vous choisir différents designs de bevel.
[3:28] Le paramètre distance set le nombre de bevels.
[3:32] Le paramètre smooth se coulore le masque original pour créer des bevels smooth.
[3:37] Si le smooth est trop bas, l'artefax va s'appliquer sur les bevels.
[3:41] Si le smooth est trop bas, le masque original va perdre la définition.
[3:45] Le paramètre offset de la mousse s'éteint ou au-delà des bordes de bevel.
[3:51] Le paramètre de la mousse s'applique à un point de pince ou à une courbe de la mousse.
[3:56] Le paramètre de la mousse offset de la bordes de la mousse et aide à récover des areas soft.
[4:03] Vous pouvez localement contrôler le nombre de bevels en utilisant l'input du map distance.
[4:08] Juste de plier un map ou un bruit ici pour créer des designs de bevels uniques.
[4:14] Le filtre bevel est créé pour transformer tous les égages de la mousse à des bevels de mousse.


### Direction Distance [4:21]
**Transcript (timestamped):**
[4:21] Ensuite, nous allons examiner le filtre de distance directionale.
[4:25] J'ai créé un masque noir sur ce filtre.
[4:28] Nous allons painter avec le bruit sur le masque.
[4:31] Vous pouvez appliquer le filtre de distance directionale sur le masque pour faire le coup.
[4:36] Le paramètre de distance vous permet de l'adjuster à la length de la mousse qui est sur le masque.
[4:41] Le paramètre de angle s'étend à la direction de la mousse.
[4:45] C'est important de noter que le filtre est basé sur le espace UV.
[4:49] Cela signifie que les bevels suivent l'église polygonique de la mousse.
[4:54] Le paramètre de contraste contrôle le contraste des bevels.
[4:58] Le map distance, qui est un outil important, permet de créer des bevels organiques.
[5:03] Juste de plier un bruit ou un texture grunge pour simuler des variations de troupes intéressantes.
[5:09] La intensité de la bevel sera évoluée par l'influence de la scale et de l'église de la bevel.
[5:15] En fait, vous pouvez continuer de painting sur votre masque et voir le lique en réel temps.
[5:21] Un autre intéressant fonctionnement est de utiliser le filtre sur une couche de peinture.
[5:25] Cela vous permet de mélanger différentes couleurs ou finissances dans un autre.
[5:30] La distance directionale permet de créer tous les valeurs RGB et alpha.
[5:35] Vous pourrez créer des effets de lique réaliste en jouant avec le fleur de bruit et de l'opération.
[5:42] La filter distance directionale est un outil fort pour simuler des liques organiques,
[5:47] aidant à faire que vos modèles appuient plus vieillement.


### Grayscale Conversion [5:51]
**Transcript (timestamped):**
[5:51] La conversion grayscale convertit vos couleurs maps dans les maps grayscale avec des ajustements de l'advance.
[5:59] Sur la masque, appliquez le filtre et le changement de la caméra pour l'input custom.
[6:03] Vous pouvez maintenant draguer et droper chaque map de couleur dans l'input custom.
[6:08] Vous pouvez jouer avec les paramètres de la caméra pour inclure tous les valeurs que vous voulez garder dans la masque.
[6:16] Félicitez le masque avec la balance et les paramètres contrastés ou utilisez les modèles différents de la menu dropdown.
[6:23] En général, la conversion grayscale est un filtre technique créé pour finir votre lait ou les masts
[6:30] quand en utilisant les textures de couleur.


### Quantize [6:33]
**Transcript (timestamped):**
[6:33] Maintenant, let's examinez le filtre quantiser.
[6:36] Vous pouvez draguer et dropir le filtre quantiser directement sur un set de texture pour appliquer à tous les layers.
[6:42] Le filtre quantiser diminue le nombre de couleurs qui définissent vos matériaux.
[6:47] Par défaut, il modifie la base couleur mais vous pouvez activer
[6:51] d'autres canaux que vous voulez procéder.
[6:54] Le nombre de couleurs permet à vous dire le nombre de couleurs que vous souhaitez sur le map de votre texture.
[7:00] Les valeurs la plus bas seront résultées en un looks minimaliste et plus flat.
[7:04] Les valeurs la plus hautes seront résultées en un look plus détaillé.
[7:08] Le smooth contour permet à vous smoother tous les couleurs.
[7:12] Cela transformera votre texture dans un style de vecteur de la forme unique.
[7:17] Vous pouvez mettre des valeurs à l'arrière de 8 pour avoir un look plus fort mais cela
[7:22] sera drastiquement descendu sur le filtre.
[7:24] Le paramètre de la haute-brief appuie un pattern de bruit pour réétrecir le gradient de l'original texture.
[7:30] Faites surement que le smooth contour est prêt à 0 pour voir l'effet.
[7:34] La mode de mode de couleur distance dépend de la chaîne de matériaux qui est processe.
[7:39] La base couleur est adaptée à les maps couleurs comme la base couleur.
[7:43] La base colorise est adaptée aux maps de données comme la normale, la rafinité et d'autres.
[7:48] Si vous appliquez le filtre de quantité sur une lèvres avec alpha comme une lèvres avec des
[7:54] mâches bruchées sur le filtre, vous pouvez utiliser l'appli à la option alpha pour contrôler
[7:59] si l'alpha est processe ou pas.
[8:01] Le paramètre de la rèche alpha vous permet de l'offrir les bordards de votre alpha.
[8:06] Et il y a un point.
[8:07] Le filtre de quantité va transformer votre texture dans une illustration de vecteur avec un look
[8:12] fort de flat design.


### Stylization [8:14]
**Transcript (timestamped):**
[8:14] La filtre de stylisation va vous convertir vos modèles
[8:17] dans des assets stylisés et peintés.
[8:21] Vous pouvez le draguer et le droiter sur un set de texture pour appliquer l'effet
[8:25] à toutes les lèvres.
[8:26] Les plateurs de filtre bruchent les mâches bruchées sur les modèles
[8:30] par les projections 3D.
[8:31] Ensuite, il y a une coûté isotropique pour créer des variations stylées subtiles.
[8:38] Ce filtre a beaucoup d'options.
[8:40] Vous pouvez le faire attention pour obtenir le look stylisé que vous avez aimé.
[8:44] Nous avons récordé un tutoriel deep dive dédié sur ce filtre spécifique
[8:48] pour apprendre comment utiliser cela efficacement.
[8:51] Je vais mettre le lien dans la description.
[8:53] Juste記得 que l'asset stylisé peut être exporté
[8:57] du peinture à aucun végénage ou de rendition
[9:00] par le soutenir de son unique look peinté.
[9:02] Ici, pour exemple, pour faire le final rendition,
[9:05] j'ai utilisé l'ensemble du filtre stylisé dans Cinema 4D avec Redshift.
[9:09] Toutes les features de l'application de l'application sont
[9:13] bâtes et convaincées par les maps de texture PBR.
[9:16] En général, avec l'utilisation de l'utilisation,
[9:18] vous pourrez faire votre animation 3D ou les jeux qui sont
[9:23] pantallons.
[9:25] Donc, dans cette vidéo, vous avez découvert beaucoup d'interessants workflows.


### Conclusion [9:26]
**Transcript (timestamped):**
[9:28] J'espère que vous avez aimé jouer avec tout ce nouveau contenu
[9:31] en 3D painter.
[9:32] Merci d'avoir regardé et que vous vous souhaitiez
[9:35] d'avoir été tune pour plus de tutoriels vidéo.



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
