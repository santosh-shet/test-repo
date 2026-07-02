# 03 – Future Improvements

## Purpose

This document captures potential improvements identified during the threat modelling exercise for the Orange Infrastructure Services supporting Tieto Banktech applications.

The objective is to support continuous improvement of the architecture, security controls, monitoring capabilities, and threat modelling process.

---

# Overview

Threat modelling is an ongoing process.

As the environment evolves, new technologies, threats, business requirements, and regulatory expectations may require updates to the threat model and associated security controls.

Future improvements should be prioritized based on business value and risk reduction.

---

# Improvement Opportunities

## Architecture

Potential improvements include:

- Improve architectural documentation.
- Increase automation of infrastructure documentation.
- Enhance dependency mapping.
- Improve asset inventory accuracy.

---

## Security Controls

Potential improvements include:

- Expand Multi-Factor Authentication (MFA) coverage.
- Enhance Privileged Access Management (PAM).
- Improve network segmentation.
- Strengthen backup protection.
- Improve encryption coverage.

---

## Monitoring

Potential improvements include:

- Expand SIEM coverage.
- Improve detection rules.
- Reduce false positives.
- Improve alert correlation.
- Increase monitoring automation.

---

## Threat Modelling

Potential improvements include:

- Review the threat model after significant architectural changes.
- Expand STRIDE analysis to new components.
- Improve MITRE ATT&CK mapping.
- Develop additional attack scenarios.
- Enhance risk scoring methodology.

---

## Operational Improvements

Potential improvements include:

- Improve vulnerability management.
- Increase security awareness.
- Enhance incident response procedures.
- Perform regular tabletop exercises.
- Improve disaster recovery testing.

---

# Improvement Register

| ID | Improvement | Priority | Owner | Status |
|----|-------------|----------|-------|--------|
| FI-001 | Review threat model annually or after major architectural changes | High | Shared | Planned |
| FI-002 | Expand detection coverage for infrastructure services | High | Orange | Planned |
| FI-003 | Improve privileged access monitoring | High | Orange | Planned |
| FI-004 | Enhance backup validation and restore testing | Medium | Orange | Planned |
| FI-005 | Improve asset inventory automation | Medium | Shared | Planned |
| FI-006 | Review third-party dependencies periodically | Medium | Shared | Planned |

---

# Continuous Improvement

The threat model should evolve as:

- Infrastructure changes.
- Business requirements change.
- New technologies are introduced.
- New threats emerge.
- Security controls improve.
- Regulatory requirements evolve.

Continuous improvement helps maintain an effective and relevant threat model.

---

# Success Criteria

The threat model should:

- Reflect the current architecture.
- Cover critical assets and trust boundaries.
- Identify realistic threats.
- Support effective risk management.
- Drive continuous security improvements.

---

# Related Documents

- 01-Threat_Model_Review.md
- 02-Open_Issues.md
- ../05-Threat-Analysis/05-Threat_Register.md
- ../06-Risk-Assessment/03-Risk_Treatment.md