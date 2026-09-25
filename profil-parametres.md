---
description: Les menus Profil, Statistiques, Classements, Titres, Paramètres et Minerais protégés.
---

# 👤 Menus · Profil et paramètres

## Profil

* Titre de l'inventaire : `STRATA · Profil`
* Taille : 54 emplacements, 6 lignes
* Ouverture : `/profil [joueur]`, Menu principal
* Permission : `strata.player.profil`
* Retour vers : Menu principal
* Remplissage : Vitre grise `minecraft:gray_stained_glass_pane`, sans nom

```
      0   1   2   3   4   5   6   7   8 
 0-8  ··  ··  ··  ··  PH  ··  ··  ··  ··
 9-17 ··  ··  ··  ··  ··  ··  ··  ··  ··
18-26 ··  PI  PE  AR  SK  CO  BO  GU  ··
27-35 ··  ··  ··  ··  ST  ··  ··  ··  ··
36-44 ··  ··  ··  ··  PA  ··  ··  ··  ··
45-53 RE  ··  ··  ··  FE  ··  ··  ··  SO
```

`··` : vitre de remplissage.

| Slot | Code | Objet | Nom | Contenu | Clic |
| --- | --- | --- | --- | --- | --- |
| 4 | PH | `minecraft:player_head` | Pseudo | Grade, race, Renaissance, Prestige, guilde, titre, première connexion, temps de jeu | Aucun |
| 19 | PI | pioche du joueur | Pioche | Tier, niveau, skin | Aucun |
| 20 | PE | `minecraft:lead` | Pets actifs | Noms, niveaux, étoiles, traits | Aucun |
| 21 | AR | plastron porté | Armure | Pièces portées, bonus de set | Aucun |
| 22 | SK | `minecraft:painting` | Apparence | Skins portés, son de minage | Aucun |
| 23 | CO | `minecraft:bookshelf` | Collections | Progression en % | Aucun |
| 24 | BO | `minecraft:wither_skeleton_skull` | Boss | Victoires par boss | Aucun |
| 25 | GU | bannière de la guilde | Guilde | Nom, niveau, rôle | Aucun |
| 31 | ST | `minecraft:writable_book` | Statistiques |  | Clic : ouvre Statistiques de ce joueur |
| 40 | PA | `minecraft:comparator` | Paramètres | Profil personnel seulement | Clic : ouvre Paramètres |
| 45, 49, 53 | RE, FE, SO | Barre de navigation | Voir [Conventions](menus.md) | | |

## Statistiques

* Titre de l'inventaire : `STRATA · Statistiques`
* Taille : 54 emplacements, 6 lignes
* Ouverture : `/stats [joueur]`, menu Profil
* Permission : `strata.player.stats`
* Retour vers : Profil
* Remplissage : Vitre grise `minecraft:gray_stained_glass_pane`, sans nom

```
      0   1   2   3   4   5   6   7   8 
 0-8  ··  ··  ··  ··  HD  ··  ··  ··  ··
 9-17 ··  ··  ··  ··  ··  ··  ··  ··  ··
18-26 ··  S1  S2  S3  S4  S5  S6  S7  ··
27-35 ··  ··  ··  ··  ··  ··  ··  ··  ··
36-44 ··  ··  ··  ··  PO  ··  ··  ··  ··
45-53 RE  ··  ··  ··  FE  ··  ··  ··  SO
```

`··` : vitre de remplissage.

