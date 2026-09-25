---
description: Correspondance entre les assets fournis et leur usage, et liste des assets conservés pour plus tard.
---

# 📦 Assets

Aucune texture et aucun modèle nouveaux ne sont nécessaires. Chaque élément visuel du serveur utilise un asset fourni, un bloc ou un son vanilla, ou un skin de joueur existant.

* **Pioches** : textures et couleurs finales gérées par la direction, comme convenu. Le document donne seulement une couleur de référence par tier.
* **PNJ** : skins de joueur existants, choisis selon la description de chaque PNJ.
* **Biomes de l'Aether** : couleurs de ciel et de brouillard définies dans le datapack, sans texture.

## ✅ Utilisation des assets fournis

| Famille | Fournis | Utilisés | Où |
| --- | --- | --- | --- |
| Textures de minerai | 39 | 36 | [Minerais](../minerais/minerais.md) |
| Pets | 22 | 22 | [Pets](../pets/pets.md) |
| Armures de minéral | 12 | 12 | [Armures](../armures/armures.md) |
| Sets à thème | 11 | 11 | [Skins](../skins/skins.md) |

## 🔁 Correspondances à connaître

**Minerais dont le nom en jeu diffère de la texture**

| Nom en jeu | Texture |
| --- | --- |
| Ocre | `limonite` |
| Bois pétrifié | `patrified` |
| Grenat | `rhodolite` |
| Bitume | `oil` |
| Sanguine | `bloodstone` |
| Braise | `wulfenite` |
| Carmin | `rhodonite` |
| Infernium | `arcanite` |
| Spodumène | `lithium` |
| Vesper | `iolite` |
| Pulsar | `labradorite` |
| Nova | `crystalite` |
| Givre | `silver` |
| Orichalque | `bismuth` |
| Disthène | `kyanite` |
| Aurore | `charoite` |
| Éther | `pearl` |

Le minerai Givre utilise la texture `silver` pour éviter toute confusion avec la monnaie Argent.

**Armures de minéral**

| Armure | Asset |
| --- | --- |
| Galène | Galenite |
| Quartz fumé | Smoky Quartz |
| Ambre | Amber |
| Sanguine | Bloodstone |
| Rubis | Rubis |
| Carmin | Rhodonite |
| Vesper | Iolite |
| Pulsar | Labradorite |
| Nova | Crystalite |
| Aigue-marine | Aquamarine |
| Disthène | Kyanite |
| Aurore | Charoite |

**Sets à thème** : utilisés comme skins d'armure et, à la complétion d'un thème, comme skin de pioche. Si un set ne contient pas de texture de pioche, la récompense de complétion devient un titre « Thème <nom du thème> ».

## 🎨 Points à vérifier par le graphiste

* Le fond de chaque texture de minerai doit correspondre au bloc principal de sa dimension : Stone, Netherrack, End Stone ou Calcite.
* Couleurs proches dans une même dimension, à différencier par le motif si besoin : Aigue-marine et Disthène dans l'Aether, Améthyste et Vesper dans l'End, Givre, Platine et Mythril dans l'Aether.
* La caisse Chroma ne propose que les thèmes dont la version Chroma est fournie. Si une version manque, le thème est retiré de la caisse et ses probabilités sont réparties sur les thèmes de même rareté.

## 🗃️ ASSETS CONSERVÉS POUR PLUS TARD

| Asset | Type | Raison |
| --- | --- | --- |
| `magnesite` | Texture de minerai | Blanc, trop proche de la Calcite qui est le bloc principal de l'Aether et de la texture `pearl` |
| `garnierite` | Texture de minerai | Vert, trop proche de Malachite dans l'Overworld et de Jade dans l'Aether |
| `apatite` | Texture de minerai | Bleu-vert, trop proche de Saphir dans l'End et d'Aigue-marine dans l'Aether |

Ces trois textures restent disponibles pour un événement, un minerai saisonnier ou un remplacement si une texture utilisée pose un problème de lisibilité en jeu.

Tous les pets, toutes les armures de minéral et tous les sets à thème sont utilisés.
