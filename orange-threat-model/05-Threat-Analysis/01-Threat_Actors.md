# 01 – Threat Actors

## Purpose

This document identifies the potential threat actors that may target the Orange Infrastructure Services supporting Tieto Banktech applications.

Understanding threat actors helps evaluate attacker capabilities, motivations, attack paths, and potential impact. The identified threat actors provide input to STRIDE, MITRE ATT&CK, PASTA, and the overall risk assessment.

---

# Overview

Threat actors represent individuals, groups, or organizations capable of intentionally or unintentionally compromising the confidentiality, integrity, or availability of services hosted on the Orange Infrastructure platform.

Not all threat actors present the same level of risk. Their capabilities, objectives, and opportunities differ depending on the targeted assets and trust boundaries.

---

# Threat Actor Categories

| Threat Actor | Description | Typical Motivation | Capability | Risk |
|--------------|-------------|--------------------|------------|------|
| External Attackers | Unauthorized individuals attempting to compromise Internet-facing services. | Financial gain, disruption, data theft | Medium–High | High |
| Cybercriminal Groups | Organized groups conducting targeted attacks such as ransomware, credential theft, or extortion. | Financial gain | High | High |
| Insider Threats | Authorized personnel intentionally or unintentionally causing security incidents. | Malicious or accidental | Medium–High | High |
| Privileged Administrators | Administrators with elevated privileges over infrastructure or applications. | Misuse, compromised credentials | High | High |
| Third-Party Service Providers | External organizations providing supporting services such as DNS, PKI, or Identity Providers. | Service compromise, supply chain attacks | Medium | Medium |
| Malware / Automated Threats | Automated tools, bots, worms, and malware targeting exposed services. | Opportunistic exploitation | Medium | Medium |
| Nation-State Actors | Highly capable and well-resourced adversaries targeting critical infrastructure. | Espionage, disruption | Very High | Medium* |

> *Likelihood may be lower, but potential impact is significant.

---

# Threat Actor Objectives

Potential objectives include:

- Unauthorized access
- Credential theft
- Privilege escalation
- Data theft
- Service disruption
- Infrastructure compromise
- Ransomware deployment
- Log tampering
- Supply chain compromise
- Persistence within the environment

---

# Primary Targets

| Target | Example Threat Actors |
|---------|-----------------------|
| External-facing applications | External attackers, cybercriminals |
| Administrative interfaces | Privileged administrators, cybercriminals |
| Infrastructure services | Insider threats, nation-state actors |
| Backup systems | Ransomware operators |
| Logging platform | Insider threats, advanced attackers |
| Identity services | Credential theft groups |
| Security monitoring | Advanced attackers seeking to evade detection |

---

# High-Risk Threat Actors

The following actors represent the highest overall risk:

- External Attackers
- Cybercriminal Groups
- Insider Threats
- Privileged Administrators

These actors will be considered throughout the STRIDE, MITRE ATT&CK, and PASTA analyses.

---

# Relationship to Threat Modelling

The identified threat actors provide input to:

- STRIDE Analysis
- MITRE ATT&CK Mapping
- PASTA Analysis
- Threat Register
- Risk Assessment

---

# Related Documents

- ../03-Trust-Boundaries/02-Boundary_Analysis.md
- ../04-Data-Flows/01-Data_Flows.md
- 02-STRIDE.md
- 03-MITRE_ATTACK.md
- 04-PASTA.md
- 05-Threat_Register.md