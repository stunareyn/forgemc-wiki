---
description: Les 10 rangs de Prestige, leurs conditions, ce qu'ils réinitialisent, leurs gains et leurs durées.
---

# 🔱 Prestige

## 🎯 Objectif

Le Prestige est la boucle principale du serveur. Le joueur remet à zéro son **cycle** (pioche, niveau, enchantements, Argent, biomes) pour gagner un **multiplicateur** et aller plus loin au cycle suivant. Chaque rang ouvre du contenu nouveau : le Nether, l'End, l'Aether, puis la Renaissance.

## ⚙️ Fonctionnement

```
Cycle 0 : Overworld → Pioche en Diamant → Prestige I (ouvre le Nether)
Cycle 1 : Overworld rapide → Nether → Pioche en Sanguine → Prestige II
...
Cycle 9 : ... → Aether → Pioche d'Éther → Prestige X
Cycle 10 : tout le parcours → Pioche d'Éther et niveau 100 → Renaissance
```

## ✅ Conditions

* Posséder la pioche requise pour le rang visé
* Payer le coût du Prestige : 30 % du prix de cette pioche, en Argent

## ♻️ Ce qui est réinitialisé

* Argent et Éclats
* Pioche : retour à la Pioche en Pierre, ou à la pioche du Départ rapide
* Niveau et XP de pioche
* Tous les enchantements, sauf ceux du Départ rapide
* Biomes débloqués : retour aux Plaines
* Minerais et blocs compressés, inventaire et `/pv` compris
* Sceaux de dimension

## 🔒 Ce qui est conservé

* Rang de Prestige et son multiplicateur, jusqu'à la Renaissance
* Mémoire de forge, jusqu'à la Renaissance
* Tout le permanent : Cristaux, pets, traits, armures, race, skins, sons, collections, titres, clés, Œufs, guilde, grade, statistiques, boosters en cours

## 📋 Les 10 rangs

| Rang | Pioche requise | Coût en Argent | Multiplicateur | Déblocage |
| --- | --- | --- | --- | --- |
| I | Pioche en Diamant | 750 000 $ | x1,6 | Accès au Nether |
| II | Pioche en Sanguine | 7 800 000 $ (7,8 M) | x2,56 | · |
| III | Pioche en Rubis | 27 300 000 $ (27,3 M) | x4,1 | Départ rapide I : Efficacité 3, Fortune 5, Argent 5 au début de chaque cycle ; Vente automatique débloquée pour toujours |
| IV | Pioche de Carmin | 105 000 000 $ (105 M) | x6,55 | Accès à l'End |
| V | Pioche en Vesper | 780 000 000 $ (780 M) | x10,49 | Départ rapide II : début de cycle avec la Pioche en Fer ; 2e emplacement de pet débloqué pour toujours |
| VI | Pioche en Quartz fumé | 2 190 000 000 $ (2,19 Md) | x16,78 | · |
| VII | Pioche en Pulsar | 8 400 000 000 $ (8,4 Md) | x26,84 | Accès à l'Aether |
| VIII | Pioche en Disthène | 54 000 000 000 $ (54 Md) | x42,95 | Départ rapide III : début de cycle avec la Pioche en Diamant |
| IX | Pioche en Nova | 150 000 000 000 $ (150 Md) | x68,72 | · |
| X | Pioche d'Éther | 510 000 000 000 $ (510 Md) | x109,95 | Renaissance possible |

Le multiplicateur de Prestige vaut **1,6 par rang, cumulé** : x1,6 au Prestige I, x110 au Prestige X. Il multiplie l'Argent, l'XP et les Éclats. Il est remis à 1 à la Renaissance.

## 🎁 Récompenses de rang

| Rang | Cristaux | Clé |
| --- | --- | --- |
| I | 30 | Armure Themes |
| II | 40 | Pets F2W |
| III | 50 | Armure Themes |
| IV | 60 | Pets F2W |
| V | 70 | Armure Themes |
| VI | 80 | Pets F2W |
| VII | 90 | Armure Themes |
| VIII | 100 | Pets F2W |
| IX | 110 | Armure Themes |
| X | 120 | Pets F2W |

Ces récompenses sont données à chaque passage de rang, à chaque Renaissance.

## ⏱️ Durée des cycles jusqu'à la première Renaissance

Temps de jeu actif simulé.

| Cycle | Nouveau | Moyen | Optimisé |
| --- | --- | --- | --- |
| Prestige 0 → Prestige I | 16 h 43 | 11 h 42 | 8 h 04 |
| Prestige I → Prestige II | 32 h 24 | 21 h 06 | 14 h 22 |
| Prestige II → Prestige III | 36 h 16 | 21 h 51 | 14 h 54 |
| Prestige III → Prestige IV | 46 h 01 | 25 h 48 | 17 h 26 |
| Prestige IV → Prestige V | 75 h 02 | 40 h 44 | 26 h 21 |
| Prestige V → Prestige VI | 71 h 47 | 38 h 28 | 24 h 26 |
| Prestige VI → Prestige VII | 80 h 53 | 42 h 16 | 26 h 34 |
| Prestige VII → Prestige VIII | 117 h 45 | 61 h 00 | 37 h 39 |
| Prestige VIII → Prestige IX | 111 h 57 | 56 h 26 | 34 h 26 |
| Prestige IX → Prestige X | 122 h 42 | 59 h 35 | 36 h 13 |
| Prestige X → Renaissance | 67 h 22 | 33 h 09 | 20 h 13 |
| **Total** | **778 h 52** | **412 h 05** | **260 h 38** |

Les cycles s'allongent globalement parce que chacun va plus loin. La part rejouée reste courte : au cycle 9, un joueur moyen retraverse l'Overworld, le Nether et l'End en environ 8 heures grâce au multiplicateur de x69 et à la mémoire de forge, puis passe l'essentiel du cycle dans l'Aether.

## 🔒 Règles

{% hint style="danger" %}
* Une confirmation avec délai de sécurité de 3 s, qui liste ce qui sera perdu et le nombre de minerais détruits. Voir [Menus · Prestige et Renaissance](../menus/prestige-renaissance.md).
* Aucun Prestige n'est annulable.
* Au-delà du Prestige X, le Prestige n'est plus proposé tant que le joueur n'a pas fait sa Renaissance.
{% endhint %}
