# Sac

## 🎯 Objectif

Sans sac, l'inventaire est plein en quelques minutes et le joueur passe son temps à vendre. Le sac règle deux problèmes :

* il **stocke** les minerais utiles à la forge ;
* il **trie** automatiquement ce qu'on garde et ce qu'on vend.

## ⚙️ Fonctionnement

| Élément          | Détail                                                 |
| ---------------- | ------------------------------------------------------ |
| 🔓 Déblocage     | Quête de départ de Bram, le PNJ de Lythos              |
| 🔗 Type          | Objet lié, dans un emplacement fixe de la barre rapide |
| 🖱️ Clic droit   | Ouvre le sac                                           |
| ⌨️ Touche de jet | Ne jette pas le sac : ouvre les filtres                |
| 📐 Au départ     | 1 ligne d'emplacements, capacité de base               |

### Les filtres

* Pour chaque minerai découvert, le joueur choisit : **sac** ou **inventaire**.
* Le surplus part dans l'inventaire.
* Le bouton **Préparer mon sac** de l'écran Forger règle le filtre du minerai de la prochaine pioche.

### Améliorations

Toutes s'achètent en **Éclats**, parce que le sac est permanent.

| Amélioration             | Condition                              |
| ------------------------ | -------------------------------------- |
| Capacité par emplacement | Par paliers                            |
| Ligne 2                  | Avoir atteint une fois le Prestige I   |
| Ligne 3                  | Avoir atteint une fois le Prestige III |
| Ligne 4                  | Avoir atteint une fois le Prestige V   |
| Ligne 5                  | Avoir atteint une fois le Prestige VII |
| Ligne 6                  | Avoir atteint une fois le Prestige X   |

{% hint style="success" %}
**Conservation :** le sac, son contenu et ses améliorations ne sont **jamais perdus**, ni au prestige, ni à la renaissance. Une ligne achetée reste acquise même quand les rangs de prestige reviennent à zéro.
{% endhint %}

## 👤 Expérience joueur

Le réglage idéal : « garder dans le sac le minerai de ma prochaine pioche, tout le reste part à la vente ». Le joueur n'y pense plus et mine.



{% hint style="warning" %}
* `/sellall` ne vend **jamais** le contenu du sac.
* Le sac est un objet lié.
{% endhint %}
