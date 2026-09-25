---
description: Les menus de la pioche : Pioche, Enchantements, Forge, Liste des pioches et Bonus.
---

# ⛏️ Menus · Pioche

## Pioche

* Titre de l'inventaire : `STRATA · Pioche`
* Taille : 54 emplacements, 6 lignes
* Ouverture : `/pioche`, Menu principal, Maj + clic droit avec la pioche
* Permission : `strata.player.pioche`
* Retour vers : Menu principal
* Remplissage : Vitre grise `minecraft:gray_stained_glass_pane`, sans nom

```
      0   1   2   3   4   5   6   7   8 
 0-8  ··  ··  ··  ··  PI  ··  ··  ··  ··
 9-17 ··  ··  ··  ··  ··  ··  ··  ··  ··
18-26 ··  ··  EN  ··  FO  ··  SK  ··  ··
27-35 ··  ··  NV  ··  SC  ··  MF  ··  ··
36-44 ··  ··  BS  ··  BT  ··  DR  ··  ··
45-53 RE  ··  ··  ··  FE  ··  ··  ··  SO
```

`··` : vitre de remplissage.

| Slot | Code | Objet | Nom | Contenu | Clic |
| --- | --- | --- | --- | --- | --- |
| 4 | PI | pioche du joueur, modèle de son tier | Pioche en Rubis, par exemple | Tier, niveau, XP actuelle et XP du niveau suivant, vitesse finale en blocs/s, liste des enchantements et niveaux | Aucun |
| 20 | EN | `minecraft:enchanted_book` | Enchantements | Éclats disponibles, nombre de niveaux achetables | Clic : ouvre Enchantements |
| 22 | FO | `minecraft:anvil` | Forge | Prochaine pioche, conditions remplies 2 / 3 | Clic : ouvre Forge |
| 24 | SK | `minecraft:painting` | Skin de pioche | Skin actif, skins débloqués par les thèmes complets | Clic : ouvre Skins de pioche |
| 29 | NV | `minecraft:experience_bottle` | Niveau | Niveau, XP, multiplicateur d'XP du biome, XP par heure sur les 10 dernières minutes | Aucun |
| 31 | SC | `minecraft:heart_of_the_sea` | Sceaux | Sceaux de l'Overworld, du Nether et de l'End : obtenu ou non dans ce cycle, bonus total | Aucun |
| 33 | MF | `minecraft:knowledge_book` | Mémoire de forge | Pioches déjà forgées dans cette Renaissance, dont le minerai n'est plus requis | Aucun |
| 38 | BS | `minecraft:potion` | Boosters actifs | Liste des boosters et temps de minage actif restant | Aucun |
| 40 | BT | `minecraft:recovery_compass` | Bonus totaux | Argent, XP, Fortune, Chance, Éclats, Excavation : total, plafond et détail par source | Clic : ouvre le détail des bonus |
| 42 | DR | `minecraft:firework_rocket` | Départ rapide | Paliers débloqués par le rang de Prestige | Aucun |
| 45, 49, 53 | RE, FE, SO | Barre de navigation | Voir [Conventions](menus.md) | | |

## Enchantements

* Titre de l'inventaire : `STRATA · Enchantements`
* Taille : 54 emplacements, 6 lignes
* Ouverture : `/enchant`, menu Pioche
* Permission : `strata.player.enchant`
* Retour vers : Pioche
* Remplissage : Vitre grise, ligne 3 en vitres violettes `minecraft:purple_stained_glass_pane`

```
      0   1   2   3   4   5   6   7   8 
 0-8  ··  ··  ··  ··  PI  ··  ··  ··  ··
 9-17 ··  ··  ··  ··  ··  ··  ··  ··  ··
18-26 ··  EF  FT  AG  XP  EX  AU  PR  ··
27-35 ··  ··  ··  ··  ··  ··  ··  ··  ··
36-44 ··  ··  ··  ··  EC  ··  ··  ··  ··
45-53 RE  ··  ··  ··  FE  ··  ··  ··  SO
```

`··` : vitre de remplissage.

| Slot | Code | Objet | Nom | Contenu | Clic |
| --- | --- | --- | --- | --- | --- |
| 4 | PI | pioche du joueur | Pioche | Tier, plafonds d'enchantement de la pioche actuelle | Aucun |
| 19 | EF | `minecraft:sugar` | Efficacité | Niveau, plafond de la pioche, maximum absolu, vitesse actuelle et suivante, coût du niveau suivant | Gauche +1, droit +10, Maj + clic : maximum |
| 20 | FT | `minecraft:rabbit_foot` | Fortune | Idem, quantité x actuelle et suivante | Idem |
| 21 | AG | `minecraft:gold_ingot` | Argent | Idem, bonus d'Argent de l'enchantement | Idem |
| 22 | XP | `minecraft:experience_bottle` | XP | Idem, bonus d'XP de l'enchantement | Idem |
| 23 | EX | `minecraft:iron_shovel` | Excavation | Idem, chance de zone actuelle, plafond de 18 % | Idem |
| 24 | AU | `minecraft:crafting_table` | Autocraft | Idem, bonus de valeur des blocs compressés. Clic droit sans achat : active ou coupe la compression | Idem |
| 25 | PR | `minecraft:spyglass` | Prospection | Idem, bonus de Trouvaille | Idem |
| 40 | EC | `minecraft:prismarine_crystals` | Éclats | Solde d'Éclats, Éclats par heure sur les 10 dernières minutes | Aucun |
| 45, 49, 53 | RE, FE, SO | Barre de navigation | Voir [Conventions](menus.md) | | |

