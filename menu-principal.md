---
description: Le Menu principal, porte d'entrée de tous les menus, et l'objet Menu de la barre rapide.
---

# 🏠 Menu principal

## 🗺️ Disposition

* Titre de l'inventaire : `STRATA · Menu`
* Taille : 54 emplacements, 6 lignes
* Ouverture : `/menu`, ou clic droit sur l'objet Menu STRATA
* Permission : `strata.player.menu`
* Remplissage : Vitre grise `minecraft:gray_stained_glass_pane`, sans nom

```
      0   1   2   3   4   5   6   7   8 
 0-8  ··  ··  ··  ··  PR  ··  ··  ··  ··
 9-17 ··  PI  EN  FO  VO  PG  RN  VE  ··
18-26 ··  PE  OE  AR  GR  RA  SN  CO  ··
27-35 ··  PV  SH  CA  GU  EV  BO  VT  ··
36-44 ··  ST  TO  TI  PA  AI  BQ  DI  ··
45-53 ··  ··  ··  ··  FE  ··  ··  ··  SO
```

`··` : vitre de remplissage.

| Slot | Code | Objet | Nom | Contenu | Clic |
| --- | --- | --- | --- | --- | --- |
| 4 | PR | `minecraft:player_head` | Profil | Tête du joueur. Grade, race, Renaissance, Prestige, tier et niveau de pioche, guilde | Clic : ouvre le Profil |
| 10 | PI | pioche du joueur | Pioche | Tier, niveau, barre d'XP en texte, vitesse | Clic : ouvre `/pioche` |
| 11 | EN | `minecraft:enchanted_book` | Enchantements | Éclats disponibles. « ● Disponible » si un niveau est achetable | Clic : ouvre `/enchant` |
| 12 | FO | `minecraft:anvil` | Forge | Prochaine pioche et conditions remplies, par exemple 2 / 3 | Clic : ouvre `/forge` |
| 13 | VO | `minecraft:compass` | Voyage | Biome actuel, biomes débloqués | Clic : ouvre `/biomes` |
| 14 | PG | `minecraft:beacon` | Prestige | Rang actuel, multiplicateur, conditions du rang suivant | Clic : ouvre `/prestige` |
| 15 | RN | `minecraft:totem_of_undying` | Renaissance | Renaissance actuelle, conditions de la suivante | Clic : ouvre `/renaissance` |
| 16 | VE | `minecraft:gold_ingot` | Vendre | Valeur de l'inventaire vendable, minerais protégés exclus | Clic : vend, comme `/sell` |
| 19 | PE | `minecraft:lead` | Pets | Pets actifs, emplacements utilisés | Clic : ouvre `/pets` |
| 20 | OE | `minecraft:sniffer_egg` | Œufs | Œufs en incubation et progression | Clic : ouvre `/oeufs` |
| 21 | AR | `minecraft:iron_chestplate` | Armures | Armures complètes, bonus totaux | Clic : ouvre `/armure` |
| 22 | GR | `minecraft:leather_chestplate` | Garde-robe | Thèmes complets, pièces possédées | Clic : ouvre `/garderobe` |
| 23 | RA | `minecraft:armor_stand` | Race | Race actuelle et bonus | Clic : ouvre `/race` |
| 24 | SN | `minecraft:note_block` | Sons | Son actif, sons possédés 5 / 12 | Clic : ouvre `/sons` |
| 25 | CO | `minecraft:bookshelf` | Collections | Progression totale en % | Clic : ouvre `/collections` |
| 28 | PV | `minecraft:ender_chest` | Coffres | Pages `/pv` disponibles | Clic gauche : page 1. Clic droit : ouvre Choix de la page |
| 29 | SH | `minecraft:emerald` | Shop rotatif | Temps avant la prochaine rotation | Clic : ouvre `/shop` |
| 30 | CA | `minecraft:tripwire_hook` | Caisses | Nombre de clés par caisse | Clic : ouvre `/caisses` |
| 31 | GU | `minecraft:white_banner` | Guilde | Nom, niveau, bonus. Bannière de la guilde si elle en a une | Clic : ouvre `/guilde` |
| 32 | EV | `minecraft:clock` | Événements | Prochain événement et compte à rebours | Clic : ouvre `/evenements` |
| 33 | BO | `minecraft:wither_skeleton_skull` | Boss | Prochain boss de la dimension actuelle, ou combat en cours | Clic : ouvre `/boss` |
| 34 | VT | `minecraft:paper` | Vote | Sites disponibles, Vote Party en cours, par exemple 214 / 300 | Clic : ouvre `/vote` |
| 37 | ST | `minecraft:writable_book` | Statistiques | Blocs cassés, temps de jeu | Clic : ouvre `/stats` |
| 38 | TO | `minecraft:gold_block` | Classements | Ta place au classement de progression | Clic : ouvre `/top` |
| 39 | TI | `minecraft:name_tag` | Titres | Titre actif, titres possédés | Clic : ouvre `/titre` |
| 40 | PA | `minecraft:comparator` | Paramètres |  | Clic : ouvre `/parametres` |
| 41 | AI | `minecraft:book` | Aide | Guide des commandes et de la progression | Clic : ouvre Aide |
| 42 | BQ | `minecraft:gold_nugget` | Boutique | Lien de la boutique en ligne | Clic : envoie le lien dans le chat |
| 43 | DI | `minecraft:bell` | Discord | Lien du Discord | Clic : envoie le lien dans le chat |
| 49, 53 | FE, SO | Barre de navigation | Voir [Conventions](menus.md) | | |

