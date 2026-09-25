---
description: Les votes, la Vote Party, son seuil, ses récompenses et ses règles.
---

# 🗳️ Votes et Vote Party

## 🗳️ Votes

* 3 sites de vote, 1 vote par site toutes les 24 h.
* Chaque vote donne **1 Clé Vote** au joueur, même s'il est hors ligne : la clé l'attend dans `/caisses`.
* `/vote` ouvre le menu des sites avec, pour chacun, le temps restant avant le prochain vote.
* Rappel dans le chat à la connexion si au moins un site est disponible. Désactivable dans `/parametres`.
* Contenu de la caisse : voir [Caisses](../caisses/caisses.md).

## 🎉 Vote Party

Chaque vote, de n'importe quel joueur, fait avancer un **compteur commun** au serveur.

* Seuil : **300 votes** 🟠.
* Progression visible dans `/voteparty`, sur l'hologramme du spawn et dans le chat à 50 %, 80 % et 95 %.
* Au seuil : compte à rebours de 10 s dans le chat global, puis distribution.
* Le compteur repart à 0 après chaque Vote Party. Les votes en trop sont reportés.

## 🎁 Récompenses

| Récompense | Qui |
| --- | --- |
| 1 Clé Vote | Chaque joueur connecté, actif dans les 10 dernières minutes |
| Booster global +10 % Argent, 30 min | Tous les joueurs connectés du réseau |
| Feu d'artifice et son `entity.firework_rocket.large_blast`, volume 0,4 | Spawn et hubs des biomes |

* Un joueur doit être actif pour la clé : un joueur inactif depuis plus de 10 minutes ne reçoit rien.
* Les seuls boosters d'Argent du serveur sont celui de la Vote Party, celui des boss et la Ferveur de guilde. Aucun ne s'achète.
* Deux Vote Party rapprochées prolongent le booster au lieu de le cumuler.

## 🧮 Fréquence

```
Vote Party par jour = votants par jour x 3 / 300
```

| Votants distincts par jour | Votes par jour | Vote Party par jour |
| --- | --- | --- |
| 200 | 600 | 2 |
| 500 | 1 500 | 5 |
| 1 000 | 3 000 | 10 |

Si la moyenne dépasse 6 Vote Party par jour sur 7 jours glissants, le seuil passe à 500 votes 🟠 : le booster doit rester un moment fort, pas un état permanent.

## 🔒 Règles

{% hint style="warning" %}
* Un vote n'est compté qu'après confirmation du site, par le plugin de vote (NuVotifier).
* 3 comptes au maximum par adresse IP, par site et par 24 h, pour les foyers qui partagent une connexion. Au-delà, les votes ne donnent ni clé ni avancée du compteur.
* Le staff peut lancer une Vote Party manuelle avec `/strata event voteparty`, pour un événement communautaire annoncé.
{% endhint %}
