---
description: Les 4 PNJ de dimension, leur emplacement, leurs dialogues, leurs options et les actions déclenchées.
---

# 👤 PNJ

## ⚙️ Principes

* Un PNJ par dimension, placé à côté du portail de sa dimension au spawn.
* Répliques courtes, une ou deux phrases.
* Un PNJ ne parle que de ce qui existe sur le serveur.
* Clic droit : réplique adaptée à la progression du joueur, puis menu d'options.
* Les PNJ n'existent qu'au spawn. Aucun PNJ dans les mines.
* Apparence : skin de joueur existant, choisi selon la description.

## 🪨 Bram · Overworld

* Emplacement : portail de l'Overworld, spawn
* Apparence : vieux mineur, casque cabossé, lampe
* Rôle : accueil et tutoriel

**Répliques**

| Situation | Réplique |
| --- | --- |
| Première rencontre | « Bienvenue. Cette pioche est à toi, elle ne te quittera pas. Casse-moi quelques blocs à La Carrière. » |
| Tutoriel en cours | « Tu vends, tu enchantes, tu forges. Le reste vient tout seul. » |
| Pioche en Baryte non obtenue | « Garde de la Baryte au lieu de tout vendre. Il en faut 48 pour ta prochaine pioche. » |
| Pioche d'Ambre obtenue | « Le Nether t'attend. Parle à Ignace, de l'autre côté. » |
| Après un Rebirth | « Te revoilà au début. Tu vas beaucoup plus vite cette fois. » |
| Retour habituel | « La pierre ne se casse pas toute seule. » |

**Tutoriel**, une fois par compte

| Étape | Objectif | Récompense |
| --- | --- | --- |
| 1 | Casser 30 blocs à La Carrière | 2 Cristaux |
| 2 | Vendre avec `/sell` | 2 Cristaux |
| 3 | Acheter Efficacité 1 dans `/pioche` | 2 Cristaux |
| 4 | Garder 48 Baryte | 2 Cristaux |
| 5 | Forger la Pioche en Baryte | Œuf de l'Overworld et 10 Cristaux |

**Options**
* Voyager : menu des biomes de l'Overworld débloqués
* Conditions : prochaine pioche, prix, minerai, niveau
* Minerais : les 9 minerais de l'Overworld et leur valeur
* Tutoriel : reprendre l'étape en cours

## 🔥 Ignace · Nether

* Emplacement : portail du Nether, spawn
* Apparence : forgeron à la barbe roussie
* Rôle : accès au Nether

| Situation | Réplique |
| --- | --- |
| Nether verrouillé | « Pas avec cette pioche. Reviens avec la Pioche d'Ambre. » |
| Première entrée | « Ça sent le brûlé, habitue-toi. Ici tu trouveras l'Excavation, sers-t'en. » |
| Retour habituel | « T'as pas fondu ? Bien. » |
| Pioche de Carmin obtenue | « L'End est ouvert. Nox t'attend, il ne voit rien mais il entend tout. » |

**Options**
* Voyager : menu des biomes du Nether débloqués
* Conditions
* Minerais : les 9 minerais du Nether

## 🌌 Nox · End

* Emplacement : portail de l'End, spawn
* Apparence : astronome aveugle, robe étoilée
* Rôle : accès à l'End

| Situation | Réplique |
| --- | --- |
| End verrouillé | « L'End ne s'ouvre qu'à la Pioche de Carmin. » |
| Première entrée | « Écoute. Même les pierres chantent, là-haut. » |
| Retour habituel | « Ta pioche sonne différemment aujourd'hui. » |
| Pioche de Nova obtenue | « Séléné t'attend au-dessus des nuages. » |

**Options**
* Voyager : menu des biomes de l'End débloqués
* Conditions
* Minerais : les 9 minerais de l'End

## ☁️ Séléné · Aether

* Emplacement : portail de l'Aether, spawn
* Apparence : gardienne de marbre, halo pâle
* Rôle : accès à l'Aether et au Rebirth

| Situation | Réplique |
| --- | --- |
| Aether verrouillé | « L'Aether demande la Pioche de Nova. » |
| Première entrée | « Tu es monté jusqu'ici. L'Éther est plus fréquent au Trône Solaire. » |
| Rebirth disponible | « Ta pioche est faite d'Éther. Tu peux renaître, si tu le veux. » |
| Retour habituel | « La lumière t'a reconnu. » |

**Options**
* Voyager : menu des biomes de l'Aether débloqués
* Conditions
* Minerais : les 9 minerais de l'Aether
* Rebirth : ouvre `/rebirth`, visible seulement quand les conditions sont remplies

## 🎬 Actions déclenchées

| Option | Action | Permission |
| --- | --- | --- |
| Voyager | Ouvre le menu de voyage de la dimension | `strata.tp.biome` |
| Conditions | Ouvre la page de la prochaine pioche | `strata.pioche` |
| Minerais | Ouvre la liste des minerais et valeurs | `strata.valeurs` |
| Tutoriel | Affiche l'étape en cours | `strata.player.tutoriel` |
| Rebirth | Ouvre le menu de Rebirth | `strata.rebirth` |
