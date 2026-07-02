# 03 – Data Flow Controls

## Purpose

This document identifies the primary security controls implemented to protect data as it moves between users, applications, infrastructure, and supporting services within the Orange Infrastructure Services supporting Tieto Banktech applications.

The controls described in this document help ensure the confidentiality, integrity, availability, and accountability of data throughout its lifecycle.

---

# Overview

Data traverses multiple trust boundaries while being processed by Tieto Banktech applications and Orange Infrastructure Services.

Each data flow requires appropriate security controls based on:

- Data sensitivity
- Trust boundary crossed
- Business criticality
- Regulatory requirements

---

# Data Flow Controls

| Data Flow | Primary Controls |
|-----------|------------------|
| **DF-01** External Users → Tieto Banktech Applications | TLS, Authentication, MFA (where applicable), Session Management, Input Validation, Rate Limiting, WAF |
| **DF-02** Tieto Banktech Applications → Orange Infrastructure Services | Secure Network Segmentation, RBAC, TLS (where applicable), Host Hardening, Least Privilege |
| **DF-03** Orange Infrastructure Services → Logging Platform | Secure Log Transport, Time Synchronization, Log Integrity Protection, Access Controls |
| **DF-04** Orange Infrastructure Services → Backup & Disaster Recovery | Backup Encryption, Backup Integrity Validation, Access Controls, Restore Testing |
| **DF-05** Orange Infrastructure Services → Security Services | Secure Telemetry Transfer, SIEM Integration, Event Validation, Alert Monitoring |
| **DF-06** Orange Infrastructure Services → External Supporting Services | Secure DNS, Certificate Validation, TLS, Authentication, Availability Monitoring |
| **DF-07** Orange Operations → Orange Infrastructure Services | MFA, Privileged Access Management (PAM), Administrative Logging, Bastion Host (where applicable), Session Monitoring |

---

# Authentication Controls

Authentication controls help ensure that only authorized users and systems initiate data flows.

Typical controls include:

- Strong authentication
- Multi-Factor Authentication (MFA)
- Service account management
- Identity verification
- Session timeout

---

# Authorization Controls

Authorization controls ensure users and systems can access only the resources required for their role.

Typical controls include:

- Role-Based Access Control (RBAC)
- Least Privilege
- Administrative separation
- Periodic access reviews

---

# Communication Security

Data transmitted between components should be protected using secure communication mechanisms.

Typical controls include:

- TLS encryption
- Secure administrative protocols
- Certificate validation
- Secure API communication

---

# Integrity Controls

Integrity controls help ensure data cannot be modified without authorization.

Typical controls include:

- Message integrity validation
- Audit logging
- Configuration management
- File integrity monitoring

---

# Confidentiality Controls

Sensitive information should be protected during transmission and storage.

Typical controls include:

- Encryption in transit
- Encryption at rest (where applicable)
- Access controls
- Secure key management

---

# Availability Controls

Availability controls reduce the risk of service disruption.

Typical controls include:

- Redundant infrastructure
- Backup and restore
- Disaster recovery
- Monitoring and alerting
- Capacity management

---

# Monitoring Controls

Monitoring provides visibility into data movement and potential security events.

Typical controls include:

- Centralized logging
- SIEM
- Security monitoring
- Alert generation
- Audit trail collection

---

# Data Flow Validation

The effectiveness of data flow controls should be periodically validated through:

- Configuration reviews
- Security monitoring
- Access reviews
- Vulnerability assessments
- Penetration testing
- Disaster recovery testing
- Log reviews

---

# Residual Risks

Despite the implemented controls, the following risks may remain:

- Compromise of privileged accounts
- Misconfiguration
- Zero-day vulnerabilities
- Third-party service failures
- Human error
- Supply chain attacks
- Insider threats

Residual risks should be evaluated as part of the overall risk assessment process.

---

# Relationship to Threat Modelling

The identified controls provide input to:

- STRIDE Analysis
- MITRE ATT&CK Mapping
- PASTA Analysis
- Risk Assessment
- Security Control Evaluation

---

# Related Documents

- 01-Data_Flows.md
- 02-Data_Classification.md
- ../03-Trust-Boundaries/03-Boundary_Controls.md
- ../05-Threat-Analysis/STRIDE.md
- ../06-Risk-Assessment/Risk_Register.md