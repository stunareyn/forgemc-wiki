---
description: Les trois monnaies, les formules de gain, les revenus par biome, les dépenses et le contrôle de l'inflation.
---

# 💰 Économie

## 🪙 Monnaies

| Monnaie | Symbole | Durée de vie | Échangeable |
| --- | --- | --- | --- |
| Argent | $ | Run, remis à 0 au Rebirth | Non |
| Éclats | ✦ | Run, remis à 0 au Rebirth | Non |
| Cristaux | ◆ | Permanente | Non |

**Argent** : monnaie principale. Gagné en vendant des minerais et en cassant le bloc principal. Dépensé en pioches, armures et boosters.

**Éclats** : monnaie des enchantements. Chaque bloc cassé donne des Éclats selon le biome (1 à 27 par bloc), multipliés par le bonus d'Éclats et le multiplicateur de Rebirth.

**Cristaux** : monnaie permanente. Gagnée lentement, dépensée en traits, races, offres du Shop rotatif et création de Compagnie.

{% hint style="danger" %}
Aucune monnaie ne se transfère entre joueurs. Il n'existe ni `/pay`, ni hôtel des ventes, ni échange de minerais. Toute la richesse d'un joueur vient de son propre minage.
{% endhint %}

## 🧮 Formules de gain

```
Vente d'un minerai  = valeur x quantité x (1 + bonus Argent) x multiplicateur de Rebirth
Quantité            = 1 + bonus Fortune  (partie décimale = probabilité d'un objet de plus)
Bloc principal      = valeur du bloc principal x (1 + bonus Argent) x multiplicateur de Rebirth
Éclats d'un bloc    = Éclats du biome x (1 + bonus Éclats) x multiplicateur de Rebirth
XP d'un bloc        = XP de base x multiplicateur du biome x (1 + bonus XP) x multiplicateur de Rebirth
Multiplicateur de Rebirth = 1 + 0,20 x Rebirth x (1 + bonus Phénix)
```

Le détail des sources de bonus et de leurs plafonds est dans [Formules](../game-design/formules.md).

## 📈 Revenus de référence

Joueur moyen, premier run, enchantements et bonus typiques de chaque étape. Ces valeurs viennent de la simulation.

| Biome | Blocs/min | Minerais/min, Fortune comprise | Argent/h |
| --- | --- | --- | --- |
| 1. La Carrière | 76 | 13 | 65 800 $ |
| 2. Grottes Verdoyantes | 97 | 23 | 190 000 $ |
| 3. Abîme Sombre | 113 | 35 | 483 000 $ |
| 4. Terres Désolées | 142 | 34 | 1 220 000 $ (1,2 M) |
| 5. Forêt Écarlate | 176 | 55 | 3 200 000 $ (3,2 M) |
| 6. Vallée des Âmes | 203 | 80 | 7 410 000 $ (7,4 M) |
| 7. Terres Stériles | 222 | 69 | 16 200 000 $ (16,2 M) |
| 8. Plateaux du Vide | 255 | 102 | 37 900 000 $ (37,9 M) |
| 9. Hauts du Néant | 300 | 147 | 87 000 000 $ (87 M) |
| 10. Îles des Nuées | 341 | 129 | 186 000 000 $ (186 M) |
| 11. Jardins Célestes | 386 | 185 | 416 000 000 $ (416 M) |
| 12. Trône Solaire | 420 | 245 | 865 000 000 $ (865 M) |

Argent par minute au premier biome : environ 1 100 $. Au dernier biome : environ 14,4 M $. L'écart de 13 000 fois sur un run vient de la valeur des biomes (x370), de la vitesse (x5,5), de la Fortune (x2,5) et des bonus d'Argent (x2,6).

## 🧾 Dépenses d'un run

| Poste | Monnaie | Part |
| --- | --- | --- |
| Pioches T2 à T13 | Argent | environ 88 % de l'Argent gagné |
| Armures | Argent et minerais | environ 12 % |
| Boosters du Shop | Argent | marginal |
| Enchantements | Éclats | 100 % des Éclats |

Somme des prix des 12 pioches : 7 405 038 000 $ (7,4 Md). Argent gagné par un joueur moyen au premier run, d'après la simulation : environ 8,4 Md, dont 88 % pour les pioches et 12 % pour les armures, soit environ 170 000 $ dans l'Overworld, 4,6 M dans le Nether, 74 M dans l'End et 930 M dans l'Aether. Ce budget couvre l'armure Rare de chaque dimension et une partie de l'armure Épique.

Éclats gagnés hors bonus d'Éclats : environ 9,1 M, pour 15,1 M nécessaires à maximiser tous les enchantements. Un joueur moyen termine son premier run avec environ 60 % du total possible, ce qui laisse une marge de progression aux runs suivants.

## 💎 Budget de Cristaux

| Source | Premier run | Run suivant |
| --- | --- | --- |
| Trouvailles, 1 chance sur 4 000 par bloc | environ 225 | environ 280 |
| Collections | environ 250 | environ 80 |
| Première entrée dans les biomes, 5 x 12 | 60 | 0 |
| Tutoriel de Bram | 18 | 0 |
| Récompense de Rebirth | 120 | 140 et plus |
| Votes, 6,6 par jour | environ 120 | environ 80 |
| Compagnie, classement hebdomadaire | environ 100 | environ 60 |
| **Total** | **environ 890** | **environ 640** |

| Dépense | Coût |
| --- | --- |
| Reroll de trait | 10, ou 30 avec type verrouillé |
| Reroll de race | 60 |
| Shop rotatif | 25 à 1 200 |
| Création de Compagnie | 50 |

## 🛑 Contrôle de l'inflation

* **Argent et Éclats** sont remis à zéro à chaque Rebirth. Aucune accumulation possible sur le long terme.
* **Cristaux** : sources bornées par le temps de jeu ; dépenses sans plafond (rerolls). La monnaie permanente est structurellement déflationniste.
* **Aucun échange** entre joueurs : pas de marché, pas de prix qui dérive, pas de transfert depuis un compte secondaire.
* **Minerais liés** et détruits au Rebirth : pas de stock caché d'un run à l'autre.
* **Coûts indexés** : prix des pioches et XP requise x (1 + 0,10 x Rebirth).

## 🏷️ Vente

* `/sell` : vend tous les minerais et blocs compressés de l'inventaire, sauf les minerais protégés.
* **Minerais protégés** : liste réglable dans `/parametres`. Par défaut, le minerai de la prochaine pioche et les minerais des armures non encore achetées sont protégés.
* **Vente de débordement** : un minerai qui ne rentre plus dans l'inventaire est vendu automatiquement à 50 % de sa valeur. Le joueur est prévenu une fois par minute.
* **Vente automatique** : vend à 100 % toutes les 10 secondes, minerais protégés exclus. Débloquée au grade Champion ou au Rebirth 3.
* Points de vente : hub et relais de chaque biome, spawn.

## 🗄️ Stockage

Le sac est supprimé. Voir [Stockage /pv](pv.md).
