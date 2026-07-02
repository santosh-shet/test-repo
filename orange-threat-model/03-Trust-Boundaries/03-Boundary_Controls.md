# 03 – Boundary Controls

## Purpose

This document identifies the primary security controls implemented to protect the trust boundaries within the Orange Infrastructure Services supporting Tieto Banktech applications.

The controls described in this document are intended to reduce the likelihood of unauthorized access, data compromise, privilege escalation, and service disruption when data or administrative actions cross trust boundaries.

---

# Control Objectives

The objectives of the trust boundary controls are to:

- Prevent unauthorized access across trust boundaries.
- Ensure only authenticated and authorized entities cross trust boundaries.
- Protect the confidentiality, integrity, and availability of information.
- Detect malicious or abnormal activities.
- Support monitoring, auditing, and incident response.

---

# Boundary Controls

| Boundary | Primary Controls |
|----------|------------------|
| **TB-01** External Users → Tieto Banktech Applications | TLS encryption, Authentication, MFA (where applicable), Session Management, Input Validation, Web Application Firewall (WAF), Rate Limiting |
| **TB-02** Tieto Banktech Applications → Orange Infrastructure Services | Network Segmentation, Secure Configuration, Least Privilege, Patch Management, Host Hardening |
| **TB-03** Orange Administrators → Orange Infrastructure Services | Privileged Access Management (PAM), Multi-Factor Authentication (MFA), Administrative Logging, Role-Based Access Control (RBAC), Session Monitoring |
| **TB-04** Orange Infrastructure Services → Logging Platform | Secure Log Transport, Log Integrity Protection, Time Synchronization, Access Controls, Log Retention |
| **TB-05** Orange Infrastructure Services → Backup & Disaster Recovery | Backup Encryption, Immutable Backups (where applicable), Restore Validation, Backup Monitoring, Access Controls |
| **TB-06** Orange Infrastructure Services → Security Services | Security Monitoring, SIEM Integration, Endpoint Protection, Threat Detection, Alerting |
| **TB-07** Orange Infrastructure Services → External Supporting Services | Secure DNS, Certificate Validation, TLS, Service Authentication, Availability Monitoring |
| **TB-08** Orange Operations Network → Orange Infrastructure Services | Secure Administrative Network, Bastion Hosts (where applicable), MFA, Administrative Session Logging, Device Hardening |
| **TB-09** Tieto Administrators → Tieto Banktech Applications *(Conditional)* | RBAC, MFA, Change Management, Administrative Logging |
| **TB-10** Production ↔ Non-Production *(Conditional)* | Environment Segregation, Separate Credentials, Data Masking, Network Isolation |

---

# Common Security Controls

The following controls apply across multiple trust boundaries.

## Identity and Access Management

- Strong authentication
- Multi-Factor Authentication (MFA)
- Role-Based Access Control (RBAC)
- Least Privilege
- Periodic access reviews

---

## Network Security

- Network segmentation
- Firewalls
- Secure communication protocols (TLS)
- Restricted administrative access
- Network monitoring

---

## System Security

- Secure configuration baselines
- Patch management
- Vulnerability management
- Endpoint protection
- Malware protection

---

## Monitoring and Logging

- Centralized logging
- Security event monitoring
- SIEM integration
- Audit logging
- Alert generation

---

## Data Protection

- Encryption in transit
- Encryption at rest (where applicable)
- Backup protection
- Secure key and certificate management

---

## Operational Security

- Change management
- Incident response
- Backup verification
- Disaster recovery testing
- Configuration management

---

# Control Effectiveness

The effectiveness of trust boundary controls should be periodically validated through:

- Security reviews
- Vulnerability assessments
- Penetration testing
- Configuration reviews
- Log reviews
- Access reviews
- Disaster recovery exercises

---

# Residual Risk

Despite the implemented controls, residual risks may remain, including:

- Compromise of privileged accounts
- Zero-day vulnerabilities
- Insider threats
- Third-party service outages
- Human error
- Supply chain risks

These residual risks should be evaluated as part of the overall risk assessment process.

---

# Related Documents

- 01-Trust_Boundaries.md
- 02-Boundary_Analysis.md
- ../04-Data-Flows/01-Data_Flows.md
- ../05-Threat-Analysis/STRIDE.md
- ../06-Risk-Assessment/Risk_Register.md