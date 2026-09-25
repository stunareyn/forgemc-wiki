---
description: Les 22 pets, leurs raretés, bonus, obtention, niveaux, Éveil et emplacements.
---

# 🐾 Pets

## 🎯 Objectif

Les pets sont la principale progression **permanente** liée au minage : ils se trouvent en minant, gagnent de l'expérience en minant et renforcent le minage. Aucun bonus de combat.

## ⚙️ Règles générales

* Emplacements actifs : 1 au départ, 2 dès le premier Prestige V atteint, 3 à la Renaissance 1, 4 à la Renaissance 4. Ces emplacements sont définitifs.
* **Un seul pet actif par type de bonus.**
* Affichage par paquets, sans entité serveur, visible du propriétaire et des joueurs proches. Option d'affichage dans `/parametres`.
* Pets conservés au Prestige et à la Renaissance, avec niveau, étoiles et trait. Non échangeables.

## 📊 Valeur des bonus

Bonus = base de la rareté x (1 + (niveau - 1) / 39) x (1 + 0,15 x étoiles).

**Argent, XP, Éclats**

| Rareté | Niveau 1 | Niveau 40 | Niveau 40 ★3 |
| --- | --- | --- | --- |
| Commun | 2 % | 4 % | 5,8 % |
| Peu commun | 3 % | 6 % | 8,7 % |
| Rare | 5 % | 10 % | 14,5 % |
| Épique | 7,5 % | 15 % | 21,75 % |
| Légendaire | 11 % | 22 % | 31,9 % |
| Mythique | 15 % | 30 % | 43,5 % |

**Fortune** : valeurs ci-dessus x 0,6. **Chance** : valeurs ci-dessus x 1,5.

**Renaissance**, Phénix seulement : 10 % au niveau 1, 20 % au niveau 40, 29 % à ★3, appliqués au bonus de Renaissance. À la Renaissance 4 (bonus +200 %), un Phénix ★3 porte ce bonus à +258 %.

## 📈 Niveaux

