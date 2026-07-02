# 01 – Risk Register

## Purpose

This document records the risks identified during the threat modelling exercise for the Orange Infrastructure Services supporting Tieto Banktech applications.

The Risk Register provides a structured view of identified risks, their likelihood, impact, existing controls, residual risk, and planned treatment actions.

The register supports risk-based decision making and serves as the primary tracking mechanism for risk management activities.

---

# Risk Assessment Method

Each identified threat is evaluated using two factors:

- Likelihood
- Business Impact

The combination of these values determines the overall risk rating.

---

# Risk Rating Scale

## Likelihood

| Rating | Description |
|---------|-------------|
| Low | Unlikely to occur |
| Medium | Could occur under certain conditions |
| High | Expected to occur or has occurred previously |

---

## Impact

| Rating | Description |
|---------|-------------|
| Low | Limited operational impact |
| Medium | Noticeable business disruption |
| High | Significant financial, operational, or regulatory impact |

---

# Risk Register

| Risk ID | Threat | Asset | Likelihood | Impact | Risk Rating | Existing Controls | Risk Owner | Treatment |
|----------|---------|--------|------------|---------|-------------|-------------------|------------|-----------|
| R-001 | Credential compromise | User Accounts | Medium | High | High | MFA, Password Policy | Tieto Banktech | Mitigate |
| R-002 | Unauthorized application access | Applications | Medium | High | High | Authentication, RBAC | Tieto Banktech | Mitigate |
| R-003 | Infrastructure compromise | Compute | Medium | High | High | Hardening, Patch Management | Orange | Mitigate |
| R-004 | Network compromise | Network | Medium | High | High | Firewalls, Segmentation | Orange | Mitigate |
| R-005 | Log tampering | Logging Platform | Low | High | Medium | Centralized Logging | Orange | Mitigate |
| R-006 | Backup compromise | Backup & DR | Medium | High | High | Backup Encryption | Orange | Mitigate |
| R-007 | Security monitoring failure | Security Services | Low | High | Medium | SIEM, Monitoring | Orange | Mitigate |
| R-008 | Privileged account misuse | Administrative Accounts | Medium | High | High | PAM, MFA | Orange | Mitigate |
| R-009 | External dependency compromise | External Services | Low | High | Medium | Secure DNS, PKI | Shared | Monitor |
| R-010 | Denial of Service | Applications / Network | Medium | High | High | Load Balancing, Monitoring | Shared | Mitigate |

---

# High Risks

The following risks are considered high priority:

- R-001 Credential compromise
- R-002 Unauthorized application access
- R-003 Infrastructure compromise
- R-004 Network compromise
- R-006 Backup compromise
- R-008 Privileged account misuse
- R-010 Denial of Service

These risks should receive priority during remediation planning.

---

# Residual Risk

Residual risk represents the level of risk remaining after existing controls have been implemented.

Residual risk should be periodically reviewed to determine whether additional controls are required.

---

# Risk Review

The Risk Register should be reviewed:

- Following significant infrastructure changes.
- Following major security incidents.
- Following threat model updates.
- During periodic security reviews.
- When new vulnerabilities or threats are identified.

---

# Related Documents

- ../05-Threat-Analysis/05-Threat_Register.md
- 02-Risk_Matrix.md
- 03-Risk_Treatment.md