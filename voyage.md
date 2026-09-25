---
description: Les menus de voyage : Voyage, dimensions, biomes, relais, file d'attente et valeurs d'un biome.
---

# 🧭 Menus · Voyage

## Voyage

* Titre de l'inventaire : `STRATA · Voyage`
* Taille : 54 emplacements, 6 lignes
* Ouverture : `/biomes`, Menu principal, option Voyager des PNJ
* Permission : `strata.player.biomes`
* Retour vers : Menu principal
* Remplissage : Vitre grise `minecraft:gray_stained_glass_pane`, sans nom

```
      0   1   2   3   4   5   6   7   8 
 0-8  ··  ··  ··  ··  PO  ··  ··  ··  ··
 9-17 ··  ··  ··  ··  ··  ··  ··  ··  ··
18-26 ··  OW  ··  NE  ··  EN  ··  AE  ··
27-35 ··  ··  ··  ··  ··  ··  ··  ··  ··
36-44 ··  ··  SP  ··  HB  ··  RL  ··  ··
45-53 RE  ··  ··  ··  FE  ··  ··  ··  SO
```

`··` : vitre de remplissage.

| Slot | Code | Objet | Nom | Contenu | Clic |
| --- | --- | --- | --- | --- | --- |
| 4 | PO | `minecraft:filled_map` | Position | Dimension et biome actuels, zone : hub, relais Nord, etc. | Aucun |
| 19 | OW | `minecraft:stone` | Overworld | Biomes débloqués 3 / 4, joueurs dans la dimension, prochain boss | Clic : ouvre la dimension |
| 21 | NE | `minecraft:magma_block` | Nether | Idem, ou « ✖ Prestige I et Pioche en Diamant » | Clic : ouvre la dimension |
| 23 | EN | `minecraft:ender_eye` | End | Idem, ou « ✖ Prestige IV et Pioche de Carmin » | Clic : ouvre la dimension |
| 25 | AE | `minecraft:calcite` | Aether | Idem, ou « ✖ Prestige VII et Pioche en Pulsar » | Clic : ouvre la dimension |
| 38 | SP | `minecraft:lodestone` | Spawn | Portails des dimensions, PNJ, caisses | Clic : `/spawn` |
| 40 | HB | `minecraft:lantern` | Hub du biome actuel | Nom du biome actuel | Clic : téléporte au hub |
| 42 | RL | `minecraft:soul_lantern` | Relais du biome actuel | 4 relais | Clic : ouvre Relais |
| 45, 49, 53 | RE, FE, SO | Barre de navigation | Voir [Conventions](menus.md) | | |

## Dimension

* Titre de l'inventaire : `STRATA · Overworld`
* Taille : 54 emplacements, 6 lignes
* Ouverture : menu Voyage. Même disposition pour Nether, End et Aether
* Permission : `strata.player.biomes`
* Retour vers : Voyage
* Remplissage : Vitre de la couleur de la dimension : verte, rouge, violette ou bleu clair

```
      0   1   2   3   4   5   6   7   8 
 0-8  ··  ··  ··  ··  DI  ··  ··  ··  ··
 9-17 ··  ··  ··  ··  ··  ··  ··  ··  ··
18-26 ··  B1  ··  B2  ··  B3  ··  B4  ··
27-35 ··  ··  ··  ··  ··  ··  ··  ··  ··
36-44 ··  ··  ··  ··  BO  ··  ··  ··  ··
45-53 RE  ··  ··  ··  FE  ··  ··  ··  SO
```

`··` : vitre de remplissage.

