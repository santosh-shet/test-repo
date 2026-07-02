# 02 – System Model

## Overview

The **System Model** describes the technical architecture of the Orange Infrastructure Services supporting Tieto Banktech applications. It identifies the assets, components, technologies, dependencies, ownership, and logical security zones that form the environment being assessed.

This section establishes a shared understanding of the system before analysing trust boundaries, data flows, threats, and risks.

---

# Objectives

The objectives of this section are to:

- Identify the assets within the scope of the threat model.
- Define ownership and operational responsibilities.
- Describe the logical system components.
- Document the technology stack supporting the environment.
- Identify technical dependencies between components.
- Define logical security zones within the architecture.

---

# Documents

| Document | Purpose |
|----------|---------|
| **01-Assets.md** | Identifies the information assets, infrastructure assets, and supporting services that require protection. |
| **02-Shared_Responsibility.md** | Defines the shared responsibilities between Tieto Banktech and Orange Infrastructure Services. |
| **03-Components.md** | Describes the major logical components that comprise the environment. |
| **04-Technology_Stack.md** | Documents the technology categories supporting the hosted services. |
| **05-Dependencies.md** | Identifies the technical dependencies and relationships between system components. |
| **06-Security_Zones.md** | Defines the logical security zones used for segmentation and threat modelling. |

---

# Relationship to Other Sections

The System Model builds upon the Service Context and provides the technical foundation for the remainder of the threat model.

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
| **02-Logical.png** | Logical architecture of Orange Infrastructure Services supporting Tieto Banktech applications. |

Diagrams are located in:

```
/diagrams/
```

---

# Expected Outcomes

Upon completion of this section, readers should understand:

- The assets within the scope of the assessment.
- The ownership and operational responsibilities for each component.
- The logical components that make up the environment.
- The technology stack supporting the hosted services.
- The technical dependencies between components.
- The logical security zones that define the system architecture.

This information provides the technical baseline for identifying trust boundaries, analysing data flows, and performing threat modelling.

---

# References

The documents within this folder provide direct input to:

- **03-Trust-Boundaries**
- **04-Data-Flows**
- **05-Threat-Analysis**
- **06-Risk-Assessment**