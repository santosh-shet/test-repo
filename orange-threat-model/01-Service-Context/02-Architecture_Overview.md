# Architecture Overview

## Purpose

This document provides a high-level overview of the Orange managed infrastructure services supporting Tietoevry Banking. It identifies the primary infrastructure components and their relationships to establish a common understanding before threat identification.

---

# High-Level Architecture

```
                         Users
                           │
                           │
                    Customer Network
                           │
──────────────────────── Trust Boundary ────────────────────────
                           │
                    Orange Network Services
                           │
        ┌──────────────────┼──────────────────┐
        │                  │                  │
     Compute           Storage          Security Services
        │                  │                  │
        └──────────────────|──────────────────┘
                           │
                Logging & Monitoring
                           │
                           │
              Backup & Disaster Recovery
                           │
                           │
                 Data Centre Hosting
```

---

# Infrastructure Components

## Compute

Provides virtual and physical compute resources hosting customer workloads.

Typical components include:

- Physical Servers
- Virtual Machines
- Hypervisors
- Operating Systems

---

## Storage

Provides persistent storage services supporting hosted workloads.

Typical components include:

- Block Storage
- File Storage
- Storage Arrays
- Storage Replication

---

## Network

Provides secure connectivity between infrastructure components and external consumers.

Typical components include:

- Routers
- Switches
- Firewalls
- VPN
- Load Balancers

---

## Backup & Disaster Recovery

Provides business continuity capabilities through backup, restoration and disaster recovery services.

Typical components include:

- Backup Repositories
- Replication
- Recovery Services
- Disaster Recovery Sites

---

## Logging

Provides centralized collection and monitoring of infrastructure logs.

Typical capabilities include:

- Log Collection
- Log Aggregation
- Monitoring
- Alerting
- Log Retention

---

## Security Services

Provides security capabilities protecting the managed infrastructure.

Typical capabilities include:

- Identity and Access Management
- Endpoint Protection
- Vulnerability Management
- Security Monitoring
- Security Operations

---

## Data Centre Hosting

Provides physical facilities supporting the managed infrastructure.

Typical capabilities include:

- Physical Security
- Rack Infrastructure
- Power
- Cooling
- Environmental Monitoring

---

# Key Interactions

The infrastructure services operate together to support customer workloads.

- Compute relies on Network connectivity.
- Compute consumes Storage services.
- Infrastructure components generate logs collected by the Logging service.
- Security Services monitor infrastructure events.
- Backup & Disaster Recovery protects hosted workloads and infrastructure configurations.
- Data Centre Hosting provides the physical environment supporting all infrastructure services.

---

# Scope

This architecture overview is intended to provide sufficient context for:

- Asset identification
- Trust boundary analysis
- Data flow analysis
- STRIDE threat analysis
- Risk assessment

Detailed implementation and configuration information is outside the scope of this document.