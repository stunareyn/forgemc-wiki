---
description: Les 22 pets, leurs raretés, bonus, obtention, niveaux, Éveil et emplacements.
---

# 🐾 Pets

## 🎯 Objectif

Les pets sont la principale progression **permanente** liée au minage. Ils se trouvent en minant, gagnent de l'expérience en minant et renforcent le minage. Aucun pet ne donne de bonus de combat.

## ⚙️ Règles générales

* Emplacements actifs : 1 au départ, 2 au Rebirth 2, 3 au Rebirth 5, 4 au Rebirth 15.
* **Un seul pet actif par type de bonus.** Deux pets Argent ne se cumulent pas.
* Les pets suivent le joueur visuellement. Ils n'existent pas comme entités serveur : ils sont affichés par paquets, visibles du propriétaire et des joueurs proches. Option d'affichage dans `/parametres`.
* Pets conservés au Rebirth, avec niveau, étoiles et trait.
* Pets non échangeables.

## 📊 Valeur des bonus

Bonus = base de la rareté x (1 + (niveau - 1) / 39) x (1 + 0,15 x étoiles). Le niveau 40 double la base. Les trois étoiles ajoutent 45 %.

**Argent, XP, Éclats**

| Rareté | Niveau 1 | Niveau 40 | Niveau 40 ★3 |
| --- | --- | --- | --- |
| Commun | 2 % | 4 % | 5,8 % |
| Peu commun | 3 % | 6 % | 8,7 % |
| Rare | 5 % | 10 % | 14,5 % |
| Épique | 7,5 % | 15 % | 21,75 % |
| Légendaire | 11 % | 22 % | 31,9 % |
| Mythique | 15 % | 30 % | 43,5 % |

**Fortune** : valeurs ci-dessus x 0,6. Légendaire niveau 40 ★3 : 19,1 %.

**Chance** : valeurs ci-dessus x 1,5. Légendaire niveau 40 ★3 : 47,9 %.

**Rebirth**, Phénix seulement : 10 % au niveau 1, 20 % au niveau 40, 29 % à ★3. Ce pourcentage s'applique au bonus de Rebirth : au Rebirth 10 (bonus +200 %), un Phénix ★3 porte ce bonus à +258 %.

## 📈 Niveaux

