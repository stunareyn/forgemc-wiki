# PNJ

## 🎯 Objectif

Un nouveau joueur ne lit pas un tutoriel : il parle à quelqu'un. Les PNJ guident le joueur **au moment où il en a besoin**, avec des phrases courtes, et donnent les quêtes de monde **directement dans leurs dialogues**.

## 👥 Les quatre PNJ

Il y a **exactement un PNJ par monde**, placé à côté du portail de ce monde au spawn.

| PNJ        | Monde     | Apparence                           | Personnalité           |
| ---------- | --------- | ----------------------------------- | ---------------------- |
| **Bram**   | 🪨 Lythos | Vieux mineur, casque cabossé, lampe | Bourru et bienveillant |
| **Ignace** | 🔥 Nether | Forgeron à la barbe roussie         | Direct, un peu moqueur |
| **Nox**    | 🌌 End    | Astronome aveugle, robe étoilée     | Calme et poétique      |
| **Séléné** | ☁️ Aether | Gardienne de marbre, halo pâle      | Solennelle             |

## ⚙️ Comment une quête est donnée

```
Clic droit sur le PNJ → Réplique selon l'avancement → Demande dans la phrase → Objectif vérifié par le plugin → Réplique suivante et récompense
```

> « Pas mal. Mais tu ne vas pas tout porter dans tes poches. Rapporte-moi un peu de cuivre et je te donne un vrai sac. »

Le joueur comprend seul l'objectif, la raison et la récompense. Chaque quête de monde se fait **une seule fois** et ne revient pas après un prestige.

## 🪨 Bram, Lythos

Bram est le **tutoriel du serveur**. L'ordre est pensé pour que chaque fonctionnalité arrive au moment où le joueur en a besoin.

| # | Ce que Bram demande                                            | Ce que le joueur apprend     | Récompense             |
| - | -------------------------------------------------------------- | ---------------------------- | ---------------------- |
| 1 | Casser 50 blocs dans La Carrière                               | Miner                        | Argent                 |
| 2 | Rapporter 20 Cuivre                                            | L'inventaire se remplit vite | 🎒 Le sac              |
| 3 | Vendre des minerais                                            | La vente                     | Argent                 |
| 4 | Forger la Pioche en Charbon                                    | La forge                     | Éclats                 |
| 5 | Miner 10 minerais sous la première couche                      | Creuser profond              | 🪝 Le grappin          |
| 6 | Faire éclore l'œuf qu'il donne (quand les pets sont débloqués) | Les pets                     | Éclats                 |
| 7 | Découvrir les 10 minerais de Lythos                            | La collection                | Titre Mineur de Lythos |

<details>

<summary>💬 Dialogues complets de Bram</summary>

**Première rencontre**

« Encore un nouveau mineur. Bienvenue à Lythos. Cette pioche est à toi, elle ne te quittera plus. Avant de parler de forge, montre-moi comment tu la tiens : descends à La Carrière et casse-moi cinquante blocs. »

**Après les cinquante blocs**

« Pas mal. Mais tu ne vas pas tout porter dans tes poches. Rapporte-moi un peu de cuivre et je te donne un vrai sac. »

**Après le sac**

« Garde dans ton sac ce qui te servira à forger. Le reste, vends-le. Reviens me voir quand tu auras gagné ta première paie. »

**Après la vente**

« Tu as de quoi payer la forge. Avec assez de charbon, ta pioche peut devenir une Pioche en Charbon. Ouvre ton menu de pioche et essaie. »

**Après la forge**

« Plus tu creuses, plus remonter devient pénible. Va sous la première couche, trouve-moi quelques minerais, et je te confie de quoi revenir à la surface. »

**Quand les pets sont débloqués**

« Tiens, j'ai trouvé cet œuf dans une galerie. Garde-le sur toi pendant que tu mines, il finira par éclore. »

**Plus tard**

« Lythos cache dix minerais, du charbon jusqu'à l'ambre. Trouve-les tous et je te considérerai comme un vrai mineur d'ici. »

