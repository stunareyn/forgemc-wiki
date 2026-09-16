# Blocs chanceux

## 🎯 Objectif

Le minage est répétitif par nature. Les blocs chanceux ajoutent de la **surprise à chaque coup de pioche**, sans rien changer à la lisibilité du biome.

## ⚙️ Fonctionnement

{% stepper %}
{% step %}
## Le joueur casse un bloc

Le bloc peut être un bloc principal ou un minerai.
{% endstep %}

{% step %}
## Le serveur effectue un tirage

Le tirage est fait **pour ce joueur uniquement** afin de déterminer si le bloc était chanceux.
{% endstep %}

{% step %}
## Le joueur reçoit une récompense

Si le bloc est chanceux, le joueur reçoit une récompense d'une rareté donnée, affichée selon cette rareté.
{% endstep %}
{% endstepper %}

{% hint style="info" %}
**Rien n'est placé dans le monde à l'avance.** Dans un biome partagé, c'est essentiel : deux joueurs ne se disputent jamais un bloc chanceux, et un client modifié ne peut pas les repérer.
{% endhint %}

### Les règles d'équilibre

| Règle                                    | Pourquoi                                                                       |
| ---------------------------------------- | ------------------------------------------------------------------------------ |
| **Un coup de pioche, un tirage**         | Sinon Excavation donnerait jusqu'à 25 fois plus de chance                      |
| **Une explosion de dynamite, un tirage** | Même logique                                                                   |
| **Fortune n'a aucun effet**              | Fortune multiplie les minerais, pas la chance                                  |
| **Plafond de chance**                    | Trèfle, pets et auras augmentent la chance jusqu'à une limite                  |
| **Système de pitié**                     | Après une longue série sans récompense rare, une meilleure rareté est garantie |

## 🎁 Récompenses

| Rareté     | Récompenses possibles                         | Affichage                   |
| ---------- | --------------------------------------------- | --------------------------- |
| Commun     | Argent, XP de pioche, Éclats                  | Barre d'action              |
| Peu commun | Argent, Éclats, boost court                   | Barre d'action              |
| Rare       | Clé de caisse, œuf, somme d'argent importante | Titre à l'écran             |
| Épique     | Œuf rare, fragment d'aura, dynamite           | Titre à l'écran             |
| Légendaire | Œuf épique, aura                              | Annonce dans le biome       |
| Mythique   | Œuf légendaire, apparence exclusive           | Annonce sur tout le serveur |

Les montants d'argent et d'XP sont calculés à partir du **revenu de référence du biome** : une récompense Commune reste intéressante dans l'Aether comme dans Lythos.

Si l'inventaire est plein, la récompense part dans `/recompenses`.
