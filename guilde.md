---
description: Les menus de guilde : sans guilde, invitations, guilde, paramètres, couleur du tag, membres, actions, banque et défis.
---

# 🛡️ Menus · Guilde

## Guilde, sans guilde

* Titre de l'inventaire : `STRATA · Guilde`
* Taille : 54 emplacements, 6 lignes
* Ouverture : `/guilde` sans guilde
* Permission : `strata.player.guilde`
* Retour vers : Menu principal
* Remplissage : Vitre grise `minecraft:gray_stained_glass_pane`, sans nom

```
      0   1   2   3   4   5   6   7   8 
 0-8  ··  ··  ··  ··  HD  ··  ··  ··  ··
 9-17 ··  ··  ··  ··  ··  ··  ··  ··  ··
18-26 ··  ··  CR  ··  IN  ··  TO  ··  ··
27-35 ··  ··  ··  ··  ··  ··  ··  ··  ··
36-44 ··  ··  ··  ··  ··  ··  ··  ··  ··
45-53 RE  ··  ··  ··  FE  ··  ··  ··  SO
```

`··` : vitre de remplissage.

| Slot | Code | Objet | Nom | Contenu | Clic |
| --- | --- | --- | --- | --- | --- |
| 4 | HD | `minecraft:white_banner` | Sans guilde | Avantages d'une guilde | Aucun |
| 20 | CR | `minecraft:writable_book` | Créer une guilde | 50 Cristaux, règles du nom et du tag | Clic : propose `/guilde creer ` dans le chat |
| 22 | IN | `minecraft:paper` | Invitations | Invitations reçues, valables 5 min | Clic : ouvre les invitations |
| 24 | TO | `minecraft:gold_block` | Classement des guildes | Top 10 de la semaine | Clic : ouvre le classement |
| 45, 49, 53 | RE, FE, SO | Barre de navigation | Voir [Conventions](menus.md) | | |

## Invitations

* Titre de l'inventaire : `STRATA · Invitations`
* Taille : 54 emplacements, 6 lignes
* Ouverture : menu Guilde sans guilde
* Permission : `strata.player.guilde`
* Retour vers : Guilde, sans guilde
* Remplissage : Vitre grise `minecraft:gray_stained_glass_pane`, sans nom

```
      0   1   2   3   4   5   6   7   8 
 0-8  ··  ··  ··  ··  HD  ··  ··  ··  ··
 9-17 ··  IV  IV  IV  IV  IV  IV  IV  ··
18-26 ··  IV  IV  IV  IV  IV  IV  IV  ··
27-35 ··  IV  IV  IV  IV  IV  IV  IV  ··
36-44 ··  IV  IV  IV  IV  IV  IV  IV  ··
45-53 RE  ··  ··  ··  FE  ··  ··  ··  SO
```

`··` : vitre de remplissage.

| Slot | Code | Objet | Nom | Contenu | Clic |
| --- | --- | --- | --- | --- | --- |
| 4 | HD | `minecraft:paper` | Invitations | Invitations reçues, valables 5 min | Aucun |
| 10 | IV | bannière de la guilde | [TAG] Nom | 28 par page. Niveau, membres, bonus d'Argent, officier qui invite, temps restant | Gauche : accepter. Droit : refuser |
| 45, 49, 53 | RE, FE, SO | Barre de navigation | Voir [Conventions](menus.md) | | |

## Guilde, membre

* Titre de l'inventaire : `STRATA · Guilde`
* Taille : 54 emplacements, 6 lignes
* Ouverture : `/guilde` avec une guilde
* Permission : `strata.player.guilde`
* Retour vers : Menu principal
* Remplissage : Vitre grise `minecraft:gray_stained_glass_pane`, sans nom

```
      0   1   2   3   4   5   6   7   8 
 0-8  ··  ··  ··  ··  GB  ··  ··  ··  ··
 9-17 ··  ··  ··  ··  ··  ··  ··  ··  ··
18-26 ··  ME  ··  BK  ··  DF  ··  CL  ··
27-35 ··  ··  FV  ··  CG  ··  PG  ··  ··
36-44 ··  ··  ··  ··  QU  ··  ··  ··  ··
45-53 RE  ··  ··  ··  FE  ··  ··  ··  SO
```

