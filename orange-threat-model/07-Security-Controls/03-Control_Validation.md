# 03 – Control Validation

## Purpose

This document describes the approach for validating the effectiveness of security controls protecting the Orange Infrastructure Services supporting Tieto Banktech applications.

Control validation helps ensure that implemented security controls continue to operate as intended and remain effective against evolving threats.

---

# Overview

Security controls should be periodically validated to confirm they:

- Operate as designed.
- Continue to reduce identified risks.
- Detect and prevent relevant threats.
- Meet business and regulatory requirements.

Validation activities should be performed throughout the service lifecycle.

---

# Validation Objectives

The objectives of control validation are to:

- Verify control effectiveness.
- Identify control gaps.
- Confirm security controls remain appropriately configured.
- Support continuous improvement.
- Reduce residual risk.

---

# Validation Activities

| Activity | Purpose |
|----------|---------|
| Configuration Reviews | Verify secure configurations remain in place |
| Access Reviews | Validate user and privileged access |
| Vulnerability Assessments | Identify known vulnerabilities |
| Penetration Testing | Validate resistance to real-world attacks |
| Security Monitoring Reviews | Confirm monitoring coverage and alert quality |
| Backup & Restore Testing | Verify recovery capability |
| Disaster Recovery Exercises | Validate business continuity procedures |
| Log Reviews | Confirm audit logs are complete and protected |
| Change Reviews | Ensure security controls remain effective after changes |

---

# Validation Scope

The following components should be periodically validated.

| Component | Validation Examples |
|-----------|---------------------|
| Tieto Banktech Applications | Authentication, authorization, secure configuration |
| Compute | Patch level, hardening, configuration compliance |
| Storage | Access permissions, encryption, integrity |
| Network | Firewall rules, segmentation, connectivity |
| Logging Platform | Log collection, retention, integrity |
| Backup & Disaster Recovery | Backup success, restore testing |
| Security Services | Alert generation, detection coverage |
| Administrative Access | MFA, privileged access, account reviews |

---

# Validation Frequency

Validation activities should be performed according to organizational policies and risk requirements.

| Activity | Suggested Frequency |
|----------|---------------------|
| Access Reviews | Periodically |
| Vulnerability Assessments | Periodically and after significant changes |
| Penetration Testing | Periodically or following major changes |
| Backup Restore Testing | Periodically |
| Disaster Recovery Testing | Periodically |
| Security Monitoring Review | Continuous with periodic review |
| Configuration Reviews | After significant infrastructure changes |

---

# Validation Success Criteria

Security controls should demonstrate that they:

- Prevent unauthorized access.
- Detect malicious activity.
- Protect sensitive information.
- Maintain service availability.
- Generate reliable audit logs.
- Support timely incident response.

---

# Findings Management

Validation findings should be:

- Documented.
- Risk assessed.
- Assigned to an appropriate owner.
- Tracked until remediation is complete.
- Verified following remediation.

---

# Continuous Improvement

Control validation should support continuous improvement by:

- Updating security controls where required.
- Improving monitoring and detection.
- Addressing lessons learned from incidents.
- Incorporating new threat intelligence.
- Updating the threat model when significant changes occur.

---

# Relationship to Threat Modelling

Control validation confirms that the mitigations identified during the threat modelling process remain effective.

The results should be used to:

- Update the Threat Register.
- Reassess identified risks.
- Improve security controls.
- Support future threat model reviews.

---

# Related Documents

- 01-Security_Controls.md
- 02-Detection_and_Monitoring.md
- ../05-Threat-Analysis/05-Threat_Register.md
- ../06-Risk-Assessment/01-Risk_Register.md
- ../08-Validation/01-Threat_Model_Review.md