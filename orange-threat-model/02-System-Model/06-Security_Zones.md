# 06 – Security Zones

## Purpose

This document defines the logical security zones within the Orange Infrastructure Services supporting Tieto Banktech applications.

Security zones group components with similar trust levels and security requirements. Identifying these zones supports trust boundary identification, attack surface analysis, network segmentation, and security control placement.

This document focuses on logical security segmentation rather than physical or network implementation.

---

# Security Zone Overview

The environment is divided into multiple logical security zones based on function, ownership, administrative access, and exposure.

Each zone has a different security posture and trust level.

---

# Security Zone Architecture

```
                        Internet
                            │
                            ▼

+--------------------------------------------------------+
| Zone 1 - External Users                               |
+--------------------------------------------------------+

                            │

                            ▼

+--------------------------------------------------------+
| Zone 2 - Tieto Banktech Applications                  |
+--------------------------------------------------------+

                            │

                            ▼

+--------------------------------------------------------+
| Zone 3 - Orange Infrastructure Services               |
|                                                        |
| • Compute                                              |
| • Storage                                              |
| • Network                                               |
| • Data Centre Hosting                                  |
+--------------------------------------------------------+

            │                 │                │

            ▼                 ▼                ▼

+---------------+   +----------------+   +----------------+
| Zone 4        |   | Zone 5         |   | Zone 6         |
| Logging       |   | Backup & DR    |   | Security       |
| Platform      |   |                |   | Services       |
+---------------+   +----------------+   +----------------+

                            │

                            ▼

+--------------------------------------------------------+
| Zone 7 - Orange Operations                            |
+--------------------------------------------------------+

                            │

                            ▼

+--------------------------------------------------------+
| Zone 8 - External Supporting Services                 |
| DNS | NTP | PKI | Identity Provider                   |
+--------------------------------------------------------+
```

---

# Zone Descriptions

## Zone 1 – External Users

### Description

Represents customers, business users, and external systems accessing Tieto Banktech applications.

### Characteristics

- Untrusted
- Internet-facing
- Authentication required
- Limited privileges

---

## Zone 2 – Tieto Banktech Applications

### Description

Business applications owned and managed by Tieto Banktech.

### Characteristics

- Business processing
- API services
- Authentication
- Transaction processing

### Primary Assets

- Applications
- Business logic
- Customer data
- API endpoints

---

## Zone 3 – Orange Infrastructure Services

### Description

Core managed infrastructure hosting the applications.

### Components

- Compute
- Storage
- Network
- Data Centre Hosting

### Characteristics

- Managed by Orange
- Internal infrastructure
- High-value assets
- Restricted administrative access

---

## Zone 4 – Logging Platform

### Description

Centralized collection of operational and security logs.

### Characteristics

- Audit logging
- Event collection
- Monitoring
- Investigation support

---

## Zone 5 – Backup & Disaster Recovery

### Description

Provides backup, replication, restore, and disaster recovery capabilities.

### Characteristics

- Business continuity
- Recovery services
- Long-term data protection

---

## Zone 6 – Security Services

### Description

Provides centralized security capabilities.

### Components

- Security Monitoring
- SIEM
- Endpoint Protection
- Vulnerability Management
- Threat Detection

---

## Zone 7 – Orange Operations

### Description

Represents Orange operational personnel responsible for managing infrastructure.

### Responsibilities

- Monitoring
- Incident response
- Change management
- Infrastructure administration
- Operational support

---

## Zone 8 – External Supporting Services

### Description

External services supporting infrastructure operations.

### Components

- DNS
- NTP
- PKI / Certificate Authority
- Identity Provider
- Vendor Software Repositories

---

# Trust Level

| Zone | Trust Level |
|-------|-------------|
| External Users | Low |
| Tieto Banktech Applications | Medium |
| Orange Infrastructure Services | High |
| Logging Platform | High |
| Backup & Disaster Recovery | High |
| Security Services | High |
| Orange Operations | High |
| External Supporting Services | Medium |

---

# Communication Between Zones

| Source Zone | Destination Zone | Purpose |
|-------------|------------------|---------|
| External Users | Tieto Banktech Applications | User access |
| Tieto Banktech Applications | Orange Infrastructure Services | Application hosting |
| Orange Infrastructure Services | Logging Platform | Log forwarding |
| Orange Infrastructure Services | Backup & Disaster Recovery | Backup and restore |
| Orange Infrastructure Services | Security Services | Security monitoring |
| Orange Operations | Orange Infrastructure Services | Infrastructure administration |
| Orange Infrastructure Services | External Supporting Services | DNS, NTP, PKI, Identity |

---

# Security Objectives

The security zones support the following objectives:

- Network segmentation
- Least privilege
- Separation of duties
- Administrative isolation
- Secure communications
- Monitoring and auditing
- Controlled access between zones

---

# Relationship to Threat Modelling

Security zones provide the basis for:

- Trust Boundary Analysis
- Data Flow Analysis
- Attack Surface Identification
- STRIDE Analysis
- MITRE ATT&CK Mapping
- PASTA Analysis
- Risk Assessment

---

# Related Documents

- 01-Assets.md
- 02-Shared_Responsibility.md
- 03-Components.md
- 04-Technology_Stack.md
- 05-Dependencies.md
- ../03-Trust-Boundaries/01-Trust_Boundaries.md
- ../04-Data-Flows/01-Data_Flows.md