**Exemple de description, Efficacité avec une Pioche en Diamant**

```
Efficacité
Vitesse de minage

+0,2 bloc/s par niveau

Niveau : 6 / 20   Plafond de la Pioche en Diamant : 6
Vitesse : 1,8 + 1,2 = 3,0 blocs/s

✖ Plafond atteint. La Pioche en Citrine permet le niveau 7.
Coût du niveau 7 : 1 394 Éclats
```

**États d'un enchantement**

| État | Affichage |
| --- | --- |
| Non débloqué par le tier | `minecraft:gray_dye`, « ✖ Débloqué à T5, Pioche en Diamant » |
| Achetable | Brillance, « ● Disponible », coût en vert |
| Éclats insuffisants | Coût en rouge, « Il te manque 412 Éclats » |
| Plafond de la pioche atteint | « ✖ Plafond atteint », tier qui permet le niveau suivant |
| Maximum absolu | « ✔ Maximum » en or |

**Achat**

* Clic gauche : 1 niveau. Clic droit : 10 niveaux, ou moins si le plafond ou le solde l'impose. Maj + clic : autant de niveaux que possible.
* Chaque niveau acheté est débité et appliqué immédiatement. Le coût de chaque niveau suit la formule de [Enchantements](../enchantements/enchantements.md).
* Pas de confirmation : les Éclats sont remis à zéro au Prestige, une erreur coûte peu.

## Forge

* Titre de l'inventaire : `STRATA · Forge`
* Taille : 54 emplacements, 6 lignes
* Ouverture : `/forge`, menu Pioche, option Prochaine pioche des PNJ
* Permission : `strata.player.forge`
* Retour vers : Pioche
* Remplissage : Vitre grise `minecraft:gray_stained_glass_pane`, sans nom

```
      0   1   2   3   4   5   6   7   8 
 0-8  ··  ··  ··  ··  FG  ··  ··  ··  ··
 9-17 ··  ··  ··  ··  ··  ··  ··  ··  ··
18-26 ··  ··  AC  ··  FL  ··  PX  ··  ··
27-35 ··  ··  CP  ··  CM  ··  CN  ··  ··
36-44 ··  ··  ··  ··  BF  ··  LI  ··  ··
45-53 RE  ··  ··  ··  FE  ··  ··  ··  SO
```

`··` : vitre de remplissage.

| Slot | Code | Objet | Nom | Contenu | Clic |
| --- | --- | --- | --- | --- | --- |
| 4 | FG | `minecraft:anvil` | Forge | Rappel : prix, minerai au premier forgeage, niveau | Aucun |
| 20 | AC | pioche actuelle | Pioche actuelle | Tier, vitesse de base, plafonds | Aucun |
| 22 | FL | `minecraft:yellow_stained_glass_pane` | → |  | Aucun |
| 24 | PX | prochaine pioche, modèle de son tier | Prochaine pioche | Tier, vitesse de base, plafonds, biome débloqué, Sceau éventuel | Aucun |
| 29 | CP | `minecraft:gold_ingot` | Prix | Prix, x (1 + 0,20 x Renaissance) compris. ✔ ou ✖ et montant manquant | Aucun |
| 31 | CM | minerai requis | Minerai | Quantité requise et possédée, inventaire et `/pv` compris. Ou « ◆ Mémoire de forge : minerai non requis » | Aucun |
| 33 | CN | `minecraft:experience_bottle` | Niveau | Niveau requis et niveau actuel | Aucun |
| 40 | BF | `minecraft:lime_concrete` ou `minecraft:red_concrete` | Forger | Vert si les 3 conditions sont remplies, rouge sinon avec la condition manquante | Clic : forge |
| 42 | LI | `minecraft:book` | Liste des pioches | Les 17 pioches et leur état | Clic : ouvre Liste des pioches |
| 45, 49, 53 | RE, FE, SO | Barre de navigation | Voir [Conventions](menus.md) | | |

**Forge**

* Le clic sur Forger revérifie les 3 conditions, débite l'Argent, retire le minerai (minerais simples d'abord, puis blocs compressés, voir [Pioches](../pioches/pioches.md)), remplace la pioche du slot 1 et conserve les enchantements.
* Titre à l'écran « Pioche en Rubis », son `block.anvil.use`, message dans le chat : « Tu as forgé la Pioche en Rubis. La Vallée des âmes est ouverte. »
* Pioche de fin de dimension : le message annonce le Sceau et, si le rang de Prestige le permet, la dimension suivante. Sinon : « Porte de Prestige : passe Prestige IV pour ouvrir l'End. »
* Pas de confirmation : forger est toujours un progrès.
* Si la prochaine pioche n'est pas forgeable au rang actuel, l'objet 24 affiche « ✖ Biome non accessible avant le Prestige IV ».

