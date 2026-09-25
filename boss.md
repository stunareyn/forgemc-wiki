---
description: Les 4 boss invisibles de dimension, leurs horaires, points de vie, dégâts, récompenses et fonctionnement technique.
---

# 👹 Boss

## 🎯 Objectif

Réunir tous les joueurs d'une dimension autour d'un objectif commun, sans combat et sans interrompre le minage. Le boss n'a **aucune apparence** : il existe seulement par sa barre de boss. Chaque bloc cassé dans un biome de sa dimension lui retire des points de vie.

## 📋 Les 4 boss

| Boss | Dimension | Fréquence | Horaires, heure de Paris | Pet | Cristaux de participation |
| --- | --- | --- | --- | --- | --- |
| Le Colosse enfoui | Overworld | Toutes les 2 h | 00 h 10, 02 h 10, 04 h 10, puis toutes les 2 h jusqu'à 22 h 10 | Dragon de la Nature, Épique, Fortune | 3 |
| Le Seigneur des Cendres | Nether | Toutes les 3 h | 00 h 40, 03 h 40, 06 h 40, 09 h 40, 12 h 40, 15 h 40, 18 h 40, 21 h 40 | Dragon Mort-Vivant, Légendaire, Argent | 5 |
| Le Dévoreur du Vide | End | Toutes les 4 h | 01 h 25, 05 h 25, 09 h 25, 13 h 25, 17 h 25, 21 h 25 | Dragon de Glace, Légendaire, Éclats | 8 |
| Le Roi des Tempêtes | Aether | Toutes les 6 h | 03 h 55, 09 h 55, 15 h 55, 21 h 55 | Dragon de Foudre, Mythique, Chance | 12 |

Soit 12 + 8 + 6 + 4 = 30 boss par jour. Les horaires sont décalés pour qu'aucune annonce ne se superpose.

## 📜 Déroulement

1. **Annonce, 60 s avant** : message dans le chat de la dimension et titre à l'écran : « Le Colosse enfoui s'éveille sous vos pieds. 60 secondes. »
2. **Apparition** : la barre de boss apparaît pour tous les joueurs présents dans un biome de la dimension, avec le nom du boss, ses points de vie et le temps restant. Son d'apparition joué une fois : `entity.wither.spawn`, volume 0,3.
3. **Combat, 15 minutes au maximum** : chaque bloc cassé retire des points de vie. La barre se met à jour chaque seconde.
4. **Fin** : boss vaincu, ou boss enfui après 15 minutes.

Un joueur qui entre dans la dimension pendant le combat voit la barre et peut participer.

## ❤️ Points de vie

```
PV max = PV par joueur x max(joueurs présents, 20)
```

| Boss | PV par joueur | PV minimum, 20 joueurs |
| --- | --- | --- |
| Le Colosse enfoui | 500 | 10 000 |
| Le Seigneur des Cendres | 900 | 18 000 |
| Le Dévoreur du Vide | 1 500 | 30 000 |
| Le Roi des Tempêtes | 2 200 | 44 000 |

* **Joueurs présents** : joueurs connectés dans un biome de la dimension à l'apparition, hors joueurs inactifs depuis plus de 2 minutes.
* Chaque joueur qui entre dans la dimension pendant le combat ajoute ses PV par joueur au total, une seule fois par combat. La barre affiche un pourcentage : elle ne remonte pas, les PV restants sont recalculés à pourcentage constant.

**Calcul de la durée visée** : environ 10 minutes pour une population au premier passage dans la dimension, dont 70 % minent réellement 🟠.

| Boss | Blocs/min au premier biome de la dimension | Durée = PV par joueur / (blocs/min x 0,7) |
| --- | --- | --- |
| Le Colosse enfoui | 69 | 500 / 48,3 = 10,4 min |
| Le Seigneur des Cendres | 130 | 900 / 91 = 9,9 min |
| Le Dévoreur du Vide | 217 | 1 500 / 151,9 = 9,9 min |
| Le Roi des Tempêtes | 323 | 2 200 / 226,1 = 9,7 min |

Les joueurs de rang de Prestige plus élevé cassent plus vite : le boss meurt plus tôt quand ils sont nombreux. La limite de 15 minutes laisse 50 % de marge aux populations lentes.

## ⚔️ Dégâts

| Bloc cassé | Dégâts |
| --- | --- |
| Bloc principal | 1 |
| Minerai Commun ou Peu commun | 1 |
| Minerai Rare | 3 |
| Minerai Épique | 10 |
| Minerai Légendaire | 30 |
| Minerai Mythique | 100 |

* Seuls les blocs cassés **directement** par le joueur comptent. Les blocs de la zone d'Excavation n'infligent pas de dégâts : le boss récompense la présence et l'activité, pas l'équipement.
* Les dégâts sont affichés en petit dans la barre d'action : « +10 · Colosse enfoui ».
* Un minerai Légendaire ou Mythique déclenche un message dans le chat de la dimension : « Lyra frappe le Colosse enfoui : 100 dégâts ! ».
* Un joueur ne peut pas infliger plus de 16 dégâts de base par seconde, soit le plafond technique de 16 blocs par seconde. Les bonus de rareté s'ajoutent.

