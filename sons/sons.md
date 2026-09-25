---
description: Les sons de minage, leur obtention et leur réglage.
---

# 🔊 Sons de minage

## ⚙️ Fonctionnement

* Le joueur choisit le son joué quand **il** casse un bloc, dans `/sons`.
* Le son est envoyé **au joueur seul**. Personne d'autre ne l'entend.
* Réglage de fréquence dans `/parametres` : tous les blocs, minerais seulement, minerais Rares et plus seulement, désactivé.
* Tous les sons sont des sons vanilla : aucune ressource ajoutée.
* Sons conservés au Rebirth.

## 📋 Les 12 sons de la collection

| Son | Rareté | Son vanilla | Obtention |
| --- | --- | --- | --- |
| Classique | Commun | Son normal du bloc | Par défaut |
| Pierre | Peu commun | `block.deepslate.break` | Collection Overworld, 9 minerais au palier II |
| Cendre | Peu commun | `block.fire.extinguish`, volume 0,4 | Collection Nether, 9 minerais au palier II |
| Écho | Rare | `block.sculk.break` | Collection End, 9 minerais au palier II |
| Carillon | Rare | `block.amethyst_block.chime` | Collection Aether, 9 minerais au palier II |
| Pièces | Rare | `entity.experience_orb.pickup` | Caisse Vote, 0,2 % |
| Forge | Rare | `block.anvil.land`, volume 0,25 | Shop rotatif, 150 Cristaux |
| Cloche | Épique | `block.note_block.bell` | Shop rotatif, 250 Cristaux |
| Verre | Épique | `block.glass.break`, hauteur 1,4 | Shop rotatif Vedette, 400 Cristaux |
| Aube | Épique | `block.respawn_anchor.charge` | Rebirth 1 |
| Tintement | Légendaire | `block.note_block.pling`, volume 0,4 | Collection Armures, 12 armures complètes |
| Éternité | Mythique | `block.end_portal_frame.fill` | Rebirth 25 |

Les 12 sons s'obtiennent tous sans achat.

## 👑 Sons de grade, hors collection

| Son | Son vanilla | Obtention |
| --- | --- | --- |
| Couronne | `block.note_block.chime` | Grade Monarque |
| Immortel | `entity.player.levelup`, hauteur 2 | Grade Immortal |

Ces deux sons ne comptent pas dans la collection, pour qu'elle reste complétable gratuitement.

## 🔗 Collection

* Posséder les 12 sons de la collection : titre « Mélomane ».
* Aucun son ne donne de bonus de jeu.

## 📏 Contraintes techniques

* Volume maximal 0,6, jamais au-dessus du son vanilla du bloc.
* Un seul son par bloc cassé, même avec l'Excavation : les blocs de la zone ne jouent pas de son supplémentaire.
