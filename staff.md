---
description: Commandes de modération réservées au staff, par rôle.
---

# 🛡️ Commandes staff

Deux rôles : **Guide** (groupe `guide`) et **Modérateur** (groupe `moderateur`). Le Modérateur hérite du Guide. Les sanctions passent par LibertyBans ; les autres outils par le module Staff du plugin STRATA.

| Commande | Utilité | Permission | Rôle |
| --- | --- | --- | --- |
| `/staffchat <message>`, alias `/sc` | Chat staff, relayé sur Discord | `strata.staff.chat` | Guide |
| `/strata inspect <joueur>` | Profil complet en lecture seule : progression, monnaies, pets, historique des Prestiges | `strata.staff.inspect` | Guide |
| `/signalements` | Liste des signalements `/signaler` et questions `/helpop` en attente | `strata.staff.signalements` | Guide |
| `/history <joueur>` | Historique des sanctions | `libertybans.history` | Guide |
| `/warn <joueur> <raison>` | Avertissement | `libertybans.warn` | Guide |
| `/mute <joueur> <durée> <raison>` | Rendre muet | `libertybans.mute` | Guide |
| `/unmute <joueur>` | Lever un mute | `libertybans.unmute` | Guide |
| `/kick <joueur> <raison>` | Expulser | `libertybans.kick` | Guide |
| `/vanish` | Invisibilité, exclue des boss, Concours et classements | `strata.staff.vanish` | Modérateur |
| `/tp <joueur>` | Se téléporter à un joueur, sans condition de biome | `strata.staff.tp` | Modérateur |
| `/tphere <joueur>` | Téléporter un joueur à soi | `strata.staff.tphere` | Modérateur |
| `/invsee <joueur>` | Voir l'inventaire, lecture seule | `strata.staff.invsee` | Modérateur |
| `/strata pv voir <joueur> [page]` | Voir un `/pv`, lecture seule | `strata.staff.pv` | Modérateur |
| `/strata gel <joueur>` | Immobiliser un joueur pendant une vérification. Le minage et les commandes sont bloqués | `strata.staff.gel` | Modérateur |
| `/strata anticheat <joueur>` | Alertes anti-triche récentes : cadence, blocs par seconde, clics | `strata.staff.anticheat` | Modérateur |
| `/ban <joueur> <raison>` | Bannir | `libertybans.ban` | Modérateur |
| `/tempban <joueur> <durée> <raison>` | Bannir temporairement | `libertybans.ban` | Modérateur |
| `/unban <joueur>` | Lever un bannissement | `libertybans.unban` | Modérateur |
| `/strata chat clear` | Vider le chat global | `strata.staff.chatclear` | Modérateur |
| `/strata chat slow <secondes>` | Mode lent du chat global | `strata.staff.chatslow` | Modérateur |

Exemple : `/tempban Lyra 3d Macro de minage`.

{% hint style="warning" %}
* Aucune commande staff ne modifie une ressource, une progression ou un objet. Toute correction passe par un administrateur.
* Un membre du staff en `/vanish` ne compte pas comme joueur présent : il n'augmente pas les PV d'un boss et ne reçoit aucune récompense d'événement.
{% endhint %}
