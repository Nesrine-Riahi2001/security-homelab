# 05 — Méthodologie d'appréciation des risques (clause 6.1.2)

**Statut : proposition à valider.** Les échelles, seuils et critères d'acceptation sont à faire approuver par la direction ; ils sont paramétrables dans l'onglet `Méthode` de `registres/Registres_SMSI.xlsx`.

## Choix de méthode

Approche par scénarios inspirée d'ISO/IEC 27005 : on décrit un scénario (cause, événement, conséquence), on cote la **vraisemblance** et l'**impact** de 1 à 4, le niveau de risque est leur produit. Variante possible : EBIOS Risk Manager (ANSSI), plus orientée sources de risque et scénarios opérationnels.

## Ce que la norme demande, et où c'est traité

| Exigence 6.1.2 | Réponse dans ce projet |
|---|---|
| Critères de risque, dont critères d'acceptation | Onglet Méthode : échelles et seuils |
| Résultats cohérents, valides et comparables | Mêmes échelles pour tous les risques, définitions écrites |
| Identification des risques de perte de C, I ou D, avec propriétaires | Onglet Risques : colonnes C / I / D et propriétaire |
| Analyse : conséquences, vraisemblance, niveau | Colonnes vraisemblance, impact, niveau brut |
| Évaluation : comparaison aux critères, priorisation | Colonnes classe et décision |
| Informations documentées | Ce fichier et le registre |

## Déroulé

1. Partir de la liste des écarts et des actifs.
2. Regrouper les écarts en scénarios de risque (11 scénarios candidats sont préremplis).
3. Coter vraisemblance et impact **en justifiant** chaque note par un fait du cas.
4. Lire la classe et la décision calculées.
5. Choisir une option de traitement (réduire, accepter, transférer, éviter) et relier le risque à des contrôles.
6. Recoter le risque résiduel après traitement.

## Exemple de justification de cotation

> R-01, vraisemblance 3 : un incident de ce type s'est déjà produit le 3 septembre 2026 (§13). Impact 4 : un compte à privilèges Azure peut affecter les données de transaction et la disponibilité de la plateforme.

(Exemple de format, les notes restent à décider par vous.)

## À faire

- [ ] Relire et ajuster les définitions d'échelle.
- [ ] Faire valider les seuils (hypothèse de départ : seuil d'acceptation ≤ 3).
- [ ] Coter les 11 risques et justifier chaque note dans ce document ou dans le rapport.
