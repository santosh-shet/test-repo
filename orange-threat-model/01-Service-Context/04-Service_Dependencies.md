# 04 – Service Dependencies

## Purpose

This document identifies the internal and external dependencies required for the operation of the Orange Infrastructure Services supporting Tieto Banktech applications.

Understanding these dependencies helps identify potential attack paths, trust boundaries, single points of failure, and security considerations during threat modelling.

---

# Service Dependency Overview

Tieto Banktech applications rely on Orange Infrastructure Services to provide the underlying platform required to host, operate, monitor, secure, and recover business services.

The environment also depends on several supporting services provided by Orange and external service providers.

---

# High-Level Dependency Model

```
External Users
        │
        ▼
Tieto Banktech Applications
        │
        ▼
Orange Infrastructure Services
        │
 ┌──────┼───────────┬──────────┬─────────────┐
 │      │           │          │             │
 ▼      ▼           ▼          ▼             ▼
Compute Storage   Network   Logging   Backup & DR
        │
        ▼
Security Services

        │
        ▼

External Dependencies
```

---

# Internal Dependencies

## Compute Services

Provides virtual infrastructure used to host Tieto Banktech applications.

Examples include:

- Virtual Machines
- Containers
- Hypervisors
- Compute clusters

---

## Storage Services

Provides persistent storage for applications and platform services.

Examples include:

- Block Storage
- File Storage
- Object Storage
- Snapshots

---

## Network Services

Provides connectivity between components.

Examples include:

- Firewalls
- Load Balancers
- Routing
- VLANs
- Private Networks

---

## Data Centre Hosting

Provides physical hosting facilities.

Includes:

- Physical servers
- Rack infrastructure
- Power
- Cooling
- Physical security

---

## Backup and Disaster Recovery

Supports business continuity through:

- Scheduled backups
- Replication
- Restore capabilities
- Disaster recovery

---

## Logging Platform

Provides centralized logging.

Typical log sources include:

- Operating systems
- Infrastructure
- Applications
- Security devices
- Administrative activities

---

## Security Services

Provides security capabilities including:

- Security monitoring
- SIEM
- Vulnerability Management
- Endpoint Protection
- Threat Detection

---

# Operational Dependencies

The service relies on operational processes including:

- Infrastructure administration
- Monitoring
- Incident response
- Patch management
- Change management
- Backup operations
- Capacity management

---

# External Dependencies

## Identity Provider

Provides authentication and identity services for administrators and applications.

---

## DNS Services

Provides hostname resolution required for application and infrastructure communications.

---

## NTP Services

Provides synchronized time across infrastructure components.

---

## PKI / Certificate Authority

Supports:

- TLS certificates
- Certificate validation
- Secure communications

---

## Vendor Repositories

Provides:

- Software packages
- Security updates
- Platform patches

---

# Dependency Classification

| Dependency | Type | Managed By |
|------------|------|------------|
| Compute | Internal | Orange |
| Storage | Internal | Orange |
| Network | Internal | Orange |
| Data Centre | Internal | Orange |
| Backup & DR | Internal | Orange |
| Logging Platform | Internal | Orange |
| Security Services | Internal | Orange |
| Identity Provider | External | Organization / Third Party |
| DNS | External | Organization / Third Party |
| NTP | External | Organization / Third Party |
| PKI / Certificate Authority | External | Organization / Third Party |
| Vendor Repositories | External | Software Vendors |

---

# Critical Dependencies

The following dependencies are considered critical for service availability and security:

- Compute Services
- Storage Services
- Network Services
- Identity Services
- Logging Platform
- Security Services
- Backup & Disaster Recovery

Failure of one or more of these dependencies may significantly impact the availability, integrity, or confidentiality of the service.

---

# Security Considerations

Each dependency introduces potential risks that should be considered during threat modelling.

Examples include:

- Compromise of privileged access.
- Service unavailability.
- Network compromise.
- DNS manipulation.
- Certificate compromise.
- Supply chain attacks.
- Logging failures.
- Backup failures.
- Identity service compromise.

These dependencies will be analysed further during:

- Trust Boundary Analysis
- Data Flow Analysis
- STRIDE Analysis
- MITRE ATT&CK Mapping
- PASTA Threat Modelling

---

# Related Documents

- 01-Service_Scope.md
- 02-Architecture_Overview.md
- 03-Business_Context.md
- ../02-System-Model/Assets.md
- ../03-Trust-Boundaries/Trust_Boundaries.md
- ../04-Data-Flows/Data_Flows.md