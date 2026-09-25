---
description: Les menus de Prestige et de Renaissance, leurs états, confirmations et séquences.
---

# 🔱 Menus · Prestige et Renaissance

## Prestige

* Titre de l'inventaire : `STRATA · Prestige`
* Taille : 54 emplacements, 6 lignes
* Ouverture : `/prestige`, Menu principal, PNJ Bram
* Permission : `strata.player.prestige`
* Retour vers : Menu principal
* Remplissage : Vitre jaune `minecraft:yellow_stained_glass_pane`

```
      0   1   2   3   4   5   6   7   8 
 0-8  ··  ··  ··  ··  PG  ··  ··  ··  ··
 9-17 ··  ··  P1  P2  P3  P4  P5  ··  ··
18-26 ··  ··  P6  P7  P8  P9  PX  ··  ··
27-35 ··  ··  CP  ··  CC  ··  GA  ··  ··
36-44 ··  ··  KE  ··  BP  ··  LO  ··  ··
45-53 RE  ··  ··  ··  FE  ··  ··  ··  SO
```

`··` : vitre de remplissage.

| Slot | Code | Objet | Nom | Contenu | Clic |
| --- | --- | --- | --- | --- | --- |
| 4 | PG | `minecraft:beacon` | Prestige actuel | Rang, multiplicateur x1,6 par rang, Renaissance en cours | Aucun |
| 11 | P1 | état du rang | Prestige I | Pioche requise, coût, multiplicateur, déblocage, récompense | Aucun |
| 12 | P2 | état du rang | Prestige II | Idem | Aucun |
| 13 | P3 | état du rang | Prestige III | Idem | Aucun |
| 14 | P4 | état du rang | Prestige IV | Idem | Aucun |
| 15 | P5 | état du rang | Prestige V | Idem | Aucun |
| 20 | P6 | état du rang | Prestige VI | Idem | Aucun |
| 21 | P7 | état du rang | Prestige VII | Idem | Aucun |
| 22 | P8 | état du rang | Prestige VIII | Idem | Aucun |
| 23 | P9 | état du rang | Prestige IX | Idem | Aucun |
| 24 | PX | état du rang | Prestige X | Idem | Aucun |
| 29 | CP | pioche requise | Pioche requise | ✔ ou ✖, tier requis et tier actuel | Clic : ouvre Forge |
| 31 | CC | `minecraft:gold_ingot` | Coût | 30 % du prix de la pioche requise, ✔ ou ✖ et montant manquant | Aucun |
| 33 | GA | `minecraft:nether_star` | Gains du rang suivant | Nouveau multiplicateur, Cristaux, clé, déblocage | Aucun |
| 38 | KE | `minecraft:chest` | Ce que tu gardes | Liste du permanent | Aucun |
| 40 | BP | `minecraft:lime_concrete` ou `minecraft:red_concrete` | Passer Prestige III, par exemple | Vert si les 2 conditions sont remplies | Clic : confirmation avec délai de 3 s |
| 42 | LO | `minecraft:lava_bucket` | Ce que tu perds | Argent, Éclats, pioche, niveau, enchantements, biomes, minerais et `/pv` compris, Sceaux | Aucun |
| 45, 49, 53 | RE, FE, SO | Barre de navigation | Voir [Conventions](menus.md) | | |

**États d'un rang** (slots 11 à 15 et 20 à 24)

| État | Objet |
| --- | --- |
| Rang atteint | `minecraft:lime_stained_glass`, « ✔ Atteint » |
| Rang suivant | `minecraft:gold_block`, brillance si les conditions sont remplies |
| Rang futur | `minecraft:gray_stained_glass`, conditions visibles |

**Passage de Prestige**

1. Clic sur Passer : menu de confirmation. Le Détail liste l'Argent, les Éclats et les minerais qui seront perdus, avec leur valeur de vente.
2. Délai de sécurité de 3 s, puis Confirmer.
3. Le serveur revérifie les conditions, débite le coût, applique la remise à zéro, téléporte le joueur au hub des Plaines ou du biome de son Départ rapide.
4. Titre à l'écran « PRESTIGE III », son `ui.toast.challenge_complete`, message au serveur : « Lyra atteint le Prestige III. »
5. Récompenses de rang livrées : Cristaux, clé. Voir [Prestige](../progression/prestige.md).

Au Prestige X, le bouton devient `minecraft:totem_of_undying` « Prestige maximal », clic : ouvre Renaissance.

## Renaissance

