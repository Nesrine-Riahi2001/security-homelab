# 00 — Méthode et planning

## Principe

Chaque livrable répond à une exigence de la norme, s'appuie sur des faits tirés du cas (avec section et page) et signale ses hypothèses. Aucune preuve n'est inventée : ce qui manque est listé comme « preuve à demander ».

## Étapes et livrables

| # | Étape | Clause | Livrable | Durée indicative | Fait |
|---|---|---|---|---|---|
| 1 | Lire le cas et lister les écarts | — | `registres/Liste_des_ecarts.xlsx` | 1 jour | [ ] |
| 2 | Contexte et parties intéressées | 4.1, 4.2 | `docs/01-...` | 2 jours | [ ] |
| 3 | Analyse des écarts par clause | 4 à 10 | `docs/02-...` | 2 jours | [ ] |
| 4 | Périmètre, gouvernance, objectifs | 4.3, 5.1 à 5.3, 6.2 | `docs/03-...` | 2 jours | [ ] |
| 5 | Inventaire des actifs | 6.1.2, A.5.9 | `docs/04-...` | 2 jours | [ ] |
| 6 | Méthode et appréciation des risques | 6.1.2, 8.2 | `docs/05-...`, onglets Méthode et Risques | 4 à 5 jours | [ ] |
| 7 | Traitement des risques et SoA | 6.1.3, 8.3 | onglets Traitement et SoA | 4 à 5 jours | [ ] |
| 8 | Politiques prioritaires | 5.2, 7.5, A.5.1 | `docs/06-politiques/` | 3 jours | [ ] |
| 9 | Indicateurs et audit interne | 9.1, 9.2 | onglet Indicateurs, `docs/07-...` | 3 jours | [ ] |
| 10 | Relecture et publication | — | dépôt Git à jour | 1 à 2 jours | [ ] |

## Définition de « terminé » pour un livrable

- Chaque affirmation renvoie à une section du cas ou est marquée comme hypothèse.
- Chaque choix (risque, contrôle exclu, seuil) est justifié en une phrase.
- Les statuts « Brouillon » ont été relus et remplacés par « Validé » ou corrigés.

## Règles de travail

- Un commit par livrable ou par étape, avec un message clair.
- Ne jamais ajouter au dépôt la norme ni l'énoncé du cas.
- Écrire « fictif » partout où l'organisation est mentionnée dans un document destiné à être partagé.
