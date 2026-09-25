---
description: Les 4 PNJ de dimension, leur emplacement, leurs répliques, le tutoriel et les actions déclenchées.
---

# 👤 PNJ

## ⚙️ Principes

* Un PNJ par dimension, placé à côté du portail de sa dimension au spawn.
* Répliques courtes, une ou deux phrases.
* Un PNJ ne parle que de ce qui existe sur le serveur.
* Clic droit : réplique adaptée à la progression du joueur, puis menu d'options.
* Les PNJ n'existent qu'au spawn. Aucun PNJ dans les mines.
* Apparence : skin de joueur existant, choisi selon la description. PNJ par paquets, sans entité serveur.

## 🪨 Bram · Overworld

* Emplacement : portail de l'Overworld, spawn
* Apparence : vieux mineur, casque cabossé, lampe
* Rôle : accueil, tutoriel, Prestige

**Répliques**

| Situation | Réplique |
| --- | --- |
| Première rencontre | « Bienvenue. Cette pioche est à toi, elle ne te quittera pas. Casse-moi quelques blocs dans les Plaines. » |
| Tutoriel en cours | « Tu vends, tu enchantes, tu forges. Le reste vient tout seul. » |
| Pioche en Cuivre non forgée | « Garde ton Cuivre au lieu de tout vendre. Il en faut 40 pour ta prochaine pioche. » |
| Pioche en Diamant forgée, Prestige 0 | « Tu as ta Pioche en Diamant. Le Prestige t'attend, et le Nether derrière. » |
| Après un Prestige | « Te revoilà au début. Tu vas beaucoup plus vite cette fois. » |
| Après une Renaissance | « Tout recommencer, encore ? Tu es plus têtu que la pierre. » |
| Retour habituel | « La pierre ne se casse pas toute seule. » |

**Tutoriel**, une fois par compte

| Étape | Objectif | Récompense |
| --- | --- | --- |
| 1 | Casser 30 blocs dans les Plaines | 2 Cristaux |
| 2 | Vendre avec `/sell` | 2 Cristaux |
| 3 | Acheter Efficacité 1 dans `/enchant` | 2 Cristaux |
| 4 | Garder 40 Cuivre | 2 Cristaux |
| 5 | Forger la Pioche en Cuivre | Œuf de l'Overworld et 10 Cristaux |

Total : 18 Cristaux et 1 Œuf. Avec les 16 premières entrées de biome à 5 Cristaux, soit 80, ces récompenses uniques font les 98 Cristaux du budget de l'[Économie](../economie/economie.md).

**Options**

* Voyager : biomes de l'Overworld débloqués
* Prochaine pioche : prix, minerai, niveau requis
* Minerais : les 8 minerais de l'Overworld et leur valeur
* Prestige : ouvre `/prestige`
* Tutoriel : reprendre l'étape en cours

## 🔥 Ignace · Nether

* Emplacement : portail du Nether, spawn
* Apparence : forgeron à la barbe roussie
* Rôle : accès au Nether

| Situation | Réplique |
| --- | --- |
| Nether verrouillé, Prestige 0 | « Pas avant ton premier Prestige. Reviens avec la Pioche en Diamant et un rang de plus. » |
| Nether verrouillé, pioche manquante | « Tu as le rang, pas la pioche. Forge d'abord ta Pioche en Diamant. » |
| Première entrée | « Ça sent le brûlé, habitue-toi. Le Seigneur des Cendres rôde sous la roche, frappe fort quand il se réveille. » |
| Retour habituel | « T'as pas fondu ? Bien. » |
| Prestige IV et Pioche de Carmin | « L'End est ouvert. Nox t'attend, il ne voit rien mais il entend tout. » |

**Options**

* Voyager : biomes du Nether débloqués
* Prochaine pioche
* Minerais : les 9 minerais du Nether

## 🌌 Nox · End

* Emplacement : portail de l'End, spawn
* Apparence : astronome aveugle, robe étoilée
* Rôle : accès à l'End

| Situation | Réplique |
| --- | --- |
| End verrouillé | « L'End ne s'ouvre qu'au Prestige IV, avec la Pioche de Carmin. » |
| Première entrée | « Écoute. Même les pierres chantent, là-haut. Et quelque chose les dévore. » |
| Retour habituel | « Ta pioche sonne différemment aujourd'hui. » |
| Prestige VII et Pioche en Pulsar | « Séléné t'attend au-dessus des nuages. » |

**Options**

* Voyager : biomes de l'End débloqués
* Prochaine pioche
* Minerais : les 9 minerais de l'End

## ☁️ Séléné · Aether

* Emplacement : portail de l'Aether, spawn
* Apparence : gardienne de marbre, halo pâle
* Rôle : accès à l'Aether et à la Renaissance

| Situation | Réplique |
| --- | --- |
| Aether verrouillé | « L'Aether demande le Prestige VII et la Pioche en Pulsar. » |
| Première entrée | « Tu es monté jusqu'ici. Les Pics gelés sont les plus riches, mais le Roi des Tempêtes y règne. » |
| Renaissance disponible | « Prestige X, Pioche d'Éther, niveau 100. Tu peux renaître, si tu le veux. » |
| Après une Renaissance | « Tu reviens plus fort. La lumière s'en souvient. » |
| Retour habituel | « La lumière t'a reconnu. » |

**Options**

* Voyager : biomes de l'Aether débloqués
* Prochaine pioche
* Minerais : les 9 minerais de l'Aether
* Renaissance : ouvre `/renaissance`, visible seulement quand les conditions sont remplies

## 🎬 Actions déclenchées

| Option | Action | Permission |
| --- | --- | --- |
| Voyager | Ouvre le menu de voyage sur la dimension du PNJ | `strata.player.biomes` |
| Prochaine pioche | Ouvre la Forge sur la prochaine pioche | `strata.player.forge` |
| Minerais | Ouvre la liste des minerais et valeurs | `strata.player.valeurs` |
| Prestige | Ouvre le menu de Prestige | `strata.player.prestige` |
| Tutoriel | Affiche l'étape en cours | `strata.player.tutoriel` |
| Renaissance | Ouvre le menu de Renaissance | `strata.player.renaissance` |
