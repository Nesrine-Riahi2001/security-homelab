# ISO/IEC 27001 — Mise en œuvre d'un SMSI pour Carthago FinTech

> Étude de cas pédagogique (ESPRIT, parcours ISO/IEC 27001 Lead Implementer). Carthago FinTech est une **organisation fictive** : l'entreprise, les personnes, les chiffres et les incidents sont inventés ; seules les références réglementaires tunisiennes citées dans l'énoncé sont réelles.

## Contexte

Carthago FinTech (120 collaborateurs, plateforme de paiement CarthagoPay sur Microsoft Azure) lance un SMSI conforme à ISO/IEC 27001:2022 après un incident de compromission de compte DevOps survenu le 3 septembre 2026. La direction demande de démontrer que les risques sont maîtrisés, que les responsabilités sont claires et que les mesures fonctionnent de façon cohérente. Ce dépôt documente mon travail de Lead Implementer sur ce cas.

## Contenu

| Livrable | Fichier | État |
|---|---|---|
| Méthode et planning | [docs/00-methode-et-planning.md](docs/00-methode-et-planning.md) | Plan de travail |
| Contexte et parties intéressées (4.1, 4.2) | [docs/01-contexte-et-parties-interessees.md](docs/01-contexte-et-parties-interessees.md) | Brouillon à valider |
| Analyse des écarts, clauses 4 à 10 | [docs/02-analyse-des-ecarts-clauses-4-a-10.md](docs/02-analyse-des-ecarts-clauses-4-a-10.md) | Brouillon à valider |
| Périmètre, gouvernance, objectifs (4.3, 5, 6.2) | [docs/03-perimetre-et-gouvernance.md](docs/03-perimetre-et-gouvernance.md) | Brouillon à valider |
| Inventaire des actifs | [docs/04-inventaire-des-actifs.md](docs/04-inventaire-des-actifs.md) | Base à compléter |
| Méthodologie de risque (6.1.2) | [docs/05-methodologie-de-risque.md](docs/05-methodologie-de-risque.md) | Proposition à valider |
| Politiques | [docs/06-politiques/](docs/06-politiques/) | Modèle à compléter |
| Programme d'audit interne (9.2) | [docs/07-audit-interne.md](docs/07-audit-interne.md) | Modèle à compléter |
| Liste des écarts (45 constats) | [registres/Liste_des_ecarts.xlsx](registres/Liste_des_ecarts.xlsx) | Brouillon à valider |
| Registres : méthode, risques, traitement, SoA, indicateurs | [registres/Registres_SMSI.xlsx](registres/Registres_SMSI.xlsx) | À compléter |

## Démarche

1. Recenser les écarts du cas, avec leur source.
2. Analyser le contexte, les parties intéressées et le périmètre.
3. Apprécier les risques avec une méthode explicite, puis les traiter.
4. Établir la déclaration d'applicabilité (93 contrôles de l'Annexe A) et les indicateurs.
5. Rédiger les politiques prioritaires et planifier l'audit interne.

## Hypothèses et limites

- Les constats viennent uniquement de l'énoncé du cas ; aucune preuve détaillée n'est disponible, les ateliers à venir devant en fournir.
- Les notes de criticité, les échelles de risque, les scénarios et les cibles d'indicateurs sont des propositions de travail, signalées comme telles dans les documents.
- Les liens entre écarts, clauses et contrôles sont indicatifs.

## Droits d'auteur

La norme ISO/IEC 27001:2022 est protégée par le droit d'auteur et n'est pas reproduite ici : seuls les intitulés des contrôles sont repris. L'énoncé du cas n'est pas inclus.

## Auteure

Nesrine Riahi — étudiante ingénieure en cybersécurité (ESPRIT).
