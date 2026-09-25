---
description: Les guildes, leurs rôles, niveaux, bonus, banque de Cristaux, défis hebdomadaires, classements et commandes.
---

# 🛡️ Guildes

## 🎯 Objectif

La guilde est le groupe permanent du joueur. Elle donne un petit bonus d'Argent, des objectifs communs chaque semaine et un classement entre groupes. Elle ne permet **aucun échange** d'objets ou de monnaie entre joueurs.

## ⚙️ Règles générales

* Une seule guilde par joueur.
* Création : `/guilde creer <nom> <tag>`, 50 Cristaux payés par le créateur.
* Nom : 3 à 16 caractères, lettres, chiffres et espaces. Tag : 2 à 4 caractères, majuscules et chiffres. Nom et tag uniques.
* Tags réservés : STAFF, ADMIN, MODO, MOD, STRATA, et tout tag refusé par le filtre de langage.
* Le tag s'affiche devant le pseudo dans le chat et dans la liste des joueurs : `[MINE] Lyra`.
* La guilde est conservée au Prestige et à la Renaissance.
* Quitter une guilde : 24 h d'attente avant d'en rejoindre ou d'en créer une autre.

## 👥 Rôles

| Action | Chef | Officier | Membre |
| --- | --- | --- | --- |
| Inviter un joueur | Oui | Oui | Non |
| Exclure un membre | Oui | Oui, sauf un officier | Non |
| Promouvoir ou rétrograder | Oui | Non | Non |
| Dépenser la banque | Oui | Oui | Non |
| Activer la Ferveur | Oui | Oui | Non |
| Déposer des Cristaux | Oui | Oui | Oui |
| Renommer, changer le tag, dissoudre | Oui | Non | Non |
| Transmettre le rôle de chef | Oui | Non | Non |

* 1 chef, 5 officiers au maximum.
* Chef inactif depuis 30 jours : le rôle passe automatiquement à l'officier le plus ancien, sinon au membre le plus ancien.

## 📈 Niveaux

L'XP de guilde est égale au nombre de blocs cassés par ses membres, Excavation comprise.

| Niveau | XP totale requise | XP de ce niveau | Membres au maximum | Bonus d'Argent des membres |
| --- | --- | --- | --- | --- |
| 1 | 0 | · | 10 | +1 % |
| 2 | 10 000 000 | 10 000 000 | 12 | +2 % |
| 3 | 20 000 000 | 10 000 000 | 14 | +3 % |
| 4 | 30 000 000 | 10 000 000 | 16 | +4 % |
| 5 | 40 000 000 | 10 000 000 | 18 | +5 % |
| 6 | 50 000 000 | 10 000 000 | 20 | +6 % |
| 7 | 70 000 000 | 20 000 000 | 22 | +7 % |
| 8 | 90 000 000 | 20 000 000 | 24 | +8 % |
| 9 | 110 000 000 | 20 000 000 | 26 | +9 % |
| 10 | 130 000 000 | 20 000 000 | 28 | +10 % |

**Déblocages** :

* Niveau 3 : Ferveur
* Niveau 5 : troisième défi hebdomadaire, Salle agrandie II
* Niveau 7 : couleur du tag achetable
* Niveau 10 : tag encadré d'étoiles dans le chat, `[★MINE★]`

**À chaque niveau atteint** : 20 Cristaux pour chaque membre actif dans les 7 derniers jours.

**Calibrage** 🟠 : une guilde de joueurs moyens, 3 h de jeu par jour chacun, environ 16 000 blocs par heure et par joueur (6,6 millions de blocs en 412 h). Elle démarre à 10 membres, achète la Salle agrandie I au 7e jour, puis se remplit jusqu'à 20 membres dès que son plafond le permet. Elle réussit 2 défis sur 3.

```
XP par jour à 10 membres  = 10 x 3 x 16 000 = 480 000
XP par jour à 20 membres  = 20 x 3 x 16 000 = 960 000
XP des défis par jour     = défis par semaine x 2/3 x 500 000 / 7
                            = 95 238 avant le niveau 5, 142 857 ensuite

Résultat de la simulation au pas de 0,01 jour :
Niveau 2  : jour 13,9,  soit 42 h de jeu par membre
Niveau 6  : jour 52,4,  soit 157 h
Niveau 10 : jour 124,9, soit 375 h
```

La simulation de progression utilise un bonus de guilde de +2 % à 30 h, +6 % à 150 h et +10 % à 400 h de jeu : l'écart est de 12 h au niveau 2, 7 h au niveau 6 et 25 h d'avance au niveau 10. Écart accepté, à vérifier en test.

## 🏦 Banque de Cristaux

* Tout membre peut déposer des Cristaux : `/guilde deposer <montant>`.
* Un dépôt est **définitif** : personne ne peut retirer de Cristaux de la banque, pas même le chef.
* Pour limiter les comptes secondaires : dépôt possible à partir de 10 h de minage actif sur le compte, et 300 Cristaux par membre et par semaine au maximum.
* Journal des dépôts et des dépenses visible par tous les membres.
* Dissolution de la guilde : la banque est perdue.

