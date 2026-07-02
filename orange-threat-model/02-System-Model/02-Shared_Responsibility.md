# Shared Responsibility Model

## Purpose

This document defines the shared security responsibilities between Orange and Tieto for the managed infrastructure services supporting Tieto Banktech.

The objective is to clearly identify ownership and operational responsibilities for infrastructure, platforms, applications, and data, ensuring that security controls, threat ownership, and risk treatment activities are assigned to the appropriate party during the threat modelling process.

---

# Overview

Orange provides and manages the underlying infrastructure services that host Tieto Banktech workloads.

Tieto is responsible for the business applications, business data, and application-level security deployed on the Orange managed infrastructure.

Threat modelling activities should consider both responsibilities when identifying threats, assessing risks, and recommending security controls.

---

# Responsibility Matrix

| Component | Orange | Tieto | Notes |
|-----------|:------:|:---------:|------|
| Data Centre Facilities | ✓ | | Physical facilities, power, cooling and environmental controls |
| Physical Security | ✓ | | Physical access to infrastructure |
| Physical Servers | ✓ | | Hardware lifecycle and maintenance |
| Hypervisors | ✓ | | Virtualization platform |
| Virtual Machines | ✓ | | Provisioning, maintenance and lifecycle |
| Operating Systems | ✓ | | Installation, patching and hardening |
| Storage Infrastructure | ✓ | | SAN, NAS, storage management |
| Network Infrastructure | ✓ | | Routers, switches, firewalls and load balancers |
| Backup Infrastructure | ✓ | | Backup platform and recovery services |
| Disaster Recovery Infrastructure | ✓ | | DR platform and infrastructure |
| Central Logging Platform | ✓ | | Log collection and retention platform |
| Security Services | ✓ | | Monitoring, endpoint protection and infrastructure security |
| Infrastructure Monitoring | ✓ | | Availability and operational monitoring |
| Infrastructure Vulnerability Management | ✓ | | Infrastructure vulnerability management |
| Business Applications | | ✓ | Banktech applications and supporting services |
| Application Configuration | | ✓ | Application settings and configuration |
| Customer Data | | ✓ | Business and customer information |
| Application Security | | ✓ | Secure development and application controls |
| Business Roles & Permissions | | ✓ | Application authorization model |
| Application Logging Configuration | | ✓ | Business event logging |
| Application Secrets & Certificates | | ✓ | Application certificates, secrets and cryptographic material |

---

# Shared Security Activities

The following security activities require collaboration between Orange and Tieto.

| Activity | Orange | Tieto |
|----------|:------:|:---------:|
| Incident Response | ✓ | ✓ |
| Security Incident Investigation | ✓ | ✓ |
| Change Management | ✓ | ✓ |
| Security Reviews | ✓ | ✓ |
| Disaster Recovery Testing | ✓ | ✓ |
| Backup Validation | ✓ | ✓ |
| Major Security Incident Communication | ✓ | ✓ |
| Risk Assessments | ✓ | ✓ |
| Threat Modelling | ✓ | ✓ |

---

# Responsibility Principles

The following principles apply throughout the managed service.

- Orange is responsible for protecting and operating the managed infrastructure.
- Tieto is responsible for protecting the applications, business services and business data deployed on the managed infrastructure.
- Both organisations are responsible for effective collaboration during security incidents, investigations and recovery activities.
- Security controls should be implemented by the party responsible for the affected service or asset.
- Shared security responsibilities should be documented, reviewed and agreed by both organisations.

---

# Threat Modelling Considerations

The shared responsibility model supports threat modelling by:

- Defining ownership of infrastructure and business assets.
- Identifying which organisation is responsible for implementing security controls.
- Supporting assignment of risks and mitigation actions.
- Reducing ambiguity when analysing threats that span organisational boundaries.

---

# References

This document should be read together with:

- Service_Scope.md
- Architecture_Overview.md
- Assets.md
- Trust_Boundaries.md