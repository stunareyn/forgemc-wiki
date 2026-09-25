---
description: Les statistiques suivies, leur portée, leur affichage et les classements.
---

# 📊 Statistiques

## ⚙️ Principes

* Deux portées : **Run** (remise à zéro au Rebirth) et **Vie** (jamais remise à zéro).
* Les compteurs vivent en mémoire et sont enregistrés par lots toutes les 30 à 60 secondes, jamais à chaque bloc.
* Consultation : `/stats` pour soi, `/stats <joueur>` pour un autre joueur.
* Classements : `/top <catégorie>`, mis à jour toutes les 10 minutes.

## 📋 Liste

| Statistique | Portée | Classement |
| --- | --- | --- |
| Blocs cassés | Run et Vie | Vie |
| Minerais obtenus, par rareté | Run et Vie | Non |
| Argent gagné | Run et Vie | Vie |
| Éclats gagnés | Run et Vie | Non |
| XP de pioche gagnée | Run et Vie | Non |
| Niveau de pioche | Run | Non |
| Tier de pioche | Run | Non |
| Rebirth | Vie | Oui |
| Durée du run en cours | Run | Non |
| Meilleur temps de run | Vie | Oui, par tranche de Rebirth |
| Temps de jeu | Vie | Non |
| Temps de minage actif | Run et Vie | Non |
| Dimensions débloquées | Run | Non |
| Biomes débloqués | Run | Non |
| Minerais découverts | Vie | Non |
| Minerais Mythiques trouvés | Vie | Oui |
| Pets découverts | Vie | Non |
| Pets au niveau 40 | Vie | Non |
| Armures obtenues | Vie | Non |
| Thèmes complets | Vie | Non |
| Progression des collections, en % | Vie | Oui |
| Trouvailles | Vie | Non |
| Cristaux gagnés | Vie | Non |
| Contribution à la Compagnie | Semaine et Vie | Oui, par Compagnie |

## 🏆 Classements

| Classement | Récompense |
| --- | --- |
| Rebirth | Aucune, classement honorifique |
| Meilleur temps de run, par tranche : R0 à R4, R5 à R9, R10 à R14, R15 à R19, R20 et plus | Titre du mois pour le premier de chaque tranche |
| Blocs cassés, vie | Aucune |
| Argent gagné, vie | Aucune |
| Minerais Mythiques trouvés | Aucune |
| Collections | Aucune |
| Compagnies, semaine | Cristaux, voir [Compagnies](../social/compagnies.md) |

Le classement du meilleur temps de run par tranche est le seul classement qui récompense l'optimisation plutôt que le temps passé : il reste intéressant pour les joueurs déjà au Rebirth 25.

## 🧾 Profil

`/profil` affiche : grade, race, Rebirth, tier et niveau de pioche, dimension actuelle, pets actifs, armure portée, titre, progression des collections, Compagnie.
