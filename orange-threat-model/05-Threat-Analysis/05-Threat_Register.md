# 05 – Threat Register

## Purpose

This document consolidates the threats identified during the threat modelling exercise for the Orange Infrastructure Services supporting Tieto Banktech applications.

The Threat Register provides a centralized view of identified threats, affected assets, attack vectors, existing controls, and recommended mitigations. It serves as the primary input for the Risk Assessment.

---

# Overview

Threats have been identified using:

- Service Context
- System Model
- Trust Boundaries
- Data Flows
- STRIDE
- MITRE ATT&CK
- PASTA

Each threat is assigned a unique identifier for tracking throughout the risk management process.

---

# Threat Register

| ID | Threat | Asset | STRIDE | MITRE ATT&CK | Likelihood | Impact | Existing Controls | Recommended Mitigation |
|----|---------|-------|---------|---------------|------------|--------|-------------------|------------------------|
| TH-001 | Credential compromise | User Accounts | Spoofing | Credential Access | Medium | High | MFA, Password Policy | Monitor failed logins, strengthen authentication |
| TH-002 | Unauthorized application access | Applications | Spoofing | Initial Access | Medium | High | Authentication, RBAC | Regular access reviews |
| TH-003 | Infrastructure compromise | Compute | Elevation of Privilege | Privilege Escalation | Medium | High | Hardening, Patch Management | Continuous vulnerability management |
| TH-004 | Network compromise | Network | Tampering | Lateral Movement | Medium | High | Firewalls, Segmentation | Review network segmentation regularly |
| TH-005 | Log tampering | Logging Platform | Tampering | Defense Evasion | Low | High | Centralized Logging | Log integrity monitoring |
| TH-006 | Backup compromise | Backup & DR | Information Disclosure | Impact | Medium | High | Backup Encryption | Immutable backups, restore testing |
| TH-007 | Security monitoring bypass | Security Services | Defense Evasion | Defense Evasion | Low | High | SIEM, Monitoring | Continuous alert validation |
| TH-008 | Privileged account misuse | Administrative Accounts | Elevation of Privilege | Valid Accounts | Medium | High | PAM, MFA | Privileged session monitoring |
| TH-009 | DNS or Identity service compromise | External Services | Spoofing | Initial Access | Low | High | Secure DNS, PKI | Redundant trusted services |
| TH-010 | Denial of Service | Network / Applications | Denial of Service | Impact | Medium | High | Load Balancing, Monitoring | Capacity planning and DDoS protection |

---

# Threat Summary

| Category | Number of Threats |
|----------|-------------------|
| Spoofing | 3 |
| Tampering | 2 |
| Repudiation | 0 |
| Information Disclosure | 1 |
| Denial of Service | 1 |
| Elevation of Privilege | 2 |
| Defense Evasion | 1 |

---

# Highest Priority Threats

The following threats require the highest priority for mitigation:

- TH-001 Credential compromise
- TH-003 Infrastructure compromise
- TH-005 Log tampering
- TH-006 Backup compromise
- TH-008 Privileged account misuse
- TH-010 Denial of Service

---

# Risk Treatment

Each identified threat should be evaluated during the Risk Assessment process to determine the appropriate treatment.

Possible treatment options include:

- Mitigate
- Accept
- Transfer
- Avoid

The selected treatment and any residual risk should be documented in the Risk Register.

---

# Review and Maintenance

The Threat Register should be reviewed:

- Following significant architectural changes.
- After major security incidents.
- Following infrastructure changes.
- During periodic security reviews.
- When new threats or vulnerabilities are identified.

---

# Related Documents

- 01-Threat_Actors.md
- 02-STRIDE.md
- 03-MITRE_ATTACK.md
- 04-PASTA.md
- ../06-Risk-Assessment/Risk_Register.md