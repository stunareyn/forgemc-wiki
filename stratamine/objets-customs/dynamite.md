# Dynamite

## 🎯 Objectif

La dynamite offre un moment différent du minage classique : lancer, attendre la mèche, voir la zone se dégager. C'est un **outil ponctuel**, utile pour ouvrir une galerie ou dégager une paroi. Elle ne doit **jamais** devenir la meilleure façon de miner.

## ⚙️ Fonctionnement

{% stepper %}
{% step %}
## Clic droit

La dynamite est lancée.
{% endstep %}

{% step %}
## Explosion

Elle explose après une **mèche de 1,5 seconde**.
{% endstep %}

{% step %}
## Récompenses

Les blocs dans le rayon sont cassés et leur butin va **au lanceur**.
{% endstep %}
{% endstepper %}

### Valeurs de départ

| Paramètre   | Valeur                          |
| ----------- | ------------------------------- |
| 💥 Rayon    | X blocs (sphère)                |
| ⏱️ Recharge | 2 secondes entre chaque lancers |

### Blocs affectés

* Uniquement le **bloc principal** et les **minerais** du biome.
* Jamais la bordure, le sol indestructible, ni le bloc sous les pieds d'un autre joueur.
* Aucun dégât ni recul sur les joueurs.

## 🔗 Interactions : la règle la plus importante

| Élément                                | Effet sur l'explosion                 |
| -------------------------------------- | ------------------------------------- |
| Minerais                               | Quantité de base, sans bonus          |
| **Fortune**                            | ❌ Aucun effet                         |
| **Excavation**                         | ❌ Aucun effet                         |
| Filon, Élan, Maîtrise, Trèfle, Aubaine | ❌ Aucun effet                         |
| Négoce                                 | ✅ S'applique normalement à la vente   |
| Blocs chanceux                         | Un seul tirage par explosion          |
| Œufs                                   | Un point de progression par explosion |
| Collection                             | Découvertes et compteurs normaux      |

<details>

<summary>Pourquoi Fortune et Excavation ne s'appliquent pas ?</summary>

* **Avec Fortune**, une dynamite qui casse 30 blocs deviendrait bien plus rentable qu'un coup de pioche : les joueurs mineraient à la dynamite.
* **Avec Excavation**, chaque bloc cassé déclencherait un 3x3, et une explosion couvrirait des centaines de blocs.

</details>
