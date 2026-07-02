# 03 – Components

## Purpose

This document identifies the major components that make up the Orange Infrastructure Services supporting Tieto Banktech applications.

The objective is to establish a common understanding of the system architecture by describing the primary infrastructure, application, operational, and supporting components that participate in the delivery of the service.

The identified components provide the basis for trust boundary analysis, data flow analysis, attack surface identification, and threat modelling.

---

# Component Overview

The environment consists of components managed by both Tieto Banktech and Orange Infrastructure Services.

The components collectively provide the infrastructure required to host, secure, monitor, and operate the banking applications.

---

# Component Categories

The system consists of the following logical component groups:

- External Components
- Application Components
- Infrastructure Components
- Platform Services
- Operational Components
- External Supporting Services

---

# External Components

## External Users

Represents customers, users, and external systems accessing Tieto Banktech applications.

### Responsibilities

- Access banking applications
- Authenticate to services
- Submit business transactions

---

# Application Components

## Tieto Banktech Applications

Business applications hosted on Orange Infrastructure Services.

### Responsibilities

- Banking services
- Business logic
- API processing
- Authentication
- Transaction processing

---

# Infrastructure Components

## Compute

Provides the processing resources required to host applications.

Examples include:

- Virtual Machines
- Containers
- Hypervisors

---

## Storage

Provides persistent storage.

Examples include:

- Block Storage
- File Storage
- Object Storage
- Snapshots

---

## Network

Provides connectivity between infrastructure and applications.

Examples include:

- Firewalls
- Load Balancers
- Routing
- VLANs

---

## Data Centre Hosting

Provides physical infrastructure.

Includes:

- Physical Servers
- Rack Infrastructure
- Power
- Cooling
- Physical Connectivity

---

# Platform Services

## Logging Platform

Provides centralized collection of operational and security logs.

Typical functions include:

- Log collection
- Log storage
- Monitoring
- Audit logging

---

## Backup & Disaster Recovery

Provides business continuity capabilities.

Functions include:

- Backup
- Replication
- Restore
- Disaster Recovery

---

## Security Services

Provides centralized security capabilities.

Examples include:

- Security Monitoring
- SIEM
- Endpoint Protection
- Vulnerability Management
- Threat Detection

---

# Operational Components

## Orange Operations

Responsible for operating and maintaining the infrastructure.

Typical activities include:

- Monitoring
- Incident Management
- Patch Management
- Backup Operations
- Change Management

---

## Orange Administrators

Responsible for privileged administration of infrastructure components.

Typical activities include:

- Infrastructure administration
- Configuration management
- Maintenance
- Operational support

---

# External Supporting Services

The platform depends on several external services.

Examples include:

- DNS
- NTP
- PKI / Certificate Authority
- Identity Provider
- Vendor Software Repositories

---

# Component Relationships

The logical relationship between the components is illustrated below.

```
External Users
        │
        ▼
Tieto Banktech Applications
        │
        ▼
Orange Infrastructure Services
        │
 ┌──────┼──────────┬──────────────┐
 │      │          │              │
 ▼      ▼          ▼              ▼
Compute Storage Network Data Centre
        │
        ▼
Platform Services
        │
 ┌──────┼──────────┐
 │      │          │
 ▼      ▼          ▼
Logging Backup Security

        │
        ▼

External Services
```

---

# Security Relevance

Each component represents a potential attack surface and will be analysed during:

- Trust Boundary Analysis
- Data Flow Analysis
- STRIDE Analysis
- MITRE ATT&CK Mapping
- PASTA Analysis
- Risk Assessment

---

# Related Documents

- 01-Assets.md
- 02-Shared_Responsibility.md
- ../03-Trust-Boundaries/Trust_Boundaries.md
- ../04-Data-Flows/Data_Flows.md
- ../05-Threat-Analysis/Threat_Actors.md