# Fonctionnement des biomes

## 🎯 Objectif

Un serveur de minage vit de sa foule. Voir d'autres joueurs miner autour de soi, remarquer une aura rare, croiser une pioche plus avancée : c'est ce qui donne envie de progresser. C'est pour cela que STRATA n'a **aucune mine personnelle** et que tous les biomes sont **partagés**.

## ⚙️ Un biome

| Règle      | Détail                                                                                |
| ---------- | ------------------------------------------------------------------------------------- |
| 🗺️ Format | Un monde dédié : une grande zone minière fermée par une bordure indestructible        |
| 🚪 Arrivée | Téléportation à une position de surface aléatoire et sûre, répartie sur toute la zone |

## 🪨 Génération et couches

Le système est volontairement **simple** :

| Couche                | Contenu                                      |
| --------------------- | -------------------------------------------- |
| **Première couche**   | Uniquement le bloc principal. Aucun minerai. |
| **Couches suivantes** | Bloc principal et minerais, tirés au hasard. |

* Les probabilités sont **identiques à toutes les profondeurs**.
* Les minerais ne deviennent ni plus rares ni plus fréquents en descendant.
* Le bloc principal reste le bloc le plus fréquent partout.
* Un biome contient ses minerais **et ceux du biome précédent** du même monde.

<details>

<summary>Pourquoi une première couche sans minerai ?</summary>

Elle donne une surface propre et lisible, et évite que les joueurs qui arrivent ramassent des minerais sans creuser.

</details>

<details>

<summary>Pourquoi les mêmes probabilités à toutes les profondeurs ?</summary>

Une rareté liée à la profondeur pousse tout le monde au fond : embouteillages en bas, zones mortes en haut. Avec des probabilités identiques, chacun mine où il veut et la population se répartit naturellement.

</details>

## ♻️ Régénération

{% stepper %}
{% step %}
## Un bloc cassé devient de l'air
{% endstep %}

{% step %}
## Après **3 minutes**, il réapparaît

Il réapparaît **seulement si aucun joueur n'est à moins de 8 blocs**.
{% endstep %}

{% step %}
## Le nouveau bloc est tiré à nouveau

Il est généré selon la règle de sa couche.
{% endstep %}
{% endstepper %}

## 🔒 Règles importantes

{% hint style="danger" %}
* Un bloc cassé rapporte **au joueur qui l'a cassé**, y compris par Excavation ou dynamite.
* Le butin va directement dans le sac ou l'inventaire. **Rien ne tombe au sol.**
* Pas de combat, de faim, de mort ni de construction.
* Première couche sans minerai.
* Probabilités identiques quelle que soit la profondeur.
{% endhint %}
