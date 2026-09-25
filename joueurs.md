---
description: Toutes les commandes accessibles aux joueurs, par catégorie, avec alias, permission et grade requis.
---

# ⌨️ Commandes joueurs

Syntaxe : `<obligatoire>` et `[facultatif]`. Grade « Tous » : disponible dès le grade Joueur. Toutes les permissions joueur sont accordées au groupe `default`, sauf mention contraire. Liste complète : [Permissions](permissions.md).

Les commandes sociales et utilitaires (`/tpa`, `/msg`, `/mail`, `/trash`, etc.) sont fournies par le module Social du plugin STRATA, pas par EssentialsX : le serveur n'installe aucun plugin qui ajouterait `/pay`, `/home` ou `/fly`.

## 🧭 Navigation et téléportation

| Commande | Alias | Utilité | Permission | Grade |
| --- | --- | --- | --- | --- |
| `/spawn` | `/lobby` | Téléporte au spawn, délai de 5 s | `strata.player.spawn` | Tous |
| `/hub` | | Téléporte au hub du biome actuel, délai de 5 s | `strata.player.hub` | Tous |
| `/relais [nord/sud/est/ouest]` | | Sans argument : menu des relais. Avec argument : téléporte au relais | `strata.player.relais` | Tous |
| `/biomes [biome]` | `/voyage`, `/mines` | Sans argument : menu Voyage. Avec argument : téléporte au hub du biome, s'il est débloqué | `strata.player.biomes` | Tous |
| `/back` | | Revient à la position qui précédait la dernière téléportation, si elle est dans un biome débloqué. Délai de 5 s, utilisable une fois par téléportation | `strata.player.back` | Tous |
| `/tpa <joueur>` | | Demande à se téléporter vers un joueur | `strata.player.tpa` | Tous |
| `/tpahere <joueur>` | | Demande à un joueur de venir à soi | `strata.player.tpahere` | Tous |
| `/tpaccept [joueur]` | `/tpyes` | Accepte la dernière demande, ou celle du joueur indiqué | `strata.player.tpa` | Tous |
| `/tpdeny [joueur]` | `/tpno` | Refuse une demande | `strata.player.tpa` | Tous |
| `/tpacancel [joueur]` | | Annule une demande envoyée | `strata.player.tpa` | Tous |
| `/tptoggle` | | Accepte ou refuse toutes les demandes de téléportation | `strata.player.tptoggle` | Tous |

Délai de 5 s sans bouger avant chaque téléportation. Héros et supérieurs : immédiat (`strata.tp.nodelay`).

**Règles de `/tpa` et `/tpahere`**

* La demande expire après 60 s.
* Délai entre deux demandes : 60 s pour Joueur, 45 s Pilier, 30 s Héros et Champion, 15 s Légende et supérieurs.
* Le joueur téléporté doit avoir débloqué, **dans son cycle en cours**, le biome de destination. Sinon la demande est refusée avec le message : « Lyra est dans les Badlands, que tu n'as pas encore débloqués. »
* Destination au spawn ou dans un hub : toujours autorisée.
* Arrivée à la position exacte du joueur cible si elle est sûre, sinon sur le bloc sûr le plus proche.
* Impossible pendant une file d'attente de biome plein : le biome doit avoir une place libre.

## 💬 Chat et social

| Commande | Alias | Utilité | Permission | Grade |
| --- | --- | --- | --- | --- |
| `/msg <joueur> <message>` | `/m`, `/tell`, `/w` | Message privé | `strata.player.msg` | Tous |
| `/r <message>` | `/reply` | Répond au dernier message privé | `strata.player.msg` | Tous |
| `/ignore <joueur>` | | Ignore ou n'ignore plus un joueur : chat, messages, demandes de téléportation | `strata.player.ignore` | Tous |
| `/ignorelist` | | Liste des joueurs ignorés | `strata.player.ignore` | Tous |
| `/mail send <joueur> <message>` | | Message laissé à un joueur hors ligne | `strata.player.mail` | Tous |
| `/mail read` | | Lit ses messages | `strata.player.mail` | Tous |
| `/mail clear` | | Supprime ses messages lus | `strata.player.mail` | Tous |
| `/gc [message]` | | Chat de guilde, ou bascule du canal par défaut | `strata.player.guilde` | Tous |
| `/list` | `/who`, `/online` | Joueurs connectés, par dimension | `strata.player.list` | Tous |
| `/seen <joueur>` | | Dernière connexion d'un joueur | `strata.player.seen` | Tous |
| `/ping [joueur]` | | Latence | `strata.player.ping` | Tous |
| `/tempsdejeu [joueur]` | `/playtime` | Temps de jeu total et temps de minage actif | `strata.player.tempsdejeu` | Tous |
| `/afk` | | Se déclare absent. Automatique après 5 min sans action | `strata.player.afk` | Tous |
| `/signaler <joueur> <raison>` | `/report` | Signale un joueur au staff | `strata.player.signaler` | Tous |
| `/helpop <message>` | | Question au staff connecté | `strata.player.helpop` | Tous |

