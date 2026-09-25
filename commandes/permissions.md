---
description: Arborescence complète des permissions, par niveau d'accès.
---

# 🔑 Permissions

Trois niveaux, qui ne se mélangent jamais : joueur, staff, administration.

## 👤 Joueur

Accordées explicitement au groupe `default` :

| Permission | Accès |
| --- | --- |
| `strata.profil` | `/profil` |
| `strata.stats`, `strata.top` | Statistiques et classements |
| `strata.titre` | Choix du titre |
| `strata.pioche` | `/pioche`, `/forge`, `/enchant` |
| `strata.solde`, `strata.sell`, `strata.valeurs` | Économie de base |
| `strata.pv` | `/pv` |
| `strata.pets`, `strata.traits` | Pets, Œufs, traits |
| `strata.armure`, `strata.race`, `strata.garderobe`, `strata.sons` | Personnalisation et progression permanente |
| `strata.collections`, `strata.rebirth` | Collections et Rebirth |
| `strata.shop`, `strata.caisses`, `strata.vote` | Shop, caisses, vote |
| `strata.tp.spawn`, `strata.tp.biome`, `strata.tp.hub`, `strata.tp.relais` | Téléportations |
| `strata.compagnie`, `strata.compagnie.creer`, `strata.compagnie.chat` | Compagnie |
| `strata.parametres`, `strata.aide`, `strata.player.tutoriel` | Réglages, aide, tutoriel |
| `essentials.msg`, `essentials.ignore` | Messages privés et ignorer un joueur |

Accordées par grade :

| Permission | Grade |
| --- | --- |
| `strata.pv.pages.<1 à 8>` | Selon le grade, voir [Grades](../grades/grades.md) |
| `strata.grade.bonus.<2 à 12>` | Pilier à Immortal |
| `strata.tp.hub.nodelay` | Héros |
| `strata.sell.auto` | Champion |
| `strata.queue.priority.1` | Légende |
| `strata.join.message` | Légende |
| `strata.sons.couronne` | Monarque |
| `strata.queue.priority.2`, `strata.sons.immortel` | Immortal |

Deux règles gérées par le plugin, sans permission :
* **Vente automatique au Rebirth 3** : le plugin autorise `/autosell` si le joueur a `strata.sell.auto` **ou** au moins 3 Rebirth.
* **Page /pv du Rebirth 5** : le plugin ajoute 1 page au nombre donné par `strata.pv.pages.<n>` dès 5 Rebirth. Un Immortal au Rebirth 5 a donc 9 pages.

## 🛡️ Staff

Groupes LuckPerms : `guide` et `moderateur`, le second hérite du premier. Les nœuds `staff.guide` et `staff.moderateur` servent uniquement à identifier le rôle dans les autres plugins.

| Permission | Guide | Modérateur |
| --- | --- | --- |
| `strata.staff.chat` | Oui | Oui |
| `strata.staff.inspect` | Oui | Oui |
| `libertybans.history`, `libertybans.warn`, `libertybans.mute`, `libertybans.kick` | Oui | Oui |
| `essentials.vanish`, `essentials.tp`, `essentials.tphere`, `essentials.invsee` | Non | Oui |
| `strata.staff.pv`, `strata.staff.gel` | Non | Oui |
| `libertybans.ban`, `libertybans.unban` | Non | Oui |

## 🔧 Administration

| Permission | Accès |
| --- | --- |
| `strata.admin.eco` | Monnaies |
| `strata.admin.booster`, `strata.admin.shop` | Boosters globaux, rotation du Shop |
| `strata.admin.pioche` | Tier, niveau, enchantements |
| `strata.admin.rebirth`, `strata.admin.race`, `strata.admin.collection` | Progression permanente |
| `strata.admin.pet`, `strata.admin.armure`, `strata.admin.theme`, `strata.admin.son`, `strata.admin.cle`, `strata.admin.pv` | Objets |
| `strata.admin.biome` | Mondes |
| `strata.admin.reload`, `strata.admin.debug`, `strata.admin.journal` | Maintenance |

## 🔒 Règles

{% hint style="danger" %}
* Aucun grade de joueur ne reçoit une permission `strata.staff.*` ou `strata.admin.*`.
* Aucun rôle staff ne reçoit une permission `strata.admin.*`.
* `strata.admin.*` est réservé à la direction et au développeur.
* Un grade supérieur hérite toujours du grade inférieur. Un grade inférieur ne reçoit jamais une permission d'un grade supérieur. Les avantages de Rebirth ne passent pas par des permissions de grade.
{% endhint %}
