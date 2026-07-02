# 04 – Data Flows

## Overview

The **Data Flows** section describes how information moves between users, applications, infrastructure, operational services, and external supporting services within the Orange Infrastructure Services supporting Tieto Banktech applications.

Understanding data movement is fundamental to threat modelling because threats typically exploit weaknesses where information crosses trust boundaries or moves between components.

This section identifies the primary data flows, classifies the information being processed, and documents the security controls that protect data throughout its lifecycle.

---

# Objectives

The objectives of this section are to:

- Identify the primary data flows within the environment.
- Document how data moves across trust boundaries.
- Classify information based on its sensitivity.
- Identify the security controls protecting data during transmission and processing.
- Provide input to threat analysis and risk assessment.

---

# Documents

| Document | Purpose |
|----------|---------|
| **01-Data_Flows.md** | Identifies the primary data flows between users, applications, infrastructure, platform services, and external supporting services. |
| **02-Data_Classification.md** | Classifies the information processed, transmitted, and stored within the environment according to its sensitivity. |
| **03-Data_Flow_Controls.md** | Documents the security controls protecting each data flow and supporting secure information exchange. |

---

# Relationship to Other Sections

The Data Flows section builds upon the Service Context, System Model, and Trust Boundaries and provides the foundation for Threat Analysis.

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
| **04-DataFlow.png** | High-level representation of the primary data flows between users, applications, infrastructure, platform services, operational services, and external supporting services. |

Diagrams are located in:

```
/diagrams/
```

---

# Expected Outcomes

Upon completion of this section, readers should understand:

- How information moves throughout the environment.
- Which trust boundaries are crossed by each data flow.
- The sensitivity of information being processed.
- The security controls protecting each data flow.
- The critical data flows that require additional protection.

This understanding provides the basis for identifying attack paths, evaluating threats, and selecting appropriate security controls.

---

# References

The documents within this folder provide direct input to:

- **05-Threat-Analysis**
- **06-Risk-Assessment**
- **07-Security-Controls**