* `/mail` : 5 messages en attente par destinataire pour Joueur, 20 pour Héros et supérieurs. 200 caractères par message.
* Un joueur absent ne compte pas comme présent pour les boss, la Vote Party et les défis.

## 🧰 Utilitaires

| Commande | Alias | Utilité | Permission | Grade |
| --- | --- | --- | --- | --- |
| `/menu` | | Menu principal | `strata.player.menu` | Tous |
| `/pv [page]` | `/coffre` | Coffre personnel. Sans argument : page 1 | `strata.player.pv` et `strata.pv.pages.<n>` | Tous, pages selon le grade |
| `/trash` | `/poubelle`, `/disposal` | Poubelle de 36 emplacements. Tout ce qui y reste est détruit à la fermeture | `strata.player.trash` | Tous |
| `/parametres` | `/settings` | Menu des paramètres | `strata.player.parametres` | Tous |
| `/aide [sujet]` | `/help` | Aide par sujet : pioche, prestige, renaissance, pets, boss, guilde, commandes | `strata.player.aide` | Tous |
| `/regles` | `/rules` | Règlement du serveur | `strata.player.regles` | Tous |
| `/discord` | | Lien du Discord | `strata.player.liens` | Tous |
| `/site` | | Lien du site | `strata.player.liens` | Tous |
| `/boutique` | `/store` | Lien de la boutique | `strata.player.liens` | Tous |

**Règles de `/trash`** : la pioche, l'objet Menu STRATA et les Œufs ne peuvent pas y être déposés. Un minerai ou un bloc compressé déposé affiche un avertissement : « Ces objets seront détruits, pas vendus. Utilise /sell. »

## 💰 Économie et vente

| Commande | Alias | Utilité | Permission | Grade |
| --- | --- | --- | --- | --- |
| `/solde` | `/bal`, `/money` | Argent, Éclats, Cristaux | `strata.player.solde` | Tous |
| `/sell` | `/sellall` | Vend minerais et blocs compressés de l'inventaire, sauf minerais protégés | `strata.player.sell` | Tous |
| `/sell main` | | Vend seulement la pile tenue en main, même protégée | `strata.player.sell` | Tous |
| `/autosell` | | Active ou coupe la vente automatique | `strata.sell.auto` | Champion, ou premier Prestige III atteint |
| `/valeurs [biome]` | `/taux` | Taux, valeurs et minerai favori d'un biome | `strata.player.valeurs` | Tous |
| `/boosters` | | Boosters actifs et temps restant | `strata.player.boosters` | Tous |

## ⛏️ Pioche et progression

| Commande | Alias | Utilité | Permission | Grade |
| --- | --- | --- | --- | --- |
| `/pioche` | `/pickaxe` | Menu de la pioche | `strata.player.pioche` | Tous |
| `/enchant` | `/enchants` | Menu des enchantements | `strata.player.enchant` | Tous |
| `/forge` | | Menu de forge | `strata.player.forge` | Tous |
| `/prestige` | | Menu de Prestige | `strata.player.prestige` | Tous |
| `/renaissance` | | Menu de Renaissance | `strata.player.renaissance` | Tous |
| `/tutoriel` | | Étape en cours du tutoriel de Bram | `strata.player.tutoriel` | Tous |

## 🐾 Progression permanente

| Commande | Alias | Utilité | Permission | Grade |
| --- | --- | --- | --- | --- |
| `/pets` | | Menu des pets | `strata.player.pets` | Tous |
| `/oeufs` | `/eggs` | Œufs en incubation | `strata.player.oeufs` | Tous |
| `/traits` | | Traits et rerolls | `strata.player.traits` | Tous |
| `/armure` | `/armures` | Armures | `strata.player.armure` | Tous |
| `/garderobe` | `/skins` | Thèmes et skins de pioche | `strata.player.garderobe` | Tous |
| `/race` | | Race et reroll | `strata.player.race` | Tous |
| `/sons` | | Sons de minage | `strata.player.sons` | Tous |
| `/collections [catégorie]` | `/collection` | Collections | `strata.player.collections` | Tous |
| `/titre [titre]` | `/titres` | Titres, ou active un titre | `strata.player.titre` | Tous |

