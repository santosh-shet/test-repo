# 01 – Data Flows

## Purpose

This document identifies the primary data flows within the Orange Infrastructure Services supporting Tieto Banktech applications.

Understanding how information moves between users, applications, infrastructure, platform services, and external supporting services is essential for identifying attack paths, validating trust boundaries, and performing threat modelling.

This document describes logical data flows rather than implementation-specific network traffic.

---

# Overview

Tieto Banktech applications hosted on Orange Infrastructure Services exchange data with users, infrastructure components, operational services, and external supporting services.

Each data flow crossing a trust boundary introduces potential security risks that require appropriate controls.

---

# Primary Data Flows

| ID | Source | Destination | Data |
|----|--------|-------------|------|
| DF-01 | External Users | Tieto Banktech Applications | User requests, authentication credentials, business transactions |
| DF-02 | Tieto Banktech Applications | Orange Infrastructure Services | Application execution, system requests |
| DF-03 | Orange Infrastructure Services | Logging Platform | System logs, audit logs, security events |
| DF-04 | Orange Infrastructure Services | Backup & Disaster Recovery | Backup data, configuration data, recovery data |
| DF-05 | Orange Infrastructure Services | Security Services | Security telemetry, alerts, monitoring events |
| DF-06 | Orange Infrastructure Services | External Supporting Services | DNS queries, time synchronization, certificate validation, authentication requests |
| DF-07 | Orange Operations | Orange Infrastructure Services | Administrative actions, configuration changes, monitoring activities |

---

# Data Flow Description

## DF-01 — External Users → Tieto Banktech Applications

Purpose

- User authentication
- Business transactions
- Application access

Typical data

- User credentials
- Session information
- Business requests

---

## DF-02 — Tieto Banktech Applications → Orange Infrastructure Services

Purpose

- Application hosting
- Compute processing
- Storage access
- Network communication

Typical data

- Application traffic
- System requests
- Storage operations

---

## DF-03 — Orange Infrastructure Services → Logging Platform

Purpose

- Centralized logging
- Security monitoring
- Audit trail generation

Typical data

- System logs
- Security events
- Administrative activities

---

## DF-04 — Orange Infrastructure Services → Backup & Disaster Recovery

Purpose

- Backup
- Recovery
- Business continuity

Typical data

- Backup images
- Configuration
- Recovery information

---

## DF-05 — Orange Infrastructure Services → Security Services

Purpose

- Security monitoring
- Threat detection
- Alert generation

Typical data

- Security telemetry
- Events
- Alerts

---

## DF-06 — Orange Infrastructure Services → External Supporting Services

Purpose

- Name resolution
- Time synchronization
- Certificate validation
- Identity verification

Typical data

- DNS requests
- NTP requests
- Certificate validation
- Authentication requests

---

## DF-07 — Orange Operations → Orange Infrastructure Services

Purpose

- Infrastructure administration
- Monitoring
- Maintenance
- Configuration

Typical data

- Administrative commands
- Configuration updates
- Operational information

---

# High-Risk Data Flows

The following data flows are considered critical due to the sensitivity of the data or the privileges involved.

| Data Flow | Risk |
|-----------|------|
| DF-01 | High |
| DF-02 | High |
| DF-04 | High |
| DF-05 | High |
| DF-07 | High |

---

# Relationship to Trust Boundaries

Each data flow crosses one or more trust boundaries identified in the Trust Boundaries section.

| Data Flow | Trust Boundary |
|-----------|----------------|
| DF-01 | TB-01 |
| DF-02 | TB-02 |
| DF-03 | TB-04 |
| DF-04 | TB-05 |
| DF-05 | TB-06 |
| DF-06 | TB-07 |
| DF-07 | TB-08 |

---

# Security Considerations

Each data flow should be evaluated for:

- Authentication
- Authorization
- Confidentiality
- Integrity
- Availability
- Logging
- Monitoring
- Encryption
- Input validation
- Error handling

These considerations provide input to the subsequent threat analysis.

---

# Related Documents

- ../03-Trust-Boundaries/01-Trust_Boundaries.md
- ../03-Trust-Boundaries/02-Boundary_Analysis.md
- 02-Data_Classification.md
- 03-Data_Flow_Controls.md
- ../05-Threat-Analysis/STRIDE.md