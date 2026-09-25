---
description: Les menus des collections : Collections, Minerais, Pets et Boss.
---

# 📚 Menus · Collections

## Collections

* Titre de l'inventaire : `STRATA · Collections`
* Taille : 54 emplacements, 6 lignes
* Ouverture : `/collections`, Menu principal
* Permission : `strata.player.collections`
* Retour vers : Menu principal
* Remplissage : Vitre grise `minecraft:gray_stained_glass_pane`, sans nom

```
      0   1   2   3   4   5   6   7   8 
 0-8  ··  ··  ··  ··  HD  ··  ··  ··  ··
 9-17 ··  ··  ··  ··  ··  ··  ··  ··  ··
18-26 ··  MI  ··  PE  ··  AR  ··  GR  ··
27-35 ··  ··  ··  BO  ··  SN  ··  ··  ··
36-44 ··  ··  ··  ··  BN  ··  ··  ··  ··
45-53 RE  ··  ··  ··  FE  ··  ··  ··  SO
```

`··` : vitre de remplissage.

| Slot | Code | Objet | Nom | Contenu | Clic |
| --- | --- | --- | --- | --- | --- |
| 4 | HD | `minecraft:bookshelf` | Collections | Progression totale en %, bonus permanents obtenus : Argent, XP, XP de pet | Aucun |
| 19 | MI | `minecraft:diamond_ore` | Minerais | Minerais découverts 21 / 35, paliers IV 3 / 35 | Clic : ouvre Minerais |
| 21 | PE | `minecraft:lead` | Pets | Pets découverts 9 / 18 | Clic : ouvre la collection de pets |
| 23 | AR | `minecraft:iron_chestplate` | Armures | Armures complètes 4 / 15 | Clic : ouvre `/armure` |
| 25 | GR | `minecraft:leather_chestplate` | Garde-robe | Thèmes complets 2 / 11 | Clic : ouvre `/garderobe` |
| 30 | BO | `minecraft:wither_skeleton_skull` | Boss | Boss vaincus 3 / 4 | Clic : ouvre la collection Boss |
| 32 | SN | `minecraft:note_block` | Sons | Sons possédés 5 / 12 | Clic : ouvre `/sons` |
| 40 | BN | `minecraft:nether_star` | Récompenses | Prochains paliers et leurs récompenses | Aucun |
| 45, 49, 53 | RE, FE, SO | Barre de navigation | Voir [Conventions](menus.md) | | |

## Collection · Minerais

* Titre de l'inventaire : `STRATA · Collection · Minerais`
* Taille : 54 emplacements, 6 lignes
* Ouverture : menu Collections
* Permission : `strata.player.collections`
* Retour vers : Collections
* Remplissage : Vitre grise `minecraft:gray_stained_glass_pane`, sans nom

```
      0   1   2   3   4   5   6   7   8 
 0-8  ··  ··  ··  ··  HD  ··  ··  ··  ··
 9-17 ··  DO  ··  DN  ··  DE  ··  DA  ··
18-26 ··  OR  OR  OR  OR  OR  OR  OR  ··
27-35 ··  OR  OR  ··  ··  ··  ··  ··  ··
36-44 ··  ··  ··  ··  RD  ··  ··  ··  ··
45-53 RE  ··  ··  ··  FE  ··  ··  ··  SO
```

`··` : vitre de remplissage.

| Slot | Code | Objet | Nom | Contenu | Clic |
| --- | --- | --- | --- | --- | --- |
| 4 | HD | `minecraft:diamond_ore` | Minerais | Bonus obtenus : +0,25 % Argent et XP par minerai au palier IV | Aucun |
| 10 | DO | `minecraft:stone` | Onglet Overworld | 8 minerais | Clic : affiche l'Overworld |
| 12 | DN | `minecraft:netherrack` | Onglet Nether | 9 minerais | Clic : affiche le Nether |
| 14 | DE | `minecraft:end_stone` | Onglet End | 9 minerais | Clic : affiche l'End |
| 16 | DA | `minecraft:calcite` | Onglet Aether | 9 minerais | Clic : affiche l'Aether |
| 19 | OR | bloc du minerai | Minerai | Slots 19 à 25, 28 et 29. Rareté, quantité cassée, palier atteint, prochain palier et sa récompense | Aucun |
| 40 | RD | `minecraft:nether_star` | Récompenses de la dimension | Tous au palier II : son. Tous au palier IV : titre et 150 Cristaux | Aucun |
| 45, 49, 53 | RE, FE, SO | Barre de navigation | Voir [Conventions](menus.md) | | |

