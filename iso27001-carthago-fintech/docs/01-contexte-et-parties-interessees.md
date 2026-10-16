# 01 — Contexte de l'organisation et parties intéressées (clauses 4.1 et 4.2)

**Statut : brouillon construit à partir du cas, à valider et compléter.** Les renvois (§) pointent vers les sections de l'énoncé.

## 1. L'organisation en bref

| Élément | Valeur | Source |
|---|---|---|
| Création | 2021, Tunis | §1 |
| Effectif | 120 collaborateurs (28 en 2022) | §1 |
| Clients professionnels | environ 420 | §1 |
| Transactions | environ 1,2 million par mois | §1 |
| Disponibilité visée | 99,95 % pour les APIs et le portail | §1 |
| Hébergement | Microsoft Azure, région France Central | §1, §4 |
| Supervision | SOC hybride : équipe interne 8x5 et MSSP 24/7 | §1, §8 |
| Objectif | certification ISO/IEC 27001:2022 sous 12 mois | §14 |

## 2. Enjeux externes (4.1)

| Enjeu | Détail issu du cas | Source | Effet possible sur le SMSI |
|---|---|---|---|
| Exigences de grands comptes | Un partenaire conditionne un nouveau contrat à une démarche ISO 27001 | §1 | Le SMSI doit être démontrable et certifiable |
| Cadre réglementaire tunisien | Loi 2016-48, circulaire BCT 2018-61, loi 2004-63, décret-loi 2023-17 | §11 | Registre des exigences légales à établir |
| Exigences contractuelles de paiement | PCI DSS possible, périmètre dépendant du flux et de la tokenisation | §11, §5 | Périmètre PCI DSS à déterminer |
| Menaces sur les identités | Phishing et fatigue MFA lors de l'incident du 3 septembre 2026 | §13 | Priorité aux contrôles d'identité et de détection |
| Dépendance à des tiers | Azure, MSSP, banques et acquéreurs, eKYC, OTP, SaaS | §10 | Maîtrise des fournisseurs (A.5.19 à A.5.23) |
| Hébergement des données en France | Société tunisienne, production en France Central | §11 | Transferts et exigences de protection des données à analyser |
| Expansion vers le Maghreb | Ambition 2026 à 2028 | §1 | Nouvelles exigences réglementaires possibles |

## 3. Enjeux internes (4.1)

| Enjeu | Détail issu du cas | Source |
|---|---|---|
| Croissance rapide | De 28 à 120 personnes entre 2022 et 2026 | §1 |
| Gouvernance informelle | Rôles SMSI non formalisés, décisions dépendantes de relations entre CTO, CIO et CISO | §3 |
| Hétérogénéité des pratiques | Sécurité présente mais formalisation, pilotage et preuves inégaux | §12 |
| Architecture cloud | Microservices sur Azure, majoritairement automatisée, quelques ressources manuelles | §4 |
| Organisation du SOC | Équipe interne 8x5 et MSSP 24/7, couverture de logs incomplète | §8 |
| Travail hybride | Environ 25 % des collaborateurs travaillent à distance plusieurs jours par semaine | §1 |
| Événements récents | Compte externe actif 11 jours, test de restauration hors objectif, incident du 3 septembre | §12, §13 |

## 4. Parties intéressées et exigences (4.2)

La colonne « Traitée par le SMSI ? » est à décider et à justifier (clause 4.2 c).

| Partie intéressée | Attentes (cas §2) | Exigences à retenir (à compléter) | Traitée par le SMSI ? |
|---|---|---|---|
| Clients professionnels | Disponibilité, exactitude des transactions, confidentialité, support rapide, preuves de sécurité | | |
| Utilisateurs finaux | Protection des données, sécurité des comptes, traitement correct des paiements | | |
| Banques et acquéreurs | Fiabilité des échanges, gestion de la fraude, traçabilité | | |
| Direction et actionnaires | Croissance, réputation, maîtrise du risque, continuité, conformité | | |
| Collaborateurs | Accès adaptés au rôle, outils sûrs, règles claires | | |
| Autorités et organismes de contrôle | Respect des textes applicables, coopération, traçabilité | | |
| Fournisseurs cloud et MSSP | Répartition claire des responsabilités, SLA, gestion des changements et incidents | | |

Parties à confirmer comme distinctes : prestataire eKYC, fournisseur SMS / OTP, réseau de paiement, et, parmi les autorités, BCT, INPDP et ANCS.

## 5. Exigences légales, réglementaires et contractuelles

| Texte ou exigence | Rôle dans le cas (§11) | Applicabilité | À faire |
|---|---|---|---|
| Loi 2016-48 du 11 juillet 2016 | Cadre des banques et établissements financiers | À analyser | Identifier les obligations liées à la sécurité |
| Circulaire BCT 2018-61 du 31 décembre 2018 | Établissements de paiement | À analyser | Idem |
| Loi organique 2004-63 du 27 juillet 2004 | Protection des données à caractère personnel | À analyser | Traitements, transferts, formalités INPDP |
| Décret-loi 2023-17 du 11 mars 2023 | Cybersécurité | À analyser | Vérifier l'applicabilité précise |
| PCI DSS | Exigence contractuelle possible | À analyser | Déterminer le périmètre selon le flux de carte |
| RGPD | Non cité dans le cas | À confirmer | Vérifier si des personnes concernées sont dans l'Union européenne |
| ISO/IEC 27001:2022 | Norme cible | Applicable | — |

## 6. À faire

- [ ] Valider ou corriger chaque ligne avec le cas.
- [ ] Compléter les exigences par partie intéressée et décider de leur prise en compte.
- [ ] Instruire l'applicabilité de chaque texte et alimenter le registre des exigences (A.5.31).
