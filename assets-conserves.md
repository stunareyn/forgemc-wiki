---
description: Correspondance entre les assets fournis et leur usage, et liste des assets conservés pour plus tard.
---

# 📦 Assets

Aucune texture et aucun modèle nouveaux ne sont nécessaires. Chaque élément visuel du serveur utilise un asset fourni, un bloc, un objet ou un son vanilla, ou un skin de joueur existant.

* **Overworld** : minerais, objets, blocs compressés, armures de Fer, d'Or et de Diamant, pioches T1 à T5 : tout est vanilla.
* **Pioches T6 à T17** : textures finales fournies par la direction, hors du périmètre de ce document. Sans texture fournie, aucune n'est créée : T6 à T12 utilisent le modèle vanilla de la pioche en diamant, T13 à T17 celui de la pioche en netherite, nom à la couleur de référence du tier.
* **PNJ et têtes de race** : skins de joueur existants.
* **Menus** : uniquement des objets vanilla, voir [Menus GUI](../menus/menus.md).
* **Boss** : aucun modèle, ils sont invisibles.
* **Biomes** : biomes vanilla, avec leur ciel, leur brouillard, leur musique et leurs particules d'origine.

## ✅ Utilisation des assets fournis

| Famille | Fournis | Utilisés | Où |
| --- | --- | --- | --- |
| Textures de minerai | 39 | 27 | [Minerais](../minerais/minerais.md), Nether, End et Aether |
| Pets | 22 | 22 | [Pets](../pets/pets.md) |
| Armures de minéral | 12 | 12 | [Armures](../armures/armures.md), Nether, End et Aether |
| Sets à thème | 11 | 11 | [Skins](../skins/skins.md) |

## 🔁 Correspondances à connaître

**Minerais dont le nom en jeu diffère de la texture**

| Nom en jeu | Texture | Dimension |
| --- | --- | --- |
| Bitume | `oil` | Nether |
| Braise | `wulfenite` | Nether |
| Tungstène | `tungsten` | Nether |
| Ambre | `amber` | Nether |
| Sanguine | `bloodstone` | Nether |
| Rubis | `ruby` | Nether |
| Carmin | `rhodonite` | Nether |
| Infernium | `arcanite` | Nether |
| Spodumène | `lithium` | End |
| Améthyste | `amethyst` | End |
| Galène | `galenite` | End |
| Vesper | `iolite` | End |
| Quartz fumé | `smoky quartz` | End |
| Pulsar | `labradorite` | End |
| Opale | `opal` | End |
| Givre | `silver` | Aether |
| Orichalque | `bismuth` | Aether |
| Aigue-marine | `aquamarine` | Aether |
| Disthène | `kyanite` | Aether |
| Nova | `crystalite` | Aether |
| Aurore | `charoite` | Aether |
| Éther | `pearl` | Aether |

Citrine, Onyx, Iridium, Jade et Mythril gardent le nom de leur texture. Le minerai Givre utilise la texture `silver` pour éviter toute confusion avec la monnaie Argent.

**Armures de minéral**

| Armure | Asset | Dimension |
| --- | --- | --- |
| Ambre | Amber | Nether |
| Sanguine | Bloodstone | Nether |
| Rubis | Rubis | Nether |
| Carmin | Rhodonite | Nether |
| Galène | Galenite | End |
| Vesper | Iolite | End |
| Quartz fumé | Smoky Quartz | End |
| Pulsar | Labradorite | End |
| Aigue-marine | Aquamarine | Aether |
| Disthène | Kyanite | Aether |
| Nova | Crystalite | Aether |
| Aurore | Charoite | Aether |

**Sets à thème** : utilisés comme skins d'armure et, à la complétion d'un thème, comme skin de pioche. Si un set ne contient pas de texture de pioche, la récompense de complétion devient un titre « Thème <nom du thème> ».

## 🎨 Points à vérifier par le graphiste

* Le fond de chaque texture de minerai doit correspondre au bloc principal de sa dimension : Netherrack, End Stone ou Calcite.
* Couleurs proches dans une même dimension, à différencier par le motif si besoin : Aigue-marine et Disthène dans l'Aether, Améthyste et Vesper dans l'End, Givre et Mythril dans l'Aether, Carmin et Rubis dans le Nether.
* La caisse Chroma ne propose que les thèmes dont la version Chroma est fournie. Si une version manque, le thème est retiré de la caisse et ses probabilités sont réparties sur les thèmes de même rareté.

## 🗃️ ASSETS CONSERVÉS POUR PLUS TARD

| Asset | Type | Raison |
| --- | --- | --- |
| `limonite` | Texture de minerai | L'Overworld utilise désormais les minerais vanilla |
| `barite` | Texture de minerai | Idem |
| `patrified` | Texture de minerai | Idem |
| `malachite` | Texture de minerai | Idem |
| `fluorite` | Texture de minerai | Idem |
| `rhodolite` | Texture de minerai | Idem |
| `sapphire` | Texture de minerai | 27 textures suffisent pour 3 dimensions de 9 minerais ; bleu proche de l'Aigue-marine et du Disthène |
| `adamantium` | Texture de minerai | 27 textures suffisent ; nom trop proche de Mythril dans le même registre |
| `platinum` | Texture de minerai | 27 textures suffisent ; gris clair proche de Givre (`silver`) |
| `magnesite` | Texture de minerai | Blanc, trop proche de la Calcite, bloc principal de l'Aether, et de `pearl` |
| `garnierite` | Texture de minerai | Vert, trop proche du Jade dans l'Aether |
| `apatite` | Texture de minerai | Bleu-vert, trop proche de l'Aigue-marine dans l'Aether |

**Total : 12 textures de minerai conservées.** Elles restent disponibles pour un événement, un minerai saisonnier ou un remplacement si une texture utilisée pose un problème de lisibilité en jeu.

Tous les pets, toutes les armures de minéral et tous les sets à thème sont utilisés.
