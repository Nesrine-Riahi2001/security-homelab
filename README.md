# Security Home Lab

![Status](https://img.shields.io/badge/status-in%20progress-brightgreen) ![Focus](https://img.shields.io/badge/focus-SOC%20%7C%20SIEM%20%7C%20IAM-blue)

Hands-on security labs I build, break, and document to go beyond theory: detection engineering, identity and access management, and offensive/defensive exercises in my own isolated environment.

## About me

Nesrine - Computer Engineering student (Network Infrastructure & Data Security), with a background in SOC operations and full-stack development. Cisco CyberOps Associate and Network Security certified.

This repo is where I document practical labs that back up what's on my CV: real deployments, real configs, real screenshots, not just tool names.

## Labs

| # | Lab | Focus | Stack | Status |
|---|---|---|---|---|
| 01 | [SIEM Home Lab](01-siem-home-lab/) | Detection engineering, log analysis, active response | Wazuh, VMware, Windows 11, Ubuntu 22.04 | ✅ Documented |
| 02 | Healthcare IAM Lab | Identity & access management, AD hardening | Active Directory, Keycloak, midPoint, PingCastle | 🚧 To document |
| 03 | `<next lab>` | `<topic>` | `<stack>` | 🔜 Planned |

Each lab folder contains its own README with objective, architecture, step-by-step setup, results, and lessons learned.

## What each lab follows

- **Objective** - what the lab sets out to demonstrate
- **Architecture** - diagram and machine specs
- **Implementation** - step-by-step, with screenshots
- **Results** - what worked and what it proves
- **Challenges & lessons learned** - real problems hit and how they were solved

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
└── ...
```

## Disclaimer

All labs are built and tested in isolated, self-owned environments (local VMs). No external systems are targeted. Any credentials, API keys, or sensitive data are removed before publishing.

## Connect

If you're reviewing this for a PFE, internship, or role - feel free to reach out via LinkedIn or open an issue with questions about any lab.