# 02 – STRIDE Analysis

## Purpose

This document applies the STRIDE threat modelling methodology to the Orange Infrastructure Services supporting Tieto Banktech applications.

STRIDE provides a structured approach for identifying potential threats affecting system components, trust boundaries, and data flows.

The objective is to identify threats early, evaluate potential impact, and support the selection of appropriate security controls.

---

# STRIDE Overview

STRIDE categorizes threats into six classes.

| Category | Description |
|----------|-------------|
| **S – Spoofing** | Impersonating a legitimate user, service, or system. |
| **T – Tampering** | Unauthorized modification of data, software, or configuration. |
| **R – Repudiation** | Performing actions without sufficient evidence or auditability. |
| **I – Information Disclosure** | Unauthorized exposure of sensitive information. |
| **D – Denial of Service** | Reducing or preventing system availability. |
| **E – Elevation of Privilege** | Gaining permissions beyond those intended. |

---

# STRIDE Analysis

| Component | S | T | R | I | D | E |
|----------|---|---|---|---|---|---|
| External Users | ✓ | | | | | |
| Tieto Banktech Applications | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ |
| Compute | | ✓ | | ✓ | ✓ | ✓ |
| Storage | | ✓ | | ✓ | ✓ | ✓ |
| Network | ✓ | ✓ | | ✓ | ✓ | ✓ |
| Data Centre Hosting | | ✓ | | | ✓ | ✓ |
| Logging Platform | | ✓ | ✓ | ✓ | ✓ | |
| Backup & Disaster Recovery | | ✓ | | ✓ | ✓ | |
| Security Services | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ |
| Orange Administrators | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ |
| External Supporting Services | ✓ | ✓ | | ✓ | ✓ | |

---

# Threat Analysis

## Spoofing

### Examples

- Credential theft
- Session hijacking
- Service impersonation
- DNS spoofing
- Administrator impersonation

Typical targets

- User authentication
- Identity Provider
- Administrative interfaces

---

## Tampering

### Examples

- Configuration modification
- Infrastructure manipulation
- Backup modification
- Log alteration
- Software replacement

Typical targets

- Compute
- Storage
- Logging
- Backup
- Configuration

---

## Repudiation

### Examples

- Missing audit logs
- Deleted administrative logs
- Untracked configuration changes

Typical targets

- Logging Platform
- Administrative activities

---

## Information Disclosure

### Examples

- Sensitive data exposure
- Backup disclosure
- Credential leakage
- Log disclosure

Typical targets

- Storage
- Backups
- Logs
- Applications

---

## Denial of Service

### Examples

- Network flooding
- Resource exhaustion
- Service outage
- Infrastructure failure

Typical targets

- Network
- Compute
- Applications

---

## Elevation of Privilege

### Examples

- Administrator compromise
- Misconfigured permissions
- Privilege escalation vulnerabilities
- Service account abuse

Typical targets

- Infrastructure
- Administrative accounts
- Operating systems

---

# High Priority Threats

The following threats are considered the highest priority.

| Threat | STRIDE |
|---------|---------|
| Credential compromise | Spoofing |
| Infrastructure compromise | Elevation of Privilege |
| Log tampering | Tampering |
| Backup compromise | Information Disclosure |
| Ransomware | Denial of Service |
| Privileged account misuse | Elevation of Privilege |
| Unauthorized configuration changes | Tampering |

---

# Existing Mitigations

Examples include:

- Multi-Factor Authentication (MFA)
- Role-Based Access Control (RBAC)
- Least Privilege
- Network Segmentation
- Secure Configuration
- Patch Management
- Centralized Logging
- Security Monitoring
- Backup Protection
- Incident Response

---

# Residual Risks

Residual risks may remain due to:

- Zero-day vulnerabilities
- Insider threats
- Supply chain attacks
- Human error
- Third-party service failures

These risks are addressed further in the Risk Assessment section.

---

# Relationship to Threat Modelling

The identified STRIDE threats provide direct input to:

- MITRE ATT&CK Mapping
- PASTA Analysis
- Threat Register
- Risk Assessment

---

# Related Documents

- 01-Threat_Actors.md
- 03-MITRE_ATTACK.md
- 04-PASTA.md
- 05-Threat_Register.md