| Slot | Code | Objet | Nom | Contenu | Clic |
| --- | --- | --- | --- | --- | --- |
| 4 | HD | `minecraft:writable_book` | Statistiques | Joueur, portée affichée | Aucun |
| 19 | S1 | `minecraft:diamond_pickaxe` | Minage | Blocs cassés, minerais par rareté, temps de minage actif | Aucun |
| 20 | S2 | `minecraft:gold_ingot` | Économie | Argent, Éclats, Cristaux gagnés | Aucun |
| 21 | S3 | `minecraft:beacon` | Progression | Prestiges, Renaissances, meilleurs temps | Aucun |
| 22 | S4 | `minecraft:lead` | Pets | Pets découverts, niveau 40, ★3, Œufs éclos | Aucun |
| 23 | S5 | `minecraft:wither_skeleton_skull` | Boss | Victoires, dégâts, meilleure part, pets de boss | Aucun |
| 24 | S6 | `minecraft:clock` | Événements | Chat réaction gagnés, podiums de Concours, votes | Aucun |
| 25 | S7 | `minecraft:recovery_compass` | Trouvailles | Cristaux, Œufs, clés trouvés en minant | Aucun |
| 40 | PO | `minecraft:hopper` | Portée | Cycle, Renaissance, Vie, Semaine | Clic : portée suivante |
| 45, 49, 53 | RE, FE, SO | Barre de navigation | Voir [Conventions](menus.md) | | |

## Classements

* Titre de l'inventaire : `STRATA · Classements`
* Taille : 54 emplacements, 6 lignes
* Ouverture : `/top [catégorie]`, Menu principal
* Permission : `strata.player.top`
* Retour vers : Menu principal
* Remplissage : Vitre grise `minecraft:gray_stained_glass_pane`, sans nom

```
      0   1   2   3   4   5   6   7   8 
 0-8  ··  ··  ··  ··  HD  ··  ··  ··  ··
 9-17 ··  ··  ··  ··  ··  ··  ··  ··  ··
18-26 ··  C1  C2  C3  C4  C5  C6  C7  ··
27-35 ··  ··  C8  CN  C9  ··  CG  ··  ··
36-44 ··  ··  ··  ··  ··  ··  ··  ··  ··
45-53 RE  ··  ··  ··  FE  ··  ··  ··  SO
```

`··` : vitre de remplissage.

| Slot | Code | Objet | Nom | Contenu | Clic |
| --- | --- | --- | --- | --- | --- |
| 4 | HD | `minecraft:gold_block` | Classements | Mise à jour toutes les 10 minutes | Aucun |
| 19 | C1 | `minecraft:beacon` | Progression |  | Clic : ouvre le classement |
| 20 | C2 | `minecraft:totem_of_undying` | Meilleur temps de Renaissance | Par numéro de Renaissance | Idem |
| 21 | C3 | `minecraft:clock` | Meilleur temps par rang de Prestige |  | Idem |
| 22 | C4 | `minecraft:iron_pickaxe` | Blocs cassés, semaine |  | Idem |
| 23 | C5 | `minecraft:diamond_pickaxe` | Blocs cassés, vie |  | Idem |
| 24 | C6 | `minecraft:wither_skeleton_skull` | Dégâts de boss, semaine |  | Idem |
| 25 | C7 | `minecraft:oak_sign` | Chat réaction, semaine |  | Idem |
| 29 | C8 | `minecraft:emerald_ore` | Minerais Mythiques |  | Idem |
| 30 | CN | `minecraft:recovery_compass` | Meilleur temps de Nouveau départ | Après la Renaissance 10 | Idem |
| 31 | C9 | `minecraft:bookshelf` | Collections |  | Idem |
| 33 | CG | `minecraft:white_banner` | Guildes, semaine |  | Idem |
| 45, 49, 53 | RE, FE, SO | Barre de navigation | Voir [Conventions](menus.md) | | |

## Classement

* Titre de l'inventaire : `STRATA · Classement`
* Taille : 54 emplacements, 6 lignes
* Ouverture : clic sur une catégorie
* Permission : `strata.player.top`
* Retour vers : Classements
* Remplissage : Vitre grise `minecraft:gray_stained_glass_pane`, sans nom

```
      0   1   2   3   4   5   6   7   8 
 0-8  ··  ··  ··  ··  HD  ··  ··  ··  ··
 9-17 ··  TP  TP  TP  TP  TP  TP  TP  ··
18-26 ··  TP  TP  TP  TP  TP  TP  TP  ··
27-35 ··  TP  TP  TP  TP  TP  TP  TP  ··
36-44 ··  TP  TP  TP  MP  TP  TP  TP  ··
45-53 RE  ··  PP  ··  FE  ··  PS  ··  SO
```

