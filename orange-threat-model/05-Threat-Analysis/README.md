# 05 – Threat Analysis

## Overview

The **Threat Analysis** section identifies, analyses, and documents the threats relevant to the Orange Infrastructure Services supporting Tieto Banktech applications.

This section applies multiple threat modelling methodologies to ensure comprehensive coverage of potential attack vectors, adversary behaviors, and business risks.

The objective is to identify realistic threats, understand how they could affect the environment, and provide the foundation for risk assessment and security control selection.

---

# Objectives

The objectives of this section are to:

- Identify potential threat actors.
- Analyze threats using the STRIDE methodology.
- Map adversary techniques to the MITRE ATT&CK framework.
- Perform a risk-centric analysis using the PASTA methodology.
- Consolidate identified threats into a centralized Threat Register.

---

# Documents

| Document | Purpose |
|----------|---------|
| **01-Threat_Actors.md** | Identifies potential threat actors, their motivations, capabilities, and likely targets. |
| **02-STRIDE.md** | Applies the STRIDE methodology to identify threats affecting system components, trust boundaries, and data flows. |
| **03-MITRE_ATTACK.md** | Maps identified threats to relevant MITRE ATT&CK tactics and techniques to understand adversary behavior. |
| **04-PASTA.md** | Applies the PASTA methodology to analyze business objectives, technical scope, attack scenarios, and risk. |
| **05-Threat_Register.md** | Consolidates identified threats, affected assets, existing controls, and recommended mitigations. |

---

# Relationship to Other Sections

The Threat Analysis section builds upon the previous architectural analysis and provides direct input to the Risk Assessment.

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

The following diagrams support this section.

| Diagram | Description |
|----------|-------------|
| **05-STRIDE.png** | High-level STRIDE threat mapping across the environment. |
| **06-MITRE-ATTACK.png** | MITRE ATT&CK tactics and techniques relevant to the environment. |
| **07-PASTA.png** | Seven-stage PASTA threat modelling process. |

Diagrams are located in:

```
/diagrams/
```

---

# Expected Outcomes

Upon completion of this section, readers should understand:

- Who the potential threat actors are.
- Which threats affect the environment.
- How attackers may exploit the infrastructure.
- Which attack techniques are most relevant.
- Which threats present the greatest business risk.
- Which threats should be prioritized for mitigation.

This information forms the basis for the Risk Assessment and the selection of appropriate security controls.

---

# References

The documents within this folder provide direct input to:

- **06-Risk-Assessment**
- **07-Security-Controls**