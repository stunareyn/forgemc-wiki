---
description: Règles communes des 35 minerais, échelle de valeur, XP, blocs compressés.
---

# 💎 Minerais

35 minerais : les 8 minerais vanilla de l'Overworld, puis 9 minerais par dimension tirés des textures fournies.

## 🧮 Échelle de valeur

Valeur de vente = unité de la dimension x multiplicateur de la place du minerai.

| Place | Rareté | Multiplicateur | Overworld | Nether, End, Aether |
| --- | --- | --- | --- | --- |
| Commun 1 | Commun | x1 | Charbon | Bitume, Onyx, Givre |
| Commun 2 | Commun | x1,6 | Cuivre | Braise, Spodumène, Jade |
| Commun 3 | Commun | x2,5 | · | Tungstène, Iridium, Orichalque |
| Peu commun 1 | Peu commun | x3,5 | Fer | Citrine, Améthyste, Mythril |
| Peu commun 2 | Peu commun | x5 | Redstone | Ambre, Galène, Aigue-marine |
| Rare | Rare | x12 | Lapis-lazuli | Sanguine, Vesper, Disthène |
| Épique | Épique | x45 | Or | Rubis, Quartz fumé, Nova |
| Légendaire | Légendaire | x200 | Diamant | Carmin, Pulsar, Aurore |
| Mythique | Mythique | x1 000 | Émeraude | Infernium, Opale, Éther |

| Dimension | Unité |
| --- | --- |
| Overworld | 30 $ |
| Nether | 150 $ |
| End | 770 $ |
| Aether | 4 000 $ |

Exemple : Aurore, Légendaire de l'Aether = 4 000 x 200 = **800 000 $**.

## ⚖️ Pourquoi ces valeurs

* Dans le Nether, l'End et l'Aether, un Rare vaut 4,8 fois le meilleur Commun, un Mythique 400 fois. Dans l'Overworld, le Lapis-lazuli vaut 7,5 fois le Cuivre.
* Dans la plupart des biomes, les minerais Rares et plus font 38 % à 42 % de la valeur d'un bloc ; 62 % dans les Badlands, dont le minerai favori est l'Or ; 65 % à 75 % dans les zones riches.
* Aucun Commun ne vaut plus qu'un Peu commun de sa dimension, aucun Peu commun plus qu'un Rare.

## ✨ XP

| Contenu | XP de base |
| --- | --- |
| Bloc principal | 1 |
| Commun | 2 |
| Peu commun | 3 |
| Rare | 6 |
| Épique | 15 |
| Légendaire | 40 |
| Mythique | 120 |

XP gagnée = XP de base x multiplicateur du biome x (1 + bonus d'XP) x multiplicateur de Prestige x multiplicateur de Renaissance. Aucune orbe d'expérience vanilla n'apparaît.

## 📦 Blocs compressés

* Avec Autocraft, 9 minerais identiques deviennent 1 bloc compressé.
* Overworld : blocs de stockage vanilla (bloc de charbon, de cuivre brut, de fer brut, de redstone, de lapis-lazuli, d'or brut, de diamant, d'émeraude).
* Autres dimensions : bloc du minerai concerné.
* Valeur : 9 x valeur du minerai x (1 + 3 % par niveau d'Autocraft). Un bloc compressé compte pour 9 unités dans les recettes.

## 🔒 Règles

{% hint style="danger" %}
* Les minerais et objets de minage sont **liés au joueur** : impossibles à jeter au sol, échanger, fondre, fabriquer ou poser. Seule la poubelle `/trash` peut les détruire, avec un avertissement. Les objets vanilla de l'Overworld portent un marqueur STRATA qui bloque toutes les recettes vanilla.
* Au Prestige et à la Renaissance, tous les minerais et blocs compressés sont détruits, inventaire et `/pv` compris.
* Pour les dimensions à textures, le champ Texture fait foi pour le graphiste.
{% endhint %}

## 🗂️ Pages détaillées

* [Overworld](overworld.md)
* [Nether](nether.md)
* [End](end.md)
* [Aether](aether.md)
