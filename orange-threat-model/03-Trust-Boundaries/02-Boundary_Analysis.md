# 02 – Boundary Analysis

## Purpose

This document analyses the trust boundaries identified within the Orange Infrastructure Services supporting Tieto Banktech applications.

Each trust boundary represents a transition between different trust levels, ownership domains, or administrative control. Understanding these boundaries helps identify potential attack paths and determine where security controls should be applied.

---

# Boundary Analysis Overview

Trust boundaries exist where users, applications, infrastructure, administrators, or external services interact across different security domains.

Each boundary should be evaluated to determine:

- Assets crossing the boundary
- Trust relationship
- Primary threats
- Potential impact
- Security considerations

---

# Boundary Analysis

| Boundary | Trust Relationship | Primary Assets | Example Threats | Risk |
|----------|--------------------|----------------|-----------------|------|
| **TB-01** External Users → Tieto Banktech Applications | Untrusted → Trusted | User credentials, application services | Credential attacks, unauthorized access, malicious input, session hijacking | High |
| **TB-02** Tieto Banktech Applications → Orange Infrastructure Services | Application → Infrastructure | Applications, compute, storage, network | Privilege escalation, infrastructure compromise, insecure configurations | High |
| **TB-03** Orange Administrators → Orange Infrastructure Services | Privileged Administration | Infrastructure, operating systems, configuration | Privileged account compromise, insider threats, unauthorized changes | High |
| **TB-04** Orange Infrastructure Services → Logging Platform | Infrastructure → Monitoring | Audit logs, security events | Log tampering, log deletion, incomplete logging | Medium |
| **TB-05** Orange Infrastructure Services → Backup & Disaster Recovery | Infrastructure → Backup | Business data, backups | Backup corruption, ransomware, unauthorized restore | High |
| **TB-06** Orange Infrastructure Services → Security Services | Infrastructure → Security Monitoring | Security telemetry, alerts | Disabled monitoring, alert suppression, detection failures | High |
| **TB-07** Orange Infrastructure Services → External Supporting Services | Internal → External Services | DNS, NTP, PKI, Identity | DNS spoofing, certificate compromise, external dependency failure | Medium |
| **TB-08** Orange Operations Network → Orange Infrastructure Services | Operations → Production | Administrative sessions | Administrative workstation compromise, unauthorized remote access | High |
| **TB-09** Tieto Administrators → Tieto Banktech Applications *(Conditional)* | Privileged Administration | Application configuration | Unauthorized configuration changes, privilege misuse | Medium |
| **TB-10** Production ↔ Non-Production *(Conditional)* | Environment Separation | Production data | Data leakage, shared credentials, environment crossover | Medium |

---

# Trust Relationships

The following trust relationships exist within the environment.

| Trust Relationship | Description |
|--------------------|-------------|
| External User → Application | External users access trusted banking applications. |
| Application → Infrastructure | Applications depend on Orange-managed infrastructure. |
| Administrator → Infrastructure | Orange administrators manage infrastructure components. |
| Infrastructure → Logging | Infrastructure generates operational and security logs. |
| Infrastructure → Backup | Infrastructure sends backup data for business continuity. |
| Infrastructure → Security Services | Security telemetry is sent to centralized monitoring platforms. |
| Infrastructure → External Services | Infrastructure depends on external services such as DNS, NTP, PKI, and Identity Providers. |

---

# High-Risk Boundaries

The following trust boundaries represent the highest potential security risk due to privileged access, critical assets, or exposure.

- TB-01 – External Users → Tieto Banktech Applications
- TB-02 – Applications → Orange Infrastructure
- TB-03 – Orange Administrators → Infrastructure
- TB-05 – Infrastructure → Backup & Disaster Recovery
- TB-06 – Infrastructure → Security Services
- TB-08 – Orange Operations → Infrastructure

These boundaries should receive particular attention during threat analysis and control validation.

---

# Threat Modelling Considerations

The identified trust boundaries will be further analysed using:

- STRIDE
- MITRE ATT&CK
- PASTA

The objective is to identify threats, assess risk, and determine appropriate security controls for each trust boundary.

---

# Related Documents

- 01-Trust_Boundaries.md
- 03-Boundary_Controls.md
- ../04-Data-Flows/01-Data_Flows.md
- ../05-Threat-Analysis/STRIDE.md
- ../05-Threat-Analysis/MITRE_ATTACK.md
- ../05-Threat-Analysis/PASTA.md