---
description: Les menus d'équipement : Armures, fiche d'armure, Garde-robe, thèmes, skins de pioche, Race et Sons.
---

# 🛡️ Menus · Équipement

## Armures

* Titre de l'inventaire : `STRATA · Armures`
* Taille : 54 emplacements, 6 lignes
* Ouverture : `/armure`, Menu principal
* Permission : `strata.player.armure`
* Retour vers : Menu principal
* Remplissage : Vitre grise `minecraft:gray_stained_glass_pane`, sans nom

```
      0   1   2   3   4   5   6   7   8 
 0-8  ··  ··  ··  ··  HD  ··  ··  ··  ··
 9-17 ··  W1  ··  AO  AO  AO  ··  ··  ··
18-26 ··  W2  ··  AN  AN  AN  AN  ··  ··
27-35 ··  W3  ··  AE  AE  AE  AE  ··  ··
36-44 ··  W4  ··  AA  AA  AA  AA  ··  ··
45-53 RE  ··  ··  ··  FE  ··  ··  ··  SO
```

`··` : vitre de remplissage.

| Slot | Code | Objet | Nom | Contenu | Clic |
| --- | --- | --- | --- | --- | --- |
| 4 | HD | `minecraft:iron_chestplate` | Armures | Armures complètes 4 / 15, bonus totaux portés : XP, Argent, Fortune, Chance, Mobilité, bonus de set | Aucun |
| 10 | W1 | casque porté ou minecraft:gray_stained_glass_pane | Casque porté | Armure, statistique | Clic : retire la pièce |
| 12 | AO | plastron de l'armure | Armures de l'Overworld | Fer, Or, Diamant : slots 12 à 14 | Clic : ouvre la fiche de l'armure |
| 19 | W2 | plastron porté | Plastron porté | Idem | Idem |
| 21 | AN | plastron de l'armure | Armures du Nether | Ambre, Sanguine, Rubis, Carmin : slots 21 à 24 | Idem |
| 28 | W3 | jambières portées | Jambières portées | Idem | Idem |
| 30 | AE | plastron de l'armure | Armures de l'End | Galène, Vesper, Quartz fumé, Pulsar : slots 30 à 33 | Idem |
| 37 | W4 | bottes portées | Bottes portées | Idem, Mobilité | Idem |
| 39 | AA | plastron de l'armure | Armures de l'Aether | Aigue-marine, Disthène, Nova, Aurore : slots 39 à 42 | Idem |
| 45, 49, 53 | RE, FE, SO | Barre de navigation | Voir [Conventions](menus.md) | | |

Chaque armure affiche : dimension, rareté, pièces possédées 2 / 4, bonus de set, état « ✔ Complète », « ● Achetable » ou « ✖ Dimension non accessible dans ce cycle ».

Les armures de l'Overworld utilisent les armures vanilla en fer, en or et en diamant. Les 12 autres utilisent les textures de minéral existantes.

## Fiche d'armure

* Titre de l'inventaire : `STRATA · Fiche d'armure`
* Taille : 54 emplacements, 6 lignes
* Ouverture : clic sur une armure
* Permission : `strata.player.armure`
* Retour vers : Armures
* Remplissage : Vitre grise `minecraft:gray_stained_glass_pane`, sans nom

```
      0   1   2   3   4   5   6   7   8 
 0-8  ··  ··  ··  ··  HD  ··  ··  ··  ··
 9-17 ··  ··  ··  ··  ··  ··  ··  ··  ··
18-26 ··  ··  P1  P2  ··  P3  P4  ··  ··
27-35 ··  ··  ··  ··  SE  ··  ··  ··  ··
36-44 ··  ··  ··  ··  MI  ··  ··  ··  ··
45-53 RE  ··  ··  ··  FE  ··  ··  ··  SO
```

`··` : vitre de remplissage.

| Slot | Code | Objet | Nom | Contenu | Clic |
| --- | --- | --- | --- | --- | --- |
| 4 | HD | plastron de l'armure | Nom de l'armure | Dimension, rareté, valeur de l'armure, bonus de set, coût du set | Aucun |
| 20 | P1 | casque | Casque | +X % XP. Coût : Argent et minerai. État : possédé, porté ou à acheter | Gauche : acheter ou porter |
| 21 | P2 | plastron | Plastron | +X % Argent | Idem |
| 23 | P3 | jambières | Jambières | +X % Fortune, 75 % de la valeur | Idem |
| 24 | P4 | bottes | Bottes | +X % Chance, 125 % de la valeur, et Mobilité | Idem |
| 31 | SE | `minecraft:armor_stand` | Porter le set | Porte toutes les pièces possédées de cette armure | Clic : porte |
| 40 | MI | minerai de l'armure | Minerai possédé | Quantité dans l'inventaire et `/pv`, quantité requise par pièce, alerte si ce minerai sert à la prochaine pioche | Aucun |
| 45, 49, 53 | RE, FE, SO | Barre de navigation | Voir [Conventions](menus.md) | | |

* Achat d'une pièce : confirmation standard. Si le minerai dépensé est aussi celui de la prochaine pioche non mémorisée, le Détail l'indique en rouge : « Ce minerai sert aussi à forger la Pioche en Rubis. »
* Une pièce achetée est portée automatiquement si l'emplacement est vide.

## Garde-robe

* Titre de l'inventaire : `STRATA · Garde-robe`
* Taille : 54 emplacements, 6 lignes
* Ouverture : `/garderobe`, Menu principal
* Permission : `strata.player.garderobe`
* Retour vers : Menu principal
* Remplissage : Vitre grise `minecraft:gray_stained_glass_pane`, sans nom

```
      0   1   2   3   4   5   6   7   8 
 0-8  ··  ··  ··  ··  HD  ··  ··  ··  ··
 9-17 ··  ··  ··  ··  ··  ··  ··  ··  ··
