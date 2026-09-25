---
description: Vérifications de cohérence, rapports de puissance, contournements testés, valeurs à confirmer en test et checklist finale.
---

# ✅ Contrôles de cohérence

## 📐 Rapports de puissance

| Vérification | Résultat | Statut |
| --- | --- | --- |
| Pet Légendaire contre pet Rare, niveau 40 | 22 % contre 10 %, x2,2 | ✅ |
| Pet Mythique contre pet Légendaire, niveau 40 | 30 % contre 22 %, x1,36 | ✅ |
| Trait Mythique contre pet Légendaire | 10 % contre 22 % : le trait reste secondaire | ✅ |
| Armure Peu commune d'une dimension contre Légendaire de la précédente | Ambre 4,5 > Diamant 3,5 ; Galène 10 > Carmin 8,5 ; Aigue-marine 18 > Pulsar 16 | ✅ |
| Valeurs des 15 armures | Croissantes de 1,5 à 28 | ✅ |
| Biome suivant, même dimension | Valeur moyenne d'un bloc x1,39 à x1,56 | ✅ |
| Premier biome d'une dimension contre dernier de la précédente | x1,58, x1,70, x1,72 | ✅ |
| Prestige | Multiplicateur x1,6 par rang, x109,95 au Prestige X | ✅ |
| Boucle après la Renaissance 1 | 38 % plus courte que la première | ✅ |
| Boucle après la Renaissance 9 | 67 % plus courte que la première | ✅ |
| Grade maximal | +12 % Argent ; avec tous les avantages payants, 10,6 % de temps gagné sur la première Renaissance | ✅ |
| Caisse Premium | Plafonds égaux ou inférieurs aux plafonds gratuits, type par type | ✅ |
| Race | Aucune statistique au-delà de 12 % | ✅ |

## 💎 Économie des minerais

| Vérification | Résultat | Statut |
| --- | --- | --- |
| Somme des taux de chaque biome | 100 % exactement sur les 16 biomes | ✅ |
| Part des minerais Rares et plus dans la valeur d'un bloc | 38 % à 42 % dans la plupart des biomes, 62 % dans les Badlands dont le minerai favori est l'Or, 65 % à 75 % dans les zones riches | ✅ |
| Aucun Commun ne vaut plus qu'un Rare de sa dimension | Vérifié sur les 4 dimensions | ✅ |
| Rareté des minerais vanilla | Suit leur fréquence réelle : Charbon et Cuivre communs, Émeraude la plus rare | ✅ |
| Taux identiques à toutes les profondeurs sous la couche 1 | Tables par biome sans paramètre de hauteur | ✅ |

## 👹 Boss et événements

| Vérification | Résultat | Statut |
| --- | --- | --- |
| Durée d'un boss pour une population au premier passage | 9,7 à 10,4 min, limite 15 min | ✅ 🟠 |
| Aucun chevauchement d'annonces de boss | 15 min d'écart minimum entre deux apparitions | ✅ |
| Poids des événements dans les Cristaux | Environ 25 % du budget, votes compris | ✅ |
| Aucune récompense d'événement ne dépend du grade | Vérifié | ✅ |
| Excavation sans effet sur les boss et Concours | Vérifié | ✅ |

## 🚧 Contournements testés

| Stratégie | Effet | Parade |
| --- | --- | --- |
| Tout miser sur l'Argent, grade et pet Mythique | 232 h 55 au lieu de 260 h 38 | Bonus additifs, minerai de premier forgeage non achetable |
| Rester dans un biome ancien pour farmer | Valeur d'un bloc 1,4 à 1,7 fois plus faible par biome de retard, vitesse de base plus faible | Aucune nécessaire, choix perdant |
| Stocker les minerais du cycle suivant dans `/pv` | Aurait supprimé le début de cycle | Destruction au Prestige, `/pv` compris |
| Compte secondaire qui donne ses ressources | Aurait doublé les revenus | Aucun échange, minerais liés |
| Comptes secondaires qui remplissent la banque de guilde | Aurait financé la Ferveur chaque jour | 10 h de minage minimum et 300 Cristaux par semaine et par membre |
| Mémoriser l'emplacement d'un Mythique | Aurait permis de le re-miner toutes les 2 min | Régénération par nouveau tirage |
| Acheter des boosters d'Argent à la chaîne | Aurait rendu le Shop obligatoire | Aucun booster d'Argent en vente |
| Empiler plusieurs pets Argent | Aurait doublé le bonus | Un pet par type |
| Garder ses Éclats pour le cycle suivant | Aurait accéléré le début de cycle | Éclats remis à zéro au Prestige |
| Rester AFK pendant un boss | Récompense sans effort | 100 dégâts minimum, joueurs inactifs exclus |
| Bot de Chat réaction | Cristaux sans jouer | Réponse en moins de 1,0 s ignorée, 3 victoires par heure et 15 par jour |
| Farmer le boss de l'Overworld depuis une dimension avancée | Chance de pet facile | Autorisé : les PV augmentent avec chaque joueur, les Cristaux restent ceux du boss de l'Overworld |
| Sauter un tier de pioche | Aurait raccourci un cycle | Impossible : T(n+1) exige T(n) |
| Jouer 16 à 20 h par jour avec tous les achats | Renaissance 1 en 11,6 à 14,6 jours | Verrou calendaire de 15 jours pleins |

