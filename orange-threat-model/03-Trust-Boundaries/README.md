# 03 – Trust Boundaries

## Overview

The **Trust Boundaries** section identifies and analyses the logical trust boundaries within the Orange Infrastructure Services supporting Tieto Banktech applications.

A trust boundary exists whenever communication, data, or administrative control crosses between different trust levels, ownership domains, or security zones. These boundaries represent areas where additional security controls are typically required to reduce the risk of unauthorized access, privilege escalation, data compromise, or service disruption.

This section establishes the foundation for the subsequent threat analysis using STRIDE, MITRE ATT&CK, and PASTA.

---

# Objectives

The objectives of this section are to:

- Identify logical trust boundaries within the environment.
- Analyse interactions between different trust domains.
- Understand potential attack paths across trust boundaries.
- Identify security controls protecting each boundary.
- Support data flow analysis and threat modelling activities.

---

# Documents

| Document | Purpose |
|----------|---------|
| **01-Trust_Boundaries.md** | Identifies the trust boundaries (TB-01 to TB-10) within the Orange Infrastructure Services environment and describes the interactions between trust domains. |
| **02-Boundary_Analysis.md** | Analyses each trust boundary, including trust relationships, protected assets, potential threats, and security considerations. |
| **03-Boundary_Controls.md** | Documents the security controls implemented to protect each trust boundary and identifies residual risks. |

---

# Relationship to Other Sections

The Trust Boundaries section builds upon the Service Context and System Model and provides the foundation for Data Flow Analysis and Threat Analysis.

```
Service Context
        │
        ▼
System Model
        │
        ▼
Trust Boundaries
        │
        ▼
Data Flows
        │
        ▼
Threat Analysis
        │
        ▼
Risk Assessment
        │
        ▼
Security Controls
        │
        ▼
Validation
```

---

# Diagrams

The following diagram supports this section.

| Diagram | Description |
|----------|-------------|
| **03-TrustBoundaries.png** | High-level view of the trust boundaries, trust domains, and interactions between Tieto Banktech applications, Orange Infrastructure Services, administrators, and external supporting services. |

Diagrams are located in:

```
/diagrams/
```

---

# Expected Outcomes

Upon completion of this section, readers should understand:

- The logical trust boundaries within the environment.
- Where trust changes occur.
- Which assets are protected by each boundary.
- Which users, systems, and services cross each boundary.
- The primary risks associated with each trust boundary.
- The security controls protecting each boundary.

This information provides the basis for identifying attack paths and performing structured threat analysis.

---

# References

The documents within this folder provide direct input to:

- **04-Data-Flows**
- **05-Threat-Analysis**
- **06-Risk-Assessment**
```