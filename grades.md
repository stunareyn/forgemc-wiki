---
description: Les 7 grades, couleurs, prix, avantages, permissions et limites.
---

# 👑 Grades

## ⚙️ Principes

* Sept grades, dans cet ordre : Joueur → Pilier → Héros → Champion → Légende → Monarque → Immortal.
* Les grades Pilier à Monarque s'achètent sur la boutique. Monter d'un grade coûte la différence de prix.
* **Immortal ne s'achète pas** : il est attribué automatiquement quand le total des achats boutique d'un compte atteint 1 000 €.
* Un grade est permanent, conservé au Prestige et à la Renaissance. Il est retiré en cas de remboursement ou d'opposition de paiement.
* Chaque grade inclut tous les avantages des grades inférieurs.

## 📋 Vue d'ensemble

| Grade | Couleur | Prix | Bonus d'Argent | Pages `/pv` |
| --- | --- | --- | --- | --- |
| Joueur | Gris `#AAAAAA` | Gratuit | 0 % | 1 |
| Pilier | Vert `#55FF55` | 9,99 € | +2 % | 2 |
| Héros | Bleu clair `#55FFFF` | 19,99 € | +4 % | 3 |
| Champion | Or `#FFAA00` | 34,99 € | +6 % | 4 |
| Légende | Violet `#FF55FF` | 59,99 € | +8 % | 5 |
| Monarque | Rouge `#FF5555` | 99,99 € | +10 % | 6 |
| Immortal | Dégradé or et blanc `#FFD86B` → `#FFFFFF` | 1 000 € d'achats cumulés | +12 % | 8 |

La Renaissance 1 ajoute 1 page `/pv` à tous les grades.

## 🎁 Avantages

### Joueur
* Délai entre deux messages : 3 s
* Délai de `/tpa` : 60 s
* `/mail` : 5 messages en attente au maximum

### Pilier
* Préfixe et couleur de pseudo
* Délai entre deux messages : 2 s
* Délai de `/tpa` : 45 s

### Héros
* `/spawn`, `/hub` et `/relais` sans le délai de 5 s
* Délai de `/tpa` : 30 s
* `/mail` : 20 messages en attente

### Champion
* **Vente automatique**. Les joueurs sans grade la débloquent pour toujours au premier Prestige III atteint.
* Délai entre deux messages : 1 s
* Couleurs dans les messages de chat (codes `&` hors gras, souligné et magique)

### Légende
* **Priorité** dans la file d'attente des biomes pleins
* Message de connexion au serveur
* Délai de `/tpa` : 15 s

### Monarque
* 1 clé Pets Premium à l'achat du grade
* Son de minage Couronne
* Tag de guilde en couleur au choix, sans passer par la banque de guilde

### Immortal
* Priorité maximale dans la file d'attente
* Son de minage Immortel
* Titre « Immortal » et pseudo en dégradé

## 🔑 Permissions par grade

| Grade | Groupe LuckPerms | Permissions ajoutées |
| --- | --- | --- |
| Joueur | `default` | `strata.player.*`, `strata.pv.pages.1`, `strata.tpa.cooldown.60`, `strata.mail.limit.5` |
| Pilier | `pilier` | `strata.pv.pages.2`, `strata.grade.bonus.2`, `strata.tpa.cooldown.45`, `strata.chat.delay.2` |
| Héros | `heros` | `strata.pv.pages.3`, `strata.grade.bonus.4`, `strata.tp.nodelay`, `strata.tpa.cooldown.30`, `strata.mail.limit.20` |
| Champion | `champion` | `strata.pv.pages.4`, `strata.grade.bonus.6`, `strata.sell.auto`, `strata.chat.delay.1`, `strata.chat.color` |
| Légende | `legende` | `strata.pv.pages.5`, `strata.grade.bonus.8`, `strata.queue.priority.1`, `strata.join.message`, `strata.tpa.cooldown.15` |
| Monarque | `monarque` | `strata.pv.pages.6`, `strata.grade.bonus.10`, `strata.sons.couronne`, `strata.guilde.tagcolor` |
| Immortal | `immortal` | `strata.pv.pages.8`, `strata.grade.bonus.12`, `strata.queue.priority.2`, `strata.sons.immortel` |

Chaque groupe hérite du groupe précédent. Pour une permission numérique (`pv.pages`, `grade.bonus`, `tpa.cooldown`, `mail.limit`, `chat.delay`), seule la valeur la plus avantageuse est prise en compte.

## ⚖️ Limites

{% hint style="warning" %}
* Le seul bonus de puissance d'un grade est l'Argent, **+12 % au maximum**.
* Aucun grade ne donne d'XP, d'Éclats, de Cristaux, d'emplacement de pet, de reroll, de pioche, ni d'avantage sur les boss ou les événements.
* Les bonus d'Argent s'additionnent : +12 % de grade pèse peu à côté de l'enchantement Argent, jusqu'à +150 %, et des autres sources. Le minerai du premier forgeage, lui, ne s'achète pas. Un joueur optimisé Immortal avec un pet Mythique Argent ★3 niveau 40 dès la première minute atteint sa première Renaissance en 232 h 55, contre 260 h 38 pour le même joueur sans achat, soit 10,6 % de moins. Voir [Équilibrage](../equilibrage/equilibrage.md).
{% endhint %}
