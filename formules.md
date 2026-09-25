---
description: Formules de rendement, multiplicateurs, empilement des bonus, Trouvailles, boss et plafonds de sécurité. Référence pour le développeur.
---

# 🧮 Formules

## ✖️ Multiplicateurs

```
MP = multiplicateur de Prestige    = 1,6 ^ rang de Prestige           (x1 au Prestige 0, x109,95 au Prestige X)
MR = multiplicateur de Renaissance = 1 + 0,5 x Renaissance x (1 + bonus_Phénix)
MC = multiplicateur de coût        = 1 + 0,20 x Renaissance
```

* MP et MR multiplient l'Argent, l'XP de pioche et les Éclats. Ils ne multiplient ni les Cristaux, ni les Trouvailles, ni l'XP de pet, ni les dégâts de boss.
* MC multiplie le prix des pioches et l'XP requise par niveau. Le coût de Prestige est 30 % du prix de la pioche de porte, MC compris.

## ⛏️ Par bloc cassé

```
Bloc principal
  Argent = valeur_bloc_principal x (1 + Argent%) x MP x MR          (crédité directement, aucun objet)
  XP     = 1 x mult_XP_biome x (1 + XP%) x MP x MR
  Éclats = eclats_biome x (1 + Éclats%) x MP x MR

Minerai
  Quantité = 1 + Fortune%            (partie décimale = chance d'un objet supplémentaire)
  Argent   = valeur x quantité x (1 + Argent%) x MP x MR   (à la vente)
  XP       = XP_base_rareté x mult_XP_biome x (1 + XP%) x MP x MR   (non multipliée par la Fortune)
  Éclats   = eclats_biome x (1 + Éclats%) x MP x MR

XP_base_rareté : Commun 2, Peu commun 3, Rare 6, Épique 15, Légendaire 40, Mythique 120

Bloc compressé (Autocraft)
  Valeur = 9 x valeur du minerai x (1 + 0,03 x niveau_Autocraft)
```

Tous les pourcentages d'un même type s'**additionnent** entre eux, puis le total est plafonné. Seuls MP et MR multiplient le total.

**Exemple** : un Diamant (Légendaire de l'Overworld, 6 000 $ de base, voir [Minerais de l'Overworld](../minerais/overworld.md)) vendu au Prestige III, à la Renaissance 1, avec +80 % d'Argent :

```
6 000 x 1,80 x 1,6^3 x 1,5 = 6 000 x 1,80 x 4,096 x 1,5 = 66 355 $
```

## 🍀 Trouvailles

Un tirage indépendant par type et par bloc cassé, Excavation comprise.

```
P(Cristal)             = 1 / 4 000   x (1 + Chance%) x Heure_dorée     → 1 Cristal
P(Œuf)                 = 1 / 100 000 x (1 + Chance%) x Heure_dorée     → 1 Œuf de la dimension
P(clé Pets F2W)        = 1 / 300 000 x (1 + Chance%) x Heure_dorée
P(clé Armure Themes)   = 1 / 300 000 x (1 + Chance%) x Heure_dorée
Heure_dorée = 2 pendant l'Heure dorée, sinon 1
```

## ⚡ Vitesse

```
Blocs/s au clic     = vitesse_base_tier + 0,2 x niveau_Efficacité
vitesse_base_tier   = 1,5 + 0,075 x (tier - 1)                  (T1 1,5 · T17 2,7)
Chance_Excavation   = min(18 %, 1,5 % x niveau_Excavation x (1 + Cadence% + Golem%))
Blocs par clic      = 1 + Chance_Excavation x 8 x part_pleine
                      part_pleine = part des 8 blocs de la zone qui ne sont pas de l'air, environ 0,9 en pratique
Plafond technique   = 16 blocs/s effectifs par joueur
Vitesse de déplacement bonus = min(35 %, Mobilité des bottes + talents de race)
```

## 👹 Boss

```
PV max              = PV_par_joueur x max(joueurs_présents, 20)      (500, 900, 1 500, 2 200)
Dégât d'un bloc     = 1, ou 3 / 10 / 30 / 100 pour un minerai Rare / Épique / Légendaire / Mythique
                      0 pour un bloc cassé par l'Excavation
Chance de pet       = min(plafond, base + bonus x part_des_dégâts_en_%)
```

Valeurs : [Boss](../evenements/boss.md).

## 📚 Sources de chaque bonus

**Argent %**

