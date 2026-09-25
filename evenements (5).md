---
description: Les menus des événements : Événements, Boss et Vote.
---

# 🎪 Menus · Événements

## Événements

* Titre de l'inventaire : `STRATA · Événements`
* Taille : 54 emplacements, 6 lignes
* Ouverture : `/evenements`, Menu principal
* Permission : `strata.player.evenements`
* Retour vers : Menu principal
* Remplissage : Vitre grise `minecraft:gray_stained_glass_pane`, sans nom

```
      0   1   2   3   4   5   6   7   8 
 0-8  ··  ··  ··  ··  HD  ··  ··  ··  ··
 9-17 ··  ··  ··  ··  ··  ··  ··  ··  ··
18-26 ··  BO  ··  CR  ··  CM  ··  HO  ··
27-35 ··  ··  ··  ··  VP  ··  ··  ··  ··
36-44 ··  ··  ··  ··  ··  ··  ··  ··  ··
45-53 RE  ··  ··  ··  FE  ··  ··  ··  SO
```

`··` : vitre de remplissage.

| Slot | Code | Objet | Nom | Contenu | Clic |
| --- | --- | --- | --- | --- | --- |
| 4 | HD | `minecraft:clock` | Événements | Heure du serveur, 7 prochains événements avec leur heure | Aucun |
| 19 | BO | `minecraft:wither_skeleton_skull` | Boss | Prochain boss de chaque dimension | Clic : ouvre Boss |
| 21 | CR | `minecraft:oak_sign` | Chat réaction | Dernier défi, 10 derniers gagnants, tes victoires du jour 1 / 15 | Aucun |
| 23 | CM | `minecraft:iron_pickaxe` | Concours de minage | Prochain Concours, dernier podium de chaque dimension | Aucun |
| 25 | HO | `minecraft:glowstone` | Heure dorée | En cours avec temps restant, annoncée, ou « Aujourd'hui entre 18 h et 22 h » | Aucun |
| 31 | VP | `minecraft:cake` | Vote Party | Progression 214 / 300 | Clic : ouvre Vote |
| 45, 49, 53 | RE, FE, SO | Barre de navigation | Voir [Conventions](menus.md) | | |

## Boss

* Titre de l'inventaire : `STRATA · Boss`
* Taille : 54 emplacements, 6 lignes
* Ouverture : `/boss`, menu Événements
* Permission : `strata.player.boss`
* Retour vers : Événements
* Remplissage : Vitre grise `minecraft:gray_stained_glass_pane`, sans nom

```
      0   1   2   3   4   5   6   7   8 
 0-8  ··  ··  ··  ··  HD  ··  ··  ··  ··
 9-17 ··  ··  ··  ··  ··  ··  ··  ··  ··
18-26 ··  B1  ··  B2  ··  B3  ··  B4  ··
27-35 ··  ··  ··  ··  TP  ··  ··  ··  ··
36-44 ··  ··  ··  ··  RW  ··  ··  ··  ··
45-53 RE  ··  ··  ··  FE  ··  ··  ··  SO
```

`··` : vitre de remplissage.

| Slot | Code | Objet | Nom | Contenu | Clic |
| --- | --- | --- | --- | --- | --- |
| 4 | HD | `minecraft:wither_skeleton_skull` | Boss | Boss de ta dimension : combat en cours ou prochain passage | Aucun |
| 19 | B1 | `minecraft:zombie_head` | Le Colosse enfoui | Hors combat : prochain passage 00:43:12. En combat : PV en %, temps restant, tes dégâts, ta place. Victoires, compteur de garantie | Aucun |
| 21 | B2 | `minecraft:wither_skeleton_skull` | Le Seigneur des Cendres | Idem | Aucun |
| 23 | B3 | `minecraft:dragon_head` | Le Dévoreur du Vide | Idem | Aucun |
| 25 | B4 | `minecraft:creeper_head` | Le Roi des Tempêtes | Idem | Aucun |
| 31 | TP | `minecraft:gold_block` | Combat en cours | Top 3 des dégâts, en direct | Aucun |
| 40 | RW | `minecraft:chest` | Récompenses | Cristaux, booster, chances de pet, classement, coup fatal | Aucun |
| 45, 49, 53 | RE, FE, SO | Barre de navigation | Voir [Conventions](menus.md) | | |

## Vote

* Titre de l'inventaire : `STRATA · Vote`
* Taille : 54 emplacements, 6 lignes
* Ouverture : `/vote`, `/voteparty`, Menu principal
* Permission : `strata.player.vote`
* Retour vers : Menu principal
* Remplissage : Vitre grise `minecraft:gray_stained_glass_pane`, sans nom

```
      0   1   2   3   4   5   6   7   8 
 0-8  ··  ··  ··  ··  HD  ··  ··  ··  ··
 9-17 ··  ··  ··  ··  ··  ··  ··  ··  ··
18-26 ··  ··  S1  ··  S2  ··  S3  ··  ··
27-35 ··  ··  ··  ··  VP  ··  ··  ··  ··
36-44 ··  ··  ··  ··  CV  ··  ··  ··  ··
45-53 RE  ··  ··  ··  FE  ··  ··  ··  SO
```

`··` : vitre de remplissage.

| Slot | Code | Objet | Nom | Contenu | Clic |
| --- | --- | --- | --- | --- | --- |
| 4 | HD | `minecraft:paper` | Votes | Votes du jour 2 / 3, votes du mois | Aucun |
| 20 | S1 | `minecraft:lime_dye` ou `minecraft:gray_dye` | Site 1 | Disponible, ou temps avant le prochain vote | Clic : envoie le lien dans le chat |
| 22 | S2 | `minecraft:lime_dye` ou `minecraft:gray_dye` | Site 2 | Idem | Idem |
| 24 | S3 | `minecraft:lime_dye` ou `minecraft:gray_dye` | Site 3 | Idem | Idem |
| 31 | VP | `minecraft:cake` | Vote Party | Progression 214 / 300, récompenses | Aucun |
| 40 | CV | `minecraft:white_shulker_box` | Caisse Vote | Clés Vote possédées | Clic : ouvre l'aperçu de la caisse |
| 45, 49, 53 | RE, FE, SO | Barre de navigation | Voir [Conventions](menus.md) | | |
