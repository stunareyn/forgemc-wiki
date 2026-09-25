---
description: Dimensions d'une mine, couches, hub, relais, régénération et règles de génération.
---

# 🧱 Structure des mines

Chaque biome est un monde de minage public, identique dans sa structure pour les 12 biomes.

## 📐 Dimensions

* Surface : 20 000 x 20 000 blocs, bordure de monde à ±10 000 du centre
* Hauteur minable : 300 blocs
* Fond : une couche de bedrock incassable sous la hauteur minable
* Couche : tranche de 10 blocs de haut. Une mine compte 30 couches.

## 🪜 Couches

| Couche | Hauteur relative | Contenu |
| --- | --- | --- |
| Couche 1 | 291 à 300, surface | Bloc principal uniquement |
| Couches 2 à 30 | 1 à 290 | Bloc principal et minerais, taux fixes du biome |
| Fond | 0 | Bedrock |

{% hint style="danger" %}
* Aucun minerai dans la couche 1.
* Les taux de génération sont **identiques** de la couche 2 à la couche 30.
* Aucun minerai n'est réservé à une profondeur.
{% endhint %}

Conséquence voulue : creuser profond n'est jamais plus rentable que creuser près de la surface. Le joueur choisit sa zone pour le confort et la foule, pas pour le rendement.

## 🏛️ Hub et relais

La mine est immense, mais l'activité doit rester concentrée pour que les joueurs se croisent et pour que le serveur tienne la charge.

**Hub central**
* Position : centre du monde, en surface
* Contenu : point d'arrivée du biome, panneau des taux du biome, point de vente, décor du thème, accès aux relais
* Surface construite : 60 x 60 blocs maximum, hors zone minable

**Quatre relais**
* Position : à 1 000 blocs du hub, un par point cardinal
* Accès : `/relais` ou plaques du hub, téléportation instantanée
* Contenu : petit point de vente, retour au hub

Les joueurs ont une raison d'aller aux relais : répartir la foule. Ils n'ont aucune raison d'aller au-delà de quelques centaines de blocs d'un relais, puisque les taux sont identiques partout.

## ♻️ Régénération

Les règles viennent du document « STRATA Architecture technique v1 ».

* Un bloc cassé se régénère **120 secondes** après avoir été cassé.
* Si un joueur se trouve à moins de 8 blocs, la régénération est reportée d'une seconde, jusqu'à 10 reports. Au-delà, le bloc revient sauf s'il chevauche un joueur.
* Les blocs reviennent **du bas vers le haut** dans une même zone.
* Un bloc régénéré est **tiré à nouveau au hasard** selon les taux du biome. Il ne reprend pas son ancien contenu.
* Exception : en couche 1, un bloc régénéré redevient toujours le bloc principal.
* Au redémarrage du serveur, toutes les mines sont intactes.

Le nouveau tirage à la régénération empêche de mémoriser l'emplacement d'un minerai rare pour y revenir toutes les deux minutes.

## 👥 Capacité

* 250 joueurs par biome au lancement
* Biome plein : file d'attente à l'entrée, priorité aux grades Légende et supérieurs
* Aucun biome n'est dupliqué : un biome plein reste un biome unique

## 🚫 Ce que la mine ne contient pas

* Aucun mob, aucun spawn naturel
* Aucun objet au sol : tout va directement dans l'inventaire
* Aucune pose de bloc par les joueurs
* Aucun fluide, aucun bloc à gravité, aucune source de lumière posée
* Aucune structure vanilla générée
