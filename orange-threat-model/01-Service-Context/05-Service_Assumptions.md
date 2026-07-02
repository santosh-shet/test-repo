# 05 – Service Assumptions

## Purpose

This document records the assumptions made during the threat modelling exercise for Orange Infrastructure Services supporting Tieto Banktech applications.

These assumptions define the expected operating conditions and security baseline used throughout the threat model. If any assumption changes, the threat model should be reviewed and updated accordingly.

---

# Assumptions Overview

The following assumptions are considered valid at the time this threat model was created.

---

# Business Assumptions

- Orange provides managed infrastructure services for Tieto Banktech.
- Tieto Banktech owns and manages the hosted applications.
- Orange is responsible for infrastructure operations within the agreed service scope.
- Security responsibilities are shared between Orange and Tieto Banktech.
- Business services hosted on the platform require high availability.

---

# Infrastructure Assumptions

- Compute resources are provisioned and managed by Orange.
- Storage infrastructure is managed by Orange.
- Network infrastructure is managed by Orange.
- Physical data centre facilities are managed by Orange.
- Backup and disaster recovery services are available.
- Centralized logging services are available.
- Security monitoring services are operational.

---

# Administrative Access Assumptions

- Administrative access is restricted to authorized personnel.
- Administrative accounts are individually assigned.
- Administrative activities are logged.
- Privileged access follows the principle of least privilege.
- Administrative access is protected using strong authentication mechanisms.

---

# Network Assumptions

- Internal network segmentation is implemented.
- Internet-facing services are protected using appropriate network security controls.
- Administrative access is separated from customer access where applicable.
- Network traffic between components uses secure communication protocols where appropriate.

---

# Identity and Access Management Assumptions

- User identities are uniquely assigned.
- Authentication mechanisms are centrally managed.
- Access permissions are reviewed periodically.
- Service accounts are managed according to organizational procedures.
- Administrative identities are managed separately from standard user accounts.

---

# Logging Assumptions

- Security events are logged.
- Administrative activities are logged.
- System logs are centrally collected.
- Log integrity is protected.
- Time synchronization is maintained across systems.

---

# Backup and Recovery Assumptions

- Backup processes operate successfully according to defined schedules.
- Backup data is protected against unauthorized access.
- Recovery procedures are documented.
- Disaster recovery procedures are periodically tested.

---

# Security Operations Assumptions

- Vulnerability management processes are established.
- Security monitoring is operational.
- Security incidents are managed through defined incident response procedures.
- Security patches are deployed through change management processes.

---

# External Service Assumptions

The following services are assumed to be available when required:

- DNS
- NTP
- PKI / Certificate Authority
- Identity Provider
- Vendor software repositories

---

# Trust Assumptions

The threat model assumes:

- Orange Infrastructure Services operate according to documented security procedures.
- Authorized administrators perform activities using approved management interfaces.
- Security controls operate as designed.
- Trusted communications remain protected against unauthorized modification.
- Changes follow approved change management procedures.

---

# Assumption Validation

These assumptions should be reviewed whenever:

- Service scope changes.
- New infrastructure components are introduced.
- Responsibilities change between Orange and Tieto Banktech.
- Significant architectural changes occur.
- New third-party dependencies are introduced.
- Major security incidents occur.

---

# Risks if Assumptions Become Invalid

If one or more assumptions are no longer valid, potential impacts include:

- Increased attack surface.
- Incorrect threat analysis.
- Inaccurate risk assessment.
- Missing security controls.
- Undetected attack paths.
- Reduced effectiveness of mitigations.

The threat model should be updated whenever assumptions change.

---

# Related Documents

- 01-Service_Scope.md
- 02-Architecture_Overview.md
- 03-Business_Context.md
- 04-Service_Dependencies.md
- 06-Out_of_Scope.md
- ../02-System-Model/Shared_Responsibilities.md