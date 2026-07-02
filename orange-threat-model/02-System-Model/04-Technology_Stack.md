# 04 – Technology Stack

## Purpose

This document identifies the primary technologies used within the Orange Infrastructure Services supporting Tieto Banktech applications.

The objective is to provide a technology inventory that supports threat modelling, vulnerability assessment, security reviews, and risk analysis.

This document focuses on technology categories rather than specific product versions or configurations.

---

# Technology Overview

Orange Infrastructure Services provide the underlying technology platform used to host and operate Tieto Banktech applications.

The technology stack consists of infrastructure, networking, storage, security, monitoring, backup, and supporting platform services.

---

# Technology Layers

The environment consists of the following technology layers:

- Compute
- Storage
- Network
- Data Centre Hosting
- Platform Services
- Security Services
- External Supporting Services

---

# Compute Technologies

Provides the processing resources required to host applications.

Typical technologies include:

- Virtual Machines
- Hypervisors
- Containers (where applicable)
- Guest Operating Systems

Primary functions:

- Application hosting
- Compute resource allocation
- Operating system execution

---

# Storage Technologies

Provides persistent storage for infrastructure and applications.

Typical technologies include:

- Block Storage
- File Storage
- Object Storage
- Snapshots

Primary functions:

- Data persistence
- Backup storage
- Application storage
- System storage

---

# Network Technologies

Provides secure connectivity between infrastructure components.

Typical technologies include:

- Firewalls
- Load Balancers
- Routers
- Switches
- VLANs
- Private Networks
- Secure Network Segmentation

Primary functions:

- Traffic routing
- Network isolation
- Secure communications
- Internet connectivity

---

# Data Centre Technologies

Provides the physical hosting environment.

Typical technologies include:

- Physical Servers
- Rack Infrastructure
- Power Distribution
- Environmental Controls
- Physical Connectivity

Primary functions:

- Infrastructure hosting
- Hardware platform
- Physical resilience

---

# Platform Technologies

Provides operational capabilities.

## Logging Platform

Typical capabilities:

- Log Collection
- Log Storage
- Audit Logging
- Operational Monitoring

---

## Backup & Disaster Recovery

Typical capabilities:

- Scheduled Backups
- Replication
- Restore Operations
- Disaster Recovery

---

## Security Services

Typical capabilities:

- Security Monitoring
- SIEM
- Endpoint Protection
- Vulnerability Management
- Threat Detection

---

# Identity Technologies

Authentication and identity services may include:

- Identity Provider
- Directory Services
- Multi-Factor Authentication
- Single Sign-On
- Role-Based Access Control

---

# Communication Technologies

Communication between components may use secure protocols including:

- HTTPS
- TLS
- SSH
- Secure administrative channels

Specific protocol implementations are outside the scope of this document.

---

# External Technologies

The environment depends on several external technology services.

Examples include:

- DNS
- NTP
- PKI / Certificate Authority
- Vendor Software Repositories

---

# Technology Classification

| Technology Area | Purpose | Managed By |
|-----------------|---------|------------|
| Compute | Application hosting | Orange |
| Storage | Persistent storage | Orange |
| Network | Connectivity | Orange |
| Data Centre | Physical hosting | Orange |
| Logging | Monitoring and audit | Orange |
| Backup & DR | Business continuity | Orange |
| Security Services | Security monitoring | Orange |
| Identity Services | Authentication | Organization / Third Party |
| DNS | Name resolution | Organization / Third Party |
| PKI | Certificate management | Organization / Third Party |

---

# Security Considerations

Each technology introduces specific security considerations that will be analysed during later stages of the threat model.

Examples include:

- Unauthorized administrative access
- Infrastructure compromise
- Network attacks
- Data exposure
- Privilege escalation
- Service disruption
- Misconfiguration
- Supply chain risks

---

# Relationship to Threat Modelling

The identified technologies provide inputs for:

- Trust Boundary Analysis
- Data Flow Analysis
- STRIDE Analysis
- MITRE ATT&CK Mapping
- PASTA Analysis
- Risk Assessment
- Security Control Evaluation

---

# Related Documents

- 01-Assets.md
- 02-Shared_Responsibility.md
- 03-Components.md
- 05-Dependencies.md
- ../03-Trust-Boundaries/Trust_Boundaries.md
- ../05-Threat-Analysis/Attack_Surface.md