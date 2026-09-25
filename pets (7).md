---
description: Les menus des pets : Pets, fiche d'un pet, Éveil, Traits, Recyclage et Œufs.
---

# 🐾 Menus · Pets

## Pets

* Titre de l'inventaire : `STRATA · Pets`
* Taille : 54 emplacements, 6 lignes
* Ouverture : `/pets`, Menu principal
* Permission : `strata.player.pets`
* Retour vers : Menu principal
* Remplissage : Vitre grise `minecraft:gray_stained_glass_pane`, sans nom

```
      0   1   2   3   4   5   6   7   8 
 0-8  ··  ··  ··  ··  HD  ··  ··  ··  ··
 9-17 ··  A1  ··  A2  ··  A3  ··  A4  ··
18-26 ··  LP  LP  LP  LP  LP  LP  LP  ··
27-35 ··  LP  LP  LP  LP  LP  LP  LP  ··
36-44 ··  LP  LP  LP  LP  LP  LP  LP  ··
45-53 RE  ··  PP  FI  FE  TR  PS  ··  SO
```

`··` : vitre de remplissage.

| Slot | Code | Objet | Nom | Contenu | Clic |
| --- | --- | --- | --- | --- | --- |
| 4 | HD | `minecraft:lead` | Pets | Emplacements utilisés 2 / 3, bonus totaux des pets actifs par type | Aucun |
| 10 | A1 | pet actif ou minecraft:iron_bars | Emplacement 1 | Pet actif : nom, rareté, niveau, étoiles, bonus | Gauche : retirer. Droit : fiche |
| 12 | A2 | pet actif ou minecraft:iron_bars | Emplacement 2 | Verrouillé : « ✖ Premier Prestige V » | Idem |
| 14 | A3 | pet actif ou minecraft:iron_bars | Emplacement 3 | Verrouillé : « ✖ Renaissance 1 » | Idem |
| 16 | A4 | pet actif ou minecraft:iron_bars | Emplacement 4 | Verrouillé : « ✖ Renaissance 4 » | Idem |
| 19 | LP | modèle du pet | Pets possédés | 21 par page, slots 19 à 25, 28 à 34, 37 à 43 | Gauche : équiper. Droit : fiche |
| 48 | FI | `minecraft:hopper` | Filtre | Tous, Argent, XP, Fortune, Éclats, Chance, Renaissance | Clic : filtre suivant |
| 50 | TR | `minecraft:comparator` | Tri | Rareté, niveau, type, date d'obtention | Clic : tri suivant |
| 45, 47, 49, 51, 53 | RE, PP, FE, PS, SO | Barre de navigation | Voir [Conventions](menus.md) | | |

Les slots marqués `LP` suivent le format du slot 19. Les slots 11, 13 et 15 sont des vitres.

* **Équiper** : le pet va dans le premier emplacement libre. Si un pet du même type de bonus est déjà actif, il est remplacé : un seul pet actif par type.
* Pet actif dans la liste : brillance et « ▶ Actif ».
* Pet prêt pour l'Éveil : ligne « ● Éveil disponible ».
* Les pets s'affichent avec leur modèle d'asset existant ; aucun nouvel asset.

## Fiche du pet

* Titre de l'inventaire : `STRATA · Fiche du pet`
* Taille : 54 emplacements, 6 lignes
* Ouverture : clic droit sur un pet
* Permission : `strata.player.pets`
* Retour vers : Pets
* Remplissage : Vitre grise `minecraft:gray_stained_glass_pane`, sans nom

```
      0   1   2   3   4   5   6   7   8 
 0-8  ··  ··  ··  ··  PT  ··  ··  ··  ··
 9-17 ··  ··  ··  ··  ··  ··  ··  ··  ··
18-26 ··  ··  LV  ··  EV  ··  TA  ··  ··
27-35 ··  ··  ··  EQ  ··  RC  ··  ··  ··
36-44 ··  ··  ··  ··  OB  ··  ··  ··  ··
45-53 RE  ··  ··  ··  FE  ··  ··  ··  SO
```

`··` : vitre de remplissage.

| Slot | Code | Objet | Nom | Contenu | Clic |
| --- | --- | --- | --- | --- | --- |
| 4 | PT | modèle du pet | Nom du pet | Rareté, type, niveau, étoiles, bonus actuel, trait, date d'obtention | Aucun |
| 20 | LV | `minecraft:experience_bottle` | Niveau | Niveau / 40, XP actuelle et XP du niveau suivant, XP de pet par bloc | Aucun |
| 22 | EV | `minecraft:nether_star` | Éveil | Étoiles, conditions de l'étoile suivante : niveau, Essences, minerais, chacune ✔ ou ✖ | Clic : éveille, avec confirmation |
| 24 | TA | `minecraft:enchanted_book` | Trait | Trait actuel, ou « ✖ Débloqué au niveau 10 » | Clic : ouvre Traits |
| 30 | EQ | `minecraft:lead` | Équiper ou retirer | État actif ou non | Clic : équipe ou retire |
| 32 | RC | `minecraft:grindstone` | Recycler | Essences obtenues : 1 de sa rareté plus la moitié des Essences de ses étoiles. Détruit le trait | Clic : confirmation, délai de 3 s pour Légendaire et Mythique |
| 40 | OB | `minecraft:book` | Obtention | Source du pet : Œuf, boss, caisse, Renaissance | Aucun |
| 45, 49, 53 | RE, FE, SO | Barre de navigation | Voir [Conventions](menus.md) | | |

