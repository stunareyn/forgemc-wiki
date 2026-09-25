---
description: Conventions communes à tous les menus : structure, navigation, couleurs, descriptions, clics, confirmation, sons et règles techniques.
---

# 🧩 Menus GUI · Conventions

## 🎯 Rôle

Tous les systèmes de progression du serveur sont accessibles par des menus d'inventaire. Chaque menu principal a une commande directe et un accès depuis le Menu principal. Seules les commandes sociales et utilitaires existent uniquement en commande : chat, messages, `/mail`, `/ignore`, téléportation entre joueurs, `/back`, `/trash`, `/sell main`.

## 🗂️ Liste des menus

| Menus | Commandes | Page |
| --- | --- | --- |
| Menu principal | `/menu`, objet Menu de la barre rapide | [menu-principal](menu-principal.md) |
| Pioche, Enchantements, Forge, Liste des pioches | `/pioche`, `/enchant`, `/forge` | [pioche](pioche.md) |
| Voyage, dimensions, relais, file d'attente | `/biomes`, `/relais` | [voyage](voyage.md) |
| Prestige, Renaissance | `/prestige`, `/renaissance` | [prestige-renaissance](prestige-renaissance.md) |
| Pets, fiche de pet, Éveil, Traits, Œufs | `/pets`, `/traits`, `/oeufs` | [pets](pets.md) |
| Armures, Garde-robe, Race, Sons | `/armure`, `/garderobe`, `/race`, `/sons` | [equipement](equipement.md) |
| Collections | `/collections` | [collections](collections.md) |
| Shop rotatif, Caisses, aperçu d'une caisse | `/shop`, `/caisses` | [shop-et-caisses](shop-et-caisses.md) |
| Guilde | `/guilde` | [guilde](guilde.md) |
| Événements, Boss, Votes | `/evenements`, `/boss`, `/vote`, `/voteparty` | [evenements](evenements.md) |
| Profil, Statistiques, Classements, Titres, Paramètres | `/profil`, `/stats`, `/top`, `/titre`, `/parametres` | [profil-parametres](profil-parametres.md) |

## 📐 Structure d'un menu de 54 emplacements

```
      0   1   2   3   4   5   6   7   8
 0-8  ··  ··  ··  ··  HD  ··  ··  ··  ··     ligne 1 : en-tête, slot 4
 9-17 ··  C   C   C   C   C   C   C   ··     lignes 2 à 5 : contenu
18-26 ··  C   C   C   C   C   C   C   ··
27-35 ··  C   C   C   C   C   C   C   ··
36-44 ··  C   C   C   C   C   C   C   ··
45-53 RE  ··  PP  ··  FE  ··  PS  ··  SO     ligne 6 : navigation
```

* **Slot 4** : objet d'en-tête, résumé du menu (profil, pioche, dimension, etc.).
* **Zone de contenu des listes** : 28 emplacements, slots 10 à 16, 19 à 25, 28 à 34, 37 à 43. Les listes plus longues sont paginées.
* **Colonnes 0 et 8** : vitres de remplissage.

## 🧭 Barre de navigation

| Slot | Code | Objet | Nom | Affichage | Clic |
| --- | --- | --- | --- | --- | --- |
| 45 | RE | `minecraft:arrow` | Retour | Quand le menu a été ouvert depuis un autre menu. Ouvert par sa commande, le slot reçoit une vitre | Revient au menu d'où le joueur vient |
| 47 | PP | `minecraft:arrow` | Page précédente | Seulement s'il existe une page précédente. Lore : « Page 2 / 4 » | Page précédente |
| 49 | FE | `minecraft:barrier` | Fermer | Toujours | Ferme le menu |
| 51 | PS | `minecraft:arrow` | Page suivante | Seulement s'il existe une page suivante | Page suivante |
| 53 | SO | `minecraft:sunflower` | Solde | Toujours. Lore : Argent, Éclats, Cristaux du joueur | Aucun |

Quand un bouton n'est pas affiché, son emplacement reçoit une vitre de remplissage.

## 🎨 Couleurs et remplissage

| Usage | Objet |
| --- | --- |
| Remplissage par défaut | `minecraft:gray_stained_glass_pane` |
| Menus de l'Overworld | `minecraft:lime_stained_glass_pane` |
| Menus du Nether | `minecraft:red_stained_glass_pane` |
| Menus de l'End | `minecraft:purple_stained_glass_pane` |
| Menus de l'Aether | `minecraft:light_blue_stained_glass_pane` |
| Menus de Prestige et de Renaissance | `minecraft:yellow_stained_glass_pane` |

* Nom d'un objet : couleur de sa rareté (voir [Raretés](../concept/raretes.md)), sinon blanc.
* Objet disponible ou action possible : **brillance d'enchantement** et ligne « ● Disponible » en vert.
* Objet verrouillé : pas de brillance, nom en gris, ligne « ✖ Verrouillé » en rouge suivie de la condition.
* Objet acquis : ligne « ✔ Obtenu » en vert.

## 📝 Format des descriptions