* Titre de l'inventaire : `STRATA · Renaissance`
* Taille : 54 emplacements, 6 lignes
* Ouverture : `/renaissance`, Menu principal, PNJ Séléné
* Permission : `strata.player.renaissance`
* Retour vers : Menu principal
* Remplissage : Vitre jaune

```
      0   1   2   3   4   5   6   7   8 
 0-8  ··  ··  ··  ··  RN  ··  ··  ··  ··
 9-17 ··  ··  R1  R2  R3  R4  R5  ··  ··
18-26 ··  ··  R6  R7  R8  R9  RX  ··  ··
27-35 ··  C1  ··  C2  ··  C3  ··  GA  ··
36-44 ··  ··  KE  ··  BR  ··  LO  ··  ··
45-53 RE  ··  ··  ··  FE  ··  ··  ··  SO
```

`··` : vitre de remplissage.

| Slot | Code | Objet | Nom | Contenu | Clic |
| --- | --- | --- | --- | --- | --- |
| 4 | RN | `minecraft:totem_of_undying` | Renaissance actuelle | Numéro, multiplicateur de Renaissance, multiplicateur de coûts, bonus du Phénix | Aucun |
| 11 | R1 | état du rang | Renaissance 1 | Multiplicateur de gains, multiplicateur de coûts, Cristaux, récompense spéciale | Aucun |
| 12 | R2 | état du rang | Renaissance 2 | Idem | Aucun |
| 13 | R3 | état du rang | Renaissance 3 | Idem | Aucun |
| 14 | R4 | état du rang | Renaissance 4 | Idem | Aucun |
| 15 | R5 | état du rang | Renaissance 5 | Idem | Aucun |
| 20 | R6 | état du rang | Renaissance 6 | Idem | Aucun |
| 21 | R7 | état du rang | Renaissance 7 | Idem | Aucun |
| 22 | R8 | état du rang | Renaissance 8 | Idem | Aucun |
| 23 | R9 | état du rang | Renaissance 9 | Idem | Aucun |
| 24 | RX | état du rang | Renaissance 10 | Idem | Aucun |
| 28 | C1 | `minecraft:beacon` | Prestige X | ✔ ou ✖, rang actuel | Aucun |
| 30 | C2 | Pioche d'Éther | Pioche d'Éther | ✔ ou ✖ | Clic : ouvre Forge |
| 32 | C3 | `minecraft:experience_bottle` | Niveau 100 | ✔ ou ✖, niveau actuel | Aucun |
| 34 | GA | `minecraft:nether_star` | Gains de la Renaissance suivante | +0,5 au multiplicateur, Cristaux, clés, récompense spéciale | Aucun |
| 38 | KE | `minecraft:chest` | Ce que tu gardes | Tout le permanent, multiplicateur de Renaissance | Aucun |
| 40 | BR | `minecraft:lime_concrete` ou `minecraft:red_concrete` | Renaître | Vert si les 3 conditions sont remplies | Clic : double confirmation |
| 42 | LO | `minecraft:lava_bucket` | Ce que tu perds | Tout ce que perd un Prestige, plus le rang de Prestige, son multiplicateur et la Mémoire de forge | Aucun |
| 45, 49, 53 | RE, FE, SO | Barre de navigation | Voir [Conventions](menus.md) | | |

**Renaissance**

1. Clic sur Renaître : première confirmation, délai de 3 s.
2. Seconde confirmation, délai de 5 s. Titre : « Renaissance 2 · Tout recommence, en plus fort. »
3. Le serveur revérifie les conditions, applique la remise à zéro, téléporte le joueur au hub des Plaines.
4. Titre à l'écran « RENAISSANCE 2 », feu d'artifice, message à tout le serveur.
5. Récompenses livrées : Cristaux, 2 clés Pets F2W, 2 clés Armure Themes, récompense spéciale. Voir [Renaissance](../progression/renaissance.md).

À la Renaissance 10, les slots 11 à 24 sont tous atteints. Au Prestige X, le bouton devient **Nouveau départ** (`minecraft:recovery_compass`) : double confirmation (3 s puis 5 s), même remise à zéro qu'une Renaissance, aucun gain, chronomètre du classement « meilleur temps de Nouveau départ » remis à zéro.

Avant 15 jours pleins depuis l'ouverture du serveur, le bouton Renaître reste rouge avec « ✖ Renaissance ouverte dans 3 j 04 h », même si les 3 conditions sont remplies. Voir le verrou calendaire dans [Renaissance](../progression/renaissance.md).
