---
description: Commandes d'administration du plugin STRATA, par domaine.
---

# 🔧 Commandes d'administration

Toutes sous `/strata`. Permission racine : `strata.admin.*`. Chaque action est journalisée avec l'auteur, la cible, l'ancienne et la nouvelle valeur. Un joueur dont la progression a été modifiée est marqué et exclu des classements de meilleur temps pour le cycle en cours.

## 💰 Économie

| Commande | Utilité | Permission |
| --- | --- | --- |
| `/strata eco <give/take/set> <joueur> <argent/eclats/cristaux> <montant>` | Modifier une monnaie | `strata.admin.eco` |
| `/strata booster global <argent/xp/eclats/chance> <pourcent> <minutes>` | Booster global | `strata.admin.booster` |
| `/strata booster give <joueur> <xp/eclats/chance> <pourcent> <minutes>` | Booster personnel | `strata.admin.booster` |
| `/strata shop rotate` | Forcer une rotation du Shop | `strata.admin.shop` |

Exemple : `/strata eco give Lyra cristaux 50`.

## ⛏️ Progression

| Commande | Utilité | Permission |
| --- | --- | --- |
| `/strata pioche set <joueur> <tier>` | Fixer le tier de pioche | `strata.admin.pioche` |
| `/strata niveau set <joueur> <niveau>` | Fixer le niveau de pioche | `strata.admin.pioche` |
| `/strata enchant set <joueur> <enchant> <niveau>` | Fixer un enchantement | `strata.admin.pioche` |
| `/strata prestige set <joueur> <0-10>` | Fixer le rang de Prestige | `strata.admin.prestige` |
| `/strata renaissance set <joueur> <0-10>` | Fixer la Renaissance | `strata.admin.renaissance` |
| `/strata memoire <add/remove/reset> <joueur> [tier]` | Modifier la Mémoire de forge | `strata.admin.prestige` |
| `/strata biome unlock <joueur> <biome>` | Débloquer un biome dans le cycle | `strata.admin.prestige` |
| `/strata race set <joueur> <race>` | Fixer la race | `strata.admin.race` |
| `/strata collection reset <joueur> <catégorie>` | Réinitialiser une collection | `strata.admin.collection` |
| `/strata stats reset <joueur> <statistique> <portée>` | Corriger une statistique | `strata.admin.stats` |

## 🐾 Objets

| Commande | Utilité | Permission |
| --- | --- | --- |
| `/strata pet give <joueur> <pet_id> [niveau] [étoiles]` | Donner un pet | `strata.admin.pet` |
| `/strata trait set <joueur> <pet_id> <trait> <rareté>` | Fixer un trait | `strata.admin.pet` |
| `/strata oeuf give <joueur> <dimension> [n]` | Donner des Œufs | `strata.admin.pet` |
| `/strata essence give <joueur> <rareté> [n]` | Donner des Essences | `strata.admin.pet` |
| `/strata armure give <joueur> <armure> <pièce/all>` | Donner une armure | `strata.admin.armure` |
| `/strata theme give <joueur> <thème> <pièce/all> [chroma]` | Donner un skin | `strata.admin.theme` |
| `/strata poussiere <give/take> <joueur> <n>` | Modifier la Poussière Chroma | `strata.admin.theme` |
| `/strata son give <joueur> <son>` | Donner un son | `strata.admin.son` |
| `/strata titre give <joueur> <titre>` | Donner un titre | `strata.admin.titre` |
| `/strata cle give <joueur> <caisse> <n>` | Donner des clés | `strata.admin.cle` |
| `/strata pv voir <joueur> [page] edit` | Modifier un `/pv` | `strata.admin.pv` |

Identifiants de caisse : `vote`, `pets_f2w`, `pets_premium`, `themes`, `themes_chroma`.

Exemple : `/strata pet give Lyra pet_aether_dragon 40 3`.

## 👹 Boss