| Slot | Code | Objet | Nom | Contenu | Clic |
| --- | --- | --- | --- | --- | --- |
| 4 | DI | icône de la dimension | Overworld | Biomes débloqués, bloc principal, Sceau obtenu ou non dans ce cycle | Aucun |
| 19 | B1 | icône du biome 1 | Plaines | Voir description ci-dessous | Gauche : hub. Droit : relais |
| 21 | B2 | icône du biome 2 | Cavernes de spéléothèmes | Idem | Idem |
| 23 | B3 | icône du biome 3 | Badlands | Idem | Idem |
| 25 | B4 | icône du biome 4 | Pics dentelés | Idem | Idem |
| 40 | BO | `minecraft:wither_skeleton_skull` | Boss de la dimension | Nom du boss, prochain passage, combat en cours avec PV restants | Clic : ouvre Boss |
| 45, 49, 53 | RE, FE, SO | Barre de navigation | Voir [Conventions](menus.md) | | |

**Icônes des 16 biomes**

| Biome | Objet |
| --- | --- |
| Plaines | `minecraft:grass_block` |
| Cavernes de spéléothèmes | `minecraft:pointed_dripstone` |
| Badlands | `minecraft:terracotta` |
| Pics dentelés | `minecraft:snow_block` |
| Terres désolées du Nether | `minecraft:netherrack` |
| Forêt carmin | `minecraft:crimson_nylium` |
| Forêt biscornue | `minecraft:warped_nylium` |
| Vallée des âmes | `minecraft:soul_sand` |
| Terres stériles de l'End | `minecraft:end_stone` |
| Petites îles de l'End | `minecraft:end_stone_bricks` |
| Terres moyennes de l'End | `minecraft:purpur_block` |
| Hautes terres de l'End | `minecraft:chorus_flower` |
| Prairie | `minecraft:cornflower` |
| Bosquet de cerisiers | `minecraft:cherry_leaves` |
| Pentes enneigées | `minecraft:powder_snow_bucket` |
| Pics gelés | `minecraft:packed_ice` |

**Description d'un biome**

```
Plaines
Overworld · biome 1 sur 16

✔ Débloqué
Joueurs : 143 / 250
Minerai favori : Charbon
Valeur moyenne d'un bloc : 13,6 $
Éclats par bloc : 1 · XP x1

Clic gauche : hub · Clic droit : relais
```

| État | Affichage |
| --- | --- |
| Biome actuel | Brillance, « ▶ Tu es ici » |
| Débloqué | « ✔ Débloqué », nombre de joueurs |
| Plein | « ⚠ Plein : 250 / 250 », clic : entrer dans la file d'attente |
| Verrouillé par la pioche | Pas de brillance, « ✖ Pioche en Fer (T3) requise » |
| Verrouillé par le Prestige | « ✖ Prestige IV requis » |

## Relais

* Titre de l'inventaire : `STRATA · Relais`
* Taille : 45 emplacements, 5 lignes
* Ouverture : `/relais`, menu Voyage, clic droit sur un biome
* Permission : `strata.player.relais`
* Retour vers : Dimension
* Remplissage : Vitre de la couleur de la dimension

```
      0   1   2   3   4   5   6   7   8 
 0-8  ··  ··  ··  ··  BI  ··  ··  ··  ··
 9-17 ··  ··  ··  ··  NO  ··  ··  ··  ··
18-26 ··  ··  ··  OU  HB  ES  ··  ··  ··
27-35 ··  ··  ··  ··  SU  ··  ··  ··  ··
36-44 RE  ··  ··  ··  FE  ··  ··  ··  ··
```

`··` : vitre de remplissage.

| Slot | Code | Objet | Nom | Contenu | Clic |
| --- | --- | --- | --- | --- | --- |
| 4 | BI | icône du biome | Nom du biome | Joueurs dans le biome | Aucun |
| 13 | NO | `minecraft:soul_lantern` | Relais Nord | Joueurs à moins de 200 blocs du relais | Clic : téléporte |
| 21 | OU | `minecraft:soul_lantern` | Relais Ouest | Idem | Clic : téléporte |
| 22 | HB | `minecraft:lantern` | Hub | Idem | Clic : téléporte |
| 23 | ES | `minecraft:soul_lantern` | Relais Est | Idem | Clic : téléporte |
| 31 | SU | `minecraft:soul_lantern` | Relais Sud | Idem | Clic : téléporte |
| 36 | RE | `minecraft:arrow` | Retour |  | Clic : revient au menu de la dimension |
| 40 | FE | `minecraft:barrier` | Fermer |  | Clic : ferme le menu |

