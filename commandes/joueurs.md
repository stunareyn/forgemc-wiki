---
description: Toutes les commandes accessibles aux joueurs, par catégorie, avec permission et grade requis.
---

# ⌨️ Commandes joueurs

Syntaxe : `<obligatoire>` et `[facultatif]`. Grade « Tous » : disponible dès le grade Joueur.

## 👤 Profil et statistiques

| Commande | Utilité | Permission | Grade |
| --- | --- | --- | --- |
| `/profil [joueur]` | Fiche d'un joueur | `strata.profil` | Tous |
| `/stats [joueur]` | Statistiques de run et de vie | `strata.stats` | Tous |
| `/top <catégorie>` | Classements | `strata.top` | Tous |
| `/titre [titre]` | Choisir le titre affiché | `strata.titre` | Tous |

Catégories de `/top` : `rebirth`, `temps`, `blocs`, `argent`, `mythiques`, `collections`, `compagnies`.

Exemple : `/top temps` affiche le meilleur temps de run de la tranche de Rebirth du joueur.

## ⛏️ Pioche et enchantements

| Commande | Utilité | Permission | Grade |
| --- | --- | --- | --- |
| `/pioche` | Menu de la pioche : forge, enchantements, statistiques | `strata.pioche` | Tous |
| `/forge` | Ouvre directement l'onglet de forge | `strata.pioche` | Tous |
| `/enchant` | Ouvre directement l'onglet des enchantements | `strata.pioche` | Tous |

## 💰 Économie et vente

| Commande | Utilité | Permission | Grade |
| --- | --- | --- | --- |
| `/solde` | Argent, Éclats, Cristaux | `strata.solde` | Tous |
| `/sell` | Vend les minerais de l'inventaire, sauf protégés | `strata.sell` | Tous |
| `/autosell` | Active ou coupe la vente automatique | `strata.sell.auto` | Champion, ou Rebirth 3 |
| `/valeurs [biome]` | Taux et valeurs du biome | `strata.valeurs` | Tous |
| `/pv [page]` | Coffre personnel | `strata.pv` et `strata.pv.pages.<n>` | Tous, pages selon grade |

## 🐾 Pets, traits, armures, race, skins

| Commande | Utilité | Permission | Grade |
| --- | --- | --- | --- |
| `/pets` | Menu des pets : équiper, Éveil, recyclage, Essences | `strata.pets` | Tous |
| `/traits` | Menu des traits et rerolls | `strata.traits` | Tous |
| `/oeufs` | Œufs en incubation et progression | `strata.pets` | Tous |
| `/armure` | Fabrication et port des armures | `strata.armure` | Tous |
| `/race` | Race actuelle, reroll | `strata.race` | Tous |
| `/garderobe` | Appliquer les thèmes et skins de pioche | `strata.garderobe` | Tous |
| `/sons` | Choisir son son de minage | `strata.sons` | Tous |

## 📚 Collections et Rebirth

| Commande | Utilité | Permission | Grade |
| --- | --- | --- | --- |
| `/collections [catégorie]` | Progression des collections | `strata.collections` | Tous |
| `/rebirth` | Menu et confirmation du Rebirth | `strata.rebirth` | Tous |

Catégories de `/collections` : `minerais`, `pets`, `armures`, `garderobe`, `sons`.

## 🛒 Shop et caisses

| Commande | Utilité | Permission | Grade |
| --- | --- | --- | --- |
| `/shop` | Shop rotatif | `strata.shop` | Tous |
| `/caisses` | Clés possédées, téléportation aux caisses | `strata.caisses` | Tous |
| `/vote` | Liens de vote et compteur du jour | `strata.vote` | Tous |

## 🧭 Téléportation

| Commande | Utilité | Permission | Grade |
| --- | --- | --- | --- |
| `/spawn` | Retour au spawn | `strata.tp.spawn` | Tous |
| `/biomes` | Menu de voyage vers les biomes débloqués | `strata.tp.biome` | Tous |
| `/hub` | Retour au hub du biome actuel, délai de 5 s | `strata.tp.hub` | Tous |
| `/relais` | Menu des 4 relais du biome actuel | `strata.tp.relais` | Tous |

Héros et plus : `/hub` sans délai (`strata.tp.hub.nodelay`).

## 🏢 Compagnie

| Commande | Utilité | Permission | Grade |
| --- | --- | --- | --- |
| `/compagnie creer <nom>` | Créer, 50 Cristaux | `strata.compagnie.creer` | Tous |
| `/compagnie inviter <joueur>` | Inviter | `strata.compagnie` | Officier |
| `/compagnie rejoindre <nom>` | Accepter une invitation | `strata.compagnie` | Tous |
| `/compagnie quitter` | Quitter | `strata.compagnie` | Tous |
| `/compagnie expulser <joueur>` | Expulser | `strata.compagnie` | Officier |
| `/compagnie promouvoir <joueur>` | Nommer Officier | `strata.compagnie` | Fondateur |
| `/compagnie info [nom]` | Niveau, membres, points | `strata.compagnie` | Tous |
| `/compagnie dissoudre` | Supprimer la Compagnie | `strata.compagnie` | Fondateur |
| `/cc <message>` | Chat de Compagnie | `strata.compagnie.chat` | Tous |

Les rôles Officier et Fondateur sont des rôles internes à la Compagnie, pas des grades serveur.

## ⚙️ Paramètres et messagerie

| Commande | Utilité | Permission | Grade |
| --- | --- | --- | --- |
| `/parametres` | Réglages personnels | `strata.parametres` | Tous |
| `/msg <joueur> <message>` | Message privé | `essentials.msg` | Tous |
| `/r <message>` | Répondre | `essentials.msg` | Tous |
| `/ignore <joueur>` | Ignorer un joueur | `essentials.ignore` | Tous |
| `/aide` | Aide et liens vers les menus | `strata.aide` | Tous |

Réglages de `/parametres` : fréquence du son de minage, seuil de notification de rareté, affichage des pets des autres joueurs, minerais protégés, messages de vente, confirmation de vente.
