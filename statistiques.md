---
description: Les statistiques suivies, leur portée, leur affichage, les classements et le profil.
---

# 📊 Statistiques

## ⚙️ Principes

* Trois portées : **Cycle** (remise à zéro au Prestige), **Renaissance** (remise à zéro à la Renaissance) et **Vie** (jamais remise à zéro).
* Deux portées courtes pour les classements : **Semaine** (lundi 04 h 00) et **Jour** (04 h 00).
* Les compteurs vivent en mémoire et sont enregistrés par lots toutes les 30 à 60 secondes, jamais à chaque bloc.
* Consultation : `/stats` pour soi, `/stats <joueur>` pour un autre joueur.
* Classements : `/top <catégorie>`, mis à jour toutes les 10 minutes.

## 📋 Liste

| Statistique | Portées | Classement |
| --- | --- | --- |
| Blocs cassés | Cycle, Renaissance, Vie, Semaine | Vie et Semaine |
| Minerais cassés, par rareté | Cycle, Vie | Non |
| Argent gagné | Cycle, Vie | Non |
| Éclats gagnés | Cycle, Vie | Non |
| XP de pioche gagnée | Cycle, Vie | Non |
| Niveau et tier de pioche | Cycle | Non |
| Rang de Prestige | Renaissance | Oui, avec la Renaissance |
| Renaissance | Vie | Oui |
| Prestiges effectués | Vie, Semaine | Non |
| Durée du cycle en cours | Cycle | Non |
| Meilleur temps pour chaque rang de Prestige | Vie | Oui, par rang |
| Meilleur temps de Renaissance | Vie | Oui, par numéro de Renaissance |
| Meilleur temps de Nouveau départ | Vie | Oui |
| Nouveaux départs effectués | Vie | Non |
| Temps de jeu | Vie | Non |
| Temps de minage actif | Cycle, Renaissance, Vie | Non |
| Biomes et dimensions débloqués | Cycle | Non |
| Minerais découverts | Vie | Non |
| Minerais Mythiques cassés | Vie | Oui |
| Pets découverts, pets au niveau 40, pets ★3 | Vie | Non |
| Œufs éclos | Vie, Semaine | Non |
| Armures complètes, thèmes complets | Vie | Non |
| Progression des collections, en % | Vie | Oui |
| Trouvailles, par type | Vie | Non |
| Cristaux gagnés | Vie | Non |
| Boss vaincus, par boss | Vie | Non |
| Dégâts de boss | Vie, Semaine | Semaine |
| Meilleure part de dégâts sur un boss | Vie | Non |
| Pets de boss obtenus | Vie | Non |
| Chat réaction gagnés | Vie, Semaine | Semaine |
| Concours de minage : podiums | Vie | Non |
| Votes | Vie, Semaine | Non |
| Contribution à la guilde, XP de guilde | Semaine, Vie | Oui, dans la guilde |

## 🏆 Classements

| Classement | Récompense |
| --- | --- |
| Progression : Renaissance, puis rang de Prestige, puis tier | Aucune, classement honorifique |
| Meilleur temps de Renaissance, par numéro | Titre « Record de la Renaissance N » pour le premier, tant que le record tient |
| Meilleur temps pour chaque rang de Prestige | Aucune |
| Meilleur temps de Nouveau départ, après la Renaissance 10 | Titre « Record des Strates » pour le premier, tant que le record tient |
| Blocs cassés, semaine | Titre « Infatigable » pendant la semaine suivante, pour le premier |
| Blocs cassés, vie | Aucune |
| Dégâts de boss, semaine | Titre « Fléau des colosses » pendant la semaine suivante, pour le premier |
| Chat réaction, semaine | Titre « Plus rapide que l'éclair » pendant la semaine suivante, pour le premier |
| Minerais Mythiques cassés | Aucune |
| Collections | Aucune |
| Guildes, semaine | Cristaux et clés, voir [Guildes](../social/guildes.md) |

Le meilleur temps de Renaissance est le classement qui récompense l'optimisation plutôt que le temps passé. Il compte le **temps de minage actif**, pas le temps calendaire.

## 🧾 Profil

`/profil [joueur]` affiche : grade, race, Renaissance, rang de Prestige, tier et niveau de pioche, dimension actuelle, pets actifs, armure portée, skin, son de minage, titre, progression des collections, guilde, date de première connexion, temps de jeu.

Menu : voir [Menus GUI · Profil, paramètres et classements](../menus/profil-parametres.md).

## 🧑‍💻 Stockage

* Table `player_stats` : une ligne par joueur et par statistique, colonnes `cycle`, `renaissance`, `vie`, `semaine`, `jour`.
* Remises à zéro faites en une requête au moment du Prestige, de la Renaissance ou du changement de semaine, pas ligne par ligne.
* Classements calculés sur une copie en lecture toutes les 10 minutes, jamais sur la base principale pendant le jeu.