| Source | Maximum |
| --- | --- |
| Enchantement Argent | 150 |
| Pet Argent Mythique ★3 avec Symbiose Mythique : 43,5 x 1,35 | 58,7 |
| Traits Négociant sur les 3 autres pets, 3 x 10 | 30 |
| Armure Aurore complète : plastron 28 + set 12 | 40 |
| Race Draconide | 10 |
| Grade Immortal | 12 |
| Collection Minerais, 35 x 0,25 | 8,75 |
| Guilde niveau 10 | 10 |
| Sceaux de dimension, 3 x 5 | 15 |
| Booster de Vote Party | 10 |
| Booster de boss | 10 |
| Ferveur de guilde | 10 |
| **Plafond de sécurité** | **350** |

**XP %**

| Source | Maximum |
| --- | --- |
| Enchantement XP | 120 |
| Pet XP Légendaire ★3 avec Symbiose Mythique : 31,9 x 1,35 | 43,1 |
| Traits Érudit sur les 3 autres pets, 3 x 10 | 30 |
| Armure Aurore complète : casque 28 + set 12 | 40 |
| Race Elfe | 12 |
| Collections Minerais 8,75 et Garde-robe 2 | 10,75 |
| Sceaux de dimension | 15 |
| Booster XP du Shop | 25 |
| Booster de boss | 10 |
| **Plafond de sécurité** | **300** |

**Fortune %**

| Source | Maximum |
| --- | --- |
| Enchantement Fortune | 200 |
| Pet Fortune Légendaire ★3 avec Symbiose Mythique : 31,9 x 0,6 x 1,35 | 25,8 |
| Traits Veine sur les 3 autres pets, 3 x 6 | 18 |
| Armure Disthène complète : jambières 15,75 + set 16 | 31,75 |
| Race Draconide | 10 |
| **Plafond de sécurité** | **300** |

**Chance %**

| Source | Maximum |
| --- | --- |
| Enchantement Prospection | 100 |
| Pet Chance Mythique ★3 avec Symbiose Mythique : 43,5 x 1,5 x 1,35 | 88,1 |
| Traits Prospecteur sur les 3 autres pets, 3 x 18 | 54 |
| Armure Aigue-marine complète : bottes 22,5 + set 14 | 36,5 |
| Race Gnome | 12 |
| Booster Trouvailles du Shop | 50 |
| **Plafond de sécurité** | **320** |

**Éclats %**

| Source | Maximum |
| --- | --- |
| Pet Éclats Légendaire ★3 avec Symbiose Mythique : 31,9 x 1,35 | 43,1 |
| Traits Collecteur sur les 3 autres pets, 3 x 10 | 30 |
| Bonus de set d'armure Aurore | 12 |
| Race Golem | 12 |
| Booster Éclats | 25 |
| **Plafond de sécurité** | **200** |

**Lecture des plafonds**

* Somme des maximums : Argent 364,45, XP 305,85, Fortune 285,55, Chance 340,6, Éclats 122,1.
* Ces sommes supposent 4 emplacements de pet (Renaissance 4), un trait Mythique sur chaque pet, la meilleure armure pour la statistique et tous les boosters en même temps. Un même pet ne porte qu'un trait, un joueur ne porte qu'un set complet et n'a qu'une race : les colonnes ne sont pas atteignables ensemble.
* Les plafonds d'Argent, d'XP et de Chance ne coupent donc qu'une combinaison extrême de fin de jeu : l'excédent est de 4 % pour l'Argent (364,45 / 350), 2 % pour l'XP (305,85 / 300) et 6 % pour la Chance (340,6 / 320). Ils servent de garde-fou contre une combinaison imprévue ou une erreur de configuration.

## 📈 XP de pioche

```
XP pour passer du niveau N à N+1 = 300 x 1,09^(N-1) x MC
Niveau maximal = 100 ; l'XP au-delà est perdue
```

Table des niveaux clés : voir [Pioches](../pioches/pioches.md).

## 🐾 Pets

```
Bonus = base_rareté x (1 + (niveau - 1) / 39) x (1 + 0,15 x étoiles)
XP de pet du niveau N à N+1 = 400 x 1,12^(N-1)
```

Bases : [Pets](../pets/pets.md).

## 🧱 Règles de calcul

* Les bonus sont recalculés à chaque changement d'équipement, de pet, de trait, de race, de grade, de palier de collection, de niveau de guilde ou de booster, puis mis en cache. Jamais recalculés à chaque bloc.
* Tirages : un générateur par joueur, graine non prévisible.
* Arrondi : les gains en $ sont arrondis à l'entier à la vente. Les Éclats et l'XP sont cumulés en décimal et affichés arrondis.
* Le bloc principal ne produit aucun objet.
* Les très grands nombres sont stockés en `double` côté serveur et en `DECIMAL(30,2)` en base : le revenu dépasse 10^11 $ par heure aux derniers Prestiges.
