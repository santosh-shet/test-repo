# 05 – Dependencies

## Purpose

This document identifies the technical dependencies between the components that comprise the Orange Infrastructure Services supporting Tieto Banktech applications.

Understanding these dependencies helps identify critical communication paths, potential single points of failure, trust relationships, and attack paths that will be analysed during subsequent threat modelling activities.

---

# Overview

Tieto Banktech applications depend on multiple infrastructure and platform services provided by Orange. These dependencies enable application hosting, storage, networking, security, monitoring, backup, and operational management.

The relationships described in this document represent logical dependencies rather than implementation-specific configurations.

---

# Dependency Model

```
External Users
        │
        ▼
Tieto Banktech Applications
        │
        ▼
Orange Infrastructure Services
        │
 ┌──────┼──────────┬──────────┬──────────┐
 │      │          │          │          │
 ▼      ▼          ▼          ▼          ▼
Compute Storage Network Logging Security
        │
        ▼
Backup & DR
        │
        ▼
External Services
```

---

# Component Dependencies

## External Users

Depends on:

- Tieto Banktech Applications
- Network connectivity
- Authentication services

---

## Tieto Banktech Applications

Depends on:

- Compute
- Storage
- Network
- Identity services
- Logging
- Backup
- Security services

---

## Compute

Depends on:

- Data Centre Hosting
- Storage
- Network
- Security Services
- Logging

---

## Storage

Depends on:

- Compute
- Network
- Backup
- Data Centre Hosting

---

## Network

Depends on:

- Data Centre Hosting
- Security Services
- DNS
- Routing infrastructure

---

## Logging Platform

Depends on:

- Network
- Storage
- Compute
- Security Services

Receives data from:

- Applications
- Operating Systems
- Infrastructure
- Security Services

---

## Backup & Disaster Recovery

Depends on:

- Compute
- Storage
- Network

Receives data from:

- Infrastructure
- Applications

---

## Security Services

Depends on:

- Logging
- Network
- Compute
- Identity Services

Receives information from:

- Infrastructure
- Applications
- Logging Platform

---

# External Dependencies

The following external services support the environment.

| Service | Purpose |
|----------|---------|
| DNS | Name resolution |
| NTP | Time synchronization |
| PKI / Certificate Authority | Certificate issuance and validation |
| Identity Provider | Authentication and authorization |
| Vendor Repositories | Software updates and patches |

---

# Dependency Classification

| Dependency | Category | Criticality |
|------------|----------|-------------|
| Compute | Internal | High |
| Storage | Internal | High |
| Network | Internal | High |
| Logging | Internal | High |
| Security Services | Internal | High |
| Backup & Disaster Recovery | Internal | High |
| DNS | External | Medium |
| NTP | External | Medium |
| PKI | External | High |
| Identity Provider | External | High |
| Vendor Repositories | External | Medium |

---

# Critical Dependency Paths

The following dependency chains are considered critical.

### Application Hosting

External Users

↓

Tieto Banktech Applications

↓

Compute

↓

Storage

---

### Authentication

External Users

↓

Identity Provider

↓

Tieto Banktech Applications

---

### Security Monitoring

Applications

↓

Logging Platform

↓

Security Services

---

### Business Continuity

Applications

↓

Storage

↓

Backup & Disaster Recovery

---

# Dependency Risks

Failure or compromise of dependencies may result in:

- Service disruption
- Authentication failures
- Loss of monitoring capability
- Backup failures
- Infrastructure compromise
- Data unavailability
- Security monitoring gaps

These risks will be analysed further during threat modelling and risk assessment.

---

# Relationship to Threat Modelling

Dependencies are used during:

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
- 06-Security_Zones.md
- ../03-Trust-Boundaries/Trust_Boundaries.md
- ../04-Data-Flows/Data_Flows.md