* Un pet actif ne peut pas être recyclé : il faut d'abord le retirer.
* Le Phénix ne peut pas être recyclé : l'objet Recycler affiche « ✖ Pet unique ».

## Traits

* Titre de l'inventaire : `STRATA · Traits`
* Taille : 54 emplacements, 6 lignes
* Ouverture : `/traits` puis choix d'un pet, ou objet Trait de la fiche
* Permission : `strata.player.traits`
* Retour vers : Fiche du pet
* Remplissage : Vitre grise `minecraft:gray_stained_glass_pane`, sans nom

```
      0   1   2   3   4   5   6   7   8 
 0-8  ··  ··  ··  ··  PT  ··  ··  ··  ··
 9-17 ··  ··  ··  ··  ··  ··  ··  ··  ··
18-26 ··  ··  TA  ··  LT  ··  PB  ··  ··
27-35 ··  ··  RR  ··  ··  ··  RV  ··  ··
36-44 ··  ··  ··  ··  ··  ··  ··  ··  ··
45-53 RE  ··  ··  ··  FE  ··  ··  ··  SO
```

`··` : vitre de remplissage.

| Slot | Code | Objet | Nom | Contenu | Clic |
| --- | --- | --- | --- | --- | --- |
| 4 | PT | modèle du pet | Pet | Pet concerné et son trait | Aucun |
| 20 | TA | `minecraft:enchanted_book` | Trait actuel | Type, rareté, valeur | Aucun |
| 22 | LT | `minecraft:paper` | Les 8 traits | Effet et valeurs par rareté | Aucun |
| 24 | PB | `minecraft:book` | Probabilités | Table de rareté, compteur de garantie 12 / 40 | Aucun |
| 29 | RR | `minecraft:amethyst_shard` | Reroll complet | 10 Cristaux. Nouveau type et nouvelle rareté | Clic : reroll |
| 33 | RV | `minecraft:echo_shard` | Reroll avec type verrouillé | 30 Cristaux. Garde le type, tire la rareté | Clic : reroll |
| 45, 49, 53 | RE, FE, SO | Barre de navigation | Voir [Conventions](menus.md) | | |

* `/traits` sans pet choisi ouvre la liste des pets de niveau 10 ou plus, au format du menu Pets.
* Confirmation : demandée si le trait actuel est Épique ou mieux. Pour les traits de rareté inférieure, la confirmation peut être coupée dans `/parametres`.
* Après un reroll, le nouveau trait s'affiche 2 s en brillance, avec le son `block.enchantment_table.use`. Un trait Mythique est annoncé à tout le serveur.

## Œufs

* Titre de l'inventaire : `STRATA · Œufs`
* Taille : 54 emplacements, 6 lignes
* Ouverture : `/oeufs`, Menu principal
* Permission : `strata.player.oeufs`
* Retour vers : Menu principal
* Remplissage : Vitre grise `minecraft:gray_stained_glass_pane`, sans nom

```
      0   1   2   3   4   5   6   7   8 
 0-8  ··  ··  ··  ··  HD  ··  ··  ··  ··
 9-17 ··  ··  I1  ··  I2  ··  I3  ··  ··
18-26 ··  ··  ··  ··  ··  ··  ··  ··  ··
27-35 ··  O1  ··  O2  ··  O3  ··  O4  ··
36-44 ··  ··  ··  ··  ··  ··  ··  ··  ··
45-53 RE  ··  ··  ··  FE  ··  ··  ··  SO
```

`··` : vitre de remplissage.

| Slot | Code | Objet | Nom | Contenu | Clic |
| --- | --- | --- | --- | --- | --- |
| 4 | HD | `minecraft:sniffer_egg` | Œufs | Œufs en incubation 2 / 3, Œufs dans l'inventaire et dans `/pv` | Aucun |
| 11 | I1 | `minecraft:sniffer_egg` | Incubation 1 | Dimension de l'Œuf, progression 843 / 1 500 blocs, ou « Vide » | Aucun |
| 13 | I2 | `minecraft:sniffer_egg` | Incubation 2 | Idem | Aucun |
| 15 | I3 | `minecraft:sniffer_egg` | Incubation 3 | Idem | Aucun |
| 28 | O1 | `minecraft:grass_block` | Œuf de l'Overworld | Pets possibles et probabilités, pets déjà possédés cochés | Aucun |
| 30 | O2 | `minecraft:netherrack` | Œuf du Nether | Idem | Aucun |
| 32 | O3 | `minecraft:end_stone` | Œuf de l'End | Idem | Aucun |
| 34 | O4 | `minecraft:calcite` | Œuf de l'Aether | Idem | Aucun |
| 45, 49, 53 | RE, FE, SO | Barre de navigation | Voir [Conventions](menus.md) | | |

* Un Œuf est un objet `minecraft:sniffer_egg` lié au joueur, nommé et coloré selon sa dimension.
* Les 3 Œufs en incubation sont les 3 premiers Œufs de l'inventaire, barre rapide de gauche à droite puis inventaire de haut en bas. Un Œuf rangé dans `/pv` n'incube pas.
* À l'éclosion, le pet va directement dans le menu Pets. Titre à l'écran, son `entity.chicken.egg`. Pet Légendaire : annonce au joueur ; pet Mythique : annonce à tout le serveur.
