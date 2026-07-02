# 04 – PASTA Analysis

## Purpose

This document applies the **Process for Attack Simulation and Threat Analysis (PASTA)** methodology to the Orange Infrastructure Services supporting Tieto Banktech applications.

PASTA is a risk-centric threat modelling methodology that helps identify realistic attack scenarios, evaluate business impact, and prioritize security improvements based on risk.

The analysis builds upon the Service Context, System Model, Trust Boundaries, Data Flows, STRIDE Analysis, and MITRE ATT&CK Mapping completed in the previous sections.

---

# PASTA Overview

PASTA consists of seven stages.

| Stage | Description |
|--------|-------------|
| Stage 1 | Define Business Objectives |
| Stage 2 | Define Technical Scope |
| Stage 3 | Application Decomposition |
| Stage 4 | Threat Analysis |
| Stage 5 | Weakness & Vulnerability Analysis |
| Stage 6 | Attack Modelling & Simulation |
| Stage 7 | Risk Analysis & Treatment |

---

# Stage 1 – Business Objectives

The primary business objectives are to:

- Protect Tieto Banktech applications.
- Maintain confidentiality, integrity, and availability.
- Ensure reliable infrastructure operations.
- Support regulatory and contractual requirements.
- Minimize operational disruption.

Reference:

- 01-Service-Context

---

# Stage 2 – Technical Scope

The assessment covers:

- Orange Infrastructure Services
- Compute
- Storage
- Network
- Data Centre Hosting
- Logging Platform
- Backup & Disaster Recovery
- Security Services

Excluded components are documented in:

- 01-Service-Context/06-Out_of_Scope.md

---

# Stage 3 – Application Decomposition

The environment consists of:

- External Users
- Tieto Banktech Applications
- Orange Infrastructure Services
- Orange Operations
- External Supporting Services

The following architectural artifacts support this stage:

- Context Diagram
- Logical Architecture
- Trust Boundaries
- Data Flows

---

# Stage 4 – Threat Analysis

Threats identified during STRIDE include:

- Credential compromise
- Privilege escalation
- Infrastructure compromise
- Log tampering
- Information disclosure
- Service disruption
- Backup compromise
- Unauthorized administrative access

Threat actors include:

- External attackers
- Cybercriminals
- Insider threats
- Privileged administrators
- Third-party service providers

---

# Stage 5 – Weakness & Vulnerability Analysis

Potential weaknesses include:

- Weak authentication
- Excessive privileges
- Misconfiguration
- Unpatched systems
- Insufficient logging
- Inadequate monitoring
- Insecure backup protection
- Weak network segmentation
- Third-party dependency risks

These weaknesses should be validated through vulnerability management and security assessments.

---

# Stage 6 – Attack Modelling & Simulation

Example attack scenarios include:

### Scenario 1

Compromise of an administrative account resulting in unauthorized infrastructure access.

---

### Scenario 2

Ransomware attack targeting production workloads and backup infrastructure.

---

### Scenario 3

Credential theft followed by lateral movement across infrastructure components.

---

### Scenario 4

Compromise of an external supporting service leading to unauthorized access or service disruption.

---

### Scenario 5

Deletion or manipulation of audit logs to evade detection.

---

# Stage 7 – Risk Analysis & Treatment

Identified risks should be evaluated based on:

- Likelihood
- Business impact
- Existing controls
- Residual risk

Risk treatment options include:

- Reduce risk
- Transfer risk
- Accept risk
- Avoid risk

Detailed risk information is maintained in:

- ../06-Risk-Assessment/Risk_Register.md

---

# PASTA Summary

| Stage | Status |
|--------|--------|
| Business Objectives | Completed |
| Technical Scope | Completed |
| Application Decomposition | Completed |
| Threat Analysis | Completed |
| Weakness Analysis | Completed |
| Attack Modelling | Completed |
| Risk Analysis | Ongoing |

---

# Relationship to Threat Modelling

PASTA consolidates the outputs from:

- Service Context
- System Model
- Trust Boundaries
- Data Flows
- STRIDE
- MITRE ATT&CK

The output supports prioritization of risks and implementation of security controls.

---

# Related Documents

- 01-Threat_Actors.md
- 02-STRIDE.md
- 03-MITRE_ATTACK.md
- 05-Threat_Register.md
- ../06-Risk-Assessment/Risk_Register.md