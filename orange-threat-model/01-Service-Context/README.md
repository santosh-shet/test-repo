# 01 – Service Context

## Overview

The **Service Context** establishes the business and architectural foundation for the threat model. It describes the service being assessed, its purpose, business importance, dependencies, assumptions, and assessment boundaries.

Understanding the service context ensures that subsequent threat modelling activities are performed within the correct business and technical scope.

---

# Objectives

The objectives of this section are to:

- Define the scope of the threat model.
- Describe the business purpose of the service.
- Provide a high-level architectural overview.
- Identify key service dependencies.
- Document assumptions used throughout the assessment.
- Clearly identify items outside the scope of the threat model.

---

# Documents

| Document | Purpose |
|----------|---------|
| **01-Service_Scope.md** | Defines the overall scope, objectives, in-scope and out-of-scope services for the assessment. |
| **02-Architecture_Overview.md** | Provides a high-level overview of the Orange Infrastructure Services supporting Tieto Banktech applications. |
| **03-Business_Context.md** | Describes the business objectives, stakeholders, critical business functions, and business impact of the service. |
| **04-Service_Dependencies.md** | Identifies internal and external service dependencies required to operate the platform. |
| **05-Service_Assumptions.md** | Documents the assumptions on which the threat model is based. |
| **06-Out_of_Scope.md** | Defines systems, services, responsibilities, and activities excluded from this threat model. |

---

# Relationship to Other Sections

The Service Context provides the foundation for the remainder of the threat model.

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

The following architecture diagrams support this section.

| Diagram | Description |
|----------|-------------|
| **01-Context.png** | High-level overview of the service, stakeholders, and hosting model. |
| **02-Logical.png** | Logical architecture of Orange Infrastructure Services supporting Tieto Banktech applications. |

Diagrams are located in:

```
/diagrams/
```

---

# Expected Outcomes

Upon completion of this section, readers should understand:

- What service is being threat modelled.
- Why the service exists.
- The business objectives it supports.
- The high-level architecture.
- The major service dependencies.
- The assumptions made during the assessment.
- The boundaries of the threat model.

This understanding provides the context required for the technical analysis performed in the subsequent sections.

---

# References

The documents within this folder serve as inputs to:

- **02-System-Model**
- **03-Trust-Boundaries**
- **04-Data-Flows**
- **05-Threat-Analysis**
- **06-Risk-Assessment**