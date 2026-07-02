# 02 – Data Classification

## Purpose

This document identifies and classifies the data processed, transmitted, and stored within the Orange Infrastructure Services supporting Tieto Banktech applications.

Data classification helps determine the appropriate level of protection required for information assets and supports the selection of security controls during threat modelling.

---

# Overview

The environment processes several categories of business, operational, and security information.

Each data type has different confidentiality, integrity, and availability requirements.

---

# Classification Levels

The following classification levels are used.

| Classification | Description |
|----------------|-------------|
| Public | Information approved for public disclosure. |
| Internal | Information intended for internal organizational use. |
| Confidential | Sensitive information requiring protection from unauthorized disclosure. |
| Restricted | Highly sensitive information requiring the highest level of protection. |

---

# Data Categories

## User Authentication Data

Examples

- Usernames
- Passwords
- MFA information
- Session identifiers

Classification

**Restricted**

---

## Customer Business Data

Examples

- Customer information
- Banking transactions
- Business records
- Application data

Classification

**Confidential**

---

## Application Data

Examples

- Configuration
- Runtime information
- Application metadata

Classification

**Internal**

---

## Infrastructure Configuration

Examples

- Server configuration
- Network configuration
- Infrastructure settings

Classification

**Confidential**

---

## Administrative Data

Examples

- Administrative accounts
- Privileged sessions
- Configuration changes

Classification

**Restricted**

---

## Security Logs

Examples

- Authentication logs
- Audit logs
- Security events
- System events

Classification

**Confidential**

---

## Backup Data

Examples

- System backups
- Application backups
- Configuration backups

Classification

**Restricted**

---

## Monitoring Data

Examples

- Performance metrics
- Infrastructure monitoring
- Health status
- Availability information

Classification

**Internal**

---

# Data Classification Summary

| Data Type | Classification | Stored | Transmitted |
|-----------|----------------|--------|-------------|
| User Authentication Data | Restricted | Yes | Yes |
| Customer Business Data | Confidential | Yes | Yes |
| Application Data | Internal | Yes | Yes |
| Infrastructure Configuration | Confidential | Yes | Yes |
| Administrative Data | Restricted | Yes | Yes |
| Security Logs | Confidential | Yes | Yes |
| Backup Data | Restricted | Yes | Yes |
| Monitoring Data | Internal | Yes | Yes |

---

# Protection Requirements

## Public

- No special protection required.
- Integrity should be maintained.

---

## Internal

- Access limited to authorized personnel.
- Protected against unauthorized modification.

---

## Confidential

- Encryption in transit.
- Access control.
- Logging of administrative access.
- Regular backup.

---

## Restricted

- Strong authentication.
- Least privilege.
- Encryption at rest and in transit.
- Administrative approval for access.
- Comprehensive audit logging.
- Enhanced monitoring.

---

# Security Objectives

The classified data should be protected to ensure:

- Confidentiality
- Integrity
- Availability
- Authenticity
- Accountability

---

# Relationship to Threat Modelling

Data classification supports:

- Trust Boundary Analysis
- Data Flow Analysis
- STRIDE
- MITRE ATT&CK
- PASTA
- Risk Assessment
- Security Control Selection

---

# Related Documents

- 01-Data_Flows.md
- 03-Data_Flow_Controls.md
- ../02-System-Model/01-Assets.md
- ../05-Threat-Analysis/STRIDE.md