# 03 — Périmètre, gouvernance et objectifs (clauses 4.3, 5 et 6.2)

**Statut : brouillon avec points à trancher.** Le périmètre de départ du cas (§15) est une proposition, pas une réponse définitive.

## 1. Périmètre proposé dans le cas (résumé)

Conception, développement, exploitation, sécurisation, supervision et support de la plateforme CarthagoPay (applications web et mobile, APIs, infrastructure cloud associée, DevSecOps, IAM, SOC et processus support). Les fournisseurs (cloud, MSSP, banques, eKYC, OTP, SaaS) sont externes mais constituent des dépendances.

## 2. Points à trancher

| Sujet | Question | Piste de départ (hypothèse) | Décision |
|---|---|---|---|
| Environnements DEV et TEST | Le périmètre cite production, préproduction et services de support, mais pas DEV ni TEST ; or des jeux de données masqués issus de la production y sont utilisés (§7) | Inclure DEV et TEST, ou justifier leur exclusion | |
| Messagerie Microsoft 365 | Seule Entra ID est citée comme technologie ; l'incident est parti d'un faux message Microsoft 365 (§13) | Préciser si M365 est dans le périmètre, au moins pour l'identité et la messagerie | |
| Fonctions support | RH, juridique, achats et finance sont inclus « lorsqu'ils supportent les processus » | Lister les processus concernés (départs, contrats, fournisseurs) | |
| Siège et télétravail | Le siège garde des équipements réseau et des postes d'administration ; 25 % de télétravail (§1, §4) | Inclure les contrôles physiques du siège et le travail à distance (A.6.7, 7.x) | |
| Prestataire eKYC | Dossiers KYC stockés chez Carthago, vérification chez un tiers (§5, §10) | Dépendance externe incluse, données KYC dans le périmètre | |
| Interfaces et dépendances (4.3 c) | Azure, MSSP, banques, eKYC, OTP | Décrire pour chacun les responsabilités et les flux | |
| Exclusions | Activités non incluses (par ex. commercial) | Toute exclusion doit être justifiée | |

## 3. Gouvernance et rôles

| Rôle | Responsable (cas §3, §14) | Rôle dans le SMSI (proposition) |
|---|---|---|
| Sponsor | Amel Ben Salem, CEO | Arbitrage budgétaire, acceptation des risques résiduels, engagement de la direction |
| Chef de programme | Nader Bouaziz, CISO | Pilotage du SMSI, méthode de risque, SoA |
| Comité de pilotage | CEO, CTO, CIO, CISO, Risques & Conformité, Opérations, RH / Juridique | Suivi du programme et revue de direction |
| Produit et développement | Youssef Trabelsi, CTO | Propriétaire des risques applicatifs et DevSecOps |
| Infrastructure et cloud | Mariem Gharbi, CIO | Propriétaire des risques d'infrastructure, de continuité et d'accès techniques |
| Conformité et DPO | Rim Khelifi | Exigences légales, protection des données |
| Opérations | Hatem Mansour | Incidents côté clients, fraude |

### Matrice RACI (proposition à valider)

R = réalise · A = approuve · C = consulté · I = informé

| Activité | CEO | CTO | CIO | CISO | Conformité / DPO | Opérations |
|---|---|---|---|---|---|---|
| Politique de sécurité | A | C | C | R | C | I |
| Appréciation des risques | I | C | C | R, A | C | C |
| Acceptation des risques résiduels | A | C | C | R | C | I |
| Déclaration d'applicabilité | I | C | C | R, A | C | I |
| Gestion des incidents | I | C | C | R, A | C | C |
| Revues d'accès | I | R | R | A | I | C |
| Gestion des fournisseurs | I | C | C | R, A | C | I |
| Continuité et PRA | I | C | R | A | I | C |
| Audit interne | I | I | I | A | I | I |
| Revue de direction | R, A | C | C | R | C | C |

## 4. Objectifs de sécurité (6.2) — propositions

Les objectifs de la direction (§14) sont reformulés pour être mesurables. Les indicateurs renvoient à l'onglet `Indicateurs` de `registres/Registres_SMSI.xlsx`. Les cibles sont à valider.

| Objectif de la direction (§14) | Objectif mesurable (proposition) | Indicateur |
|---|---|---|
| Maîtriser les risques liés aux identités, privilèges et accès administrateurs | Réduire les accès non justifiés et les droits privilégiés permanents | KPI-01, KPI-02, KPI-03 |
| Améliorer la couverture de supervision et la qualité de la réponse | Couvrir les sources de logs critiques et réduire le délai de blocage | KPI-04, KPI-05 |
| Structurer la sécurité des fournisseurs | Évaluer tous les fournisseurs critiques | KPI-08 |
| Aligner continuité, sauvegardes et PRA sur des besoins métier mesurés | Tenir les RTO lors des tests | KPI-07 |
| Produire des indicateurs compréhensibles par la direction | Présenter un tableau de bord à chaque comité | KPI-01 à KPI-10 |
| Amélioration continue | Clore les actions correctives dans les délais | KPI-09 |

## 5. À faire

- [ ] Trancher chaque point de la section 2 et rédiger la déclaration de périmètre définitive.
- [ ] Valider ou corriger la matrice RACI.
- [ ] Rédiger la politique de sécurité de l'information et la faire approuver (rôle de la direction).
