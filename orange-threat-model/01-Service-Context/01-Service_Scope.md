# Orange Service Scope

## Purpose

This document defines the scope of the Orange infrastructure services included in the threat modelling exercise. It establishes the system boundaries, identifies the primary infrastructure services, and clarifies what is included and excluded from the assessment.

---

# Service Overview

Orange provides managed infrastructure services supporting Tieto Banktech environments. These services form the underlying platform hosting business applications and supporting operational capabilities.

The services covered by this threat model include:

- Compute
- Storage
- Network
- Backup & Disaster Recovery
- Data Centre Hosting
- Logging
- Security Services

---

# Objectives

The objectives of this threat model are to:

- Understand the Orange service landscape.
- Identify security-relevant infrastructure components.
- Establish the scope for threat identification.
- Define trust boundaries between Orange, Tieto, and external entities.
- Support consistent security assessments across Orange managed services.

---

# In Scope

The following managed infrastructure services are included:

## Compute

- Physical servers
- Virtual machines
- Hypervisor platforms
- Operating systems
- Infrastructure management

## Storage

- SAN/NAS
- Block storage
- File storage
- Storage replication
- Storage encryption

## Network

- Routers
- Switches
- Firewalls
- VPN
- Load balancers
- Network segmentation

## Backup & Disaster Recovery

- Backup infrastructure
- Recovery procedures
- Replication
- Backup repositories
- Disaster recovery capabilities

## Data Centre Hosting

- Physical facilities
- Rack infrastructure
- Power
- Cooling
- Physical access controls

## Logging

- Log collection
- Log aggregation
- SIEM integration
- Log retention
- Monitoring

## Security Services

- Identity and Access Management
- Endpoint Protection
- Security Monitoring
- Security Operations

---

# Out of Scope

The following are outside the scope of this threat model:

- Customer-developed applications
- Application source code
- Business logic
- End-user devices
- Third-party SaaS applications not managed by Orange
- Business processes

---

# Assumptions

The following assumptions apply:

- Orange is responsible for delivering managed infrastructure services.
- Tieto is responsible for customer workloads deployed on the platform unless otherwise agreed.
- Existing contractual and operational security controls remain in place.
- Threat modelling focuses on infrastructure services rather than application-specific functionality.

---

# Expected Outcome

This document provides the foundation for:

- Architecture modelling
- Asset identification
- Trust boundary identification
- STRIDE threat analysis
- Risk assessment