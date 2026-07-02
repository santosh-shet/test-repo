# Orange Infrastructure Services Threat Model

## Overview

This repository contains the threat model for the **Orange Infrastructure Services** supporting **Tieto Banktech Applications**.

The threat model provides a structured approach for understanding the service architecture, identifying assets, defining trust boundaries, analysing threats, assessing risks, documenting security controls, and supporting continuous improvement.

The repository is intended to serve as a living document that evolves alongside changes to the infrastructure, applications, and threat landscape.

---

# Objectives

The objectives of this threat model are to:

- Understand the architecture and service context.
- Identify critical assets requiring protection.
- Define trust boundaries and data flows.
- Identify potential threats using established threat modelling methodologies.
- Assess risks based on likelihood and business impact.
- Document security controls protecting the environment.
- Support security reviews and continuous improvement.

---

# Scope

This threat model covers the Orange Infrastructure Services used to host and support Tieto Banktech applications, including:

- Compute
- Storage
- Network
- Data Centre Hosting
- Backup & Disaster Recovery
- Logging Platform
- Security Services

Application development, business processes, and customer-managed systems are outside the scope of this repository.

---

# Threat Modelling Methodologies

The repository applies multiple complementary threat modelling methodologies.

| Methodology | Purpose |
|-------------|---------|
| STRIDE | Identify security threats affecting components and data flows |
| MITRE ATT&CK | Map threats to adversary tactics and techniques |
| PASTA | Perform risk-centric threat analysis |

---

# Repository Structure

```
orange-threat-model/
│
├── README.md
├── LICENSE
├── .gitignore
├── Glossary.md
│
├── diagrams/
│
├── 01-Service-Context/
├── 02-System-Model/
├── 03-Trust-Boundaries/
├── 04-Data-Flows/
├── 05-Threat-Analysis/
├── 06-Risk-Assessment/
├── 07-Security-Controls/
├── 08-Validation/
│
└── appendices/
```

---

# Folder Overview

| Folder | Description |
|----------|-------------|
| 01-Service-Context | Business context, scope, architecture, assumptions |
| 02-System-Model | Assets, components, technologies, dependencies |
| 03-Trust-Boundaries | Trust boundary identification and protection |
| 04-Data-Flows | Information flows, classification, protection |
| 05-Threat-Analysis | Threat actors, STRIDE, MITRE ATT&CK, PASTA, Threat Register |
| 06-Risk-Assessment | Risk evaluation, prioritization, treatment |
| 07-Security-Controls | Preventive, detective, and corrective controls |
| 08-Validation | Review, open issues, continuous improvement |
| diagrams | Supporting architecture and threat modelling diagrams |
| appendices | References, acronyms, version history |

---

# Architecture Diagrams

The following diagrams support the threat model.

| Diagram | Description |
|----------|-------------|
| 01-Context.png | Service context |
| 02-Logical.png | Logical architecture |
| 03-TrustBoundaries.png | Trust boundaries |
| 04-DataFlow.png | Data flow overview |
| 05-STRIDE.png | STRIDE analysis |
| 06-MITRE-ATTACK.png | MITRE ATT&CK mapping |
| 07-PASTA.png | PASTA methodology |

---

# Intended Audience

This repository is intended for:

- Security Architects
- Enterprise Architects
- Infrastructure Engineers
- Orange Infrastructure Teams
- Tieto Banktech Teams
- Security Operations
- Risk Managers
- Auditors

---

# Repository Maintenance

The threat model should be reviewed whenever:

- Architecture changes
- New services are introduced
- Significant security incidents occur
- New threats emerge
- Major infrastructure changes are implemented
- Regulatory requirements change

---

# References

Additional references are available in:

```
appendices/
```

---

> [!CAUTION]
> # **Confidential – Internal Use Only**
>
> This repository contains confidential information relating to the Orange Infrastructure Services supporting Tieto Banktech applications.
> Distribution outside Tieto requires appropriate authorization.