## Liste des pioches

* Titre de l'inventaire : `STRATA · Liste des pioches`
* Taille : 54 emplacements, 6 lignes
* Ouverture : menu Forge
* Permission : `strata.player.forge`
* Retour vers : Forge
* Remplissage : Vitre grise `minecraft:gray_stained_glass_pane`, sans nom

```
      0   1   2   3   4   5   6   7   8 
 0-8  ··  ··  ··  ··  HD  ··  ··  ··  ··
 9-17 ··  T1  T1  T1  T1  T1  T1  T1  ··
18-26 ··  T8  T8  T8  T8  T8  T8  T8  ··
27-35 ··  TF  TF  TF  ··  ··  ··  ··  ··
36-44 ··  ··  ··  ··  ··  ··  ··  ··  ··
45-53 RE  ··  ··  ··  FE  ··  ··  ··  SO
```

`··` : vitre de remplissage.

| Slot | Code | Objet | Nom | Contenu | Clic |
| --- | --- | --- | --- | --- | --- |
| 4 | HD | `minecraft:book` | Les 17 pioches | Pioche actuelle, pioches forgées dans ce cycle | Aucun |
| 10 | T1 | modèle de la pioche | T1 à T7 | Une pioche par emplacement, slots 10 à 16 | Aucun |
| 19 | T8 | modèle de la pioche | T8 à T14 | Slots 19 à 25 | Aucun |
| 28 | TF | modèle de la pioche | T15 à T17 | Slots 28 à 30 | Aucun |
| 45, 49, 53 | RE, FE, SO | Barre de navigation | Voir [Conventions](menus.md) | | |

Les slots 11 à 16, 20 à 25, 29 et 30 suivent le même format que 10, 19 et 28. Chaque pioche affiche :

* son état : « ✔ Forgée dans ce cycle », « ◆ Mémoire de forge », « ● Prochaine », « ✖ Verrouillée » ;
* son prix, son minerai au premier forgeage, son niveau requis ;
* le biome qu'elle débloque et, pour T5, T9, T13 et T17, son Sceau ou sa porte de Prestige.

Une pioche jamais forgée dans aucune Renaissance apparaît avec le modèle `minecraft:wooden_pickaxe` et le nom « ??? » en gris. Son prix et ses conditions restent visibles.

## Bonus

* Titre de l'inventaire : `STRATA · Bonus`
* Taille : 54 emplacements, 6 lignes
* Ouverture : menu Pioche, objet Bonus totaux
* Permission : `strata.player.pioche`
* Retour vers : Pioche
* Remplissage : Vitre grise `minecraft:gray_stained_glass_pane`, sans nom

```
      0   1   2   3   4   5   6   7   8 
 0-8  ··  ··  ··  ··  HD  ··  ··  ··  ··
 9-17 ··  ··  ··  ··  ··  ··  ··  ··  ··
18-26 ··  BA  BX  BF  BC  BE  BZ  BM  ··
27-35 ··  ··  ··  ··  MU  ··  ··  ··  ··
36-44 ··  ··  ··  ··  ··  ··  ··  ··  ··
45-53 RE  ··  ··  ··  FE  ··  ··  ··  SO
```

`··` : vitre de remplissage.

| Slot | Code | Objet | Nom | Contenu | Clic |
| --- | --- | --- | --- | --- | --- |
| 4 | HD | `minecraft:recovery_compass` | Bonus totaux | Rappel de la formule : bonus additionnés par type, puis multiplicateurs de Prestige et de Renaissance | Aucun |
| 19 | BA | `minecraft:gold_ingot` | Argent | Total et plafond, puis détail : enchantement, pets, traits, armures, race, grade, collections, guilde, Sceaux, boosters | Aucun |
| 20 | BX | `minecraft:experience_bottle` | XP | Même détail | Aucun |
| 21 | BF | `minecraft:rabbit_foot` | Fortune | Même détail | Aucun |
| 22 | BC | `minecraft:spyglass` | Chance | Même détail | Aucun |
| 23 | BE | `minecraft:prismarine_crystals` | Éclats | Même détail | Aucun |
| 24 | BZ | `minecraft:iron_shovel` | Excavation | Chance de zone et plafond de 18 % | Aucun |
| 25 | BM | `minecraft:feather` | Mobilité | Vitesse de déplacement bonus, plafond de 35 % | Aucun |
| 31 | MU | `minecraft:nether_star` | Multiplicateurs | Prestige x1,6 par rang, Renaissance +0,5 par Renaissance, Phénix | Aucun |
| 45, 49, 53 | RE, FE, SO | Barre de navigation | Voir [Conventions](menus.md) | | |
