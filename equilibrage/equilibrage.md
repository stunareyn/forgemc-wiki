---
description: Méthode de validation, hypothèses, revenus, temps de progression par profil de joueur.
---

# ⚖️ Équilibrage

## 🔬 Méthode

Toutes les valeurs du document sont issues d'une **simulation minute par minute** d'un run complet : gains, achats d'enchantements, achat des pioches dès que les trois conditions sont réunies (Argent, minerai, niveau). Les valeurs n'ont pas été fixées une par une : les prix des pioches, la courbe d'XP et les coûts d'enchantement ont été calés ensemble sur des temps cibles, puis vérifiés sur plusieurs profils de joueur.

Aucune donnée de Minerite n'a été utilisée dans ce document. Le simulateur est livré à part (`strata_simulateur.zip`) pour que l'équipe d'équilibrage puisse relancer les calculs après chaque modification.

{% hint style="warning" %}
Ce sont des estimations de conception. Le rythme réel de minage d'un joueur, le temps passé dans les menus et les écarts de chance ne sont connus qu'en jeu. Les valeurs listées dans [Ajustements à prévoir](controles.md) devront être revues après les premiers tests.
{% endhint %}

## 🧑 Profils simulés

| Profil | Enchantements | Temps effectif de minage | Bonus |
| --- | --- | --- | --- |
| Nouveau | 60 % des plafonds, achats tardifs | 60 % | Pets faibles, armures tardives |
| Moyen | 85 % des plafonds | 70 % | 1 pet, armure Rare de chaque dimension, race Humain |
| Optimisé | 100 % des plafonds | 80 % | Grade Monarque, boosters du Shop, meilleurs pets trouvables, race Draconide |

Temps effectif : part du temps connecté passée à casser des blocs. Le reste va aux déplacements, ventes et menus.

## ⛏️ Rendement du premier run, joueur moyen

| Biome | Blocs/min | Minerais/min, Fortune comprise | Argent/min | Argent/h |
| --- | --- | --- | --- | --- |
| 1. La Carrière | 76 | 13 | 1 100 $ | 65 800 $ |
| 2. Grottes Verdoyantes | 97 | 23 | 3 170 $ | 190 000 $ |
| 3. Abîme Sombre | 113 | 35 | 8 050 $ | 483 000 $ |
| 4. Terres Désolées | 142 | 34 | 20 400 $ | 1 220 000 $ (1,2 M) |
| 5. Forêt Écarlate | 176 | 55 | 53 300 $ | 3 200 000 $ (3,2 M) |
| 6. Vallée des Âmes | 203 | 80 | 124 000 $ | 7 410 000 $ (7,4 M) |
| 7. Terres Stériles | 222 | 69 | 270 000 $ | 16 200 000 $ (16,2 M) |
| 8. Plateaux du Vide | 255 | 102 | 632 000 $ | 37 900 000 $ (37,9 M) |
| 9. Hauts du Néant | 300 | 147 | 1 450 000 $ (1,4 M) | 87 000 000 $ (87 M) |
| 10. Îles des Nuées | 341 | 129 | 3 100 000 $ (3,1 M) | 186 000 000 $ (186 M) |
| 11. Jardins Célestes | 386 | 185 | 6 940 000 $ (6,9 M) | 416 000 000 $ (416 M) |
| 12. Trône Solaire | 420 | 245 | 14 400 000 $ (14,4 M) | 865 000 000 $ (865 M) |

## ⏱️ Temps de progression du premier run

Temps de jeu actif cumulé au moment de l'achat de chaque pioche.

| Pioche | Nouveau | Moyen | Optimisé |
| --- | --- | --- | --- |
| T2 Pioche en Baryte | 35 min | 30 min | 21 min |
| T3 Pioche en Malachite | 2 h 11 | 1 h 39 | 1 h 10 |
| T4 Pioche d'Ambre | 5 h 25 | 3 h 42 | 2 h 30 |
| T5 Pioche en Citrine | 9 h 03 | 5 h 48 | 3 h 58 |
| T6 Pioche en Tungstène | 13 h 54 | 8 h 18 | 5 h 42 |
| T7 Pioche de Carmin | 19 h 54 | 11 h 30 | 7 h 43 |
| T8 Pioche en Améthyste | 26 h 30 | 14 h 39 | 9 h 42 |
| T9 Pioche en Saphir | 33 h 46 | 18 h 05 | 11 h 55 |
| T10 Pioche de Nova | 42 h 53 | 22 h 20 | 14 h 51 |
| T11 Pioche en Jade | 52 h 02 | 26 h 20 | 17 h 50 |
| T12 Pioche en Platine | 62 h 19 | 30 h 50 | 21 h 07 |
| T13 Pioche d'Éther | 75 h 11 | 36 h 10 | 24 h 47 |
| **Rebirth 1** | **75 h 11** | **36 h 10** | **24 h 47** |

## 📆 Traduction en jours

| Joueur | Profil | Jeu par jour | Premier Rebirth |
| --- | --- | --- | --- |
| Nouveau joueur | Nouveau | 1,5 h | environ 51 jours |
| Joueur régulier | Moyen | 2 h | environ 19 jours |
| Joueur très actif | Moyen | 5 h | environ 8 jours |
| Joueur optimisé | Optimisé | 6 h | environ 5 jours |

## 🧭 Étapes demandées

| Étape | Joueur moyen |
| --- | --- |
| Début → première amélioration, Efficacité 1 | 2 min |
| Première amélioration → nouveau biome | 28 min |
| Nouveau biome → nouvelle pioche, T3 | 1 h 09 |
| Nouvelle pioche → nouvelle dimension, Nether | 2 h 03 |
| Nether → End | 7 h 48 |
| End → Aether | 10 h 50 |
| Aether → premier Rebirth | 13 h 50 |
| Premier Rebirth, total | 36 h 10 |

## 🔒 Ce qui limite chaque profil

* **Nouveau et moyen** : l'Argent. Leur niveau de pioche dépasse de 1 à 7 niveaux le niveau requis au moment de l'achat.
* **Optimisé** : le niveau de pioche. À partir de l'End, il achète chaque pioche au niveau exactement requis : ses bonus d'Argent ne le font plus avancer plus vite.
* **Baleine**, grade Immortal et pet Mythique Argent dès la première minute : 25 h 06 pour le premier Rebirth. Limitée par le niveau, comme l'optimisé.
* **Temps minimal d'un premier run** : environ 24 h de minage actif, quels que soient les achats.

## 📦 Ressources d'un run moyen

| Ressource | Premier run |
| --- | --- |
| Blocs cassés | environ 626 000 |
| Argent gagné | environ 8,4 Md |
| Éclats gagnés, hors bonus d'Éclats | environ 9,1 M |
| Cristaux | environ 890 |
| Œufs trouvés en minant | environ 18 |
| Clés Pets F2W | environ 11 |
| Clés Armure Themes | environ 12 |
