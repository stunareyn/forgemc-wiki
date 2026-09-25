---
description: Dimensions d'une mine, couches, hub, relais, régénération et règles de génération.
---

# 🧱 Structure des mines

Chaque biome est un monde de minage public, identique dans sa structure pour les 16 biomes.

## 📐 Dimensions

* Surface : 20 000 x 20 000 blocs, bordure de monde à ±10 000 du centre
* Hauteur minable : 300 blocs, bedrock incassable dessous
* Couche : tranche de 10 blocs de haut, 30 couches par mine

## 🪜 Couches

| Couche | Hauteur relative | Contenu |
| --- | --- | --- |
| Couche 1 | 291 à 300, surface | Bloc principal uniquement |
| Couches 2 à 30 | 1 à 290 | Bloc principal et minerais, taux fixes du biome |
| Fond | 0 | Bedrock |

{% hint style="danger" %}
* Aucun minerai dans la couche 1.
* Taux **identiques** de la couche 2 à la couche 30.
* Aucun minerai réservé à une profondeur.
{% endhint %}

## 🏛️ Hub et relais

**Hub central**

* Centre du monde, en surface
* Point d'arrivée, panneau des taux et du minerai favori, point de vente, décor du biome vanilla
* 60 x 60 blocs maximum, hors zone minable

**Quatre relais**

* À 1 000 blocs du hub, un par point cardinal
* Accès : `/relais` ou plaques du hub
* Petit point de vente, retour au hub

Les taux étant identiques partout, les joueurs n'ont aucune raison de s'éloigner à plus de quelques centaines de blocs d'un relais. L'activité reste concentrée, ce qui protège les performances décrites dans le document « STRATA Architecture technique v1 ».

## 🌿 Décor vanilla

Le biome vanilla donne son nom, sa musique, sa couleur de ciel, d'herbe et d'eau, son brouillard et ses particules d'ambiance. Le builder habille le hub et les relais avec les blocs typiques du biome : herbe et fleurs pour les Plaines, spéléothèmes pour les Cavernes, terre cuite pour les Badlands, champignons carmin pour la Forêt carmin, cerisiers pour le Bosquet de cerisiers, etc. La zone minable elle-même ne contient que le bloc principal et les minerais.

## ♻️ Régénération

* Un bloc cassé se régénère **120 secondes** après avoir été cassé.
* Un joueur à moins de 8 blocs reporte la régénération d'une seconde, jusqu'à 10 reports. Ensuite le bloc revient, sauf s'il chevauche un joueur.
* Les blocs reviennent du bas vers le haut.
* Un bloc régénéré est **tiré à nouveau au hasard** selon les taux du biome. Exception : en couche 1, il redevient toujours le bloc principal.
* Au redémarrage du serveur, toutes les mines sont intactes.

## 🌡️ Règles de monde

* Ni faim, ni dégâts de chute, de suffocation ou de lave dans les mines, les hubs et le spawn.
* Aucun monstre, aucune créature.
* Pas de pose de blocs : seuls les blocs de la zone minable se cassent.
* Cycle jour et nuit fixé par biome, météo fixée par biome.

## 👥 Capacité

* 250 joueurs par biome
* Biome plein : file d'attente, priorité aux grades Légende et supérieurs
* Aucun biome n'est dupliqué

## 🚫 Ce que la mine ne contient pas

* Aucun mob, aucun objet au sol, aucune orbe d'expérience
* Aucune pose de bloc, aucun fluide, aucun bloc à gravité, aucune source de lumière posée
* Aucune structure vanilla générée