```
<Nom, couleur de rareté>
<Rareté ou catégorie, en gris>

<Description en une ou deux lignes, en gris>

<Valeurs : libellé gris, valeur blanche>

<État : ✔ Obtenu / ● Disponible / ✖ Verrouillé>
<Actions : « Clic gauche : ... », « Clic droit : ... », « Maj + clic : ... » en jaune>
```

* Nombres avec espace des milliers : 1 250 000. Au-delà du million : 1,25 M ; au-delà du milliard : 1,25 Md.
* Durées : 1 h 23, 12 min 05 s, 00:43:12 pour un compte à rebours.
* 12 lignes de description au maximum.

## 🖱️ Clics

| Clic | Usage |
| --- | --- |
| Clic gauche | Action principale : ouvrir, équiper, acheter 1 |
| Clic droit | Action secondaire : fiche, relais, acheter 10 |
| Maj + clic | Action en masse : acheter le maximum, ouvrir par 10 |
| Clic molette, touche Q, touches 1 à 9 | Ignorés |

## ✅ Confirmation

Actions qui demandent une confirmation : Prestige, Renaissance (deux fois), recyclage d'un pet, Éveil d'un pet, reroll de race, reroll de trait (voir ci-dessous), achat d'une pièce d'armure, achat au Shop à 100 Cristaux ou plus, quitter ou dissoudre une guilde, exclure un membre, transmettre le rôle de chef, dépôt dans la banque de guilde. Aucune confirmation pour les achats d'enchantements et la forge, qui sont toujours un progrès dans le cycle.

Délai de sécurité de 3 s sur le bouton Confirmer pour : Prestige, première confirmation de Renaissance, dissolution de guilde, recyclage d'un pet Légendaire ou Mythique. La seconde confirmation de Renaissance et de Nouveau départ a un délai de 5 s.

La confirmation des rerolls de trait peut être coupée dans `/parametres` pour un trait actuel inférieur à Épique ; elle reste obligatoire pour un trait Épique ou mieux.

### Menu de confirmation

* Titre de l'inventaire : `STRATA · Confirmation`
* Taille : 27 emplacements, 3 lignes
* Ouverture : toute action irréversible ou coûteuse
* Permission : aucune, héritée du menu d'origine
* Retour vers : menu d'origine
* Remplissage : Vitre grise

```
      0   1   2   3   4   5   6   7   8 
 0-8  ··  ··  ··  ··  RS  ··  ··  ··  ··
 9-17 ··  ··  CO  ··  DE  ··  AN  ··  ··
18-26 ··  ··  ··  ··  ··  ··  ··  ··  ··
```

`··` : vitre de remplissage.

| Slot | Code | Objet | Nom | Contenu | Clic |
| --- | --- | --- | --- | --- | --- |
| 4 | RS | selon l'action | Résumé de l'action | Nom de l'action et son objet, par exemple « Prestige III » | Aucun |
| 11 | CO | `minecraft:lime_concrete` | Confirmer | Rappel du coût. Pendant le délai de sécurité : `minecraft:gray_concrete`, nom « Patiente 3 s » | Clic : exécute l'action puis ferme ou revient |
| 13 | DE | `minecraft:paper` | Détail | Ce qui est dépensé, ce qui est perdu, ce qui est gagné | Aucun |
| 15 | AN | `minecraft:red_concrete` | Annuler |  | Clic : revient au menu d'origine sans rien faire |

## 🔊 Sons

| Événement | Son vanilla | Volume |
| --- | --- | --- |
| Ouverture, changement de page | `ui.button.click` | 0,3 |
| Action réussie | `entity.experience_orb.pickup` | 0,5 |
| Achat | `block.amethyst_block.chime` | 0,6 |
| Action impossible | `block.note_block.bass` | 0,5 |
| Forge d'une pioche | `block.anvil.use` | 0,4 |
| Prestige, Renaissance | `ui.toast.challenge_complete` | 0,6 |

## 🛠️ Règles techniques

{% hint style="warning" %}
* Tous les menus sont des inventaires virtuels avec un propriétaire dédié. **Tous les clics sont annulés** ; aucun objet ne peut être pris, déposé ou déplacé. Exceptions : les pages `/pv`, qui sont de vrais coffres, et la poubelle `/trash`, dont le contenu est détruit à la fermeture.
* Un clic est ignoré s'il arrive moins de 150 ms après le précédent, pour éviter les doubles achats.
* Chaque action est revérifiée côté serveur au moment du clic : prix, conditions, solde. L'affichage peut être en retard d'une seconde, la vérification jamais.
* Aucune lecture de base de données dans le fil principal. Les données du joueur sont en cache ; un menu s'ouvre en moins de 5 ms.
* Menus dynamiques (boss, comptes à rebours, file d'attente) : mise à jour de la description des objets concernés une fois par seconde, jamais de réouverture.
* Un menu ouvert est fermé automatiquement lors d'un Prestige, d'une Renaissance, d'une téléportation ou d'un changement de serveur.
* Textes stockés dans des fichiers de langue `fr_FR`, un fichier par menu, modifiables sans recompiler.
{% endhint %}
