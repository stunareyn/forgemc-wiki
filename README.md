---
description: Game Design Document interne de STRATA. Serveur Minecraft Java de minage, de progression, de Prestige et de Renaissance.
---

# 🏠 STRATA · Game Design Document

Document **interne** de production. Il contient les valeurs d'équilibrage, les probabilités, les prix, les menus, les permissions et les commandes d'administration. Il ne s'adresse pas aux joueurs.

## 👥 Lecteurs

| Rôle | Pages à lire en priorité |
| --- | --- |
| Direction, associé | Concept, Progression, Prestige, Renaissance, Économie, Grades, Équilibrage |
| Développeur | Formules, Pioches, Prestige, Renaissance, Boss, Menus GUI, Commandes, Permissions |
| Builder | Dimensions, Structure des mines, Biomes, PNJ |
| Configurateur | Biomes, Minerais, Caisses, Shop, Grades, Événements, Sons, Menus GUI |
| Équilibrage | Économie, Équilibrage, Formules |
| Administration | Commandes, Permissions, Événements, Règles obligatoires |

## 🔁 La boucle en une ligne

```
Miner → Vendre → Enchanter et forger → Nouveau biome → Porte de Prestige → Prestige → Aller plus loin → Prestige X → Renaissance
```

## 📌 Chiffres clés

* 4 dimensions, 16 biomes vanilla, 35 minerais dont 8 minerais vanilla, 17 pioches, 7 enchantements
* 10 rangs de Prestige, 10 Renaissances
* 22 pets, 8 traits, 15 armures, 8 races, 11 thèmes de skin, 12 sons de minage
* 4 boss de dimension, 5 types d'événements
* 3 monnaies : Argent et Éclats (remis à zéro au Prestige), Cristaux (permanents)
* Première Renaissance : 260 h 38 de jeu pour un joueur optimisé sans achat, soit 16,3 à 21,7 jours à 16 ou 12 h par jour, et 412 h 05 pour un joueur moyen. Verrou de sécurité : pas de Renaissance avant 15 jours pleins d'ouverture

## 🧭 Conventions

* 🟠 valeur à confirmer en test, voir [Contrôles](equilibrage/controles.md)
* Les valeurs en $ sont des valeurs de base, avant bonus.
* « Cycle » : la période entre deux Prestiges.
* « T9 » : pioche de tier 9. « P-IV » : Prestige IV. « R2 » : Renaissance 2.
* Les temps sont des temps de **jeu actif**, pas des durées calendaires.
* Md = milliard.

{% hint style="info" %}
Toutes les valeurs chiffrées viennent d'un même modèle de simulation (voir [Équilibrage](equilibrage/equilibrage.md)). Modifier une valeur isolée sans relancer ce modèle casse la cohérence d'ensemble.
{% endhint %}
