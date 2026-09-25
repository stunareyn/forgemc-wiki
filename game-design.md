---
description: Boucles de gameplay, rôle de chaque système, dépendances, décisions de design et risques.
---

# 🧠 Game Design

## 🔁 Les quatre boucles

**Boucle courte, quelques minutes**
```
Miner → /sell ou vente automatique → enchantement → miner plus vite
```

**Boucle moyenne, quelques heures**
```
Économiser l'Argent + garder un minerai + atteindre un niveau → nouvelle pioche → nouveau biome plus rentable
```

**Boucle de Prestige, une à trois journées de jeu**
```
Pioche de porte → Prestige → multiplicateur x1,6 → reprise rapide des biomes connus → dimension suivante
```

**Boucle de Renaissance, plusieurs semaines**
```
Prestige X + Pioche d'Éther + niveau 100 → Renaissance → multiplicateur permanent +0,5 → nouvelle série de 10 Prestiges
```

Entre ces boucles, deux rythmes sociaux : un boss toutes les 2 à 6 heures selon la dimension, un événement court toutes les 20 minutes environ.

## 🧩 Pourquoi chaque système existe

| Système | Problème résolu | Boucle |
| --- | --- | --- |
| Pioche unique | Donner une identité et un fil rouge | Moyenne |
| Enchantements | Donner un achat toutes les quelques minutes | Courte |
| Biomes vanilla | Donner une destination reconnaissable à chaque pioche | Moyenne |
| Minerais vanilla dans l'Overworld | Faire reconnaître Minecraft avant de découvrir STRATA | Courte |
| Tous les minerais dans tous les biomes d'une dimension | Garder des moments forts partout, sources stables pour les armures | Courte et longue |
| Prestige | Rendre la remise à zéro désirable, ouvrir les dimensions une à une | Prestige |
| Mémoire de forge | Éviter qu'un Prestige ne redemande les mêmes minerais | Prestige |
| Départ rapide | Raccourcir les premières minutes d'un cycle déjà connu | Prestige |
| Renaissance | Objectif de plusieurs semaines, multiplicateur permanent | Renaissance |
| Armures | Premier choix entre vendre et investir | Longue |
| Pets | Récompense permanente trouvée en minant | Longue |
| Traits | Dépense de Cristaux, optimisation fine | Longue |
| Races | Spécialisation, objectif très long | Longue |
| Collections | Donner de la valeur à chaque bloc cassé, à chaque cycle | Longue |
| Boss invisibles | Objectif collectif sans interrompre le minage | Sociale |
| Chat réaction, Concours, Heure dorée, Vote Party | Rendez-vous courts et animation du chat | Sociale |
| Guildes | Groupe permanent, objectifs hebdomadaires | Sociale |
| Skins, sons | Montrer sa progression sans toucher à l'équilibrage | Aucune, cosmétique |
| Shop rotatif | Raison de revenir, conversion de l'Argent vers l'XP, les Éclats ou la Chance | Courte |
| Caisses | Canal de récompense et de monétisation | Longue |
| `/pv` | Stockage sans sac | Moyenne |
| Menus GUI | Tout faire sans connaître les commandes | Toutes |

## 🔗 Dépendances

```
Bloc cassé
 ├─ Argent ──────► Pioche (tier) ─► Biome ─► valeur des blocs
 │                ├► Coût de Prestige ─► multiplicateur de Prestige
 │                └► Armures ◄─── minerais de la dimension
 ├─ Éclats ──────► Enchantements ─► vitesse, quantité, valeur, Trouvailles
 ├─ XP ──────────► Niveau ─► condition des pioches et de la Renaissance
 ├─ XP de pet ───► Niveau de pet ─► Éveil ◄─ minerais Rares à Mythiques, Essences
 ├─ Trouvaille ──► Cristaux ─► Traits, Race, Shop, guilde
 │               └► Œufs, clés ─► Pets, Essences, Skins
 ├─ Dégât de boss ─► Cristaux, pet de boss, booster de dimension
 └─ XP de guilde ─► niveau de guilde ─► bonus d'Argent
```

