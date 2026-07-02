# 03 – MITRE ATT&CK Mapping

## Purpose

This document maps the identified threats to the MITRE ATT&CK framework to better understand how adversaries may target the Orange Infrastructure Services supporting Tieto Banktech applications.

MITRE ATT&CK provides a knowledge base of adversary tactics and techniques observed in real-world attacks. Mapping threats to ATT&CK helps improve detection, monitoring, and defensive capabilities.

---

# MITRE ATT&CK Overview

The MITRE ATT&CK framework describes the tactics and techniques used by attackers throughout the attack lifecycle.

This threat model focuses on techniques most relevant to the Orange Infrastructure Services environment.

---

# ATT&CK Mapping

| Tactic | Example Techniques | Potential Targets |
|---------|-------------------|-------------------|
| Initial Access | Phishing, Valid Accounts, External Remote Services | External Users, Applications |
| Execution | Command Execution, Scripts | Compute, Virtual Machines |
| Persistence | Account Manipulation, Scheduled Tasks | Infrastructure, Administrative Accounts |
| Privilege Escalation | Exploitation, Abuse of Privileges | Operating Systems, Infrastructure |
| Defense Evasion | Log Deletion, Obfuscated Files, Indicator Removal | Logging Platform, Security Services |
| Credential Access | Credential Dumping, Password Attacks | Identity Services, Administrative Accounts |
| Discovery | System Discovery, Network Discovery | Compute, Network |
| Lateral Movement | Remote Services, Internal Network Access | Infrastructure Components |
| Collection | Data Collection | Storage, Applications |
| Exfiltration | Encrypted Channels, Web Services | External Network |
| Impact | Data Destruction, Service Stop, Ransomware | Compute, Storage, Backup |

---

# Threat Mapping

## External Users

Possible ATT&CK tactics:

- Initial Access
- Credential Access
- Discovery

---

## Tieto Banktech Applications

Possible ATT&CK tactics:

- Initial Access
- Execution
- Collection
- Exfiltration

---

## Orange Infrastructure Services

Possible ATT&CK tactics:

- Execution
- Persistence
- Privilege Escalation
- Lateral Movement
- Impact

---

## Logging Platform

Possible ATT&CK tactics:

- Defense Evasion
- Discovery

---

## Backup & Disaster Recovery

Possible ATT&CK tactics:

- Impact
- Collection

---

## Security Services

Possible ATT&CK tactics:

- Defense Evasion
- Credential Access

---

# High-Risk ATT&CK Tactics

The following tactics are considered the most relevant for this environment:

| Tactic | Reason |
|---------|--------|
| Initial Access | Internet-facing services and authentication endpoints |
| Credential Access | Administrative and service accounts |
| Privilege Escalation | Infrastructure administration |
| Defense Evasion | Attempts to disable logging or monitoring |
| Lateral Movement | Compromise spreading across infrastructure |
| Impact | Service disruption, ransomware, data destruction |

---

# Existing Defensive Controls

Examples include:

- Multi-Factor Authentication (MFA)
- Role-Based Access Control (RBAC)
- Network Segmentation
- Privileged Access Management (PAM)
- Centralized Logging
- SIEM
- Endpoint Protection
- Vulnerability Management
- Backup & Disaster Recovery
- Security Monitoring

---

# Detection Opportunities

Potential detection activities include:

- Failed authentication attempts
- Privileged account usage
- Unexpected administrative activity
- Log deletion or modification
- Unusual network traffic
- Malware detection
- Configuration changes
- Backup failures

---

# Relationship to Threat Modelling

This MITRE ATT&CK mapping complements:

- STRIDE Analysis by describing **how** attacks may be executed.
- PASTA Analysis by supporting attack simulation.
- Risk Assessment by identifying detection and mitigation priorities.

---

# Related Documents

- 01-Threat_Actors.md
- 02-STRIDE.md
- 04-PASTA.md
- 05-Threat_Register.md
- ../06-Risk-Assessment/Risk_Register.md