| Commande | Utilité | Permission |
| --- | --- | --- |
| `/strata boss spawn <dimension>` | Fait apparaître le boss de la dimension, avec annonce de 60 s | `strata.admin.boss` |
| `/strata boss stop <dimension>` | Arrête le combat, sans récompense | `strata.admin.boss` |
| `/strata boss hp <dimension> <pourcentage>` | Fixe les PV restants en % | `strata.admin.boss` |
| `/strata boss garantie <joueur> <boss> <valeur>` | Corrige un compteur de garantie | `strata.admin.boss` |
| `/strata boss planning` | Horaires des 24 prochaines heures | `strata.admin.boss` |

Identifiants de dimension : `overworld`, `nether`, `end`, `aether`.

## 🎪 Événements

| Commande | Utilité | Permission |
| --- | --- | --- |
| `/strata event reaction [type]` | Lance un Chat réaction | `strata.admin.event` |
| `/strata event concours` | Lance un Concours de minage, annonce de 5 min | `strata.admin.event` |
| `/strata event heuredoree [minutes]` | Lance une Heure dorée | `strata.admin.event` |
| `/strata event voteparty` | Lance une Vote Party | `strata.admin.event` |
| `/strata event voteparty set <votes>` | Corrige le compteur de la Vote Party | `strata.admin.event` |
| `/strata event annuler <événement>` | Annule le prochain passage d'un événement planifié | `strata.admin.event` |
| `/strata event decaler <événement> <minutes>` | Décale le prochain passage | `strata.admin.event` |

Types de Chat réaction : `ecrire`, `melange`, `calcul`, `quiz`, `minage`, `chasse`.

## 🛡️ Guildes

| Commande | Utilité | Permission |
| --- | --- | --- |
| `/strata guilde info <guilde>` | Fiche complète, journal de banque | `strata.admin.guilde` |
| `/strata guilde renommer <guilde> <nom>` | Renommer, sans coût | `strata.admin.guilde` |
| `/strata guilde tag <guilde> <tag>` | Changer le tag, sans coût | `strata.admin.guilde` |
| `/strata guilde xp <add/set> <guilde> <montant>` | Corriger l'XP | `strata.admin.guilde` |
| `/strata guilde banque <add/set> <guilde> <montant>` | Corriger la banque | `strata.admin.guilde` |
| `/strata guilde chef <guilde> <joueur>` | Changer le chef | `strata.admin.guilde` |
| `/strata guilde dissoudre <guilde>` | Dissoudre | `strata.admin.guilde` |

## 🌍 Mondes

| Commande | Utilité | Permission |
| --- | --- | --- |
| `/strata biome info [biome]` | Joueurs, file d'attente, régénération en attente | `strata.admin.biome` |
| `/strata biome regen <biome>` | Régénération complète de secours | `strata.admin.biome` |
| `/strata biome fermer <biome>` | Fermer un biome, les joueurs vont au spawn | `strata.admin.biome` |
| `/strata biome ouvrir <biome>` | Rouvrir un biome | `strata.admin.biome` |
| `/strata biome capacite <biome> <joueurs>` | Changer la capacité d'un biome | `strata.admin.biome` |

## 🔩 Maintenance

| Commande | Utilité | Permission |
| --- | --- | --- |
| `/strata reload [module]` | Recharger la configuration | `strata.admin.reload` |
| `/strata debug perf` | Temps de tick, file de régénération, paquets, état Redis | `strata.admin.debug` |
| `/strata journal <joueur> [page]` | Journal des actions admin sur un joueur | `strata.admin.journal` |
| `/strata annonce <message>` | Annonce à tout le réseau | `strata.admin.annonce` |

Modules de `/strata reload` : `biomes`, `minerais`, `pioches`, `enchantements`, `pets`, `armures`, `caisses`, `shop`, `evenements`, `boss`, `menus`, `langue`.
