---
description: Les 7 grades, couleurs, prix, avantages, permissions et limites.
---

# 👑 Grades

## ⚙️ Principes

* Sept grades, dans cet ordre : Joueur → Pilier → Héros → Champion → Légende → Monarque → Immortal.
* Les grades Pilier à Monarque s'achètent sur la boutique. Monter d'un grade coûte la différence de prix.
* **Immortal ne s'achète pas** : il est attribué automatiquement quand le total des achats boutique d'un compte atteint 1 000 €.
* Un grade est permanent. Il est retiré en cas de remboursement ou d'opposition de paiement.
* Chaque grade inclut tous les avantages des grades inférieurs.

## 📋 Vue d'ensemble

| Grade | Couleur | Prix |
| --- | --- | --- |
| Joueur | Gris `#AAAAAA` | Gratuit |
| Pilier | Vert `#55FF55` | 9,99 € |
| Héros | Bleu clair `#55FFFF` | 19,99 € |
| Champion | Or `#FFAA00` | 34,99 € |
| Légende | Violet `#FF55FF` | 59,99 € |
| Monarque | Rouge `#FF5555` | 99,99 € |
| Immortal | Dégradé or et blanc `#FFD86B` → `#FFFFFF` | 1 000 € d'achats cumulés |

## 🎁 Avantages

### Joueur
* Bonus d'Argent : 0 %
* Pages `/pv` : 1
* Délai entre deux messages : 3 s

### Pilier
* Bonus d'Argent : +2 %
* Pages `/pv` : 2
* Préfixe et couleur de pseudo
* Délai entre deux messages : 2 s

### Héros
* Bonus d'Argent : +4 %
* Pages `/pv` : 3
* Commande `/hub` depuis n'importe quel biome sans délai de 5 s

### Champion
* Bonus d'Argent : +6 %
* Pages `/pv` : 4
* **Vente automatique**. Les joueurs sans grade la débloquent au Rebirth 3, par une condition du plugin, sans permission de grade.
* Délai entre deux messages : 1 s

### Légende
* Bonus d'Argent : +8 %
* Pages `/pv` : 5
* **Priorité** dans la file d'attente des biomes pleins
* Message de connexion au serveur

### Monarque
* Bonus d'Argent : +10 %
* Pages `/pv` : 6
* 1 clé Pets Premium à l'achat du grade
* Son de minage Couronne

### Immortal
* Bonus d'Argent : +12 %
* Pages `/pv` : 8
* Priorité maximale dans la file d'attente
* Son de minage Immortel
* Titre « Immortal » et pseudo en dégradé

## 🔑 Permissions par grade

| Grade | Groupe LuckPerms | Permissions ajoutées |
| --- | --- | --- |
| Joueur | `default` | `strata.player.*`, `strata.pv.pages.1` |
| Pilier | `pilier` | `strata.pv.pages.2`, `strata.grade.bonus.2` |
| Héros | `heros` | `strata.pv.pages.3`, `strata.grade.bonus.4`, `strata.tp.hub.nodelay` |
| Champion | `champion` | `strata.pv.pages.4`, `strata.grade.bonus.6`, `strata.sell.auto` |
| Légende | `legende` | `strata.pv.pages.5`, `strata.grade.bonus.8`, `strata.queue.priority.1`, `strata.join.message` |
| Monarque | `monarque` | `strata.pv.pages.6`, `strata.grade.bonus.10`, `strata.sons.couronne` |
| Immortal | `immortal` | `strata.pv.pages.8`, `strata.grade.bonus.12`, `strata.queue.priority.2`, `strata.sons.immortel` |

Chaque groupe hérite du groupe précédent. Seule la permission `strata.grade.bonus.X` la plus haute est prise en compte.

## ⚖️ Limites

{% hint style="warning" %}
* Le seul bonus de puissance d'un grade est l'Argent, **+12 % au maximum**.
* Aucun grade ne donne d'XP, d'Éclats, de Cristaux, d'emplacement de pet, de reroll ou de pioche.
* Le niveau de pioche, qui ne s'achète pas, borne la vitesse d'un joueur qui a tous les bonus d'Argent : un joueur Immortal avec un pet Mythique Argent dès le départ met encore 25 h pour son premier Rebirth, contre 36 h pour un joueur moyen. Voir [Équilibrage](../equilibrage/equilibrage.md).
{% endhint %}
