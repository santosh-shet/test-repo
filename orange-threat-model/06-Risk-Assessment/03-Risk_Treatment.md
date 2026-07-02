# 03 – Risk Treatment

## Purpose

This document defines the approach for managing and treating the risks identified during the threat modelling exercise for the Orange Infrastructure Services supporting Tieto Banktech applications.

The objective is to ensure identified risks are evaluated, assigned to appropriate owners, and treated using consistent risk management practices.

---

# Overview

Risk treatment determines how identified risks will be managed after assessment.

Not every risk requires additional controls. Depending on business requirements, cost, and organizational risk appetite, risks may be:

- Mitigated
- Accepted
- Transferred
- Avoided

The selected treatment should be documented and periodically reviewed.

---

# Risk Treatment Options

## Mitigate

Implement additional security controls to reduce either the likelihood or impact of the risk.

Examples include:

- Multi-Factor Authentication (MFA)
- Network Segmentation
- Privileged Access Management (PAM)
- Vulnerability Management
- Enhanced Monitoring
- Backup Protection

---

## Accept

Accept the residual risk when:

- Risk falls within the organization's risk appetite.
- Additional controls provide limited benefit.
- Mitigation costs outweigh the potential impact.

Accepted risks should be formally approved by the appropriate risk owner.

---

## Transfer

Transfer part or all of the risk to another party.

Examples include:

- Cyber insurance
- Contractual agreements
- Managed security services
- Third-party service providers

Risk ownership remains with the organization even when operational responsibility is delegated.

---

## Avoid

Avoid the activity creating the risk.

Examples include:

- Removing unnecessary services
- Disabling unused functionality
- Eliminating unsupported technologies
- Replacing high-risk components

---

# Risk Treatment Plan

| Risk ID | Treatment | Planned Action | Owner | Status |
|----------|-----------|----------------|--------|--------|
| R-001 | Mitigate | Strengthen authentication and monitor failed login attempts | Tieto Banktech | Planned |
| R-002 | Mitigate | Review access permissions and application security controls | Tieto Banktech | Planned |
| R-003 | Mitigate | Continue infrastructure hardening and vulnerability management | Orange | Ongoing |
| R-004 | Mitigate | Review firewall rules and network segmentation | Orange | Ongoing |
| R-005 | Mitigate | Protect log integrity and increase monitoring | Orange | Planned |
| R-006 | Mitigate | Validate backup integrity and recovery procedures | Orange | Ongoing |
| R-007 | Mitigate | Improve monitoring coverage and alert validation | Orange | Planned |
| R-008 | Mitigate | Strengthen privileged access management and session monitoring | Orange | Ongoing |
| R-009 | Monitor | Periodically review external service dependencies | Shared | Ongoing |
| R-010 | Mitigate | Review resilience, capacity, and DDoS protection measures | Shared | Planned |

---

# Risk Ownership

Risk owners are responsible for:

- Reviewing assigned risks.
- Approving treatment decisions.
- Monitoring mitigation activities.
- Accepting residual risks where appropriate.
- Ensuring periodic reassessment.

---

# Residual Risk

Residual risk is the level of risk remaining after treatment measures have been implemented.

Residual risks should:

- Be documented.
- Be periodically reviewed.
- Be approved by the appropriate risk owner where acceptance is required.

---

# Risk Monitoring

Risk treatment activities should be monitored through:

- Periodic security reviews
- Vulnerability assessments
- Security monitoring
- Incident management
- Audit activities
- Threat model reviews

---

# Risk Review Triggers

Risk treatment should be reviewed when:

- New threats are identified.
- Significant infrastructure changes occur.
- Major security incidents occur.
- New regulatory or contractual requirements arise.
- Existing controls are modified.
- The threat model is updated.

---

# Relationship to Threat Modelling

Risk treatment is the final outcome of the threat modelling process.

The information in this document supports:

- Security improvement planning
- Control implementation
- Risk acceptance decisions
- Continuous security improvement
- Governance and compliance activities

---

# Related Documents

- 01-Risk_Register.md
- 02-Risk_Matrix.md
- ../05-Threat-Analysis/05-Threat_Register.md
- ../07-Security-Controls/01-Security_Controls.md