`··` : vitre de remplissage.

| Slot | Code | Objet | Nom | Contenu | Clic |
| --- | --- | --- | --- | --- | --- |
| 4 | GB | bannière de la guilde | [TAG] Nom | Niveau 4, XP 34 200 000 / 40 000 000, bonus d'Argent +4 %, membres 19 / 22 avec la Salle agrandie I, banque, place au classement | Aucun |
| 19 | ME | `minecraft:player_head` | Membres | Membres connectés, rôles | Clic : ouvre Membres |
| 21 | BK | `minecraft:amethyst_shard` | Banque | Solde, améliorations achetées | Clic : ouvre Banque |
| 23 | DF | `minecraft:target` | Défis | Défis de la semaine, progression, temps restant | Clic : ouvre Défis |
| 25 | CL | `minecraft:gold_block` | Classements | Place de la guilde | Clic : ouvre le classement |
| 29 | FV | `minecraft:blaze_powder` | Ferveur | Disponible, active avec temps restant, ou recharge. 200 Cristaux de la banque | Clic, officier : active |
| 31 | CG | `minecraft:oak_sign` | Chat de guilde | Canal par défaut : global ou guilde | Clic : bascule |
| 33 | PG | `minecraft:comparator` | Paramètres de guilde | Chef seulement : nom, tag, couleur, chef, dissolution | Clic : ouvre les paramètres |
| 40 | QU | `minecraft:oak_door` | Quitter la guilde | 24 h d'attente avant une autre guilde | Clic : confirmation |
| 45, 49, 53 | RE, FE, SO | Barre de navigation | Voir [Conventions](menus.md) | | |

## Paramètres de guilde

* Titre de l'inventaire : `STRATA · Paramètres de guilde`
* Taille : 54 emplacements, 6 lignes
* Ouverture : menu Guilde, chef seulement
* Permission : `strata.player.guilde`
* Retour vers : Guilde
* Remplissage : Vitre grise `minecraft:gray_stained_glass_pane`, sans nom

```
      0   1   2   3   4   5   6   7   8 
 0-8  ··  ··  ··  ··  HD  ··  ··  ··  ··
 9-17 ··  ··  ··  ··  ··  ··  ··  ··  ··
18-26 ··  ··  RN  TG  CT  BN  CH  ··  ··
27-35 ··  ··  ··  ··  ··  ··  ··  ··  ··
36-44 ··  ··  ··  ··  DS  ··  ··  ··  ··
45-53 RE  ··  ··  ··  FE  ··  ··  ··  SO
```

`··` : vitre de remplissage.

| Slot | Code | Objet | Nom | Contenu | Clic |
| --- | --- | --- | --- | --- | --- |
| 4 | HD | bannière de la guilde | [TAG] Nom | Réglages réservés au chef | Aucun |
| 20 | RN | `minecraft:name_tag` | Renommer | 150 Cristaux de la banque | Clic : propose `/guilde renommer ` dans le chat |
| 21 | TG | `minecraft:oak_sign` | Changer le tag | 150 Cristaux de la banque | Clic : propose `/guilde tag ` dans le chat |
| 22 | CT | `minecraft:white_dye` | Couleur du tag | 100 Cristaux de la banque, niveau 7 ; gratuit pour un chef Monarque ou Immortal | Clic : ouvre Couleur du tag |
| 23 | BN | `minecraft:white_banner` | Bannière | Pose la bannière tenue en main comme bannière de guilde | Clic : enregistre la bannière |
| 24 | CH | `minecraft:golden_helmet` | Transmettre le rôle de chef |  | Clic : ouvre Membres pour choisir |
| 40 | DS | `minecraft:lava_bucket` | Dissoudre la guilde | Banque perdue | Clic : double confirmation, délai de 3 s |
| 45, 49, 53 | RE, FE, SO | Barre de navigation | Voir [Conventions](menus.md) | | |

