---
description: Formules de rendement, empilement des bonus et plafonds de sécurité. Référence pour le développeur.
---

# 🧮 Formules

## ⛏️ Par bloc cassé

```
Bloc principal
  Argent = valeur_bloc_principal x (1 + Argent%) x MR
  XP     = 1 x mult_XP_biome x (1 + XP%) x MR
  Éclats = eclats_biome x (1 + Éclats%) x MR

Minerai
  Quantité = 1 + Fortune%            (partie décimale = chance d'un objet supplémentaire)
  Argent   = valeur x quantité x (1 + Argent%) x MR   (à la vente)
  XP       = XP_base_rareté x mult_XP_biome x (1 + XP%) x MR   (non multipliée par la Fortune)
  Éclats   = eclats_biome x (1 + Éclats%) x MR

Trouvailles, un tirage par bloc, chaque Trouvaille donne 1 objet
  P(Cristal)          = 1 / 4 000   x (1 + Chance%)     1 Cristal
  P(Œuf)              = 1 / 50 000  x (1 + Chance%)
  P(clé Pets F2W)     = 1 / 100 000 x (1 + Chance%)
  P(clé Armure Themes)= 1 / 100 000 x (1 + Chance%)

MR = multiplicateur de Rebirth = 1 + 0,20 x Rebirth x (1 + bonus_Phénix)
```

Tous les pourcentages d'un même type s'**additionnent** entre eux. Seul le multiplicateur de Rebirth multiplie le total.

## ⚡ Vitesse

```
Blocs/s au clic     = vitesse_base_tier + 0,2 x niveau_Efficacité
Chance_Excavation   = min(18 %, 1,5 % x niveau_Excavation x (1 + Cadence% + Golem%))
Blocs par clic      = 1 + Chance_Excavation x 8 x part_pleine
                      part_pleine = part des 8 blocs de la zone qui ne sont pas de l'air, environ 0,9 en pratique
Plafond technique   = 16 blocs/s effectifs par joueur
```

## 📚 Sources de chaque bonus

**Argent %**

| Source | Maximum |
| --- | --- |
| Enchantement Argent | 150 |
| Pet Argent Mythique ★3 avec Symbiose Mythique | 58,7 |
| Traits Négociant sur les autres pets, 3 x 10 | 30 |
| Armure Aurore complète | 36 |
| Race Draconide | 10 |
| Grade Immortal | 12 |
| Collections | 9 |
| Compagnie niveau 10 | 10 |
| Sceaux de dimension | 15 |
| Booster global de vote | 10 |
| **Plafond de sécurité** | **350** |

**XP %**

| Source | Maximum |
| --- | --- |
| Enchantement XP | 120 |
| Pet XP Légendaire ★3 avec Symbiose Mythique | 43,1 |
| Traits Érudit, 3 x 10 | 30 |
| Armure Aurore complète | 36 |
| Race Elfe | 12 |
| Collections Minerais et Garde-robe | 11 |
| Sceaux de dimension | 15 |
| Booster XP du Shop | 25 |
| **Plafond de sécurité** | **300** |

**Fortune %**

| Source | Maximum |
| --- | --- |
| Enchantement Fortune | 200 |
| Pet Fortune Légendaire ★3 avec Symbiose Mythique | 25,8 |
| Traits Veine, 3 x 6 | 18 |
| Armure Disthène complète | 33 |
| Race Draconide | 10 |
| **Plafond de sécurité** | **300** |

**Chance %**

| Source | Maximum |
| --- | --- |
| Enchantement Prospection | 100 |
| Pet Chance Légendaire ★3 avec Symbiose Mythique | 64,6 |
| Traits Prospecteur, 3 x 18 | 54 |
| Armure Aigue-marine complète | 36,25 |
| Race Gnome | 12 |
| Booster Trouvailles du Shop | 50 |
| **Plafond de sécurité** | **320** |

**Éclats %**

| Source | Maximum |
| --- | --- |
| Pet Éclats Légendaire ★3 avec Symbiose Mythique | 43,1 |
| Traits Collecteur, 3 x 10 | 30 |
| Bonus de set d'armure | 12 |
| Race Golem | 12 |
| Booster Éclats | 25 |
| **Plafond de sécurité** | **200** |

Les maximums d'une même colonne ne sont pas tous atteignables ensemble : un pet porte un seul trait, un joueur porte une seule armure complète, a une seule race. Les plafonds ne servent qu'à bloquer une combinaison imprévue.

## 📈 XP de pioche

```
XP pour passer du niveau N à N+1 = 500 x 1,09^(N-1) x (1 + 0,10 x Rebirth)
Niveau maximal = 100 ; l'XP au-delà est perdue
```

Table des niveaux clés : voir [Pioches](../pioches/pioches.md).

## 🧱 Règles de calcul

* Les bonus sont recalculés à chaque changement d'équipement, de pet, de trait, de race, de grade, de palier de collection ou de niveau de Compagnie, puis mis en cache. Jamais recalculés à chaque bloc.
* Tirages : un seul tirage par bloc pour les Trouvailles, avec un générateur par joueur.
* Arrondi : les gains en $ sont arrondis à l'entier à la vente. Les Éclats et l'XP sont cumulés en décimal et affichés arrondis.
* Le bloc principal ne produit aucun objet.
