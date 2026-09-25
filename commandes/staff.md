---
description: Commandes de modération réservées au staff.
---

# 🛡️ Commandes staff

Deux rôles : **Guide** (`staff.guide`) et **Modérateur** (`staff.moderateur`). Le Modérateur hérite du Guide.

| Commande | Utilité | Permission | Rôle |
| --- | --- | --- | --- |
| `/staffchat <message>`, alias `/sc` | Chat staff | `strata.staff.chat` | Guide |
| `/strata inspect <joueur>` | Profil complet en lecture seule | `strata.staff.inspect` | Guide |
| `/history <joueur>` | Historique des sanctions | `libertybans.history` | Guide |
| `/warn <joueur> <raison>` | Avertissement | `libertybans.warn` | Guide |
| `/mute <joueur> <durée> <raison>` | Rendre muet | `libertybans.mute` | Guide |
| `/kick <joueur> <raison>` | Expulser | `libertybans.kick` | Guide |
| `/vanish` | Invisibilité | `essentials.vanish` | Modérateur |
| `/tp <joueur>` | Se téléporter à un joueur | `essentials.tp` | Modérateur |
| `/tphere <joueur>` | Téléporter un joueur à soi | `essentials.tphere` | Modérateur |
| `/invsee <joueur>` | Voir l'inventaire | `essentials.invsee` | Modérateur |
| `/strata pv voir <joueur> [page]` | Voir un `/pv` en lecture seule | `strata.staff.pv` | Modérateur |
| `/ban <joueur> <raison>` | Bannir | `libertybans.ban` | Modérateur |
| `/tempban <joueur> <durée> <raison>` | Bannir temporairement | `libertybans.ban` | Modérateur |
| `/unban <joueur>` | Lever un bannissement | `libertybans.unban` | Modérateur |
| `/strata gel <joueur>` | Immobiliser un joueur pendant une vérification | `strata.staff.gel` | Modérateur |

Exemple : `/tempban Lyra 3d Macro de minage`.

{% hint style="warning" %}
Aucune commande staff ne modifie une ressource, une progression ou un objet. Toute correction passe par un administrateur.
{% endhint %}