18-26 ··  TH  TH  TH  TH  TH  TH  TH  ··
27-35 ··  TH  TH  TH  TH  ··  ··  ··  ··
36-44 ··  ··  RT  ··  SP  ··  PC  ··  ··
45-53 RE  ··  ··  ··  FE  ··  ··  ··  SO
```

`··` : vitre de remplissage.

| Slot | Code | Objet | Nom | Contenu | Clic |
| --- | --- | --- | --- | --- | --- |
| 4 | HD | `minecraft:leather_chestplate` | Garde-robe | Thèmes complets 3 / 11, bonus de collection, pièces possédées, Poussière Chroma | Aucun |
| 19 | TH | casque du thème | Thèmes | 11 thèmes : slots 19 à 25 et 28 à 31. Pièces possédées 2 / 4, rareté, skin de pioche débloqué | Clic : ouvre le thème |
| 38 | RT | `minecraft:bucket` | Retirer tous les skins |  | Clic : retire les 4 skins |
| 40 | SP | `minecraft:painting` | Skins de pioche | Skin actif | Clic : ouvre Skins de pioche |
| 42 | PC | `minecraft:glowstone_dust` | Poussière Chroma | Solde, 30 par pièce Chroma, 60 pour le thème Dragon | Clic : ouvre Échange de Poussière |
| 45, 49, 53 | RE, FE, SO | Barre de navigation | Voir [Conventions](menus.md) | | |

## Thème

* Titre de l'inventaire : `STRATA · Thème`
* Taille : 54 emplacements, 6 lignes
* Ouverture : clic sur un thème
* Permission : `strata.player.garderobe`
* Retour vers : Garde-robe
* Remplissage : Vitre grise `minecraft:gray_stained_glass_pane`, sans nom

```
      0   1   2   3   4   5   6   7   8 
 0-8  ··  ··  ··  ··  HD  ··  ··  ··  ··
 9-17 ··  ··  ··  ··  ··  ··  ··  ··  ··
18-26 ··  S1  S1  S1  S1  ··  AP  ··  ··
27-35 ··  C1  C1  C1  C1  ··  ··  ··  ··
36-44 ··  ··  ··  ··  ··  ··  ··  ··  ··
45-53 RE  ··  ··  ··  FE  ··  ··  ··  SO
```

`··` : vitre de remplissage.

| Slot | Code | Objet | Nom | Contenu | Clic |
| --- | --- | --- | --- | --- | --- |
| 4 | HD | casque du thème | Nom du thème | Rareté, skin de pioche, état de la collection | Aucun |
| 19 | S1 | pièce standard | Casque, Plastron, Jambières, Bottes | Pièces standard : slots 19 à 22. Possédée ou non, appliquée ou non | Clic : applique ou retire |
| 24 | AP | `minecraft:armor_stand` | Appliquer le thème | Applique toutes les pièces possédées, Chroma en priorité si l'option est active | Clic : applique |
| 28 | C1 | pièce Chroma | Pièces Chroma | Slots 28 à 31, affichées seulement si le thème a une version Chroma | Clic : applique ou retire |
| 45, 49, 53 | RE, FE, SO | Barre de navigation | Voir [Conventions](menus.md) | | |

## Skins de pioche

* Titre de l'inventaire : `STRATA · Skins de pioche`
* Taille : 54 emplacements, 6 lignes
* Ouverture : menu Garde-robe, menu Pioche
* Permission : `strata.player.garderobe`
* Retour vers : Garde-robe
* Remplissage : Vitre grise `minecraft:gray_stained_glass_pane`, sans nom

```
      0   1   2   3   4   5   6   7   8 
 0-8  ··  ··  ··  ··  HD  ··  ··  ··  ··
 9-17 ··  ··  ··  ··  ··  ··  ··  ··  ··
