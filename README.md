# Security Home Lab

![Status](https://img.shields.io/badge/status-in%20progress-brightgreen) ![Focus](https://img.shields.io/badge/focus-SOC%20%7C%20SIEM%20%7C%20IAM%20%7C%20DevSecOps%20%7C%20GRC-blue)

Hands-on security labs and projects I build, break, and document to go beyond theory: detection engineering, identity and access management, secure delivery pipelines, offensive/defensive exercises in my own isolated environment, and governance, risk, and compliance (GRC) work.

## About me

Nesrine, Computer Engineering student (Network Infrastructure & Data Security) at ESPRIT, with a background in SOC operations, identity management, GRC, and full-stack development. Cisco CyberOps Associate and Cisco Network Security certified.

This repo documents practical labs and projects that back up what is on my CV: real deployments, real configs, real screenshots, real deliverables, not just tool names.

## Labs and projects

| # | Lab / Project | Focus | Stack | Status |
|---|---|---|---|---|
| 01 | [SIEM Home Lab](01-siem-home-lab/) | Detection engineering, log analysis, active response | Wazuh, VMware, Windows 11, Ubuntu 22.04 | ✅ Documented |
| 02 | Healthcare IAM Lab | Identity lifecycle, SSO and MFA, Active Directory hardening | Active Directory, Keycloak, midPoint, PingCastle | 🚧 To document |
| 03 | MediShield SOC | SOC design, alert enrichment, automated incident response, HIPAA audit | Wazuh, Elastic/Kibana, Shuffle, TheHive, Cortex, MISP | 🚧 To document |
| 04 | DevSecOps Pipeline | Shift-left security in CI/CD, supply-chain traceability | GitLab CI, Docker, Gitleaks, Semgrep, SonarQube, Trivy, CycloneDX, OWASP ZAP | 🚧 To document |
| 05 | [ISO 27001 ISMS: Carthago FinTech (GRC)](05-iso27001-carthago-fintech/) | Risk assessment, Statement of Applicability, policies, KPIs | ISO/IEC 27001:2022, Excel registers, Markdown and PDF documents | 🚧 In progress |

Each lab folder contains its own README with objective, architecture, step-by-step setup, results, and lessons learned. Labs marked "To document" are built and are being written up; their folders appear here as they are published.

## What each lab demonstrates

| Lab / Project | What I built or proved |
|---|---|
| 01 SIEM Home Lab | Full Wazuh deployment (manager, indexer, dashboard) with Windows and Linux agents, real-time file integrity monitoring, custom SSH decoders and rules with escalating severity for brute force, and an Active Response firewall-drop validated with a simulated SSH attack |
| 02 Healthcare IAM Lab | Active Directory with tiered administration (10 OUs, 14 groups, 7 GPOs), Keycloak SSO (OIDC/SAML, MFA) federated to AD, midPoint for joiner-mover-leaver automation, AD security review with PingCastle |
| 03 MediShield SOC | End-to-end SOC chain (collection, correlation, case management, enrichment, threat intelligence sharing), custom Wazuh rules to cut false positives, 3 automated response playbooks, and a HIPAA-oriented audit with 15 findings, a risk register, and a compliance mapping |
| 04 DevSecOps Pipeline | GitLab CI pipeline for an intentionally vulnerable Flask app: secret detection, SAST, code quality, dependency and image scanning, DAST, SBOM generation, and a pre-commit hook that blocks secrets before they reach the repo |
| 05 ISO 27001 ISMS | Implementation case study for a fictional payment company: 45 gaps analysed against ISO 27001 clauses 4 to 10, 12 scored risks with written justification, a 36-action treatment plan, a Statement of Applicability covering the 93 Annex A controls, an access-control policy, and KPIs |

## What each lab follows

Technical labs (01 to 04):

- **Objective** - what the lab sets out to demonstrate
- **Architecture** - diagram and machine specs
- **Implementation** - step-by-step, with screenshots
- **Results** - what worked and what it proves
- **Challenges & lessons learned** - real problems hit and how they were solved

GRC projects (05):

- **Context** - the organisation, scope, and requirements
- **Method** - how risks are assessed and decisions are made
- **Deliverables** - registers, policies, and reports
- **Assumptions & limits** - what comes from the case and what is a hypothesis

## Repository structure

```
security-homelab/
├── README.md                  <- you are here
├── 01-siem-home-lab/
│   ├── README.md
│   ├── architecture.puml
│   ├── configs/
│   ├── screenshots/
│   └── test-logs/
├── 02-healthcare-iam-lab/
│   └── ...
├── 03-medishield-soc/
│   └── ...
├── 04-devsecops-pipeline/
│   └── ...
├── 05-iso27001-carthago-fintech/
│   ├── README.md
│   ├── docs/
│   ├── registres/
│   └── sources/               <- local only, never published
└── ...
```

## Disclaimer

All labs are built and tested in isolated, self-owned environments (local VMs). No external systems are targeted. Scenarios such as hospitals or companies are fictional and used for learning. Reference documents (standards, case statements) are protected and are not included in this repository. Any credentials, API keys, or sensitive data are removed before publishing.

## Connect

I am looking for a 6-month end-of-studies (PFE) internship in cybersecurity starting January 2027. If you are reviewing this for a PFE, internship, or role, feel free to reach out on [LinkedIn](https://www.linkedin.com/in/nesrine-riahi-8a1b032a0) or open an issue with questions about any lab.