* Niveau 1 à 40, 1 XP de pet par bloc cassé pendant que le pet est actif.
* XP du niveau N à N+1 : 400 x 1,12^(N-1). Total jusqu'au niveau 40 : 273 604 XP.
* Un joueur qui casse 15 000 blocs par heure monte un pet au niveau 40 en environ 18 h.
* Bonus d'XP de pet : collection Pets (jusqu'à +25 %) et trait Couveur (jusqu'à +100 %).

## ⭐ Éveil

| Étoile | Niveau requis | Coût |
| --- | --- | --- |
| ★1 | 20 | 1 Essence de sa rareté et 32 minerais Rares |
| ★2 | 30 | 2 Essences de sa rareté et 16 minerais Épiques |
| ★3 | 40 | 3 Essences de sa rareté, 4 minerais Légendaires et 1 minerai Mythique |

Minerais de n'importe quelle dimension. Comme les minerais sont détruits au Prestige, l'Éveil se fait dans le cycle où les minerais ont été trouvés.

**Essences** : recycler un pet donne 1 Essence de sa rareté plus la moitié des Essences de ses étoiles. 4 Essences d'une rareté donnent 1 Essence de la rareté supérieure.

## 🥚 Œufs

* Trouvaille : 1 chance sur 100 000 par bloc cassé, multipliée par le bonus de Chance.
* L'Œuf trouvé correspond à la dimension où le joueur mine.
* Éclosion : 1 500 blocs cassés avec l'Œuf dans l'inventaire, 1 125 pour la race Gnome. Trois Œufs incubent au maximum.
* Œufs conservés au Prestige et à la Renaissance.

| Œuf | Commun | Peu commun | Rare | Épique | Légendaire | Mythique |
| --- | --- | --- | --- | --- | --- | --- |
| Overworld | Aigle 60 % | Renard Spirituel 30 % | Kitsune 10 % | | | |
| Nether | | Chien Infernal 60 % | Démon 30 % | Dragon de Feu 10 % | | |
| End | | | Loup Lunaire 60 % | Kitsune Obscur 30 % | Dragon des Ombres 10 % | |
| Aether | | | | Oiseau-Tonnerre 72 % | Ange 25 % | Dragon d'Éther 3 % |

Un joueur moyen trouve environ 100 Œufs en minant avant sa première Renaissance.

## 📇 Les 22 pets

### Pets des Œufs

* **Aigle** · `pet_eagle` · Commun · XP · Œuf de l'Overworld · premier pet
* **Renard Spirituel** · `pet_spirit_fox` · Peu commun · Chance · Œuf de l'Overworld
* **Kitsune** · `pet_kitsune` · Rare · Argent · Œuf de l'Overworld · premier bon pet Argent
* **Chien Infernal** · `pet_hellhound` · Peu commun · Argent · Œuf du Nether
* **Démon** · `pet_demon` · Rare · Fortune · Œuf du Nether · premier pet Fortune
* **Dragon de Feu** · `pet_fire_dragon` · Épique · Éclats · Œuf du Nether
* **Loup Lunaire** · `pet_lunar_wolf` · Rare · Éclats · Œuf de l'End
* **Kitsune Obscur** · `pet_dark_kitsune` · Épique · XP · Œuf de l'End
* **Dragon des Ombres** · `pet_shadow_dragon` · Légendaire · Fortune · Œuf de l'End · meilleur pet Fortune
* **Oiseau-Tonnerre** · `pet_thunderbird` · Épique · Chance · Œuf de l'Aether
* **Ange** · `pet_angel` · Légendaire · XP · Œuf de l'Aether · meilleur pet XP
* **Dragon d'Éther** · `pet_aether_dragon` · Mythique · Argent · Œuf de l'Aether, 3 % · meilleur pet Argent

### Pets des boss

Chaque boss a une chance de donner son pet aux participants. Voir [Boss](../evenements/boss.md).

* **Dragon de la Nature** · `pet_nature_dragon` · Épique · Fortune · Le Colosse enfoui, Overworld
* **Dragon Mort-Vivant** · `pet_undead_dragon` · Légendaire · Argent · Le Seigneur des Cendres, Nether
* **Dragon de Glace** · `pet_ice_dragon` · Légendaire · Éclats · Le Dévoreur du Vide, End · meilleur pet Éclats
* **Dragon de Foudre** · `pet_thunder_dragon` · Mythique · Chance · Le Roi des Tempêtes, Aether · meilleur pet Chance

### Pet de la caisse Pets F2W

* **Loup de Givre** · `pet_frost_wolf` · Peu commun · Fortune · caisse Pets F2W, 40 %

### Pets de la caisse Pets Premium

* **Ninja au Shuriken** · `pet_shuriken_ninja` · Rare · Chance · 45 %
* **Ninja au Saï** · `pet_sai_ninja` · Épique · XP · 33 %
* **Samouraï** · `pet_samurai` · Légendaire · Fortune · 18 %
* **Dragon du Vent** · `pet_wind_dragon` · Mythique · Argent · 4 %

### Pet de la Renaissance

* **Phénix** · `pet_phoenix` · Mythique · Renaissance · récompense de la Renaissance 1 · seul pet de son type

## ⚖️ Équité F2W et Premium

| Type | Meilleur pet gratuit | Meilleur pet Premium |
| --- | --- | --- |
| Argent | Dragon d'Éther, Mythique | Dragon du Vent, Mythique |
| XP | Ange, Légendaire | Ninja au Saï, Épique |
| Fortune | Dragon des Ombres, Légendaire | Samouraï, Légendaire |
| Éclats | Dragon de Glace, Légendaire | Aucun |
| Chance | Dragon de Foudre, Mythique | Ninja au Shuriken, Rare |
| Renaissance | Phénix, Mythique | Aucun |

{% hint style="success" %}
Pour chaque type, le plafond gratuit est égal ou supérieur au plafond Premium.
{% endhint %}