## ✅ Participation valide

Un joueur participe s'il inflige **au moins 100 dégâts** pendant le combat. Au premier passage dans l'Overworld, cela représente environ 1 min 30 de minage.

## 🎁 Récompenses

### Boss vaincu

| Récompense | Qui | Détail |
| --- | --- | --- |
| Cristaux | Chaque participant | 3, 5, 8 ou 12 selon le boss |
| Booster de dimension | Tous les joueurs de la dimension | +10 % Argent et +10 % XP pendant 20 min de minage actif |
| Chance de pet | Chaque participant | Voir tableau ci-dessous |
| Classement du combat | Les 3 plus gros dégâts | 1er : 3 fois les Cristaux de participation en plus. 2e : 2 fois. 3e : 1 fois |
| Coup fatal | Le joueur qui inflige le dernier dégât | 1 Clé Vote |
| Collection | Chaque participant | Première victoire : titre du boss et 25 Cristaux |

### Chance de pet

```
Chance = base + bonus x (part des dégâts en %), plafonnée
```

| Boss | Base | Bonus par 1 % des dégâts | Plafond | Garantie |
| --- | --- | --- | --- | --- |
| Le Colosse enfoui | 1 % | 0,2 % | 5 % | 150 participations valides sans le pet |
| Le Seigneur des Cendres | 0,5 % | 0,1 % | 3 % | 200 participations |
| Le Dévoreur du Vide | 0,5 % | 0,1 % | 3 % | 200 participations |
| Le Roi des Tempêtes | 0,2 % | 0,05 % | 1,5 % | 300 participations |

Exemple : 100 joueurs sur le Roi des Tempêtes, un joueur qui fait 1 % des dégâts a 0,2 + 0,05 x 1 = 0,25 % de chance.

* Le compteur de garantie est propre à chaque boss et repart à zéro quand le pet est obtenu.
* Un pet déjà possédé est livré normalement, recyclable en Essence.

### Boss enfui

* Chaque participant reçoit la moitié des Cristaux de participation, arrondie au supérieur : 2, 3, 4 ou 6.
* Pas de booster, pas de chance de pet, pas de classement. Le compteur de garantie avance quand même.

## 🧮 Poids dans la progression

Joueur moyen jusqu'à la première Renaissance, d'après le temps passé dans chaque dimension par la simulation :

| Dimension | Temps passé | Boss rencontrés = temps / fréquence | Cristaux, 90 % de victoires 🟠 |
| --- | --- | --- | --- |
| Overworld | 25,6 h | 12,8 | 12,8 x 3 x (0,9 + 0,1 x 0,5) = 36 |
| Nether | 85,7 h | 28,6 | 28,6 x 5 x 0,95 = 136 |
| End | 137,2 h | 34,3 | 34,3 x 8 x 0,95 = 261 |
| Aether | 163,6 h | 27,3 | 27,3 x 12 x 0,95 = 311 |
| **Total** | **412,1 h** | **103** | **744, environ 750** |

Les 100 Cristaux de la collection Boss et les récompenses de classement s'ajoutent, et un joueur qui change de dimension pour suivre les boss en gagne davantage. Le temps passé dans l'Aether est le plus long, parce que les cycles VII à X sont les plus longs.

## 🛠️ Fonctionnement technique

* **Aucune entité**. Le boss est un état en mémoire : identifiant, PV max, PV restants, heure de fin, table des dégâts par joueur.
* Barre de boss Adventure `BossBar`, couleur par dimension : verte, rouge, violette, blanche.
* Si une dimension tourne sur plusieurs serveurs, les PV sont stockés dans Redis. Chaque serveur additionne les dégâts localement et les envoie toutes les 250 ms par un script Lua atomique qui décrémente les PV et renvoie le nouvel état. Le script qui fait passer les PV à 0 désigne le coup fatal : un seul serveur distribue les récompenses.
* Les dégâts d'un bloc ne sont comptés qu'après validation de la casse par l'anti-triche, dans le même traitement que les récompenses du bloc. Aucune tâche par bloc n'est créée.
* Redémarrage d'un serveur pendant un combat : l'état est dans Redis, le combat continue sur les autres serveurs. Redémarrage de tous les serveurs de la dimension : le boss est annulé, sans récompense ni avancement de garantie.

## ⌨️ Commandes

* `/boss` : menu des boss, prochains horaires, combat en cours, dégâts personnels, compteurs de garantie. Voir [Menus GUI · Événements](../menus/evenements.md).
* Staff : `/strata boss spawn <dimension>`, `/strata boss stop <dimension>`, `/strata boss hp <dimension> <pourcentage>`. Voir [Commandes d'administration](../commandes/administration.md).
