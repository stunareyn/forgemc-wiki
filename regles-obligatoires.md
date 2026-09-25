---
description: Règles imposées par la direction. Elles ne se modifient pas.
---

# 🔒 Règles obligatoires

{% hint style="danger" %}
**Dimensions et biomes**

* Exactement 4 dimensions : Overworld, Nether, End, Aether, dans cet ordre de progression. Aucune dimension ajoutée, aucun renommage.
* Les biomes portent les **noms des biomes vanilla** de Minecraft.
* Chaque biome est une zone publique d'environ 20 000 x 300 x 20 000 blocs. Aucune mine personnelle, aucune instance individuelle.
* Objectif de lancement : environ 250 joueurs et plus par biome.
* Couche 1 : bloc principal uniquement. Minerais à partir de la couche 2, taux identiques à toutes les profondeurs.
* Blocs principaux : Stone, Netherrack, End Stone, Calcite pour l'Aether (choix de design).

**Minerais**

* Overworld : uniquement les **minerais vanilla** qui existent dans Minecraft.
* Nether, End, Aether : minerais tirés des textures fournies.

**Progression**

* Il existe des **Prestiges** et des **Renaissances**.
* La première Renaissance ne doit pas être atteignable avant **2 à 3 semaines** après l'ouverture, même pour les joueurs les plus actifs.
* La pioche et ses enchantements sont réinitialisés. Pets, traits, armures, skins, collections et apparences sont conservés.
* Enchantements : ceux de la version précédente, repris tels quels (Efficacité, Fortune, Argent, XP, Excavation, Autocraft, Prospection).

**Social et événements**

* Les Compagnies deviennent des **Guildes**.
* **Boss** : un par dimension, invisible, qui apparaît à intervalle fixe. Casser des blocs dans les biomes de sa dimension lui retire des points de vie affichés sur une barre de boss.
* **Événements** : chat réaction, vote party, et autres.

**Grades**

* Exactement : Joueur → Pilier → Héros → Champion → Légende → Monarque → Immortal.

**Commandes et menus**

* Liste complète des commandes joueurs, y compris les commandes utilitaires classiques.
* Menus GUI décrits dans une catégorie à part.

**Systèmes supprimés**

* Sac, bag, bundle : remplacés par `/pv`. Dynamite : supprimée.

**Assets**

* Aucune nouvelle texture ni aucun nouveau modèle.
{% endhint %}

## 📐 Conséquences de design

| Règle | Ce qu'elle impose au reste du design |
| --- | --- |
| Mines de 20 000 x 20 000 | Hub central et quatre relais pour concentrer l'activité |
| Minerais indépendants de la profondeur | La progression passe par les biomes, jamais par la profondeur |
| Minerais vanilla dans l'Overworld | Objets et blocs compressés vanilla ; pioches T1 à T5 et armures de l'Overworld vanilla |
| Première Renaissance après 2 à 3 semaines | Dix cycles de Prestige de 12 à 61 h pour un joueur moyen, minerai requis non achetable, verrou calendaire de sécurité de 15 jours pleins |
| Boss invisibles | Dégâts calculés par bloc cassé dans la dimension, partagés entre tous les serveurs de la dimension |
| Pas de sac | Autocraft, `/sell`, vente automatique et `/pv` |
| Pas de dynamite | L'Excavation est le seul outil de casse de zone, plafonné |
