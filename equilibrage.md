---
description: Méthode de validation, profils simulés, temps de progression, traduction en jours, ce qui limite chaque profil et ressources gagnées.
---

# ⚖️ Équilibrage

## 🔬 Méthode

Toutes les valeurs du document viennent d'une **simulation minute par minute** de la progression complète jusqu'à la Renaissance 10 : gains, achats d'enchantements, forge des pioches dès que les trois conditions sont réunies (Argent, minerai au premier forgeage, niveau), coût de Prestige, Mémoire de forge, Départ rapide, Sceaux, multiplicateurs de Prestige et de Renaissance, croissance des bonus permanents avec le temps de jeu.

Les prix des pioches, la courbe d'XP, les multiplicateurs et les coûts d'enchantement ont été calés ensemble sur des temps cibles, puis vérifiés sur quatre profils. Le simulateur est livré à part (`strata_simulateur_v2.zip`) pour que l'équipe relance les calculs après chaque modification.

{% hint style="warning" %}
Ce sont des estimations de conception, pas des mesures. Le rythme réel de minage, le temps passé dans les menus et les écarts de chance ne sont connus qu'en jeu. Les valeurs marquées 🟠 et la liste de [Contrôles](controles.md) sont à revoir après les premiers tests.
{% endhint %}

## 🧑 Profils simulés

| Profil | Enchantements | Temps effectif de minage | Argent détourné vers armures et boosters | Bonus |
| --- | --- | --- | --- | --- |
| Nouveau | 60 % des plafonds | 60 % | 8 % | Race Humain, bonus permanents acquis 40 % moins vite que le moyen, aucun booster |
| Moyen | 85 % des plafonds | 70 % | 10 % | Race Humain, pets, armures, traits, collections et guilde selon le temps de jeu, aucun booster |
| Optimisé | 100 % des plafonds | 80 % | 12 % | **Sans achat**. Race Draconide, boosters gratuits en moyenne +3 % Argent et +3 % XP, bonus permanents acquis 50 % plus vite |
| Baleine | 100 % des plafonds | 80 % | 12 % | Optimisé, plus grade Immortal et pet Mythique Argent ★3 niveau 40 dès la première minute (borne haute : un pet de caisse commence au niveau 1) |

Temps effectif : part du temps connecté passée à casser des blocs. Le reste va aux déplacements, ventes et menus.

**Boosters gratuits du profil optimisé**, joueur à 12 h de jeu par jour 🟠 :

```
Argent : Vote Party   5 par jour x 30 min = 2,5 h sur 24 h, soit 1,25 h pendant ses 12 h
         Boss         environ 4 victoires par jour dans sa dimension x 20 min = 1,33 h
         Ferveur      1 h par jour
         Total        1,25 + 1,33 + 1 = 3,58 h de +10 % sur 12 h → 3,58 / 12 x 10 % = +3,0 %
XP     : Boss         1,33 h de +10 %                     → 1,33 / 12 x 10 % = +1,1 %
         Booster XP   2 achats par jour x 30 min de +25 % → 1 / 12 x 25 %    = +2,1 %
         Total        +3,2 %, arrondi à +3 %
```

Aucun booster d'Argent ne s'achète : le grade est le seul avantage d'Argent payant.

**Bonus permanents du profil moyen** selon les heures de jeu, interpolation linéaire :

| Heures de jeu | 0 | 30 | 150 | 400 | 500 |
| --- | --- | --- | --- | --- | --- |
| Pets Argent + trait | 0 % | 7,3 % | 21,4 % | 37 % | 42 % |
| Armures Argent | 0 % | 2,8 % | 10,9 % | 22,5 % | 26 % |
| Collections | 0 % | 0,6 % | 2,8 % | 6 % | 7 % |
| Guilde | 0 % | 2 % | 6 % | 10 % | 10 % |

## ⛏️ Revenus de référence

Voir [Économie](../economie/economie.md) : 69 500 $/h dans les Plaines au premier cycle, 87,1 Md $/h dans les Pics gelés au Prestige IX.

## ⏱️ Première forge de chaque pioche

Temps de jeu actif cumulé depuis le premier bloc. La colonne Prestige indique le cycle où la pioche est forgée pour la première fois.

| Pioche | Prestige | Nouveau | Moyen | Optimisé |
| --- | --- | --- | --- | --- |
| T2 Pioche en Cuivre | 0 | 1 h 01 | 51 min | 40 min |
| T3 Pioche en Fer | 0 | 3 h 20 | 2 h 35 | 1 h 56 |
| T4 Pioche en Or | 0 | 7 h 52 | 5 h 38 | 4 h 01 |
| T5 Pioche en Diamant | 0 | 15 h 11 | 10 h 40 | 7 h 22 |
| T6 Pioche en Citrine | I | 34 h 36 | 23 h 59 | 16 h 31 |
| T7 Pioche en Sanguine | I | 46 h 56 | 31 h 36 | 21 h 36 |
| T8 Pioche en Rubis | II | 82 h 35 | 53 h 14 | 36 h 23 |
| T9 Pioche de Carmin | III | 126 h 52 | 77 h 55 | 53 h 07 |
| T10 Pioche en Améthyste | IV | 176 h 40 | 106 h 00 | 71 h 50 |
| T11 Pioche en Vesper | IV | 201 h 49 | 118 h 47 | 79 h 40 |
| T12 Pioche en Quartz fumé | V | 273 h 58 | 157 h 33 | 104 h 14 |
| T13 Pioche en Pulsar | VI | 351 h 24 | 197 h 58 | 129 h 44 |
| T14 Pioche en Mythril | VII | 434 h 19 | 241 h 17 | 156 h 36 |
| T15 Pioche en Disthène | VII | 469 h 55 | 259 h 37 | 167 h 49 |
| T16 Pioche en Nova | VIII | 581 h 56 | 316 h 13 | 202 h 20 |
| T17 Pioche d'Éther | IX | 699 h 47 | 373 h 32 | 237 h 07 |