18-26 ··  SK  SK  SK  SK  SK  SK  SK  ··
27-35 ··  SK  SK  SK  SK  SK  ··  ··  ··
36-44 ··  ··  ··  ··  AU  ··  ··  ··  ··
45-53 RE  ··  ··  ··  FE  ··  ··  ··  SO
```

`··` : vitre de remplissage.

| Slot | Code | Objet | Nom | Contenu | Clic |
| --- | --- | --- | --- | --- | --- |
| 4 | HD | pioche du joueur | Skin actif |  | Aucun |
| 19 | SK | pioche avec le skin | Skins | 12 skins : un par thème complet, slots 19 à 25 et 28 à 31, et Lueur de Renaissance au slot 32 | Clic : applique |
| 40 | AU | `minecraft:wooden_pickaxe` | Aucun skin | Apparence normale du tier | Clic : retire le skin |
| 45, 49, 53 | RE, FE, SO | Barre de navigation | Voir [Conventions](menus.md) | | |

## Échange de Poussière

* Titre de l'inventaire : `STRATA · Échange de Poussière`
* Taille : 54 emplacements, 6 lignes
* Ouverture : menu Garde-robe
* Permission : `strata.player.garderobe`
* Retour vers : Garde-robe
* Remplissage : Vitre grise `minecraft:gray_stained_glass_pane`, sans nom

```
      0   1   2   3   4   5   6   7   8 
 0-8  ··  ··  ··  ··  HD  ··  ··  ··  ··
 9-17 ··  ··  ··  ··  ··  ··  ··  ··  ··
18-26 ··  TC  TC  TC  TC  TC  TC  TC  ··
27-35 ··  TC  TC  TC  TC  ··  ··  ··  ··
36-44 ··  ··  ··  ··  RG  ··  ··  ··  ··
45-53 RE  ··  ··  ··  FE  ··  ··  ··  SO
```

`··` : vitre de remplissage.

| Slot | Code | Objet | Nom | Contenu | Clic |
| --- | --- | --- | --- | --- | --- |
| 4 | HD | `minecraft:glowstone_dust` | Poussière Chroma | Solde de Poussière | Aucun |
| 19 | TC | casque Chroma du thème | Thèmes Chroma | Thèmes dont la version Chroma est fournie, slots 19 à 25 et 28 à 31 | Clic : ouvre les 4 pièces du thème |
| 40 | RG | `minecraft:book` | Règle | 30 Poussières par pièce, 60 pour une pièce du thème Dragon ; une pièce déjà possédée n'est pas proposée | Aucun |
| 45, 49, 53 | RE, FE, SO | Barre de navigation | Voir [Conventions](menus.md) | | |

Clic sur un thème : sous-menu de 27 emplacements, les 4 pièces Chroma aux slots 10, 12, 14 et 16, clic : échange avec confirmation standard.

## Race

* Titre de l'inventaire : `STRATA · Race`
* Taille : 54 emplacements, 6 lignes
* Ouverture : `/race`, Menu principal
* Permission : `strata.player.race`
* Retour vers : Menu principal
* Remplissage : Vitre grise `minecraft:gray_stained_glass_pane`, sans nom

```
      0   1   2   3   4   5   6   7   8 
 0-8  ··  ··  ··  ··  HD  ··  ··  ··  ··
 9-17 ··  R1  ··  R2  ··  R3  ··  R4  ··
18-26 ··  R5  ··  R6  ··  R7  ··  R8  ··
27-35 ··  ··  ··  ··  RR  ··  ··  ··  ··
36-44 ··  ··  ··  ··  ··  ··  ··  ··  ··
45-53 RE  ··  ··  ··  FE  ··  ··  ··  SO
```

`··` : vitre de remplissage.

| Slot | Code | Objet | Nom | Contenu | Clic |
| --- | --- | --- | --- | --- | --- |
| 4 | HD | `minecraft:armor_stand` | Ta race | Race, rareté, bonus, talent | Aucun |
| 10 | R1 | `minecraft:player_head` | Humain | Rareté, probabilité, bonus, talent. « ▶ Ta race » si c'est la race actuelle | Aucun |
| 12 | R2 | `minecraft:player_head` | Nain | Idem | Aucun |
| 14 | R3 | `minecraft:player_head` | Gobelin | Idem | Aucun |
| 16 | R4 | `minecraft:player_head` | Elfe | Idem | Aucun |
| 19 | R5 | `minecraft:player_head` | Gnome | Idem | Aucun |
| 21 | R6 | `minecraft:player_head` | Golem | Idem | Aucun |
| 23 | R7 | `minecraft:player_head` | Draconide | Idem | Aucun |
| 25 | R8 | `minecraft:player_head` | Céleste | Idem | Aucun |
| 31 | RR | `minecraft:amethyst_cluster` | Reroll | 60 Cristaux. Compteur de garantie 7 / 15 | Clic : confirmation, puis tirage |
| 45, 49, 53 | RE, FE, SO | Barre de navigation | Voir [Conventions](menus.md) | | |

## Choix de race

* Titre de l'inventaire : `STRATA · Choix de race`
* Taille : 27 emplacements, 3 lignes
* Ouverture : automatique après un reroll
* Permission : `strata.player.race`
* Remplissage : Vitre grise

```
      0   1   2   3   4   5   6   7   8 
 0-8  ··  ··  ··  ··  ··  ··  ··  ··  ··
 9-17 ··  ··  AR  ··  CP  ··  NV  ··  ··
