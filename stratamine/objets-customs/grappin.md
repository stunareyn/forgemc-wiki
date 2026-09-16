# Grappin

## 🎯 Objectif

Les biomes sont immenses et les joueurs creusent profond. Sans outil de déplacement, remonter d'un trou de 30 blocs est pénible et pousse les joueurs à rester en surface. Le grappin rend la **profondeur agréable**.

## ⚙️ Fonctionnement

{% stepper %}
{% step %}
## Viser et utiliser

Le joueur vise un bloc et fait **clic droit**.
{% endstep %}

{% step %}
## Vérification de la cible

Le serveur vérifie la cible : bloc du biome, en ligne de vue, dans la portée.
{% endstep %}

{% step %}
## Traction

Le joueur est **tiré** jusqu'au bloc. C'est un vrai déplacement, pas une téléportation.
{% endstep %}

{% step %}
## Arrêt et décrochage

Il s'arrête sur une position sûre devant le bloc. **S'accroupir** le décroche en route.
{% endstep %}

{% step %}
## Cible invalide

Un message court s'affiche et **la recharge n'est pas consommée**.
{% endstep %}
{% endstepper %}

### Valeurs de départ

| Paramètre   |  Au départ | Maximum après améliorations |
| ----------- | :--------: | :-------------------------: |
| 📏 Portée   |   X blocs  |            Xblocs           |
| ⏱️ Recharge | X secondes |          X secondes         |
| 🔋 Charges  |      1     |              2              |

### Obtention et améliorations

* Obtenu par une **quête de Bram**. Tous les joueurs l'ont.
* Objet lié.
* Améliorations par paliers, achetées avec des **Éclats**.
* Le grappin et ses améliorations ne sont **jamais perdus**.

## 🚫 Limites

| Limite                                                            | Pourquoi                                                       |
| ----------------------------------------------------------------- | -------------------------------------------------------------- |
| Uniquement dans les biomes                                        | Au spawn, il servirait à contourner les décors                 |
| Cibles interdites : bordure, sol indestructible, joueurs, entités | Pas d'abus, pas de gêne                                        |
| Portée limitée                                                    | Assez pour sortir d'un trou, pas assez pour traverser un biome |

## 👤 Expérience joueur

Le grappin devient un **réflexe** : on creuse, on remonte en un clic, on atteint une paroi pleine de minerais.

## 🔒 Règle importante

{% hint style="danger" %}
* L'anti-cheat tolère le déplacement **uniquement pendant la traction**.
{% endhint %}
