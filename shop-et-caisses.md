---
description: Les menus du Shop rotatif et des caisses : offres, caisses, aperçu et ouverture.
---

# 🛒 Menus · Shop et caisses

## Shop

* Titre de l'inventaire : `STRATA · Shop`
* Taille : 54 emplacements, 6 lignes
* Ouverture : `/shop`, Menu principal
* Permission : `strata.player.shop`
* Retour vers : Menu principal
* Remplissage : Vitre grise `minecraft:gray_stained_glass_pane`, sans nom

```
      0   1   2   3   4   5   6   7   8 
 0-8  ··  ··  ··  ··  HD  ··  ··  ··  ··
 9-17 ··  ··  ··  ··  ··  ··  ··  ··  ··
18-26 ··  ··  O1  O2  O3  O4  O5  ··  ··
27-35 ··  ··  ··  CD  O6  CD  ··  ··  ··
36-44 ··  ··  ··  ··  CR  ··  ··  ··  ··
45-53 RE  ··  ··  ··  FE  ··  ··  ··  SO
```

`··` : vitre de remplissage.

| Slot | Code | Objet | Nom | Contenu | Clic |
| --- | --- | --- | --- | --- | --- |
| 4 | HD | `minecraft:emerald` | Shop rotatif | Temps avant la prochaine rotation, 00:43:12 | Aucun |
| 20 | O1 | `minecraft:potion` | Offre 1, booster | Effet, durée, prix en Argent calculé pour le joueur | Clic : achète |
| 21 | O2 | `minecraft:potion` | Offre 2, booster | Idem | Clic : achète |
| 22 | O3 | objet de l'offre | Offre 3, Collection | Prix en Cristaux | Clic : achète |
| 23 | O4 | objet de l'offre | Offre 4, Collection | Idem | Clic : achète |
| 24 | O5 | objet de l'offre | Offre 5, Rare | Idem | Clic : achète, confirmation dès 100 Cristaux |
| 30 | CD | `minecraft:yellow_stained_glass_pane` | Cadre | Seulement quand l'offre 6 est une Vedette | Aucun |
| 31 | O6 | objet de l'offre | Offre 6, Vedette ou Collection | Vedette : nom en or, brillance | Clic : achète, confirmation dès 100 Cristaux |
| 32 | CD | `minecraft:yellow_stained_glass_pane` | Cadre | Idem | Aucun |
| 40 | CR | `minecraft:amethyst_shard` | Cristaux | Solde de Cristaux | Aucun |
| 45, 49, 53 | RE, FE, SO | Barre de navigation | Voir [Conventions](menus.md) | | |

* Offre achetée : « ✔ Acheté pour cette rotation », pas de brillance.
* Solde insuffisant : prix en rouge et montant manquant.
* À la rotation, un menu ouvert est mis à jour sans fermeture.
* Prix en Argent : 10 minutes du revenu moyen du joueur, voir [Shop rotatif](../shop/shop-rotatif.md).

## Caisses

* Titre de l'inventaire : `STRATA · Caisses`
* Taille : 54 emplacements, 6 lignes
* Ouverture : `/caisses`, Menu principal, clic droit sur une caisse du spawn
* Permission : `strata.player.caisses`
* Retour vers : Menu principal
* Remplissage : Vitre grise `minecraft:gray_stained_glass_pane`, sans nom

```
      0   1   2   3   4   5   6   7   8 
 0-8  ··  ··  ··  ··  HD  ··  ··  ··  ··
 9-17 ··  ··  ··  ··  ··  ··  ··  ··  ··
18-26 ··  ··  CV  CF  CP  CT  CC  ··  ··
27-35 ··  ··  ··  ··  ··  ··  ··  ··  ··
36-44 ··  ··  ··  ··  BQ  ··  ··  ··  ··
45-53 RE  ··  ··  ··  FE  ··  ··  ··  SO
```

`··` : vitre de remplissage.

| Slot | Code | Objet | Nom | Contenu | Clic |
| --- | --- | --- | --- | --- | --- |
| 4 | HD | `minecraft:tripwire_hook` | Clés | Clés possédées par caisse | Aucun |
| 20 | CV | `minecraft:white_shulker_box` | Caisse Vote | Clés, probabilités résumées | Gauche : ouvrir. Droit : aperçu. Maj + clic : ouvrir par 10 |
| 21 | CF | `minecraft:lime_shulker_box` | Caisse Pets F2W | Idem | Idem |
| 22 | CP | `minecraft:purple_shulker_box` | Caisse Pets Premium | Idem, lien de la boutique si aucune clé | Idem |
| 23 | CT | `minecraft:orange_shulker_box` | Caisse Armure Themes | Idem | Idem |
| 24 | CC | `minecraft:magenta_shulker_box` | Caisse Armure Themes Chroma | Idem, Poussière Chroma | Idem |
| 40 | BQ | `minecraft:gold_nugget` | Boutique | Clés Premium et Chroma | Clic : envoie le lien dans le chat |
| 45, 49, 53 | RE, FE, SO | Barre de navigation | Voir [Conventions](menus.md) | | |

## Aperçu

* Titre de l'inventaire : `STRATA · Aperçu`
* Taille : 54 emplacements, 6 lignes
* Ouverture : clic droit sur une caisse
* Permission : `strata.player.caisses`
* Retour vers : Caisses
* Remplissage : Vitre grise `minecraft:gray_stained_glass_pane`, sans nom

```
      0   1   2   3   4   5   6   7   8 
 0-8  ··  ··  ··  ··  HD  ··  ··  ··  ··
 9-17 ··  ··  ··  ··  ··  ··  ··  ··  ··
18-26 ··  RC  RC  RC  RC  RC  RC  RC  ··
27-35 ··  RC  RC  RC  RC  RC  RC  RC  ··
36-44 ··  ··  ··  ··  OU  ··  ··  ··  ··
45-53 RE  ··  ··  ··  FE  ··  ··  ··  SO
```

`··` : vitre de remplissage.

| Slot | Code | Objet | Nom | Contenu | Clic |
| --- | --- | --- | --- | --- | --- |
| 4 | HD | boîte de la caisse | Nom de la caisse | Clés possédées, règle des doublons | Aucun |
| 19 | RC | objet de la récompense | Récompenses | Slots 19 à 25 et 28 à 34 : une récompense par emplacement, probabilité exacte, « ✔ Possédé » pour un pet ou un son déjà obtenu | Aucun |
| 40 | OU | `minecraft:tripwire_hook` | Ouvrir |  | Gauche : ouvrir. Maj + clic : ouvrir par 10 |
| 45, 49, 53 | RE, FE, SO | Barre de navigation | Voir [Conventions](menus.md) | | |

## Ouverture

* **Animation** : menu de 27 emplacements, la ligne du milieu défile pendant 2 s avec des récompenses possibles, puis s'arrête sur la récompense tirée au slot 13. Son `ui.button.click` à chaque pas, `entity.player.levelup` à l'arrêt.
* La récompense est **tirée avant l'animation**, côté serveur. L'animation n'est qu'un affichage : fermer le menu ne change rien, la récompense est déjà livrée.
* Clic pendant l'animation : saute l'animation.
* **Ouvrir par 10** : sans animation, récapitulatif dans un menu de 27 emplacements, slots 9 à 17 et 4.
* Pet ou thème Mythique : annonce à tout le serveur. Légendaire : annonce au joueur seul, comme partout ailleurs (voir [Raretés](../concept/raretes.md)).
