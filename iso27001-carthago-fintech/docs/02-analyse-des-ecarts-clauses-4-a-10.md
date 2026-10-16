# 02 — Analyse des écarts par clause (4 à 10)

**Statut : brouillon.** Les estimations de conformité sont des hypothèses fondées sur l'énoncé du cas ; elles doivent être confirmées par des preuves lors des ateliers. Les exigences sont résumées avec mes mots à partir de la norme ISO/IEC 27001:2022. Les identifiants renvoient à `registres/Liste_des_ecarts.xlsx`.

Légende : **Non conforme** = rien de formalisé n'est mentionné · **Partielle** = éléments existants mais incomplets ou inégaux · **À vérifier** = le cas ne permet pas de conclure.

| Clause | Exigence (résumé) | Situation observée dans le cas | Conformité estimée | Écarts liés |
|---|---|---|---|---|
| 4.1 | Déterminer les enjeux externes et internes pertinents | Contexte décrit, aucune analyse formalisée mentionnée | Partielle | — |
| 4.2 | Déterminer les parties intéressées, leurs exigences, et celles traitées par le SMSI | Attentes connues (§2), pas de registre des exigences | Partielle | LEG-01, LEG-02, LEG-03 |
| 4.3 | Documenter le périmètre en tenant compte des enjeux, des exigences et des interfaces | Proposition de périmètre fournie (§15), non validée | Partielle | FOU-04 |
| 4.4 | Établir, mettre en œuvre, tenir à jour et améliorer le SMSI | Décision de lancement le 7 septembre 2026 (§14), SMSI à construire | Non conforme | GOV-01 |
| 5.1 | Leadership : politique, objectifs, intégration aux processus, ressources, communication | CEO sponsor, CISO chef de programme (§14), comité Cyber & Risques irrégulier | Partielle | GOV-01, GOV-02 |
| 5.2 | Politique de sécurité de l'information documentée et communiquée | Politique générale existante, mises à jour 2025 partielles (§12) | Partielle | GOV-06 |
| 5.3 | Rôles, responsabilités et autorités attribués et communiqués | Non formalisés de façon exhaustive (§3) | Non conforme | GOV-01, GOV-03 |
| 6.1.1 | Planifier les actions face aux risques et opportunités | Non mentionné | À vérifier | PIL-02 |
| 6.1.2 | Processus d'appréciation des risques : critères, cohérence, identification, analyse, évaluation, propriétaires | Aucune méthodologie mentionnée | Non conforme | PIL-02 |
| 6.1.3 | Traitement des risques : choix des mesures, comparaison avec l'Annexe A, SoA, plan de traitement, approbation par les propriétaires de risques | Non réalisé à ce stade | Non conforme | — |
| 6.2 | Objectifs de sécurité mesurables, planifiés et suivis | Objectifs de la direction listés (§14), KPI surtout techniques (§12) | Partielle | GOV-05 |
| 6.3 | Modifications du SMSI réalisées de façon planifiée | Sans objet avant la mise en place du SMSI | À vérifier | — |
| 7.1 | Ressources nécessaires | Équipe de six personnes au CISO, consultants externes (§3, §14) | À vérifier | — |
| 7.2 | Compétences déterminées, assurées et prouvées | Formation spécialisée irrégulière pour les rôles à privilèges (§12) | Partielle | HUM-01, SOC-05 |
| 7.3 | Sensibilisation du personnel | Campagne annuelle et phishing simulé (§12), incident de phishing (§13) | Partielle | HUM-01 |
| 7.4 | Communication interne et externe planifiée | Non mentionné (hors comité et escalade des incidents) | À vérifier | — |
| 7.5 | Informations documentées créées, mises à jour et contrôlées | Documents existants, contrôle de version non démontré | Partielle | GOV-06, ACT-02, CON-05 |
| 8.1 | Planification et contrôle opérationnels, y compris changements et processus externalisés | Nombreux contrôles en place mais hétérogènes (§12) | Partielle | IAM-01 à IAM-09, CLD-01 à CLD-04, DEV-01 à DEV-04, FOU-01 à FOU-04 |
| 8.2 | Appréciation des risques à intervalles planifiés ou lors de changements significatifs | Non mentionné | Non conforme | PIL-02 |
| 8.3 | Mise en œuvre du plan de traitement des risques | Non réalisé à ce stade | Non conforme | — |
| 9.1 | Surveiller, mesurer, analyser, évaluer | KPI techniques, peu d'indicateurs reliés aux objectifs (§12) | Partielle | GOV-05 |
| 9.2 | Audit interne planifié selon un programme | Non mentionné | À vérifier | PIL-01 |
| 9.3 | Revue de direction avec éléments d'entrée et décisions | Comité Cyber & Risques, mais pas de revue de direction ISO mentionnée | Partielle | GOV-02, PIL-01 |
| 10.1 | Amélioration continue | Retours d'expérience existants (exercice de novembre 2025, §12) | Partielle | GOV-04 |
| 10.2 | Traiter les non-conformités et mener des actions correctives avec preuves | Plans d'action non clos (restauration, exercice de crise) | Partielle | CON-03, GOV-04, PIL-01 |

## Lecture

- Les clauses de planification des risques (6.1.2, 6.1.3, 8.2, 8.3) sont les plus éloignées de la conformité : elles sont aussi le cœur du projet.
- Le point de départ n'est pas « sans sécurité » (§12) : plusieurs contrôles techniques existent, c'est leur pilotage et leur preuve qui manquent.

## À faire

- [ ] Relire chaque ligne avec le cas et la norme, ajuster les estimations.
- [ ] Ajouter pour chaque ligne la preuve à demander en atelier.