## Couleur du tag

* Titre de l'inventaire : `STRATA · Couleur du tag`
* Taille : 27 emplacements, 3 lignes
* Ouverture : Paramètres de guilde
* Permission : `strata.player.guilde`
* Retour vers : Paramètres de guilde
* Remplissage : Vitre grise

```
      0   1   2   3   4   5   6   7   8 
 0-8  ··  ··  ··  ··  ··  ··  ··  ··  ··
 9-17 CO  CO  CO  CO  CO  CO  CO  CO  CO
18-26 ··  CO  CO  CO  CO  CO  CO  CO  FE
```

`··` : vitre de remplissage.

| Slot | Code | Objet | Nom | Contenu | Clic |
| --- | --- | --- | --- | --- | --- |
| 9 | CO | colorant | 16 couleurs | Slots 9 à 17 et 19 à 25 : les 16 colorants vanilla, aperçu du tag dans le nom | Clic : applique, confirmation si payant |
| 26 | FE | `minecraft:barrier` | Fermer |  | Clic : ferme le menu |

## Membres

* Titre de l'inventaire : `STRATA · Membres`
* Taille : 54 emplacements, 6 lignes
* Ouverture : menu Guilde
* Permission : `strata.player.guilde`
* Retour vers : Guilde
* Remplissage : Vitre grise `minecraft:gray_stained_glass_pane`, sans nom

```
      0   1   2   3   4   5   6   7   8 
 0-8  ··  ··  ··  ··  HD  ··  ··  ··  ··
 9-17 ··  MB  MB  MB  MB  MB  MB  MB  ··
18-26 ··  MB  MB  MB  MB  MB  MB  MB  ··
27-35 ··  MB  MB  MB  MB  MB  MB  MB  ··
36-44 ··  MB  MB  MB  MB  MB  MB  MB  ··
45-53 RE  ··  PP  ··  FE  ··  PS  ··  SO
```

`··` : vitre de remplissage.

| Slot | Code | Objet | Nom | Contenu | Clic |
| --- | --- | --- | --- | --- | --- |
| 4 | HD | `minecraft:player_head` | Membres | Membres 19 / 22, officiers 3 / 5 | Aucun |
| 10 | MB | `minecraft:player_head` | Membre | 28 par page. Rôle, dernière connexion, contribution de la semaine, XP de guilde totale | Officier : ouvre les actions |
| 45, 47, 49, 51, 53 | RE, PP, FE, PS, SO | Barre de navigation | Voir [Conventions](menus.md) | | |

## Actions sur un membre

* Titre de l'inventaire : `STRATA · Actions sur un membre`
* Taille : 27 emplacements, 3 lignes
* Ouverture : clic d'un officier ou du chef sur un membre
* Permission : `strata.player.guilde`
* Retour vers : Membres
* Remplissage : Vitre grise

```
      0   1   2   3   4   5   6   7   8 
 0-8  ··  ··  ··  ··  ··  ··  ··  ··  ··
 9-17 ··  PR  ··  RT  ··  EX  ··  CH  ··
18-26 ··  ··  ··  ··  ··  ··  ··  ··  ··
```

`··` : vitre de remplissage.

| Slot | Code | Objet | Nom | Contenu | Clic |
| --- | --- | --- | --- | --- | --- |
| 10 | PR | `minecraft:lime_dye` | Promouvoir | Chef seulement | Clic : membre vers officier |
| 12 | RT | `minecraft:orange_dye` | Rétrograder | Chef seulement | Clic : officier vers membre |
| 14 | EX | `minecraft:red_dye` | Exclure | Officier : membres seulement | Clic : confirmation |
| 16 | CH | `minecraft:golden_helmet` | Transmettre le rôle de chef | Chef seulement | Clic : confirmation |

## Banque