* Niveau 1 à 40.
* 1 XP de pet par bloc cassé pendant que le pet est actif, blocs d'Excavation compris.
* XP pour passer du niveau N à N+1 : 400 x 1,12^(N-1). Total du niveau 1 au niveau 40 : 273 604 XP.
* Un joueur moyen du milieu du premier run casse environ 12 000 blocs par heure : un pet atteint le niveau 40 en 20 à 25 h d'utilisation.
* Bonus d'XP de pet : collection Pets (jusqu'à +25 %) et trait Couveur (jusqu'à +100 %).

## ⭐ Éveil

L'Éveil ajoute des étoiles, de ★1 à ★3.

| Étoile | Niveau requis | Coût |
| --- | --- | --- |
| ★1 | 20 | 1 Essence de sa rareté et 32 minerais Rares |
| ★2 | 30 | 2 Essences de sa rareté et 16 minerais Épiques |
| ★3 | 40 | 3 Essences de sa rareté, 4 minerais Légendaires et 1 minerai Mythique |

Les minerais peuvent venir de n'importe quelle dimension. L'Éveil est le lien direct entre les minerais rares et la progression permanente : un joueur choisit entre vendre un Mythique et renforcer un pet.

**Essences**
* Recycler un pet donne 1 Essence de sa rareté, plus la moitié des Essences utilisées pour ses étoiles.
* Conversion : 4 Essences d'une rareté donnent 1 Essence de la rareté supérieure.
* Sources : recyclage, caisse Pets F2W, shop rotatif.

## 🥚 Œufs

* Trouvaille en minant : 1 chance sur 50 000 par bloc cassé, multipliée par le bonus de Chance.
* L'Œuf trouvé correspond à la dimension où le joueur mine.
* Éclosion : 1 500 blocs cassés avec l'Œuf dans l'inventaire, 1 125 pour la race Gnome.
* Trois Œufs au maximum incubent en même temps.
* Œufs conservés au Rebirth.

| Œuf | Commun | Peu commun | Rare | Épique | Légendaire | Mythique |
| --- | --- | --- | --- | --- | --- | --- |
| Overworld | Aigle 60 % | Renard Spirituel 30 % | Kitsune 10 % | | | |
| Nether | | Chien Infernal 60 % | Démon 30 % | Dragon de Feu 10 % | | |
| End | | | Loup Lunaire 60 % | Kitsune Obscur 30 % | Dragon des Ombres 10 % | |
| Aether | | | | Oiseau-Tonnerre 72 % | Ange 25 % | Dragon d'Éther 3 % |

Un joueur moyen trouve environ 18 Œufs en minant par run, dont la moitié dans l'Aether, plus environ 4 par la caisse Vote s'il vote chaque jour. Par les Œufs seuls, il obtient environ 3 pets Légendaires par run et un Mythique tous les 3 runs.

## 📇 Les 22 pets

### Pets des Œufs

**Aigle** · `pet_eagle`
* Rareté : Commun · Bonus : XP
* Obtention : Œuf de l'Overworld
* Rôle : premier pet, apprend le système

**Renard Spirituel** · `pet_spirit_fox`
* Rareté : Peu commun · Bonus : Chance
* Obtention : Œuf de l'Overworld
* Rôle : premier pet de Trouvailles

**Kitsune** · `pet_kitsune`
* Rareté : Rare · Bonus : Argent
* Obtention : Œuf de l'Overworld
* Rôle : premier bon pet Argent, souvent le pet actif du Nether

**Chien Infernal** · `pet_hellhound`
* Rareté : Peu commun · Bonus : Argent
* Obtention : Œuf du Nether
* Rôle : pet Argent de secours, recyclé en Essence dès qu'un Kitsune est trouvé

**Démon** · `pet_demon`
* Rareté : Rare · Bonus : Fortune
* Obtention : Œuf du Nether
* Rôle : premier pet Fortune, utile dès le 3e emplacement

**Dragon de Feu** · `pet_fire_dragon`
* Rareté : Épique · Bonus : Éclats
* Obtention : Œuf du Nether
* Rôle : accélère les enchantements, bon pet de début de run

**Loup Lunaire** · `pet_lunar_wolf`
* Rareté : Rare · Bonus : Éclats
* Obtention : Œuf de l'End
* Rôle : pet Éclats accessible, source d'Essences Rares

**Kitsune Obscur** · `pet_dark_kitsune`
* Rareté : Épique · Bonus : XP
* Obtention : Œuf de l'End
* Rôle : pet XP de milieu de parcours, précieux pour les joueurs limités par le niveau

**Dragon des Ombres** · `pet_shadow_dragon`
* Rareté : Légendaire · Bonus : Fortune
* Obtention : Œuf de l'End
* Rôle : meilleur pet Fortune gratuit

**Oiseau-Tonnerre** · `pet_thunderbird`
* Rareté : Épique · Bonus : Chance
* Obtention : Œuf de l'Aether
* Rôle : pet Chance solide, source principale d'Essences Épiques

**Ange** · `pet_angel`
* Rareté : Légendaire · Bonus : XP
* Obtention : Œuf de l'Aether
* Rôle : meilleur pet XP, clé de la vitesse des runs

**Dragon d'Éther** · `pet_aether_dragon`
* Rareté : Mythique · Bonus : Argent
* Obtention : Œuf de l'Aether, 3 %
* Rôle : meilleur pet Argent, objectif de long terme gratuit

### Pets de la caisse Pets F2W

**Loup de Givre** · `pet_frost_wolf`
* Rareté : Peu commun · Bonus : Fortune
* Obtention : caisse Pets F2W, 46 %
* Rôle : pet Fortune de départ, source d'Essences

**Dragon de la Nature** · `pet_nature_dragon`
* Rareté : Rare · Bonus : XP
* Obtention : caisse Pets F2W, 30 %
* Rôle : pet XP accessible avant l'End

**Dragon Mort-Vivant** · `pet_undead_dragon`
* Rareté : Épique · Bonus : Argent
* Obtention : caisse Pets F2W, 16,5 %
* Rôle : meilleur pet Argent avant le Dragon d'Éther

**Dragon de Glace** · `pet_ice_dragon`
* Rareté : Légendaire · Bonus : Éclats
* Obtention : caisse Pets F2W, 7 %
* Rôle : meilleur pet Éclats

### Pets de la caisse Pets Premium

**Ninja au Shuriken** · `pet_shuriken_ninja`
* Rareté : Rare · Bonus : Chance
* Obtention : caisse Pets Premium, 45 %
* Rôle : pet Chance Premium d'entrée de gamme

**Ninja au Saï** · `pet_sai_ninja`
* Rareté : Épique · Bonus : XP
* Obtention : caisse Pets Premium, 33 %
* Rôle : équivalent Premium du Kitsune Obscur

**Samouraï** · `pet_samurai`
* Rareté : Légendaire · Bonus : Fortune
* Obtention : caisse Pets Premium, 18 %
* Rôle : équivalent Premium du Dragon des Ombres

**Dragon de Foudre** · `pet_thunder_dragon`
* Rareté : Mythique · Bonus : Argent
* Obtention : caisse Pets Premium, 4 %
* Rôle : équivalent Premium du Dragon d'Éther, jamais cumulable avec lui

### Pet du Shop rotatif

**Dragon du Vent** · `pet_wind_dragon`
* Rareté : Légendaire · Bonus : Chance
* Obtention : emplacement Vedette du Shop rotatif, 900 Cristaux
* Rôle : meilleur pet Chance

### Pet du Rebirth

**Phénix** · `pet_phoenix`
* Rareté : Mythique · Bonus : Rebirth
* Obtention : récompense unique du Rebirth 10
* Rôle : amplifie le multiplicateur de Rebirth, seul pet de son type

## ⚖️ Équité F2W et Premium

| Type | Meilleur pet gratuit | Meilleur pet Premium |
| --- | --- | --- |
| Argent | Dragon d'Éther, Mythique | Dragon de Foudre, Mythique |
| XP | Ange, Légendaire | Ninja au Saï, Épique |
| Fortune | Dragon des Ombres, Légendaire | Samouraï, Légendaire |
| Éclats | Dragon de Glace, Légendaire | Aucun |
| Chance | Dragon du Vent, Légendaire | Ninja au Shuriken, Rare |
| Rebirth | Phénix, Mythique | Aucun |

{% hint style="success" %}
Pour chaque type, le plafond de puissance gratuit est **égal ou supérieur** au plafond Premium. La caisse Premium fait gagner du temps, jamais un palier de puissance inaccessible.
{% endhint %}
