# Trust Boundaries

## Purpose

This document identifies the trust boundaries within the Orange Infrastructure Services supporting Tieto Banktech.

A trust boundary represents a point where data, identities, administrative actions, or communications cross between components, systems, or organizations operating under different trust levels or security responsibilities.

Identifying trust boundaries establishes the foundation for threat identification, attack surface analysis, risk assessment, and security control evaluation.

---

# Overview

Orange provides the managed infrastructure platform hosting Tieto Banktech Applications. The environment consists of multiple security domains where trust changes between users, applications, infrastructure services, administrators, operational services, and external dependencies.

Trust boundaries help identify where security controls should be applied and where threats may emerge.

---

# Core Trust Boundaries

The following trust boundaries are considered fundamental to the Orange Infrastructure Services.

---

# TB-01 – External Users to Tieto Banktech Applications

## Description

External users access Tieto Banktech Applications hosted on Orange Infrastructure Services.

### Source

External Users

### Destination

Tieto Banktech Applications

### Assets Crossing the Boundary

- User credentials
- Authentication requests
- User sessions
- Business transactions
- Customer information

### Reason for Trust Boundary

This boundary separates external users from internal business services and represents the primary entry point into the hosted environment.

---

# TB-02 – Tieto Banktech Applications to Orange Infrastructure Services

## Description

Tieto Banktech Applications consume infrastructure services provided by Orange.

### Source

Tieto Banktech Applications

### Destination

Orange Infrastructure Services

### Assets Crossing the Boundary

- Compute resources
- Storage requests
- Network communications
- Infrastructure resources
- Application logs

### Reason for Trust Boundary

This boundary separates customer-managed applications from Orange-managed infrastructure services.

---

# TB-03 – Orange Administrators to Orange Infrastructure Services

## Description

Orange administrators perform operational, maintenance, and support activities on the managed infrastructure.

### Source

Orange Administrators

### Destination

Orange Infrastructure Services

### Assets Crossing the Boundary

- Administrative credentials
- Configuration changes
- Infrastructure management commands
- Operational activities

### Reason for Trust Boundary

This boundary protects privileged administrative access to infrastructure services.

---

# TB-04 – Orange Infrastructure Services to Orange Logging Platform

## Description

Infrastructure components generate operational and security logs that are forwarded to the centralized Orange Logging Platform.

### Source

Orange Infrastructure Services

### Destination

Orange Logging Platform

### Assets Crossing the Boundary

- Infrastructure logs
- Security logs
- Audit logs
- Monitoring events

### Reason for Trust Boundary

This boundary separates infrastructure operations from centralized logging and monitoring services.

---

# TB-05 – Orange Infrastructure Services to Orange Backup & Disaster Recovery Services

## Description

Infrastructure components exchange data with Backup & Disaster Recovery Services.

### Source

Orange Infrastructure Services

### Destination

Orange Backup & Disaster Recovery Services

### Assets Crossing the Boundary

- Backup data
- Infrastructure configurations
- Recovery information
- Backup metadata

### Reason for Trust Boundary

This boundary supports business continuity, disaster recovery, and data resilience.

---

# TB-06 – Orange Infrastructure Services to Orange Security Services

## Description

Infrastructure components communicate with centralized Orange Security Services responsible for monitoring, detection, and protection.

### Source

Orange Infrastructure Services

### Destination

Orange Security Services

### Assets Crossing the Boundary

- Security telemetry
- Detection events
- Monitoring information
- Vulnerability information
- Security alerts

### Reason for Trust Boundary

This boundary supports centralized security operations and threat detection.

---

# TB-07 – Orange Infrastructure Services to External Third-Party Services

## Description

Orange Infrastructure Services interact with trusted external services required for operational or security purposes.

### Source

Orange Infrastructure Services

### Destination

External Third-Party Services

### Assets Crossing the Boundary

- DNS requests
- Time synchronization
- Certificate validation
- Software updates
- External API communications

### Example Services

- DNS
- NTP
- Certificate Authorities
- Identity Providers
- Vendor repositories

### Reason for Trust Boundary

This boundary introduces dependencies on external trusted services that may impact security, integrity, or availability.

---

# TB-08 – Orange Operations Network to Orange Infrastructure Services

## Description

Orange operational personnel access the managed infrastructure from Orange's operational network.

### Source

Orange Operations Network

### Destination

Orange Infrastructure Services

### Assets Crossing the Boundary

- Administrative sessions
- Remote management traffic
- Infrastructure administration
- Operational commands

### Reason for Trust Boundary

This boundary protects privileged operational access between Orange's operational environment and the managed infrastructure.

---

# Conditional Trust Boundaries

The following trust boundaries should be included where applicable.

---

# TB-09 – Tieto Administrators to Tieto Banktech Applications

## Description

Tieto administrators manage, support, or maintain Tieto Banktech Applications hosted on Orange Infrastructure Services.

### Source

Tieto Administrators

### Destination

Tieto Banktech Applications

### Assets Crossing the Boundary

- Administrative credentials
- Application configuration
- Deployment packages
- Administrative sessions

### Reason for Trust Boundary

This boundary separates privileged application administration from normal application usage.

**Applicability**

Include when Tieto administrators have privileged administrative access to hosted applications.

---

# TB-10 – Environment Segregation (Production, Test, Development)

## Description

Multiple environments are segregated to prevent unauthorized access or unintended data movement between environments.

### Source

Production / Test / Development

### Destination

Production / Test / Development

### Assets Crossing the Boundary

- Application deployments
- Configuration data
- Test data
- Administrative access

### Reason for Trust Boundary

Segregation between environments reduces the risk of unauthorized access, accidental changes, and data leakage.

**Applicability**

Include when Orange Infrastructure Services host multiple isolated environments.

---

# Trust Boundary Summary

| ID | Source | Destination | Category |
|----|--------|-------------|----------|
| TB-01 | External Users | Tieto Banktech Applications | Core |
| TB-02 | Tieto Banktech Applications | Orange Infrastructure Services | Core |
| TB-03 | Orange Administrators | Orange Infrastructure Services | Core |
| TB-04 | Orange Infrastructure Services | Orange Logging Platform | Core |
| TB-05 | Orange Infrastructure Services | Orange Backup & Disaster Recovery Services | Core |
| TB-06 | Orange Infrastructure Services | Orange Security Services | Core |
| TB-07 | Orange Infrastructure Services | External Third-Party Services | Core |
| TB-08 | Orange Operations Network | Orange Infrastructure Services | Core |
| TB-09 | Tieto Administrators | Tieto Banktech Applications | Conditional |
| TB-10 | Production / Test / Development | Production / Test / Development | Conditional |

---

# Relationship to Other Documents

This document should be read together with:

- 01-Service-Context/01-Service_Scope.md
- 01-Service-Context/02-Architecture_Overview.md
- 02-System-Model/01-Assets.md
- 02-System-Model/02-Shared_Responsibility.md

The identified trust boundaries provide the basis for:

- Data Flow Analysis
- Threat Actor Identification
- Attack Surface Analysis
- STRIDE Analysis
- MITRE ATT&CK Mapping
- PASTA Analysis
- Risk Assessment
- Security Control Evaluation