Les jalons de Prestige sont dans [Progression globale](../progression/progression.md), la durée de chaque cycle dans [Prestige](../progression/prestige.md).

## 🧭 Étapes

| Étape | Joueur moyen |
| --- | --- |
| Premier enchantement, Efficacité 1 : 150 Éclats à 1 Éclat par bloc et 69 blocs/min | environ 2 min |
| Pioche en Cuivre, 2e biome | 51 min |
| Pioche en Fer, 3e biome | 2 h 35 |
| Premier Prestige | 11 h 42 |
| Entrée dans le Nether, cycle 1 | 18 h 09 |
| Entrée dans l'End, cycle 4 | 94 h 31 |
| Entrée dans l'Aether, cycle 7 | 225 h 09 |
| Première Renaissance | 412 h 05 |

## 📆 Première Renaissance en jours

| Joueur | Profil | Jeu par jour | Temps de jeu | Jours calendaires |
| --- | --- | --- | --- | --- |
| Nouveau joueur | Nouveau | 3 h | 778 h 52 | 778,9 / 3 = 259,6 jours |
| Joueur régulier | Moyen | 3 h | 412 h 05 | 412,1 / 3 = 137,4 jours |
| Joueur très actif | Moyen | 6 h | 412 h 05 | 412,1 / 6 = 68,7 jours |
| Joueur optimisé sans achat | Optimisé | 12 h | 260 h 38 | 260,6 / 12 = 21,7 jours |
| Joueur optimisé sans achat, ouverture du serveur | Optimisé | 16 h | 260 h 38 | 260,6 / 16 = 16,3 jours |
| Tous les avantages payants, ouverture du serveur | Baleine | 16 h | 232 h 55 | 232,9 / 16 = 14,6 jours |
| Cas extrême, 20 h par jour | Baleine | 20 h | 232 h 55 | 232,9 / 20 = 11,6 jours |

**Objectif demandé** : pas de première Renaissance avant 2 à 3 semaines d'ouverture.

* Joueur optimisé sans achat à 16 h par jour : 16,3 jours. Objectif tenu.
* Tous les avantages payants à 16 h par jour : 14,6 jours. Juste au-dessus de 2 semaines.
* Cas extrême à 20 h par jour : 11,6 jours.
* Le **verrou calendaire** de 15 jours pleins arrête ces deux derniers cas, voir [Renaissance](../progression/renaissance.md).

## 🔒 Ce qui limite chaque profil

* **Tous les profils** : l'Argent. Au premier forgeage, le niveau du joueur moyen dépasse le niveau requis de 5 niveaux (Pioche en Cuivre) jusqu'à 34 niveaux (Pioches en Vesper et en Quartz fumé) : l'XP, multipliée par MP comme l'Argent, n'est pas le frein. La marge se réduit dans l'Aether, où le joueur plafonne au niveau 100 : 8 niveaux pour la Pioche en Nova, 0 pour la Pioche d'Éther et la Renaissance, qui demandent le niveau 100.
* **Premier forgeage** : le minerai requis s'ajoute à l'Argent. La Mémoire de forge le supprime aux cycles suivants de la même Renaissance.
* **Baleine** : 232 h 55 pour la première Renaissance, contre 260 h 38 sans achat : 260 h 38 → 232 h 55, soit (1 - 232,9 / 260,6) x 100 = 10,6 % de temps en moins. Les bonus d'Argent s'additionnent et se diluent : +12 % de grade ou +43,5 % de pet pèsent peu à côté des +150 % de l'enchantement Argent et du multiplicateur de Prestige.
* **Temps minimal d'une première Renaissance** : environ 233 h de jeu actif, quels que soient les achats.

## 📦 Ressources jusqu'à la première Renaissance, joueur moyen

| Ressource | Quantité |
| --- | --- |
| Temps de jeu actif | 412 h 05 |
| Blocs cassés | environ 6,6 millions |
| Cristaux | environ 7 300, voir [Économie](../economie/economie.md) |
| Œufs trouvés en minant | environ 100 |
| Clés Pets F2W | environ 47, voir [Caisses](../caisses/caisses.md) |
| Clés Armure Themes | environ 61 |
| Boss rencontrés | environ 103, voir [Boss](../evenements/boss.md) |
| Prestiges | 10 |
