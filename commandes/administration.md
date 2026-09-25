---
description: Commandes d'administration du plugin STRATA.
---

# 🔧 Commandes d'administration

Toutes sous `/strata`. Permission racine : `strata.admin.*`. Chaque action est journalisée avec l'auteur, la cible, l'ancienne et la nouvelle valeur.

## 💰 Économie

| Commande | Utilité | Permission |
| --- | --- | --- |
| `/strata eco <give/take/set> <joueur> <argent/eclats/cristaux> <montant>` | Modifier une monnaie | `strata.admin.eco` |
| `/strata booster global <argent/xp/eclats/chance> <pourcent> <minutes>` | Booster global | `strata.admin.booster` |
| `/strata shop rotate` | Forcer une rotation du Shop | `strata.admin.shop` |

Exemple : `/strata eco give Lyra cristaux 50`.

## ⛏️ Progression

| Commande | Utilité | Permission |
| --- | --- | --- |
| `/strata pioche set <joueur> <tier>` | Fixer le tier de pioche | `strata.admin.pioche` |
| `/strata niveau set <joueur> <niveau>` | Fixer le niveau de pioche | `strata.admin.pioche` |
| `/strata enchant set <joueur> <enchant> <niveau>` | Fixer un enchantement | `strata.admin.pioche` |
| `/strata rebirth set <joueur> <n>` | Fixer le nombre de Rebirth | `strata.admin.rebirth` |
| `/strata race set <joueur> <race>` | Fixer la race | `strata.admin.race` |
| `/strata collection reset <joueur> <catégorie>` | Réinitialiser une collection | `strata.admin.collection` |

## 🐾 Objets

| Commande | Utilité | Permission |
| --- | --- | --- |
| `/strata pet give <joueur> <pet_id> [niveau] [étoiles]` | Donner un pet | `strata.admin.pet` |
| `/strata trait set <joueur> <pet_id> <trait> <rareté>` | Fixer un trait | `strata.admin.pet` |
| `/strata oeuf give <joueur> <dimension> [n]` | Donner des Œufs | `strata.admin.pet` |
| `/strata armure give <joueur> <armure> <pièce/all>` | Donner une armure | `strata.admin.armure` |
| `/strata theme give <joueur> <thème> <pièce/all> [chroma]` | Donner un skin | `strata.admin.theme` |
| `/strata son give <joueur> <son>` | Donner un son | `strata.admin.son` |
| `/strata cle give <joueur> <caisse> <n>` | Donner des clés | `strata.admin.cle` |
| `/strata pv voir <joueur> [page] edit` | Modifier un `/pv` | `strata.admin.pv` |

Identifiants de caisse : `vote`, `pets_f2w`, `pets_premium`, `themes`, `themes_chroma`.

Exemple : `/strata pet give Lyra pet_aether_dragon 40 3`.

## 🌍 Mondes

| Commande | Utilité | Permission |
| --- | --- | --- |
| `/strata biome info [biome]` | Joueurs, file d'attente, régénération en attente | `strata.admin.biome` |
| `/strata biome regen <biome>` | Régénération complète de secours | `strata.admin.biome` |
| `/strata biome fermer <biome>` | Fermer un biome, les joueurs vont au spawn | `strata.admin.biome` |
| `/strata biome ouvrir <biome>` | Rouvrir un biome | `strata.admin.biome` |

## 🔩 Maintenance

| Commande | Utilité | Permission |
| --- | --- | --- |
| `/strata reload [module]` | Recharger la configuration | `strata.admin.reload` |
| `/strata debug perf` | Temps de tick, file de régénération, paquets | `strata.admin.debug` |
| `/strata journal <joueur> [page]` | Journal des actions admin sur un joueur | `strata.admin.journal` |