* Minerai non découvert : `minecraft:gray_dye`, nom « ??? » à la couleur de sa rareté.
* Minerai de l'Overworld : bloc de minerai vanilla (`minecraft:coal_ore`, `minecraft:copper_ore`, etc.). Autres dimensions : bloc de minerai avec sa texture existante.
* Onglet actif : brillance.

## Collection · Pets

* Titre de l'inventaire : `STRATA · Collection · Pets`
* Taille : 54 emplacements, 6 lignes
* Ouverture : menu Collections
* Permission : `strata.player.collections`
* Retour vers : Collections
* Remplissage : Vitre grise `minecraft:gray_stained_glass_pane`, sans nom

```
      0   1   2   3   4   5   6   7   8 
 0-8  ··  ··  ··  ··  HD  ··  ··  ··  ··
 9-17 ··  ··  ··  ··  ··  ··  ··  ··  ··
18-26 ··  PT  PT  PT  PT  PT  PT  PT  ··
27-35 ··  PT  PT  PT  PT  PT  PT  PT  ··
36-44 ··  PT  PT  PT  PT  ··  ··  ··  ··
45-53 RE  ··  ··  ··  FE  ··  ··  ··  SO
```

`··` : vitre de remplissage.

| Slot | Code | Objet | Nom | Contenu | Clic |
| --- | --- | --- | --- | --- | --- |
| 4 | HD | `minecraft:lead` | Pets | Pets découverts, bonus d'XP de pet, prochain palier : 5, 10, 14, 18 | Aucun |
| 19 | PT | modèle du pet ou minecraft:gray_dye | Pets non Premium | 18 pets, slots 19 à 25, 28 à 34, 37 à 40. Découvert : modèle, date. Non découvert : « ??? », rareté et source visibles | Aucun |
| 45, 49, 53 | RE, FE, SO | Barre de navigation | Voir [Conventions](menus.md) | | |

## Collection · Boss

* Titre de l'inventaire : `STRATA · Collection · Boss`
* Taille : 54 emplacements, 6 lignes
* Ouverture : menu Collections
* Permission : `strata.player.collections`
* Retour vers : Collections
* Remplissage : Vitre grise `minecraft:gray_stained_glass_pane`, sans nom

```
      0   1   2   3   4   5   6   7   8 
 0-8  ··  ··  ··  ··  HD  ··  ··  ··  ··
 9-17 ··  ··  ··  ··  ··  ··  ··  ··  ··
18-26 ··  ··  B1  ··  B2  ··  B3  ··  ··
27-35 ··  ··  ··  ··  B4  ··  ··  ··  ··
36-44 ··  ··  ··  ··  ··  ··  ··  ··  ··
45-53 RE  ··  ··  ··  FE  ··  ··  ··  SO
```

`··` : vitre de remplissage.

| Slot | Code | Objet | Nom | Contenu | Clic |
| --- | --- | --- | --- | --- | --- |
| 4 | HD | `minecraft:wither_skeleton_skull` | Boss | Boss vaincus, titre « Tueur de colosses » | Aucun |
| 20 | B1 | `minecraft:zombie_head` | Le Colosse enfoui | Victoires, meilleure part de dégâts, titre, pet obtenu ou compteur de garantie, titre doré à 100 victoires | Aucun |
| 22 | B2 | `minecraft:wither_skeleton_skull` | Le Seigneur des Cendres | Idem | Aucun |
| 24 | B3 | `minecraft:dragon_head` | Le Dévoreur du Vide | Idem | Aucun |
| 31 | B4 | `minecraft:creeper_head` | Le Roi des Tempêtes | Idem | Aucun |
| 45, 49, 53 | RE, FE, SO | Barre de navigation | Voir [Conventions](menus.md) | | |
