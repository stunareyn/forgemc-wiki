---
description: Arborescence complète des permissions, par niveau d'accès.
---

# 🔑 Permissions

Trois niveaux, qui ne se mélangent jamais : joueur, staff, administration. Gestion par LuckPerms.

## 👤 Joueur

Le groupe `default` reçoit `strata.player.*`, qui contient les 53 permissions suivantes :

| Domaine | Permissions |
| --- | --- |
| Navigation | `strata.player.spawn`, `strata.player.hub`, `strata.player.relais`, `strata.player.biomes`, `strata.player.back`, `strata.player.tpa`, `strata.player.tpahere`, `strata.player.tptoggle` |
| Chat et social | `strata.player.msg`, `strata.player.ignore`, `strata.player.mail`, `strata.player.list`, `strata.player.seen`, `strata.player.ping`, `strata.player.tempsdejeu`, `strata.player.afk`, `strata.player.signaler`, `strata.player.helpop` |
| Utilitaires | `strata.player.menu`, `strata.player.pv`, `strata.player.trash`, `strata.player.parametres`, `strata.player.aide`, `strata.player.regles`, `strata.player.liens` |
| Économie | `strata.player.solde`, `strata.player.sell`, `strata.player.valeurs`, `strata.player.boosters` |
| Pioche et progression | `strata.player.pioche`, `strata.player.enchant`, `strata.player.forge`, `strata.player.prestige`, `strata.player.renaissance`, `strata.player.tutoriel` |
| Progression permanente | `strata.player.pets`, `strata.player.oeufs`, `strata.player.traits`, `strata.player.armure`, `strata.player.garderobe`, `strata.player.race`, `strata.player.sons`, `strata.player.collections`, `strata.player.titre` |
| Shop, caisses, votes | `strata.player.shop`, `strata.player.caisses`, `strata.player.vote` |
| Événements | `strata.player.evenements`, `strata.player.boss` |
| Guilde | `strata.player.guilde` |
| Profil et classements | `strata.player.profil`, `strata.player.stats`, `strata.player.top` |

Accordées par grade, voir [Grades](../grades/grades.md) :

| Permission | Effet | Grade |
| --- | --- | --- |
| `strata.pv.pages.<1 à 8>` | Nombre de pages `/pv` | Joueur 1, Pilier 2, Héros 3, Champion 4, Légende 5, Monarque 6, Immortal 8 |
| `strata.grade.bonus.<2 à 12>` | Bonus d'Argent du grade | Pilier à Immortal |
| `strata.tpa.cooldown.<60, 45, 30, 15>` | Délai entre deux demandes `/tpa` | Joueur 60, Pilier 45, Héros 30, Légende 15 |
| `strata.mail.limit.<5, 20>` | Messages `/mail` en attente | Joueur 5, Héros 20 |
| `strata.chat.delay.<2, 1>` | Délai entre deux messages, 3 s par défaut | Pilier 2, Champion 1 |
| `strata.tp.nodelay` | Téléportations sans délai | Héros |
| `strata.sell.auto` | Vente automatique | Champion |
| `strata.chat.color` | Couleurs dans le chat | Champion |
| `strata.queue.priority.1` | Priorité dans la file d'attente | Légende |
| `strata.join.message` | Message de connexion | Légende |
| `strata.sons.couronne` | Son de minage Couronne | Monarque |
| `strata.guilde.tagcolor` | Couleur du tag de guilde sans coût | Monarque |
| `strata.queue.priority.2`, `strata.sons.immortel` | Priorité maximale, son Immortel | Immortal |

Pour une permission numérique, le plugin retient la valeur la plus avantageuse que possède le joueur.

**Règles gérées par le plugin, sans permission** :

* **Vente automatique au Prestige III** : `/autosell` est autorisé si le joueur a `strata.sell.auto` **ou** a atteint au moins une fois le Prestige III.
* **Page `/pv` de la Renaissance 1** : le plugin ajoute 1 page au nombre donné par `strata.pv.pages.<n>` dès la Renaissance 1. Un Immortal Renaissance 1 a donc 9 pages.
* **Emplacements de pet** : calculés par le plugin à partir du Prestige maximal atteint et de la Renaissance.

## 🛡️ Staff

Groupes LuckPerms : `guide` et `moderateur`, le second hérite du premier.

| Permission | Guide | Modérateur |
| --- | --- | --- |
| `strata.staff.chat`, `strata.staff.inspect`, `strata.staff.signalements` | Oui | Oui |
| `libertybans.history`, `libertybans.warn`, `libertybans.mute`, `libertybans.unmute`, `libertybans.kick` | Oui | Oui |
| `strata.staff.vanish`, `strata.staff.tp`, `strata.staff.tphere`, `strata.staff.invsee` | Non | Oui |
| `strata.staff.pv`, `strata.staff.gel`, `strata.staff.anticheat` | Non | Oui |
| `strata.staff.chatclear`, `strata.staff.chatslow` | Non | Oui |
| `libertybans.ban`, `libertybans.unban` | Non | Oui |

## 🔧 Administration

| Permission | Accès |
| --- | --- |
| `strata.admin.eco`, `strata.admin.booster`, `strata.admin.shop` | Monnaies, boosters, Shop |
| `strata.admin.pioche`, `strata.admin.prestige`, `strata.admin.renaissance` | Pioche, Prestige, Renaissance, Mémoire de forge, biomes débloqués |
| `strata.admin.race`, `strata.admin.collection`, `strata.admin.stats` | Race, collections, statistiques |
| `strata.admin.pet`, `strata.admin.armure`, `strata.admin.theme`, `strata.admin.son`, `strata.admin.titre`, `strata.admin.cle`, `strata.admin.pv` | Objets |
| `strata.admin.boss`, `strata.admin.event` | Boss et événements |
| `strata.admin.guilde` | Guildes |
| `strata.admin.biome` | Mondes |
| `strata.admin.reload`, `strata.admin.debug`, `strata.admin.journal`, `strata.admin.annonce` | Maintenance |

## 🔒 Règles

{% hint style="danger" %}
* Aucun grade de joueur ne reçoit une permission `strata.staff.*` ou `strata.admin.*`.
* Aucun rôle staff ne reçoit une permission `strata.admin.*`.
* `strata.admin.*` est réservé à la direction et au développeur.
* Un grade supérieur hérite toujours du grade inférieur. Les avantages de Prestige et de Renaissance ne passent jamais par des permissions de grade.
{% endhint %}
