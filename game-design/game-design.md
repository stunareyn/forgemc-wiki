---
description: Boucles de gameplay, rôle de chaque système, dépendances et décisions de design.
---

# 🧠 Game Design

## 🔁 Les trois boucles

**Boucle courte, quelques minutes**
```
Miner → inventaire → /sell ou Autocraft → enchantement → miner plus vite
```

**Boucle moyenne, quelques heures**
```
Économiser Argent + garder un minerai + atteindre un niveau → nouvelle pioche → nouveau biome plus rentable
```

**Boucle longue, dizaines d'heures**
```
Traverser les 4 dimensions → pets, armures, traits, collections → Rebirth → run suivant plus court
```

## 🧩 Pourquoi chaque système existe

| Système | Problème résolu | Boucle |
| --- | --- | --- |
| Pioche unique | Donner une identité et un fil rouge | Moyenne |
| Enchantements | Donner un achat toutes les quelques minutes | Courte |
| Biomes | Donner une destination à chaque pioche | Moyenne |
| Minerais partagés R à M | Rendre chaque biome excitant, fournir les matériaux | Courte et longue |
| Armures | Premier choix entre vendre et investir | Longue |
| Pets | Récompense permanente trouvée en minant | Longue |
| Traits | Dépense de Cristaux, optimisation fine | Longue |
| Races | Spécialisation, objectif très long | Longue |
| Rebirth | Rendre la réinitialisation désirable | Longue |
| Collections | Donner de la valeur à chaque bloc après le Rebirth 25 | Longue |
| Skins, sons | Montrer sa progression sans toucher à l'équilibrage | Aucune, cosmétique |
| Shop rotatif | Raison de revenir, conversion Argent vers XP ou Éclats | Courte |
| Caisses | Canal de récompense et de monétisation | Longue |
| Compagnie | Minage collectif | Longue |
| `/pv` | Stockage sans sac | Moyenne |

## 🔗 Dépendances

```
Bloc cassé
 ├─ Argent ──────► Pioche (tier) ─► Biome ─► valeur des blocs
 │                └► Armures ◄─── minerais R, É, L
 ├─ Éclats ──────► Enchantements ─► vitesse, quantité, valeur
 ├─ XP ──────────► Niveau ─► condition des pioches
 ├─ XP de pet ───► Niveau de pet ─► Éveil ◄─ minerais R, É, L, M
 ├─ Trouvaille ──► Cristaux ─► Traits, Race, Shop
 │               └► Œufs, clés ─► Pets, Skins
 └─ Point de Compagnie ─► niveau de Compagnie ─► bonus d'Argent
```

Chaque bloc cassé alimente six progressions à la fois. Les autres sources, votes, tutoriel, récompenses de Rebirth et boutique, sont des compléments bornés : aucune ne remplace le minage.

## ⚖️ Décisions de design

| Décision | Raison |
| --- | --- |
| 3 biomes par dimension, 12 au total | Une pioche par biome, un rythme régulier, des biomes denses en joueurs |
| 9 minerais par dimension | Assez pour la variété, assez peu pour que chaque minerai soit reconnaissable |
| Minerais Rares à Mythiques partagés dans la dimension | Chaque biome garde des moments forts ; les armures ont une source stable |
| Biome 3 de chaque dimension = zone riche | Raison de rester dans le dernier biome même après avoir la pioche suivante en vue |
| 13 pioches | Chaque pioche débloque quelque chose ; aucune pioche vide |
| Niveau requis sur chaque pioche | Empêche l'Argent seul, donc les achats, de raccourcir un run |
| Pas de booster d'Argent au Shop | Il serait rentable par construction et rendrait le Shop obligatoire |
| Un pet par type de bonus | Empêche l'empilement de pets Argent, donne de la valeur à tous les types |
| Reroll de race avec choix | Un reroll ne punit jamais ; la race devient un objectif, pas une loterie punitive |
| Monnaies non échangeables, minerais liés | Pas de comptes secondaires, pas d'inflation, pas de marché à surveiller |
| Minerais détruits au Rebirth, `/pv` compris | Empêche de stocker le run suivant |
| Régénération par nouveau tirage | Empêche la mémorisation des filons rares |
| Hub et relais | Concentre 250 joueurs dans une mine de 20 000 x 20 000 |

## ⚠️ Risques et parades

| Risque | Parade |
| --- | --- |
| Macro ou autoclick de minage | Anticheat, détection de rythme parfait, gel par le staff |
| Comptes secondaires qui alimentent un compte principal | Aucun échange possible |
| Joueur qui stocke des minerais pour le run suivant | Destruction au Rebirth |
| Joueur très riche qui achète sa progression | Niveau requis sur chaque pioche |
| Pet Premium trop fort | Plafonds Premium inférieurs ou égaux aux plafonds gratuits |
| Biome saturé | File d'attente, relais pour répartir la foule |
| Nouveau joueur bloqué | Tutoriel, première pioche en 30 à 35 min, Rebirth accessible en 75 h même en jouant mal |
| Fin de progression sèche au Rebirth 25 | Collections, traits, races, classement du meilleur temps de run |
