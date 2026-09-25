---
description: Les trois monnaies, les formules de gain, les revenus de référence, les dépenses et le contrôle de l'inflation.
---

# 💰 Économie

## 🪙 Monnaies

| Monnaie | Symbole | Durée de vie | Échangeable |
| --- | --- | --- | --- |
| Argent | $ | Cycle, remis à 0 au Prestige | Non |
| Éclats | ✦ | Cycle, remis à 0 au Prestige | Non |
| Cristaux | ◆ | Permanente | Non |

**Argent** : vente des minerais et bloc principal. Dépensé en pioches, coût de Prestige, armures, boosters.

**Éclats** : un montant par bloc cassé selon le biome (1 à 90). Dépensés en enchantements.

**Cristaux** : monnaie permanente. Dépensée en traits, races, Shop rotatif, création et amélioration de guilde.

{% hint style="danger" %}
Aucune monnaie ne se transfère entre joueurs : ni `/pay`, ni hôtel des ventes, ni échange de minerais. Seule exception : un joueur peut déposer des Cristaux dans la banque de sa guilde, sans pouvoir les reprendre.
{% endhint %}

## 🧮 Formules

```
Vente d'un minerai = valeur x quantité x (1 + bonus Argent) x MP x MR
Quantité           = 1 + bonus Fortune
Bloc principal     = valeur x (1 + bonus Argent) x MP x MR
Éclats d'un bloc   = Éclats du biome x (1 + bonus Éclats) x MP x MR
MP = multiplicateur de Prestige = 1,6^rang
MR = multiplicateur de Renaissance = 1 + 0,5 x Renaissance x (1 + bonus Phénix)
```

Détail des bonus et plafonds : [Formules](../game-design/formules.md).

## 📈 Revenus de référence

Joueur moyen, **premier passage** dans chaque biome, au rang de Prestige où ce biome est découvert.

| Biome | Prestige | Blocs/min | Minerais/min, Fortune comprise | Argent/h |
| --- | --- | --- | --- | --- |
| 1. Plaines | 0 | 69 | 12 | 69 500 $ |
| 2. Cavernes de spéléothèmes | 0 | 83 | 17 | 142 000 $ |
| 3. Badlands | 0 | 94 | 17 | 302 000 $ |
| 4. Pics dentelés | 0 | 106 | 20 | 552 000 $ |
| 5. Terres désolées du Nether | I | 130 | 28 | 2 100 000 $ (2,1 M) |
| 6. Forêt carmin | I | 143 | 39 | 3 800 000 $ (3,8 M) |
| 7. Forêt biscornue | II | 171 | 57 | 11 900 000 $ (11,9 M) |
| 8. Vallée des âmes | III | 185 | 59 | 35 300 000 $ (35,3 M) |
| 9. Terres stériles de l'End | IV | 217 | 59 | 126 000 000 $ (126 M) |
| 10. Petites îles de l'End | IV | 232 | 82 | 226 000 000 $ (226 M) |
| 11. Terres moyennes de l'End | V | 247 | 103 | 599 000 000 $ (599 M) |
| 12. Hautes terres de l'End | VI | 284 | 113 | 1 910 000 000 $ (1,91 Md) |
| 13. Prairie | VII | 323 | 109 | 6 480 000 000 $ (6,48 Md) |
| 14. Bosquet de cerisiers | VII | 341 | 147 | 10 900 000 000 $ (10,9 Md) |
| 15. Pentes enneigées | VIII | 384 | 193 | 29 900 000 000 $ (29,9 Md) |
| 16. Pics gelés | IX | 403 | 192 | 87 100 000 000 $ (87,1 Md) |

L'Argent par heure grimpe d'environ 70 000 $ à 87 Md $ entre le premier et le dernier biome : valeur des biomes (x400), vitesse (x5,8), Fortune et bonus, et surtout multiplicateur de Prestige (x69 au Prestige IX).

## 🧾 Dépenses

| Poste | Monnaie | Rôle |
| --- | --- | --- |
| Pioches | Argent | Dépense principale de chaque cycle |
| Coût de Prestige | Argent | 30 % du prix de la pioche de porte |
| Armures | Argent et minerais | Investissement permanent |
| Boosters du Shop | Argent | Conversion vers l'XP, les Éclats ou la Chance |
| Enchantements | Éclats | Reconstruits à chaque cycle |
| Traits, races, Shop, guilde | Cristaux | Dépenses permanentes sans plafond |

## 💎 Budget de Cristaux jusqu'à la première Renaissance

Joueur moyen, environ 412 h de jeu et 6,6 millions de blocs cassés. Pour les sources quotidiennes (votes, Concours, guilde), hypothèse de 3 h de jeu par jour, soit environ 137 jours 🟠.

| Source | Cristaux |
| --- | --- |
| Trouvailles : 6 600 000 / 4 000 x 1,5 de bonus de Chance moyen 🟠 | environ 2 500 |
| Récompenses de Prestige, I à X | 750 |
| Renaissance 1 | 400 |
| Collections | environ 1 000 |
| Premières entrées dans les biomes et tutoriel | 98 |
| Votes : 6,6 par jour x 137 jours | environ 900 |
| Boss, participation, voir [Boss](../evenements/boss.md) | environ 750 |
| Guilde : défis, classement et niveaux, voir [Guildes](../social/guildes.md) | environ 700 |
| Chat réaction et Concours de minage | environ 200 |
| **Total** | **environ 7 300, soit 7 300 / 412 = environ 17,7 par heure** |

| Dépense | Coût |
| --- | --- |
| Reroll de trait | 10, ou 30 avec type verrouillé |
| Reroll de race | 60 |
| Shop rotatif | 25 à 1 200 |
| Création de guilde | 50 |
| Améliorations de guilde | 100 à 800, payées par la banque de guilde |

## 🛑 Contrôle de l'inflation

* **Argent et Éclats** sont remis à zéro à chaque Prestige : rien ne s'accumule sur le long terme, quel que soit le multiplicateur.
* **Prix fixes par pioche** : le multiplicateur de Prestige rend les pioches déjà connues rapides à reforger, mais chaque pioche nouvelle est calibrée sur le revenu du rang où elle est découverte.
* **Cristaux** : sources bornées par le temps de jeu, dépenses sans plafond. Monnaie permanente déflationniste.
* **Aucun échange** entre joueurs, minerais liés et détruits au Prestige.

## 🏷️ Vente

* `/sell` : vend tous les minerais et blocs compressés de l'inventaire, sauf les minerais protégés.
* **Minerais protégés** : réglables dans `/parametres`. Par défaut : le minerai de la prochaine pioche et ceux des armures non achetées.
* **Vente de débordement** : un minerai qui ne rentre plus dans l'inventaire est vendu automatiquement à 50 % de sa valeur.
* **Vente automatique** : vend à 100 % toutes les 10 secondes, minerais protégés exclus. Grade Champion, ou dès le premier Prestige III atteint.
* Points de vente : hub et relais de chaque biome, spawn.

## 🗄️ Stockage

Le sac est supprimé. Voir [Stockage /pv](pv.md).