## 🧑‍🤝‍🧑 Cohérence par type de joueur

| Joueur | Première Renaissance | Plus longue attente sur une seule pioche |
| --- | --- | --- |
| Nouveau, 3 h par jour | environ 260 jours | 47 h 16 de jeu, Pioche d'Éther au cycle IX |
| Régulier, moyen à 3 h par jour | environ 137 jours | 21 h 41 de jeu, Pioche d'Éther au cycle IX |
| Très actif, moyen à 6 h par jour | environ 69 jours | idem |
| Optimisé sans achat, 12 à 16 h par jour | 16,3 à 21,7 jours | 12 h 59 de jeu, Pioche d'Éther au cycle IX |

La plus longue attente est toujours la dernière pioche du dernier cycle : c'est la marche finale avant la Renaissance.

## 🟠 Valeurs à confirmer en test

| Valeur | Pourquoi elle est incertaine | Quoi mesurer |
| --- | --- | --- |
| Temps effectif de minage, 70 % | Dépend des déplacements et des menus réels | Temps de minage actif divisé par temps connecté |
| Vitesse de minage réelle jusqu'à 6,7 blocs/s | Un joueur humain peut ne pas tenir ce rythme | Blocs par seconde des 10 % meilleurs joueurs |
| Bonus de Chance moyen x1,5 | Dépend des pets et de Prospection réels | Trouvailles par million de blocs |
| Prix des pioches T14 à T17 | Sensibles aux bonus de fin de boucle | Temps réel des étapes de l'Aether |
| PV de boss par joueur, 70 % de joueurs actifs | Dépend de l'activité réelle pendant un boss | Durée médiane d'un boss, taux de victoire |
| Seuil de Vote Party, 300 | Dépend du nombre de votants | Vote Party par jour |
| Réussite des défis de guilde, 2 sur 3 | Dépend de l'activité des guildes | Défis réussis par guilde et par semaine |
| 3 h de jeu par jour pour le joueur moyen | Hypothèse des sources quotidiennes de Cristaux | Temps de jeu médian par jour |
| Verrou calendaire, 15 jours pleins | Filet de sécurité | Date de la première Renaissance sans verrou, sur le serveur de test |

## ✔️ Checklist finale

| Point | Statut |
| --- | --- |
| Exactement 4 dimensions : Overworld, Nether, End, Aether | ✅ |
| 16 biomes, tous des noms de biomes vanilla, identifiants vanilla indiqués | ✅ |
| Minerais de l'Overworld : 8 minerais vanilla | ✅ |
| La couche 1 ne contient que le bloc principal | ✅ |
| Les minerais apparaissent à partir de la couche 2, taux identiques à toutes les profondeurs | ✅ |
| Blocs principaux : Stone, Netherrack, End Stone, Calcite | ✅ |
| 35 minerais, valeurs et taux calculés ensemble | ✅ |
| 17 pioches, chacune débloque quelque chose | ✅ |
| Enchantements : les 7 de la version précédente, effets et coûts inchangés | ✅ |
| Prestige : 10 rangs, portes de Prestige, multiplicateur x1,6 | ✅ |
| Renaissance : 10 rangs, +0,5 par rang, coûts x(1 + 0,2 R) | ✅ |
| Première Renaissance pas avant 2 à 3 semaines d'ouverture | ✅ |
| Boss invisibles, un par dimension, dégâts par bloc cassé | ✅ |
| Chat réaction, Vote Party, Concours de minage, Heure dorée | ✅ |
| Guildes à la place des Compagnies | ✅ |
| Menus GUI dans une catégorie à part | ✅ |
| Commandes joueurs complètes, dont `/tpa`, `/trash`, `/spawn` | ✅ |
| Éléments permanents identifiés | ✅ |
| 22 pets, un par type actif | ✅ |
| 8 traits, toujours inférieurs au bonus du pet | ✅ |
| 15 armures, progression monotone | ✅ |
| 8 races, bonus plafonné à 12 % | ✅ |
| Skins sans statistique | ✅ |
| Caisse Premium plafonnée par le gratuit | ✅ |
| Shop : aucun booster d'Argent en vente | ✅ |
| 7 grades, bonus d'Argent seul, +12 % maximum | ✅ |
| Sons vanilla, entendus par le joueur seul | ✅ |
| Économie : Argent et Éclats remis à zéro, Cristaux déflationnistes | ✅ |
| Progression simulée de bout en bout, jusqu'à la Renaissance 10 | ✅ |
| Aucun sac, aucune dynamite, aucune dimension ajoutée | ✅ |
| Aucune nouvelle texture nécessaire | ✅ |
| Assets non utilisés listés | ✅ |
