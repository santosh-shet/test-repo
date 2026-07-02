# 02 – Open Issues

## Purpose

This document records open issues, assumptions requiring validation, identified gaps, and follow-up actions resulting from the threat modelling exercise for the Orange Infrastructure Services supporting Tieto Banktech applications.

Maintaining an Open Issues register helps ensure unresolved items are tracked, assigned, and reviewed until closure.

---

# Overview

Not all issues identified during threat modelling can be resolved immediately.

Some items require additional investigation, architectural clarification, operational decisions, or implementation activities.

Open issues should be periodically reviewed as part of the threat model lifecycle.

---

# Open Issues Register

| ID | Issue | Category | Priority | Owner | Status |
|----|-------|----------|----------|-------|--------|
| OI-001 | Validate infrastructure architecture against current deployment | Architecture | High | Orange | Open |
| OI-002 | Verify trust boundary assumptions | Threat Model | Medium | Shared | Open |
| OI-003 | Review privileged access implementation | Security | High | Orange | Open |
| OI-004 | Validate monitoring coverage across all infrastructure components | Monitoring | Medium | Orange | Open |
| OI-005 | Confirm backup recovery testing frequency | Business Continuity | Medium | Orange | Open |
| OI-006 | Review external supporting service dependencies | Third Party | Low | Shared | Open |

---

# Outstanding Assumptions

The following assumptions should be validated during future reviews:

- Administrative access follows organizational security requirements.
- Infrastructure logging remains enabled.
- Backup and recovery processes are operating successfully.
- Security monitoring covers all critical infrastructure.
- Network segmentation remains effective.

---

# Known Gaps

Potential gaps identified during the assessment may include:

- Missing architectural documentation.
- Incomplete asset inventory.
- Unknown third-party dependencies.
- Incomplete logging coverage.
- Limited visibility into externally managed services.

---

# Issue Management

Each issue should be:

- Assigned to an owner.
- Prioritized based on business risk.
- Reviewed periodically.
- Updated as remediation progresses.
- Closed when verification has been completed.

---

# Review

The Open Issues register should be reviewed:

- During threat model reviews.
- Following significant infrastructure changes.
- Following major security incidents.
- As part of periodic security governance activities.

---

# Related Documents

- 01-Threat_Model_Review.md
- 03-Future_Improvements.md
- ../06-Risk-Assessment/01-Risk_Register.md