* Titre de l'inventaire : `STRATA · Banque`
* Taille : 54 emplacements, 6 lignes
* Ouverture : menu Guilde
* Permission : `strata.player.guilde`
* Retour vers : Guilde
* Remplissage : Vitre grise `minecraft:gray_stained_glass_pane`, sans nom

```
      0   1   2   3   4   5   6   7   8 
 0-8  ··  ··  ··  ··  HD  ··  ··  ··  ··
 9-17 ··  ··  ··  ··  ··  ··  ··  ··  ··
18-26 ··  D1  D2  D3  ··  U1  U2  U3  ··
27-35 ··  ··  ··  ··  ··  ··  ··  ··  ··
36-44 ··  ··  ··  ··  JO  ··  ··  ··  ··
45-53 RE  ··  ··  ··  FE  ··  ··  ··  SO
```

`··` : vitre de remplissage.

| Slot | Code | Objet | Nom | Contenu | Clic |
| --- | --- | --- | --- | --- | --- |
| 4 | HD | `minecraft:amethyst_shard` | Banque | Solde. Rappel : un dépôt est définitif | Aucun |
| 19 | D1 | `minecraft:amethyst_shard` | Déposer 10 |  | Clic : confirmation |
| 20 | D2 | `minecraft:amethyst_cluster` | Déposer 100 |  | Clic : confirmation |
| 21 | D3 | `minecraft:writable_book` | Autre montant |  | Clic : propose `/guilde deposer ` dans le chat |
| 23 | U1 | `minecraft:oak_planks` | Salle agrandie I | 400, +6 membres | Officier : achète |
| 24 | U2 | `minecraft:spruce_planks` | Salle agrandie II | 800, niveau 5, +6 membres | Officier : achète |
| 25 | U3 | `minecraft:white_dye` | Couleur du tag | 100, niveau 7 | Chef : choix de la couleur |
| 40 | JO | `minecraft:book` | Journal | 20 derniers dépôts et dépenses | Aucun |
| 45, 49, 53 | RE, FE, SO | Barre de navigation | Voir [Conventions](menus.md) | | |

## Défis

* Titre de l'inventaire : `STRATA · Défis`
* Taille : 54 emplacements, 6 lignes
* Ouverture : menu Guilde
* Permission : `strata.player.guilde`
* Retour vers : Guilde
* Remplissage : Vitre grise `minecraft:gray_stained_glass_pane`, sans nom

```
      0   1   2   3   4   5   6   7   8 
 0-8  ··  ··  ··  ··  HD  ··  ··  ··  ··
 9-17 ··  ··  ··  ··  ··  ··  ··  ··  ··
18-26 ··  ··  F1  ··  F2  ··  F3  ··  ··
27-35 ··  ··  ··  ··  RW  ··  ··  ··  ··
36-44 ··  ··  ··  ··  ··  ··  ··  ··  ··
45-53 RE  ··  ··  ··  FE  ··  ··  ··  SO
```

`··` : vitre de remplissage.

| Slot | Code | Objet | Nom | Contenu | Clic |
| --- | --- | --- | --- | --- | --- |
| 4 | HD | `minecraft:target` | Défis de la semaine | Temps restant jusqu'au lundi 04 h 00 | Aucun |
| 20 | F1 | icône du défi | Défi 1 | Objectif, progression en %, ta contribution, ✔ si réussi | Aucun |
| 22 | F2 | icône du défi | Défi 2 | Idem | Aucun |
| 24 | F3 | icône du défi | Défi 3 | Idem, ou « ✖ Niveau 5 » | Aucun |
| 31 | RW | `minecraft:chest` | Récompenses | 12 Cristaux par membre et par défi, 500 000 XP de guilde | Aucun |
| 45, 49, 53 | RE, FE, SO | Barre de navigation | Voir [Conventions](menus.md) | | |

Icônes des défis : blocs `minecraft:iron_pickaxe`, minerais `minecraft:emerald_ore`, boss `minecraft:wither_skeleton_skull`, Prestiges `minecraft:beacon`, Œufs `minecraft:sniffer_egg`, Concours `minecraft:clock`.