| Amélioration | Coût, banque | Condition | Effet |
| --- | --- | --- | --- |
| Salle agrandie I | 400 | Niveau 1 | +6 membres au maximum |
| Salle agrandie II | 800 | Niveau 5 et Salle agrandie I | +6 membres au maximum |
| Ferveur | 200 par activation | Niveau 3 | +10 % Argent pendant 1 h de minage actif pour tous les membres connectés. Une fois par 24 h |
| Couleur du tag | 100 | Niveau 7 | 16 couleurs au choix |
| Renommer la guilde | 150 | Aucune | Nouveau nom, tag inchangé |
| Changer le tag | 150 | Aucune | Nouveau tag |

Membres au maximum : 28 au niveau 10, **40** avec les deux Salles agrandies.

Le chef d'une guilde qui a le grade Monarque ou Immortal choisit la couleur du tag sans payer, dès le niveau 1.

## 🎯 Défis hebdomadaires

* Chaque lundi à 04 h 00, 2 défis sont tirés, 3 à partir du niveau 5.
* Objectif = valeur par membre x nombre de membres au lundi 04 h 00.

| Défi | Valeur par membre |
| --- | --- |
| Casser des blocs | 100 000 blocs |
| Casser des minerais Épiques ou mieux | 250 minerais |
| Infliger des dégâts aux boss | 1 500 dégâts |
| Passer des Prestiges | 0,25 Prestige, arrondi au supérieur |
| Faire éclore des Œufs | 1 Œuf |
| Participer à des Concours de minage | 1 participation valide |

**Récompense par défi réussi** :

* 12 Cristaux pour chaque membre qui a contribué à au moins 2 % de l'objectif, ou à au moins une unité pour les défis de Prestige, d'Œufs et de Concours
* 500 000 XP de guilde

Un joueur moyen joue environ 21 h par semaine et casse environ 336 000 blocs : l'objectif de blocs représente 30 % de son activité, pour qu'une guilde avec des membres peu actifs puisse encore le réussir.

## 🏆 Classement hebdomadaire

Critère : XP de guilde gagnée pendant la semaine, du lundi 04 h 00 au lundi suivant 04 h 00.

| Place | Récompense pour chaque membre éligible |
| --- | --- |
| 1re | 40 Cristaux et 1 clé Pets F2W |
| 2e | 30 Cristaux et 1 clé Pets F2W |
| 3e | 20 Cristaux et 1 clé Pets F2W |
| 4e à 10e | 10 Cristaux |

**Membre éligible** : membre depuis le début de la semaine, avec au moins 3 h de minage actif dans la semaine.

Autres classements, affichés sans récompense : niveau et XP totale, dégâts de boss de la semaine, Prestiges de la semaine.

## 🧮 Cristaux attendus

Joueur moyen, 137 jours, soit 19,6 semaines, dans une guilde moyenne 🟠 :

| Source | Calcul | Cristaux |
| --- | --- | --- |
| Défis | 6,2 semaines à 2 défis, jusqu'au niveau 5 au jour 43,3, puis 13,4 semaines à 3 défis : 52,6 défis x 2/3 de réussite x 12 | 421 |
| Classement | environ 5 par semaine en moyenne x 19,6 | 98 |
| Niveaux | 9 niveaux x 20 | 180 |
| **Total** | | **699, environ 700** |

## 💬 Chat de guilde

* `/gc <message>` : message à la guilde.
* `/gc` seul : bascule le chat par défaut entre global et guilde.
* Format : `[Guilde] [Officier] Lyra : message`.

## ⌨️ Commandes

| Commande | Rôle | Effet |
| --- | --- | --- |
| `/guilde` | Tous | Menu de la guilde, voir [Menus GUI · Guilde](../menus/guilde.md) |
| `/guilde creer <nom> <tag>` | Sans guilde | Crée une guilde, 50 Cristaux |
| `/guilde inviter <joueur>` | Officier | Invitation valable 5 min |
| `/guilde accepter <guilde>` | Invité | Rejoint la guilde |
| `/guilde refuser <guilde>` | Invité | Refuse l'invitation |
| `/guilde quitter` | Membre | Quitte la guilde, confirmation demandée |
| `/guilde exclure <joueur>` | Officier | Exclut un membre |
| `/guilde promouvoir <joueur>` | Chef | Membre vers officier |
| `/guilde retrograder <joueur>` | Chef | Officier vers membre |
| `/guilde chef <joueur>` | Chef | Transmet le rôle de chef, confirmation demandée |
| `/guilde deposer <montant>` | Membre | Dépose des Cristaux dans la banque |
| `/guilde ferveur` | Officier | Active la Ferveur |
| `/guilde info [guilde]` | Tous | Fiche d'une guilde |
| `/guilde membres` | Membre | Liste des membres, rôles, dernière connexion |
| `/guilde defis` | Membre | Défis de la semaine et contributions |
| `/guilde top` | Tous | Classements |
| `/guilde renommer <nom>` | Chef | 150 Cristaux de la banque |
| `/guilde tag <tag>` | Chef | 150 Cristaux de la banque |
| `/guilde dissoudre` | Chef | Dissout la guilde, double confirmation |
| `/gc [message]` | Membre | Chat de guilde |

## 🔒 Limites

{% hint style="warning" %}
* Aucun coffre de guilde, aucun transfert d'objet, de minerai ou d'Argent.
* La banque ne reçoit que des Cristaux, et ne rend jamais rien.
* Le bonus de guilde est plafonné à +10 % Argent, dans le plafond global d'Argent. Voir [Formules](../game-design/formules.md).
{% endhint %}