18-26 ··  ··  ··  ··  ··  ··  ··  ··  ··
```

`··` : vitre de remplissage.

| Slot | Code | Objet | Nom | Contenu | Clic |
| --- | --- | --- | --- | --- | --- |
| 11 | AR | tête de l'ancienne race | Garder : Nain | Bonus et talent | Clic : garde l'ancienne race |
| 13 | CP | `minecraft:paper` | Comparaison | Bonus et talents des deux races côte à côte | Aucun |
| 15 | NV | tête de la nouvelle race | Prendre : Elfe | Bonus et talent | Clic : prend la nouvelle race |

* Les têtes de race utilisent des têtes de joueur à texture existante, choisies par la direction ; aucune ressource nouvelle.
* Le menu de choix ne peut pas être fermé avec Échap tant qu'aucun choix n'est fait : il se rouvre. En cas de déconnexion, il se rouvre à la connexion suivante ; la race actuelle reste active en attendant.
* Tirer la race déjà possédée : message « Même race », le reroll compte pour la garantie.

## Sons

* Titre de l'inventaire : `STRATA · Sons`
* Taille : 54 emplacements, 6 lignes
* Ouverture : `/sons`, Menu principal
* Permission : `strata.player.sons`
* Retour vers : Menu principal
* Remplissage : Vitre grise `minecraft:gray_stained_glass_pane`, sans nom

```
      0   1   2   3   4   5   6   7   8 
 0-8  ··  ··  ··  ··  HD  ··  ··  ··  ··
 9-17 ··  ··  ··  ··  ··  ··  ··  ··  ··
18-26 ··  SN  SN  SN  SN  SN  SN  SN  ··
27-35 ··  SN  SN  SN  SN  SN  ··  ··  ··
36-44 ··  ··  ··  CR  FQ  IM  ··  ··  ··
45-53 RE  ··  ··  ··  FE  ··  ··  ··  SO
```

`··` : vitre de remplissage.

| Slot | Code | Objet | Nom | Contenu | Clic |
| --- | --- | --- | --- | --- | --- |
| 4 | HD | `minecraft:note_block` | Sons | Son actif, fréquence, sons possédés 5 / 12 | Aucun |
| 19 | SN | icône du son | Sons de la collection | 12 sons : slots 19 à 25 et 28 à 32 | Gauche : activer. Droit : écouter |
| 39 | CR | `minecraft:golden_helmet` | Couronne | Son de grade Monarque, affiché seulement avec le grade | Idem |
| 40 | FQ | `minecraft:comparator` | Fréquence | Tous les blocs, minerais seulement, minerais Rares et plus, désactivé | Clic : réglage suivant |
| 41 | IM | `minecraft:totem_of_undying` | Immortel | Son de grade Immortal, affiché seulement avec le grade | Idem |
| 45, 49, 53 | RE, FE, SO | Barre de navigation | Voir [Conventions](menus.md) | | |

| Son | Icône |
| --- | --- |
| Classique | `minecraft:stone` |
| Pierre | `minecraft:deepslate` |
| Cendre | `minecraft:campfire` |
| Écho | `minecraft:sculk` |
| Carillon | `minecraft:amethyst_block` |
| Pièces | `minecraft:gold_nugget` |
| Forge | `minecraft:anvil` |
| Cloche | `minecraft:bell` |
| Verre | `minecraft:glass` |
| Aube | `minecraft:respawn_anchor` |
| Tintement | `minecraft:note_block` |
| Éternité | `minecraft:end_portal_frame` |

Un son non possédé affiche sa source d'obtention. Clic droit « écouter » : le son est joué au joueur seul, une fois, même s'il n'est pas possédé.
