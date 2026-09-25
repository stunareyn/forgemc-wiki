---
description: Le Shop rotatif, sa rotation, ses emplacements, ses prix et ses limites.
---

# 🛒 Shop rotatif

## 🎯 Objectif

Donner une raison de revenir plusieurs fois par jour sans rendre la visite obligatoire. Le Shop propose des accélérateurs payés en Argent du cycle et des objets permanents payés en Cristaux. Rien n'y est indispensable.

## ⚙️ Fonctionnement

* Rotation **globale** : tous les joueurs voient les mêmes offres.
* Rotation toutes les 6 heures : 00 h, 06 h, 12 h, 18 h, heure de Paris.
* 6 emplacements.
* Chaque offre s'achète **une fois par joueur et par rotation**.
* Commande : `/shop`. Un message annonce la rotation dans le chat global.
* Menu : voir [Menus GUI · Shop et caisses](../menus/shop-et-caisses.md).

## 📦 Emplacements

| Emplacement | Monnaie | Contenu |
| --- | --- | --- |
| 1 et 2 | Argent | Boosters |
| 3 et 4 | Cristaux | Collection |
| 5 | Cristaux | Rare |
| 6 | Cristaux | Vedette, 10 % des rotations ; sinon une offre Collection de plus |

## ⚡ Boosters, payés en Argent

| Offre | Effet |
| --- | --- |
| Booster XP | +25 % XP de pioche, 30 min de minage actif |
| Booster Éclats | +25 % Éclats, 30 min de minage actif |
| Booster Trouvailles | +50 % Chance, 30 min de minage actif |

**Prix** : 10 minutes du revenu d'Argent moyen du joueur, mesuré sur ses 60 dernières minutes de minage actif. Minimum 1 000 $.

Le prix suit donc le joueur quel que soit son biome, son rang de Prestige ou sa Renaissance. Un prix fixé sur la pioche serait trop cher en début de cycle et presque gratuit en fin de cycle, à cause du multiplicateur de Prestige.

Exemple, joueur moyen au premier passage dans les Badlands : 302 000 $/h, soit 302 000 x 10 / 60 = 50 333 $ le booster.

Il n'existe pas de booster d'Argent en vente : il serait rentable par construction et rendrait le Shop obligatoire. Le Booster XP est utile au joueur limité par son niveau, le Booster Éclats au joueur limité par ses enchantements. C'est une conversion d'Argent, pas un gain net.

Deux boosters du même type ne se cumulent pas : le second prolonge la durée. La durée ne s'écoule qu'en minage actif.

## 💎 Offres Collection, payées en Cristaux

| Offre | Prix |
| --- | --- |
| Clé Pets F2W | 60 |
| Clé Armure Themes | 40 |
| Œuf d'une dimension débloquée, au choix | 45 |
| Pièce de thème Commun ou Peu commun, au choix dans le thème proposé | 35 |
| Pièce de thème Rare, au choix dans le thème proposé | 70 |
| Essence Rare | 25 |
| Essence Épique | 80 |

## 🔷 Offres Rares, payées en Cristaux

| Offre | Prix |
| --- | --- |
| Essence Légendaire | 300 |
| Pièce de thème Épique, au choix dans le thème proposé | 150 |
| Son de minage Forge | 150 |
| Son de minage Cloche | 250 |

## 🌟 Offres Vedettes, payées en Cristaux

| Offre | Prix |
| --- | --- |
| Son de minage Verre | 400 |
| Pièce de thème Légendaire, au choix dans le thème proposé | 500 |
| Essence Mythique | 1 200 |
| Lot de 5 clés Pets F2W | 270 |

L'emplacement Vedette apparaît dans 10 % des rotations. Avec 4 rotations par jour, il apparaît en moyenne 0,4 fois par jour. Chaque offre Vedette y a une chance sur quatre : une offre précise revient en moyenne tous les 1 / (0,4 x 0,25) = 10 jours.

## 🔒 Limites

{% hint style="warning" %}
* Aucune offre ne vend de minerai, d'Argent, d'Éclats, de niveau, de pioche, de pet ou de race.
* Aucune offre n'est vendue contre de l'argent réel.
* Le talent Marchand du Gobelin réduit de 10 % les prix en Argent uniquement.
{% endhint %}