**Répliques de retour**

« Encore là ? Bien. La pierre ne se casse pas toute seule. »

« Quand tu auras la Pioche en Ambre, pense au prestige. Tu repartiras de zéro, mais plus fort. »

« Mon genou prévoit la pluie. Sous terre. C'est dire s'il est doué. »

</details>

## 🔥 🌌 ☁️ Ignace, Nox et Séléné

Les trois autres PNJ suivent la même structure courte.

| Étape (validation → récompense) | 🔥 Ignace                                           | 🌌 Nox                                             | ☁️ Séléné                                   |
| ------------------------------- | --------------------------------------------------- | -------------------------------------------------- | ------------------------------------------- |
| **Monde verrouillé**            | Rappelle : Pioche en Ambre et un prestige           | Rappelle : Pioche en Infernium et Prestige IV      | Rappelle : Pioche en Nova et Prestige VII   |
| **1. Première entrée**          | Découvrir 3 minerais du Nether → Éclats             | Découvrir 3 minerais de l'End → Éclats             | Découvrir 3 minerais de l'Aether → Éclats   |
| **2. Forge**                    | Pioche en Soufre → œuf du Nether                    | Pioche en Météore → œuf de l'End                   | Pioche en Albâtre → œuf de l'Aether         |
| **3. Monde**                    | Les 9 minerais du Nether → titre Forgeron du Nether | Les 9 minerais de l'End → titre Astronome de l'End | Pioche en Éther → titre Gardien de l'Aether |

<details>

<summary>💬 Dialogues complets d'Ignace (Nether)</summary>

**Nether verrouillé**

« Le Nether ? Pas avec cette pioche. Reviens avec une Pioche en Ambre et au moins un prestige. »

**Première entrée**

« Te voilà. Ça sent le brûlé, habitue-toi. Ici, pas de fer ni d'or : du soufre, du cinabre, de la scorie. Rapporte-moi la preuve que tu en as trouvé trois différents. »

**Après trois minerais**

« Bien. Maintenant, forge ta première pioche d'ici. Le soufre fera l'affaire. »

**Après la forge**

« Neuf minerais dorment dans ce monde, jusqu'à l'infernium. Trouve-les tous et tu pourras dire que tu connais le Nether. »

**Répliques de retour**

« T'as pas fondu ? Bravo. »

</details>

<details>

<summary>💬 Dialogues complets de Nox (End)</summary>

**End verrouillé**

« Je t'entends approcher, mais l'End ne s'ouvre qu'avec une Pioche en Infernium et un quatrième prestige. »

**Première entrée**

« La porte est ouverte. Écoute bien là-haut, même les pierres chantent. Rapporte-moi le son de trois minerais différents, je saurai les reconnaître. »

**Après trois minerais**

« Ta pioche sonne encore comme une pioche du Nether. Forge-la dans le météore. »

**Après la forge**

« Neuf minerais, du météore à la nova. Trouve-les tous, et raconte-moi. »

**Répliques de retour**

« Ta pioche sonne différemment aujourd'hui. »

</details>

<details>

<summary>💬 Dialogues complets de Séléné (Aether)</summary>

**Aether verrouillé**

« L'Aether demande une Pioche en Nova et un septième prestige. Reviens quand tu seras prêt. »

**Première entrée**

« Tu es monté jusqu'ici. Montre-moi que tu mérites ta place : trouve trois minerais de ce ciel. »

**Après trois minerais**

« L'albâtre est tendre, mais c'est ici que tout commence. Forge ta pioche avec. »

**Après la forge**

« Au sommet du Trône Solaire se trouve l'éther, le plus précieux des minerais de ce ciel. Reviens me voir le jour où ta pioche sera faite d'éther. »

**Répliques de retour**

« La lumière t'a reconnu. »

</details>

## 🔒 Règle importante

{% hint style="danger" %}
* **Un PNJ par monde**, pas plus.
{% endhint %}