`··` : vitre de remplissage.

| Slot | Code | Objet | Nom | Contenu | Clic |
| --- | --- | --- | --- | --- | --- |
| 4 | HD | icône de la catégorie | Nom du classement | Récompense éventuelle, prochaine remise à zéro | Aucun |
| 10 | TP | `minecraft:player_head` | 1er à 27e | 27 par page : slots 10 à 16, 19 à 25, 28 à 34, 37 à 39 et 41 à 43. Place, pseudo, valeur | Clic : ouvre le Profil |
| 40 | MP | `minecraft:compass` | Ta place | Place et valeur du joueur | Aucun |
| 45, 47, 49, 51, 53 | RE, PP, FE, PS, SO | Barre de navigation | Voir [Conventions](menus.md) | | |

## Titres

* Titre de l'inventaire : `STRATA · Titres`
* Taille : 54 emplacements, 6 lignes
* Ouverture : `/titre`, Menu principal
* Permission : `strata.player.titre`
* Retour vers : Menu principal
* Remplissage : Vitre grise `minecraft:gray_stained_glass_pane`, sans nom

```
      0   1   2   3   4   5   6   7   8 
 0-8  ··  ··  ··  ··  HD  ··  ··  ··  ··
 9-17 ··  TI  TI  TI  TI  TI  TI  TI  ··
18-26 ··  TI  TI  TI  TI  TI  TI  TI  ··
27-35 ··  TI  TI  TI  TI  TI  TI  TI  ··
36-44 ··  TI  TI  TI  NO  TI  TI  TI  ··
45-53 RE  ··  PP  ··  FE  ··  PS  ··  SO
```

`··` : vitre de remplissage.

| Slot | Code | Objet | Nom | Contenu | Clic |
| --- | --- | --- | --- | --- | --- |
| 4 | HD | `minecraft:name_tag` | Titres | Titre actif, nombre de titres possédés sur le total | Aucun |
| 10 | TI | `minecraft:name_tag` | Titre | 27 par page : mêmes slots que les classements. Aperçu dans le chat, source, date d'obtention | Clic : active |
| 40 | NO | `minecraft:paper` | Aucun titre |  | Clic : retire le titre |
| 45, 47, 49, 51, 53 | RE, PP, FE, PS, SO | Barre de navigation | Voir [Conventions](menus.md) | | |

## Paramètres

* Titre de l'inventaire : `STRATA · Paramètres`
* Taille : 54 emplacements, 6 lignes
* Ouverture : `/parametres`, Menu principal
* Permission : `strata.player.parametres`
* Retour vers : Menu principal
* Remplissage : Vitre grise `minecraft:gray_stained_glass_pane`, sans nom

```
      0   1   2   3   4   5   6   7   8 
 0-8  ··  ··  ··  ··  HD  ··  ··  ··  ··
 9-17 ··  P1  P2  P3  P4  P5  P6  P7  ··
18-26 ··  P8  P9  PA  PB  PC  PD  PH  ··
27-35 ··  PF  PG  PI  ··  ··  ··  ··  ··
36-44 ··  ··  ··  ··  ··  ··  ··  ··  ··
45-53 RE  ··  ··  ··  FE  ··  ··  ··  SO
```

`··` : vitre de remplissage.

