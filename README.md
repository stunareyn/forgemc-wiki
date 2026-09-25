---
description: Game Design Document interne de STRATA. Serveur Minecraft Java de minage, de progression et de collection.
---

# 🏠 STRATA · Game Design Document

Document **interne** de production. Il contient les valeurs d'équilibrage, les probabilités, les prix, les permissions et les commandes d'administration. Il ne s'adresse pas aux joueurs.

## 👥 Lecteurs

| Rôle | Pages à lire en priorité |
| --- | --- |
| Direction, associé | Concept, Progression, Économie, Grades, Équilibrage |
| Développeur | Formules, Pioches, Enchantements, Rebirth, Commandes, Permissions |
| Builder | Dimensions, Structure des mines, Biomes, PNJ |
| Configurateur | Biomes, Minerais, Caisses, Shop, Grades, Sons |
| Équilibrage | Économie, Équilibrage, Formules |
| Administration | Commandes, Permissions, Règles obligatoires |

## 🔁 La boucle en une ligne

```
Miner → Vendre → Enchanter et forger → Débloquer biome ou dimension → Pets, armures, traits → Rebirth → Recommencer plus vite
```

## 📌 Chiffres clés

* 4 dimensions, 12 biomes, 36 minerais, 13 pioches, 7 enchantements
* 22 pets, 8 traits, 12 armures, 8 races, 11 thèmes de skin, 12 sons de minage
* 3 monnaies : Argent et Éclats (réinitialisés au Rebirth), Cristaux (permanents)
* Premier Rebirth : environ 36 h de jeu actif pour un joueur moyen
* Rebirth maximum : 25, atteint en environ 440 h de jeu pour un joueur moyen

## 🧭 Conventions

* 🟠 valeur à confirmer en test, voir [Contrôles](equilibrage/controles.md)
* Les valeurs en $ sont des valeurs de base, avant bonus.
* « Run » : la période entre deux Rebirth.
* « T4 » : pioche de tier 4.
* Les temps sont des temps de **jeu actif**, pas des durées calendaires.

{% hint style="info" %}
Toutes les valeurs chiffrées de ce document proviennent d'un même modèle de simulation (voir [Équilibrage](equilibrage/equilibrage.md)). Modifier une valeur isolée sans relancer ce contrôle casse la cohérence d'ensemble.
{% endhint %}
