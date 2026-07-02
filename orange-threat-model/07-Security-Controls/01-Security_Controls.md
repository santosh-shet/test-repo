# 01 – Security Controls

## Purpose

This document identifies the primary security controls that protect the Orange Infrastructure Services supporting Tieto Banktech applications.

The controls described in this document reduce the likelihood and impact of the threats identified during the threat modelling exercise. They provide a baseline for protecting infrastructure, applications, administrative access, and supporting services.

---

# Overview

Security controls are implemented across multiple layers of the environment to protect information assets, infrastructure components, and business services.

The controls described in this document represent high-level security capabilities rather than implementation-specific configurations.

---

# Control Categories

The security controls are grouped into the following categories:

- Identity and Access Management
- Network Security
- Infrastructure Security
- Data Protection
- Logging and Monitoring
- Backup and Recovery
- Operational Security

---

# Identity and Access Management

The following controls help ensure that only authorized users and administrators can access systems.

Examples include:

- Strong authentication
- Multi-Factor Authentication (MFA)
- Role-Based Access Control (RBAC)
- Least Privilege
- Privileged Access Management (PAM)
- Periodic access reviews

---

# Network Security

Network controls protect communications between users, applications, and infrastructure.

Examples include:

- Network segmentation
- Firewalls
- Secure remote administration
- Load balancing
- Secure communication protocols (TLS)
- Network traffic filtering

---

# Infrastructure Security

Infrastructure controls reduce the risk of compromise of compute, storage, and network resources.

Examples include:

- Secure configuration baselines
- Patch management
- Vulnerability management
- Endpoint protection
- Malware protection
- Configuration management

---

# Data Protection

Controls protecting sensitive information include:

- Encryption in transit
- Encryption at rest (where applicable)
- Secure key and certificate management
- Access controls
- Data classification

---

# Logging and Monitoring

Security monitoring supports the detection and investigation of security events.

Examples include:

- Centralized logging
- Security Information and Event Management (SIEM)
- Audit logging
- Security event monitoring
- Alert generation

---

# Backup and Recovery

Business continuity controls include:

- Regular backups
- Backup encryption
- Restore testing
- Disaster recovery planning
- Backup monitoring

---

# Operational Security

Operational controls help maintain a secure environment.

Examples include:

- Change management
- Incident response
- Security monitoring
- Capacity management
- Periodic security reviews

---

# Control Summary

| Control Area | Primary Objective |
|--------------|-------------------|
| Identity & Access Management | Prevent unauthorized access |
| Network Security | Protect communications |
| Infrastructure Security | Protect compute, storage, and network resources |
| Data Protection | Protect sensitive information |
| Logging & Monitoring | Detect and investigate security events |
| Backup & Recovery | Support business continuity |
| Operational Security | Maintain secure operations |

---

# Relationship to Threat Modelling

The security controls documented in this section mitigate threats identified through:

- STRIDE
- MITRE ATT&CK
- PASTA
- Risk Assessment

---

# Related Documents

- ../05-Threat-Analysis/05-Threat_Register.md
- ../06-Risk-Assessment/01-Risk_Register.md
- 02-Detection_and_Monitoring.md
- 03-Control_Validation.md