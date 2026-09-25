---
description: Le Chat réaction, ses 6 types de défis, sa fréquence, ses récompenses et ses règles anti-abus.
---

# ⚡ Chat réaction

## 🎯 Objectif

Un défi court lancé dans le chat global. Le **premier** joueur qui réussit gagne. Il anime le chat entre deux boss et récompense la réactivité, pas la progression.

## ⚙️ Fonctionnement

* Fréquence : un défi toutes les 15 à 25 minutes, intervalle tiré au hasard.
* Minimum 10 joueurs connectés sur le réseau, sinon le défi est reporté.
* Pas de défi pendant les 60 secondes qui précèdent l'apparition d'un boss, ni pendant un Concours de minage.
* Annonce dans le chat global, avec un son discret : `block.note_block.pling`, volume 0,3.
* Le premier joueur qui réussit est annoncé : « Lyra a gagné en 2,84 s ! »
* Délai pour répondre : 30 s pour les défis de chat, 3 min pour les défis de minage. Sans gagnant, le défi se termine sans récompense.

## 🎲 Les 6 types de défis

| Type | Probabilité | Exemple | Bonne réponse |
| --- | --- | --- | --- |
| Écrire | 25 % | « Premier à écrire : Spodumène » | Spodumène |
| Mot mélangé | 20 % | « Remets dans l'ordre : TNAMIDA » | Diamant |
| Calcul | 20 % | « Combien font 17 x 4 + 9 ? » | 77 |
| Quiz STRATA | 15 % | « Quel minerai faut-il pour forger la Pioche en Rubis ? » | Rubis |
| Minage éclair | 10 % | « Premier à casser 150 blocs » | Action |
| Chasse au minerai | 10 % | « Premier à casser un minerai Épique ou mieux » | Action |

**Listes de mots** : noms des 35 minerais, des 16 biomes, des 17 pioches, des 22 pets et des 8 races. Les accents sont ignorés pour la réponse : « spodumene » est accepté.

**Calculs** : deux opérations, nombres de 2 à 99, résultat entier positif.

**Quiz STRATA** : 60 questions au lancement, écrites par l'équipe, dont la réponse est un seul mot ou un nombre. Exemples : minerai d'une pioche, dimension d'un biome, rareté d'un pet, nombre de rangs de Prestige.

**Minage éclair** : seuls les blocs cassés directement comptent, pas ceux de l'Excavation. Le compteur démarre à l'annonce.

**Chasse au minerai** : n'importe quel minerai Épique ou mieux, dans n'importe quelle dimension. Un joueur de l'Overworld peut gagner avec un minerai d'Or.

## 🎁 Récompenses

| Défi | Récompense du gagnant |
| --- | --- |
| Défis de chat | 5 Cristaux |
| Minage éclair, Chasse au minerai | 5 Cristaux et un Booster Éclats +25 % de 10 min |

## 🔒 Règles anti-abus

{% hint style="warning" %}
* Une réponse de chat arrivée moins de 1,0 s après l'annonce est ignorée.
* Pendant un défi de chat, un message qui contient la bonne réponse est masqué pour les autres joueurs : on ne peut pas copier la réponse d'un autre.
* Un joueur gagne au maximum **3 défis par heure et 15 par jour**. Au-delà, ses réponses sont ignorées et le défi continue pour les autres.
* Les réponses envoyées par `/msg` ou dans le chat de guilde ne comptent pas.
{% endhint %}

## 🧮 Poids dans la progression

Environ 3 défis par heure. Avec 100 joueurs qui répondent, un joueur moyen en gagne environ 1 % : 3 x 0,01 x 412 h = 12 victoires, soit 60 Cristaux 🟠 jusqu'à la première Renaissance. Le Chat réaction est une animation, pas une source de progression.

## ⌨️ Commandes

* `/evenements` : prochains événements et historique des 10 derniers gagnants.
* Staff : `/strata event reaction [type]` lance un défi immédiatement.
