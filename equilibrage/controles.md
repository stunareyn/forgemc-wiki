---
description: Vérifications de cohérence, rapports de puissance, contournements testés, checklist finale.
---

# ✅ Contrôles de cohérence

## 📐 Rapports de puissance

| Vérification | Résultat | Statut |
| --- | --- | --- |
| Pet Légendaire contre pet Rare, niveau 40 | 22 % contre 10 %, x2,2 | ✅ |
| Pet Mythique contre pet Légendaire, niveau 40 | 30 % contre 22 %, x1,36 | ✅ |
| Trait Légendaire contre pet Légendaire | 7 % contre 22 % : le trait reste secondaire | ✅ |
| Armure de fin contre armure de début | Aurore 24 % contre Galène 2 % par pièce | ✅ |
| Armure Rare d'une dimension contre Légendaire de la précédente | 5 > 4, 10 > 8, 17 > 14 | ✅ |
| Nouveau biome | Valeur d'un bloc x1,6 à x1,7 | ✅ |
| Nouvelle pioche et son biome | Argent par heure x2,1 à x2,9 | ✅ |
| Dimension suivante | Unité de base x5, premier biome x1,7 par rapport au dernier biome précédent | ✅ |
| Premier Rebirth | Run suivant 23 % plus court | ✅ |
| Rebirth 10 | Run 54 % plus court que le premier | ✅ |
| Grade maximal | +12 % Argent, aucun effet sur le niveau | ✅ |
| Caisse Premium | Plafonds égaux ou inférieurs aux plafonds gratuits | ✅ |

## 💎 Économie des minerais

| Vérification | Résultat | Statut |
| --- | --- | --- |
| Part des minerais Rares et plus dans le revenu d'un biome | 39 % à 46 % | ✅ |
| Rare contre meilleur Commun de la dimension | x3,3 | ✅ |
| Mythique contre meilleur Commun de la dimension | x278 | ✅ |
| Commun du biome 3 contre Peu commun du biome 2 | 3,6 contre 3,2 unités | ✅ |
| Aucun Commun ne vaut plus qu'un Rare de sa dimension | Vérifié sur les 4 dimensions | ✅ |
| Somme des taux de chaque biome | 100 % exactement sur les 12 biomes | ✅ |
| Taux identiques à toutes les profondeurs sous la couche 1 | Oui, tables par biome sans paramètre de hauteur | ✅ |

## 🚧 Contournements testés

| Stratégie | Effet | Parade |
| --- | --- | --- |
| Tout miser sur l'Argent, grade et pet Mythique | 25 h au lieu de 36 h | Niveau requis sur chaque pioche |
| Rester dans un biome ancien pour farmer | Revenu 2 à 3 fois plus faible par biome de retard | Aucune nécessaire, choix perdant |
| Stocker les minerais du run suivant dans `/pv` | Aurait supprimé le début de run | Destruction au Rebirth, `/pv` compris |
| Compte secondaire qui donne ses ressources | Aurait doublé les revenus | Aucun échange, minerais liés |
| Mémoriser l'emplacement d'un Mythique | Aurait permis de le re-miner toutes les 2 min | Régénération par nouveau tirage |
| Acheter des boosters d'Argent à la chaîne | Aurait rendu le Shop obligatoire | Aucun booster d'Argent |
| Empiler plusieurs pets Argent | Aurait doublé le bonus | Un pet par type |
| Garder ses Éclats pour le run suivant | Aurait accéléré le début de run | Éclats remis à zéro |
| Excavation poussée au maximum avec traits et race | Charge serveur | Plafond de 18 % et de 16 blocs/s |
| Sauter un tier de pioche | Aurait raccourci un run | Impossible : T(n+1) exige T(n) |

## 🧑‍🤝‍🧑 Cohérence par type de joueur

| Joueur | Premier Rebirth | Jamais bloqué plus de |
| --- | --- | --- |
| Nouveau, 1,5 h par jour | environ 51 jours | 12 h 52 de jeu sur une seule pioche, la dernière |
| Régulier, 2 h par jour | environ 19 jours | 5 h 20 de jeu sur une seule pioche |
| Très actif, 5 h par jour | environ 8 jours | idem |
| Optimisé, 6 h par jour | environ 5 jours | 3 h 40 de jeu sur une seule pioche |
| Multi-Rebirth, Rebirth 10 et plus | 13 à 17 h par run | environ 2 h sur une seule pioche |

## 🟠 Ajustements à prévoir après les tests

| Valeur | Pourquoi elle est incertaine | Quoi mesurer |
| --- | --- | --- |
| Temps effectif de minage, 70 % | Dépend des déplacements et des menus réels | Temps de minage actif divisé par temps connecté |
| Vitesse de minage réelle à 6,7 blocs/s | Un joueur humain peut ne pas tenir ce rythme | Blocs par seconde des 10 % meilleurs joueurs |
| Prix des pioches T11 à T13 | Sensibles aux bonus de fin de run | Temps réel des étapes Aether |
| Taux d'Œufs, 1 sur 50 000 | Détermine la vitesse d'accès aux pets Mythiques | Pets Mythiques par joueur et par semaine |
| Coût des traits | Dépend du budget réel de Cristaux | Cristaux gagnés par heure, médiane |
| Classement de Compagnie | Dépend de la taille réelle des Compagnies | Points hebdomadaires du premier et du dixième |

## ✔️ Checklist finale

| Point | Statut |
| --- | --- |
| Toutes les règles obligatoires sont respectées | ✅ |
| Il n'existe que 4 dimensions | ✅ |
| Overworld, Nether, End et Aether conservent leur nom | ✅ |
| La couche 1 ne contient que le bloc principal | ✅ |
| Les minerais apparaissent à partir de la couche 2 | ✅ |
| Les taux sont identiques à toutes les profondeurs | ✅ |
| Blocs principaux : Stone, Netherrack, End Stone, Calcite | ✅ |
| Minerais cohérents : 36, valeurs et taux calculés ensemble | ✅ |
| Pioches cohérentes : 13, chacune débloque quelque chose | ✅ |
| Enchantements cohérents : 6 obligatoires et Prospection | ✅ |
| Rebirth cohérent : 25 paliers, gains +20 %, coûts +10 % | ✅ |
| Éléments permanents identifiés | ✅ |
| Pets cohérents : 22, un par type actif | ✅ |
| Traits cohérents : 8, toujours inférieurs au bonus du pet | ✅ |
| Armures cohérentes : 12, progression monotone | ✅ |
| Races cohérentes : 8, bonus plafonné à 12 % | ✅ |
| Skins cohérents : sans statistique | ✅ |
| Caisses cohérentes : Premium plafonnée par le gratuit | ✅ |
| Shop cohérent : aucun booster d'Argent | ✅ |
| Grades cohérents : 7, bonus d'Argent seul, +12 % maximum | ✅ |
| Statistiques cohérentes | ✅ |
| Sons cohérents : sons vanilla, joueur seul | ✅ |
| Commandes complètes, permissions par niveau | ✅ |
| PNJ cohérents : 4, un par dimension, répliques sur des systèmes existants | ✅ |
| Économie équilibrée : Argent et Éclats remis à zéro, Cristaux déflationnistes | ✅ |
| Progression globale simulée de bout en bout | ✅ |
| Aucun sac, aucune dynamite, aucune dimension ajoutée | ✅ |
| Aucune nouvelle texture nécessaire | ✅ |
| Assets non utilisés listés | ✅ |
