---
description: Règles imposées par la direction. Elles ne se modifient pas.
---

# 🔒 Règles obligatoires

Ces règles ont été fixées par la direction. Aucune décision de game design, d'équilibrage ou de configuration ne peut les contredire.

{% hint style="danger" %}
**Dimensions**
* Exactement 4 dimensions : Overworld, Nether, End, Aether.
* Ordre de progression : Overworld → Nether → End → Aether.
* Aucune dimension secrète, aucune dimension ajoutée, aucun renommage.

**Biomes et mines**
* Chaque biome est une zone publique de minage d'environ 20 000 x 300 x 20 000 blocs.
* Aucune mine personnelle, aucune instance individuelle, aucune mine privée.
* Objectif de lancement : environ 250 joueurs et plus par biome.
* La première couche de chaque biome contient uniquement le bloc principal.
* Les minerais apparaissent à partir de la deuxième couche, aléatoirement.
* Aucun minerai lié à une profondeur. Les pourcentages sont identiques à toutes les profondeurs où les minerais existent.

**Blocs principaux**
* Overworld : Stone. Nether : Netherrack. End : End Stone. Aether : Calcite (choix de design).

**Pioche et Rebirth**
* La pioche et ses enchantements sont réinitialisés au Rebirth.
* Pets, traits, armures, skins, collections et apparences sont conservés au Rebirth.
* Enchantements obligatoires : Efficiency, Fortune, Excavation, Autocraft, XP, Money.

**Grades**
* Exactement : Joueur → Pilier → Héros → Champion → Légende → Monarque → Immortal.

**Systèmes supprimés**
* Sac, bag, bundle : supprimés, remplacés par `/pv`.
* Dynamite : supprimée.

**Assets**
* Aucune nouvelle texture ni aucun nouveau modèle.
{% endhint %}

## 📐 Conséquences de design

| Règle | Ce qu'elle impose au reste du design |
| --- | --- |
| Mines publiques de 20 000 x 20 000 | Un hub central et quatre relais concentrent l'activité. Voir [Structure des mines](../dimensions/structure-des-mines.md). |
| 250 joueurs par biome | Aucune récompense ne dépend d'un bloc précis ; tout est calculé au cassage, par joueur. |
| Minerais indépendants de la profondeur | La progression passe par les biomes, pas par la profondeur. Creuser plus bas n'est jamais plus rentable. |
| Pas de sac | Autocraft (compression x9), `/sell`, vente automatique et `/pv` gèrent l'encombrement. |
| Pas de dynamite | L'Excavation est le seul outil de casse de zone, plafonné. |
| Pioche réinitialisée | Le Rebirth doit offrir un multiplicateur permanent assez fort pour compenser. |