Chaque bloc cassé alimente sept progressions à la fois. Les autres sources, votes, tutoriel, récompenses de Prestige et de Renaissance, boutique, sont des compléments bornés : aucune ne remplace le minage.

## ⚖️ Décisions de design

| Décision | Raison |
| --- | --- |
| 4 biomes par dimension, 16 au total | Une pioche par biome, 17 pioches, un rythme régulier |
| Noms de biomes vanilla | Le joueur sait où il est sans lire ; musique, ciel et ambiance vanilla gratuits |
| 8 minerais vanilla dans l'Overworld, 9 minerais par autre dimension | Assez pour la variété, assez peu pour que chaque minerai soit reconnaissable |
| Biome 4 de chaque dimension = zone riche | Raison de rester dans le dernier biome même avec la pioche suivante en vue |
| Portes de Prestige sur les pioches | Le Prestige arrive au moment où le joueur a fini ce que son rang permet |
| Multiplicateur de Prestige x1,6 cumulé | Chaque Prestige rend la reprise nettement plus rapide ; un bonus additif rendait les cycles de plus en plus longs |
| Renaissance : +0,5 par Renaissance, coûts x(1 + 0,2 R) | Chaque Renaissance est plus rapide que la précédente, sans devenir instantanée |
| Première Renaissance vers 261 h pour un joueur optimisé sans achat, verrou de 15 jours pleins | Pas avant 2 à 3 semaines après l'ouverture, même à 12 à 16 h de jeu par jour |
| Niveau requis sur chaque pioche | Garde-fou contre un saut de progression. En jeu normal, le niveau est atteint avant l'Argent : la simulation ne le montre limitant qu'au niveau 100 de la Pioche d'Éther et de la Renaissance |
| Pas de booster d'Argent au Shop | Il serait rentable par construction et rendrait le Shop obligatoire |
| Boss invisibles, dégâts par bloc cassé | Aucun combat, aucune entité, aucune charge serveur ; le minage reste l'unique geste |
| Excavation sans dégâts de boss | Le boss récompense la présence et l'activité, pas l'équipement |
| Un pet par type de bonus | Empêche l'empilement de pets Argent, donne de la valeur à tous les types |
| Reroll de race avec choix | Un reroll ne punit jamais ; la race devient un objectif |
| Monnaies non échangeables, minerais liés | Pas de comptes secondaires, pas d'inflation, pas de marché à surveiller |
| Minerais détruits au Prestige, `/pv` compris | Empêche de stocker le cycle suivant |
| Régénération par nouveau tirage | Empêche la mémorisation des filons rares |
| Hub et relais | Concentre 250 joueurs dans une mine de 20 000 x 20 000 |

## ⚠️ Risques et parades

| Risque | Parade |
| --- | --- |
| Macro ou autoclick de minage | Anti-triche, détection de rythme parfait, plafond de 16 blocs/s, gel par le staff |
| Comptes secondaires qui alimentent un compte principal | Aucun échange possible, votes limités à 3 comptes par adresse IP |
| Joueur qui stocke des minerais pour le cycle suivant | Destruction au Prestige et à la Renaissance |
| Joueur très riche qui achète sa progression | Rien ne vend d'Argent, d'Éclats ni de minerai ; grade limité à +12 % Argent, additionné aux autres bonus ; minerai du premier forgeage non achetable. Gain mesuré : 10,6 % de temps en moins sur la première Renaissance |
| Pet Premium trop fort | Plafonds Premium inférieurs ou égaux aux plafonds gratuits |
| Joueur AFK dans un boss | Participation valide à 100 dégâts, joueurs inactifs exclus des PV et des récompenses |
| Biome saturé | File d'attente, relais pour répartir la foule |
| Nouveau joueur perdu | Tutoriel, boss de l'Overworld toutes les 2 h accessibles dès le premier bloc, première pioche en 51 min pour un joueur moyen |
| Joueurs arrivés après l'ouverture | Classements par numéro de Renaissance, guildes ouvertes, événements sans condition de progression |
| Fin de progression sèche après la Renaissance 10 | Collections, traits, races, classement du meilleur temps de Renaissance |
