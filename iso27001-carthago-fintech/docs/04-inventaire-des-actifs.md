# 04 — Inventaire des actifs informationnels (A.5.9, clause 6.1.2)

**Statut : base à compléter.** Les 7 premiers actifs viennent du cas (§5) avec leurs niveaux de sensibilité ; les suivants sont des propositions à valider. Classification du cas : Public, Interne, Confidentiel, Restreint.

C = confidentialité, I = intégrité, D = disponibilité.

## Actifs du cas

| ID | Actif | C | I | D | Commentaire (cas) | Propriétaire | Classification |
|---|---|---|---|---|---|---|---|
| A-01 | Données de transaction | Très élevée | Très élevée | Élevée | Montants, statuts, références, rapprochement | | |
| A-02 | Données KYC des commerçants | Très élevée | Élevée | Moyenne | Pièces d'identité, justificatifs, coordonnées | | |
| A-03 | Identités et habilitations | Très élevée | Très élevée | Élevée | Comptes, rôles, informations d'authentification | | |
| A-04 | Code source et pipelines | Élevée | Très élevée | Élevée | Applications, scripts, IaC, secrets de pipeline | | |
| A-05 | Clés, secrets et certificats | Critique | Critique | Élevée | Key Vault, secrets API, certificats TLS | | |
| A-06 | Logs de sécurité | Élevée | Très élevée | Élevée | Traçabilité, investigation, preuves | | |
| A-07 | Contrats et procédures | Élevée | Élevée | Moyenne | SLA, obligations, procédures internes | | |

## Actifs proposés (à valider)

| ID | Actif | Type | Source | Propriétaire | C | I | D |
|---|---|---|---|---|---|---|---|
| A-08 | API de paiement CarthagoPay | Application | §2, §4 | | | | |
| A-09 | Portail commerçants | Application | §2 | | | | |
| A-10 | Application mobile | Application | §2 | | | | |
| A-11 | Moteur de détection de fraude | Application | §2, §4 | | | | |
| A-12 | Cluster AKS et microservices | Infrastructure | §4 | | | | |
| A-13 | Bases Azure SQL et PostgreSQL | Données | §4 | | | | |
| A-14 | Stockage Blob (KYC, exports) | Données | §4 | | | | |
| A-15 | Key Vault | Infrastructure | §4 | | | | |
| A-16 | Microsoft Entra ID | Service | §4, §6 | | | | |
| A-17 | GitLab et registre de conteneurs | Service | §4, §7 | | | | |
| A-18 | Microsoft Sentinel et Defender XDR | Service | §4, §8 | | | | |
| A-19 | Front Door, WAF et API Management | Infrastructure | §4 | | | | |
| A-20 | Sauvegardes et environnement de reprise | Infrastructure | §9 | | | | |
| A-21 | Plans PCA et PRA, BIA | Documentation | §9 | | | | |
| A-22 | Contrat et annexes MSSP | Contrat | §8, §10 | | | | |
| A-23 | Postes d'administration et terminaux | Équipement | §4, §12 | | | | |
| A-24 | Messagerie et collaboration Microsoft 365 | Service | §4, §13 | | | | |
| A-25 | Personnel à privilèges (administrateurs, DevOps) | Personnes | §13 | | | | |

## À faire

- [ ] Valider les actifs proposés, en ajouter ou en retirer.
- [ ] Désigner un propriétaire (par rôle) pour chaque actif.
- [ ] Coter C, I, D pour les actifs proposés avec les mêmes niveaux que le cas.
- [ ] Appliquer la classification à quatre niveaux.
