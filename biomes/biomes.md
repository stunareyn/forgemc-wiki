---
description: Vue d'ensemble des 12 biomes et règles communes.
---

# 🏔️ Biomes

12 biomes publics, trois par dimension. Le biome est l'unité de progression : chaque pioche achetée ouvre un biome plus rentable.

## 📋 Vue d'ensemble

| # | Biome | Dimension | Pioche requise |
| --- | --- | --- | --- |
| 1 | La Carrière | Overworld | Départ |
| 2 | Grottes Verdoyantes | Overworld | Pioche en Baryte |
| 3 | Abîme Sombre | Overworld | Pioche en Malachite |
| 4 | Terres Désolées | Nether | Pioche d'Ambre |
| 5 | Forêt Écarlate | Nether | Pioche en Citrine |
| 6 | Vallée des Âmes | Nether | Pioche en Tungstène |
| 7 | Terres Stériles | End | Pioche de Carmin |
| 8 | Plateaux du Vide | End | Pioche en Améthyste |
| 9 | Hauts du Néant | End | Pioche en Saphir |
| 10 | Îles des Nuées | Aether | Pioche de Nova |
| 11 | Jardins Célestes | Aether | Pioche en Jade |
| 12 | Trône Solaire | Aether | Pioche en Platine |

## 📈 Valeur et vitesse par biome

| # | Valeur moyenne d'un bloc | XP x | Éclats par bloc |
| --- | --- | --- | --- |
| 1 | 12,28 $ | 1 | 1 |
| 2 | 21,25 $ | 1 | 1,4 |
| 3 | 36,57 $ | 1 | 1,8 |
| 4 | 61,38 $ | 1 | 2,5 |
| 5 | 106 $ | 1,25 | 3,3 |
| 6 | 183 $ | 1,75 | 4,5 |
| 7 | 307 $ | 3,5 | 6 |
| 8 | 531 $ | 5 | 8 |
| 9 | 914 $ | 7 | 11 |
| 10 | 1 535 $ | 15 | 15 |
| 11 | 2 656 $ | 24 | 20 |
| 12 | 4 571 $ | 42 | 27 |

La valeur moyenne est calculée sans aucun bonus : somme des taux multipliés par les valeurs de vente. Elle progresse d'environ 1,7 fois par biome.

## 🧬 Construction d'un biome

Chaque biome contient :

* le **bloc principal** de sa dimension ;
* ses **minerais propres** : un Commun et un Peu commun dans les biomes 1 et 2 de chaque dimension, un seul Commun à forte valeur dans le biome 3 ;
* les **quatre minerais partagés** de sa dimension, Rare, Épique, Légendaire et Mythique, présents dans les trois biomes.

Les minerais partagés sont 1,5 fois plus fréquents dans le biome 2 et 2,5 fois plus fréquents dans le biome 3 que dans le biome 1. Le biome 3 de chaque dimension est la **zone riche** : c'est là que se récoltent les matériaux d'armure et de pioche de fin de dimension.

| Biome local | Bloc principal | Minerais propres | Minerais partagés |
| --- | --- | --- | --- |
| 1 | 84 % | 15,2 % | 0,8 % |
| 2 | 81 % | 17,8 % | 1,2 % |
| 3 | 78 % | 20 % | 2 % |

## 🗂️ Pages détaillées

* [Overworld](overworld.md)
* [Nether](nether.md)
* [End](end.md)
* [Aether](aether.md)

{% hint style="info" %}
Les identifiants de biome vanilla ne servent qu'à l'ambiance : musique, brouillard, particules d'ambiance côté client. Ils n'influencent jamais la génération, qui est entièrement pilotée par les tables de ce document.
{% endhint %}