Catégories de `/collections` : `minerais`, `pets`, `armures`, `garderobe`, `boss`, `sons`.

## 🛒 Shop, caisses et votes

| Commande | Alias | Utilité | Permission | Grade |
| --- | --- | --- | --- | --- |
| `/shop` | | Shop rotatif | `strata.player.shop` | Tous |
| `/caisses` | `/cles`, `/crates` | Clés et ouverture des caisses | `strata.player.caisses` | Tous |
| `/vote` | | Sites de vote et Vote Party | `strata.player.vote` | Tous |
| `/voteparty` | `/vp` | Progression de la Vote Party | `strata.player.vote` | Tous |

## 🎪 Événements et boss

| Commande | Alias | Utilité | Permission | Grade |
| --- | --- | --- | --- | --- |
| `/evenements` | `/events` | Prochains événements | `strata.player.evenements` | Tous |
| `/boss` | | Boss, horaires, combat en cours | `strata.player.boss` | Tous |

## 🛡️ Guilde

Alias : `/g`. Permission : `strata.player.guilde` pour toutes les sous-commandes ; le rôle dans la guilde décide de ce qui est autorisé. Règles détaillées dans [Guildes](../social/guildes.md).

| Commande | Rôle | Effet |
| --- | --- | --- |
| `/guilde` | Tous | Menu de la guilde, voir [Menus GUI · Guilde](../menus/guilde.md) |
| `/guilde creer <nom> <tag>` | Sans guilde | Crée une guilde, 50 Cristaux |
| `/guilde inviter <joueur>` | Officier | Invitation valable 5 min |
| `/guilde accepter <guilde>` | Invité | Rejoint la guilde |
| `/guilde refuser <guilde>` | Invité | Refuse l'invitation |
| `/guilde quitter` | Membre | Quitte la guilde, confirmation demandée |
| `/guilde exclure <joueur>` | Officier | Exclut un membre |
| `/guilde promouvoir <joueur>` | Chef | Membre vers officier |
| `/guilde retrograder <joueur>` | Chef | Officier vers membre |
| `/guilde chef <joueur>` | Chef | Transmet le rôle de chef, confirmation demandée |
| `/guilde deposer <montant>` | Membre | Dépose des Cristaux dans la banque |
| `/guilde ferveur` | Officier | Active la Ferveur |
| `/guilde info [guilde]` | Tous | Fiche d'une guilde |
| `/guilde membres` | Membre | Liste des membres, rôles, dernière connexion |
| `/guilde defis` | Membre | Défis de la semaine et contributions |
| `/guilde top` | Tous | Classements |
| `/guilde renommer <nom>` | Chef | 150 Cristaux de la banque |
| `/guilde tag <tag>` | Chef | 150 Cristaux de la banque |
| `/guilde dissoudre` | Chef | Dissout la guilde, double confirmation |
| `/gc [message]` | Membre | Chat de guilde |

## 📊 Profil et classements

| Commande | Alias | Utilité | Permission | Grade |
| --- | --- | --- | --- | --- |
| `/profil [joueur]` | `/p` | Fiche d'un joueur | `strata.player.profil` | Tous |
| `/stats [joueur]` | | Statistiques | `strata.player.stats` | Tous |
| `/top [catégorie]` | `/classement` | Classements | `strata.player.top` | Tous |

Catégories de `/top` : `progression`, `renaissance`, `prestige`, `nouveaudepart`, `blocs`, `blocsvie`, `boss`, `reaction`, `mythiques`, `collections`, `guildes`.

## 🚫 Commandes volontairement absentes

| Commande | Raison |
| --- | --- |
| `/pay`, `/trade`, `/ah` | Aucun échange entre joueurs : Argent et minerais sont liés au cycle |
| `/home`, `/sethome`, `/warp` | Les déplacements passent par le spawn, les hubs et les relais |
| `/rtp`, `/wild` | Les mines sont des zones publiques concentrées autour des relais |
| `/fly` | Le vol casserait le minage et l'anti-triche |
| `/craft`, `/ec`, `/enderchest` | Pas d'artisanat vanilla ; le stockage passe par `/pv` |
| `/hat`, `/nick` | Cosmétiques gérés par les skins et les titres |
| `/kit`, `/feed`, `/heal` | Aucun objet de départ en dehors de la pioche ; ni faim ni dégâts dans les mines |