| Slot | Code | Objet | Nom | Contenu | Clic |
| --- | --- | --- | --- | --- | --- |
| 4 | HD | `minecraft:comparator` | Paramètres | Chaque clic passe à la valeur suivante. Valeur active en vert | Aucun |
| 10 | P1 | `minecraft:lead` | Affichage des pets | Tous, les miens seulement, aucun | Clic : valeur suivante |
| 11 | P2 | `minecraft:bell` | Annonces de minerais | Toutes, Épique et plus, Légendaire et plus, aucune | Idem |
| 12 | P3 | `minecraft:note_block` | Sons de minage | Fréquence, comme dans `/sons` | Idem |
| 13 | P4 | `minecraft:gold_ingot` | Récapitulatif de vente automatique | Toutes les 60 s, désactivé | Idem |
| 14 | P5 | `minecraft:chest` | Minerais protégés | Minerais jamais vendus par `/sell` ni la vente automatique | Clic : ouvre la liste |
| 15 | P6 | `minecraft:nether_star` | Objet Menu dans la barre | Oui, non | Idem |
| 16 | P7 | `minecraft:paper` | Rappel de vote | Oui, non | Idem |
| 19 | P8 | `minecraft:writable_book` | Messages privés | Tous, guilde seulement, personne | Idem |
| 20 | P9 | `minecraft:ender_pearl` | Demandes de téléportation | Acceptées, refusées. Équivaut à `/tptoggle` | Idem |
| 21 | PA | `minecraft:oak_sign` | Chat global | Affiché, masqué | Idem |
| 22 | PB | `minecraft:clock` | Annonces d'événements | Toutes, ma dimension seulement, aucune | Idem |
| 23 | PC | `minecraft:amethyst_shard` | Confirmer les rerolls de trait | Oui, non. Toujours oui pour un trait Épique ou mieux | Idem |
| 24 | PD | `minecraft:glowstone_dust` | Chroma en priorité | Oui, non | Idem |
| 25 | PH | `minecraft:wither_skeleton_skull` | Dégâts de boss en barre d'action | Oui, non | Idem |
| 28 | PF | `minecraft:item_frame` | Tableau latéral | Affiché, masqué | Idem |
| 29 | PG | `minecraft:firework_star` | Particules des autres joueurs | Affichées, masquées | Idem |
| 30 | PI | `minecraft:hopper` | Vente automatique | Active, coupée. Équivaut à `/autosell`. Affiché seulement si débloquée | Idem |
| 45, 49, 53 | RE, FE, SO | Barre de navigation | Voir [Conventions](menus.md) | | |

## Minerais protégés

* Titre de l'inventaire : `STRATA · Minerais protégés`
* Taille : 54 emplacements, 6 lignes
* Ouverture : menu Paramètres
* Permission : `strata.player.parametres`
* Retour vers : Paramètres
* Remplissage : Vitre grise `minecraft:gray_stained_glass_pane`, sans nom

```
      0   1   2   3   4   5   6   7   8 
 0-8  ··  ··  ··  ··  HD  ··  ··  ··  ··
 9-17 ··  DO  ··  DN  ··  DE  ··  DA  ··
18-26 ··  MP  MP  MP  MP  MP  MP  MP  ··
27-35 ··  MP  MP  ··  ··  ··  ··  ··  ··
36-44 ··  ··  ··  ··  RZ  ··  ··  ··  ··
45-53 RE  ··  ··  ··  FE  ··  ··  ··  SO
```

`··` : vitre de remplissage.

| Slot | Code | Objet | Nom | Contenu | Clic |
| --- | --- | --- | --- | --- | --- |
| 4 | HD | `minecraft:chest` | Minerais protégés | Par défaut : minerai de la prochaine pioche non mémorisée et minerais des armures non achetées | Aucun |
| 10 | DO | `minecraft:stone` | Onglet Overworld |  | Clic : affiche la dimension |
| 12 | DN | `minecraft:netherrack` | Onglet Nether |  | Idem |
| 14 | DE | `minecraft:end_stone` | Onglet End |  | Idem |
| 16 | DA | `minecraft:calcite` | Onglet Aether |  | Idem |
| 19 | MP | bloc du minerai | Minerai | Slots 19 à 25, 28 et 29. « Protégé » en vert ou « Vendu » en gris | Clic : bascule |
| 40 | RZ | `minecraft:water_bucket` | Réglage par défaut |  | Clic : rétablit la protection automatique |
| 45, 49, 53 | RE, FE, SO | Barre de navigation | Voir [Conventions](menus.md) | | |
