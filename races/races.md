---
description: Les 8 races, leurs bonus, talents, probabilités, reroll et limites.
---

# 🧝 Races

## 🎯 Objectif

La race est la **spécialisation permanente** du joueur. Elle oriente son style : un Nain chasse les minerais rares, un Elfe monte ses niveaux plus vite, un Gobelin optimise ses ventes. C'est aussi un objectif de collection et une dépense de Cristaux de long terme.

## ⚙️ Fonctionnement

* Une race par compte, tirée au hasard à la première connexion.
* Conservée au Rebirth.
* Reroll dans `/race`, contre des Cristaux.
* Après un reroll, le joueur **choisit** : garder sa race actuelle ou prendre la nouvelle. Un reroll ne fait jamais perdre une bonne race.

## 📋 Les 8 races

| Race | Rareté | Probabilité |
| --- | --- | --- |
| Humain | Commun | 35 % |
| Nain | Peu commun | 20 % |
| Gobelin | Peu commun | 20 % |
| Elfe | Rare | 12 % |
| Gnome | Rare | 8 % |
| Golem | Épique | 3,5 % |
| Draconide | Légendaire | 1,2 % |
| Céleste | Mythique | 0,3 % |

### Humain
* Rareté : Commun
* Bonus : +4 % Argent, +4 % XP
* Talent : aucun
* Style : polyvalent

### Nain
* Rareté : Peu commun
* Bonus : +8 % Fortune
* Talent **Flair** : les minerais Rares et supérieurs à 4 blocs ou moins brillent pour le joueur seul
* Style : chasse aux minerais rares

### Gobelin
* Rareté : Peu commun
* Bonus : +8 % Argent
* Talent **Marchand** : -10 % sur les prix en Argent du Shop rotatif
* Style : rendement brut

### Elfe
* Rareté : Rare
* Bonus : +12 % XP
* Talent **Agilité** : +15 % de vitesse de déplacement dans les mines
* Style : progression rapide des niveaux, meilleure race pour raccourcir un run

### Gnome
* Rareté : Rare
* Bonus : +12 % Chance
* Talent **Fouineur** : les Œufs éclosent en 1 125 blocs au lieu de 1 500
* Style : pets et Trouvailles

### Golem
* Rareté : Épique
* Bonus : +12 % Éclats
* Talent **Force** : +20 % de chance d'Excavation, relatif, dans la limite du plafond de 18 %
* Style : enchantements rapides, casse de zone

### Draconide
* Rareté : Légendaire
* Bonus : +10 % Argent, +10 % Fortune
* Talent **Flair étendu** : comme Flair, à 8 blocs
* Style : rendement et chasse aux rares

### Céleste
* Rareté : Mythique
* Bonus : +8 % Argent, XP, Fortune, Éclats et Chance
* Talent **Grâce** : chute lente et +10 % de vitesse de déplacement dans les mines
* Style : tout-en-un, objectif de très long terme

## 💎 Reroll

* Coût : 60 Cristaux par reroll
* Garantie : après 15 rerolls sans race Épique ou supérieure, le reroll suivant donne Golem (75 %), Draconide (20 %) ou Céleste (5 %)
* Le compteur de garantie est par compte et repart à zéro dès qu'une race Épique ou supérieure est tirée

| Objectif | Rerolls moyens | Cristaux moyens | Runs d'un joueur moyen |
| --- | --- | --- | --- |
| Draconide ou Céleste | 40 | 2 400 | environ 4 |
| Céleste | 202 | 12 100 | environ 20 |

Moyennes obtenues par simulation de 50 000 tirages, garantie comprise.

## 🔗 Interactions

* Les bonus de race s'additionnent aux bonus du même type (voir [Formules](../game-design/formules.md)).
* Flair et Flair étendu : surbrillance envoyée par paquets au seul joueur concerné, 20 blocs surlignés au maximum, rafraîchie toutes les 2 secondes.
* Les talents de vitesse de déplacement s'additionnent à la Mobilité des bottes. Vitesse de déplacement bonus plafonnée à +35 %.

## 🔒 Limites

{% hint style="warning" %}
* Aucune race ne donne plus de 12 % sur une statistique. La race compte, mais elle ne remplace ni les pets ni les armures.
* Aucune race n'est vendue. Aucune caisse ne donne de reroll de race.
{% endhint %}