## File d'attente

* Titre de l'inventaire : `STRATA · File d'attente`
* Taille : 27 emplacements, 3 lignes
* Ouverture : automatique quand un biome plein est choisi
* Permission : `strata.player.biomes`
* Retour vers : Voyage
* Remplissage : Vitre grise

```
      0   1   2   3   4   5   6   7   8 
 0-8  ··  ··  ··  ··  ··  ··  ··  ··  ··
 9-17 ··  ··  PQ  ··  BQ  ··  QQ  ··  ··
18-26 ··  ··  ··  ··  ··  ··  ··  ··  ··
```

`··` : vitre de remplissage.

| Slot | Code | Objet | Nom | Contenu | Clic |
| --- | --- | --- | --- | --- | --- |
| 11 | PQ | `minecraft:clock` | Position | Position dans la file, temps d'attente estimé, priorité du grade | Aucun |
| 13 | BQ | icône du biome | Biome demandé | Joueurs 250 / 250 | Aucun |
| 15 | QQ | `minecraft:red_concrete` | Quitter la file |  | Clic : quitte la file |

## Valeurs

* Titre de l'inventaire : `STRATA · Valeurs`
* Taille : 54 emplacements, 6 lignes
* Ouverture : `/valeurs [biome]`, option Minerais des PNJ
* Permission : `strata.player.valeurs`
* Retour vers : Voyage
* Remplissage : Vitre grise `minecraft:gray_stained_glass_pane`, sans nom

```
      0   1   2   3   4   5   6   7   8 
 0-8  ··  ··  ··  ··  HD  ··  ··  ··  ··
 9-17 ··  ··  ··  ··  ··  ··  ··  ··  ··
18-26 ··  OR  OR  OR  OR  OR  OR  OR  ··
27-35 ··  OR  OR  ··  ··  ··  ··  ··  ··
36-44 ··  ··  ··  ··  BI  ··  ··  ··  ··
45-53 RE  ··  ··  ··  FE  ··  ··  ··  SO
```

`··` : vitre de remplissage.

| Slot | Code | Objet | Nom | Contenu | Clic |
| --- | --- | --- | --- | --- | --- |
| 4 | HD | icône du biome | Nom du biome | Minerai favori, valeur moyenne d'un bloc sans bonus et avec les bonus du joueur | Aucun |
| 19 | OR | bloc du minerai | Minerais | Bloc principal et minerais du biome, slots 19 à 25, 28 et 29 : rareté, taux, valeur de base, valeur de vente pour le joueur (bonus, MP et MR compris), pioche ou armure qui l'utilise | Aucun |
| 40 | BI | `minecraft:compass` | Autre biome |  | Clic : ouvre Voyage pour choisir un biome |
| 45, 49, 53 | RE, FE, SO | Barre de navigation | Voir [Conventions](menus.md) | | |

Sans argument, `/valeurs` affiche le biome où se trouve le joueur, ou les Plaines au spawn. L'option Minerais d'un PNJ ouvre le premier biome de sa dimension.

## 🚀 Téléportation

* Délai de 5 s sans bouger avant une téléportation vers un hub, un relais ou le spawn. Grades Héros et supérieurs : immédiat.
* Le joueur ne peut être téléporté que dans un biome débloqué dans son cycle en cours.
* Arrivée sur une plateforme protégée du hub ou du relais, jamais dans la zone minable.
* File d'attente : priorité 2 pour Immortal, priorité 1 pour Légende et Monarque, puis ordre d'arrivée. Une place réservée expire 30 s après l'annonce « C'est ton tour ».