**Règles**

* L'objet **Menu STRATA** (`minecraft:nether_star`) est placé dans le slot 9 de la barre rapide. Il ne peut être ni jeté ni déplacé. Il peut être retiré dans `/parametres` ; `/menu` reste disponible.
* La pioche occupe le slot 1 de la barre rapide, verrouillée. Maj + clic droit avec la pioche ouvre `/pioche`.
* Les objets qui signalent une action possible brillent : Prestige possible, niveau d'enchantement achetable, clé disponible, vote disponible, pet prêt à l'Éveil.

## Choix de la page

* Titre de l'inventaire : `STRATA · Choix de la page`
* Taille : 27 emplacements, 3 lignes
* Ouverture : clic droit sur Coffres, ou `/pv` suivi d'un numéro indisponible
* Permission : `strata.player.pv`
* Retour vers : Menu principal
* Remplissage : Vitre grise

```
      0   1   2   3   4   5   6   7   8 
 0-8  ··  ··  ··  ··  ··  ··  ··  ··  ··
 9-17 P1  P1  P1  P1  P1  P1  P1  P1  P1
18-26 RE  ··  ··  ··  FE  ··  ··  ··  ··
```

`··` : vitre de remplissage.

| Slot | Code | Objet | Nom | Contenu | Clic |
| --- | --- | --- | --- | --- | --- |
| 9 | P1 | `minecraft:chest` | Page 1 | Nombre d'emplacements occupés 31 / 54. La quantité de l'objet affiche le numéro de page | Clic : ouvre la page |
| 18 | RE | `minecraft:arrow` | Retour |  | Clic : Menu principal |
| 22 | FE | `minecraft:barrier` | Fermer |  | Clic : ferme le menu |

Slots 9 à 17 : pages 1 à 9. Une page non débloquée est un `minecraft:iron_bars` avec sa condition : « Page 5 · Grade Légende » ou « Page supplémentaire · Renaissance 1 ». Une page Immortal au-delà de 8 n'existe qu'avec la Renaissance 1 : 9 pages au maximum.

## Aide

* Titre de l'inventaire : `STRATA · Aide`
* Taille : 54 emplacements, 6 lignes
* Ouverture : `/aide`, Menu principal
* Permission : `strata.player.aide`
* Retour vers : Menu principal
* Remplissage : Vitre grise `minecraft:gray_stained_glass_pane`, sans nom

```
      0   1   2   3   4   5   6   7   8 
 0-8  ··  ··  ··  ··  HD  ··  ··  ··  ··
 9-17 ··  ··  ··  ··  ··  ··  ··  ··  ··
18-26 ··  A1  A2  A3  A4  A5  A6  A7  ··
27-35 ··  ··  ··  ··  RG  ··  ··  ··  ··
36-44 ··  ··  ··  ··  TU  ··  ··  ··  ··
45-53 RE  ··  ··  ··  FE  ··  ··  ··  SO
```

`··` : vitre de remplissage.

| Slot | Code | Objet | Nom | Contenu | Clic |
| --- | --- | --- | --- | --- | --- |
| 4 | HD | `minecraft:book` | Aide | Rappel de la boucle : miner, vendre, enchanter, forger, Prestige, Renaissance | Aucun |
| 19 | A1 | `minecraft:diamond_pickaxe` | Pioche et enchantements |  | Clic : résumé dans le chat |
| 20 | A2 | `minecraft:beacon` | Prestige |  | Idem |
| 21 | A3 | `minecraft:totem_of_undying` | Renaissance |  | Idem |
| 22 | A4 | `minecraft:lead` | Pets, traits, Œufs |  | Idem |
| 23 | A5 | `minecraft:wither_skeleton_skull` | Boss et événements |  | Idem |
| 24 | A6 | `minecraft:white_banner` | Guildes |  | Idem |
| 25 | A7 | `minecraft:oak_sign` | Commandes | Liste des commandes utiles | Idem |
| 31 | RG | `minecraft:writable_book` | Règlement |  | Clic : règlement dans le chat, comme `/regles` |
| 40 | TU | `minecraft:compass` | Tutoriel | Étape en cours du tutoriel de Bram | Clic : affiche l'étape |
| 45, 49, 53 | RE, FE, SO | Barre de navigation | Voir [Conventions](menus.md) | | |

Chaque résumé tient en 5 lignes de chat au plus, avec les commandes cliquables. `/aide <sujet>` affiche le même texte : `pioche`, `prestige`, `renaissance`, `pets`, `boss`, `guilde`, `commandes`.
