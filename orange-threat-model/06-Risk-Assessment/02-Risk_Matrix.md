# 02 – Risk Matrix

## Purpose

This document defines the risk assessment methodology used during the threat modelling exercise for the Orange Infrastructure Services supporting Tieto Banktech applications.

The Risk Matrix provides a consistent approach for evaluating identified risks based on their likelihood and business impact.

The resulting risk ratings support prioritization of mitigation activities and risk treatment decisions.

---

# Risk Assessment Methodology

Each identified risk is evaluated using two factors:

- Likelihood
- Business Impact

The combination of these values determines the overall risk rating.

---

# Likelihood Ratings

| Rating | Description |
|---------|-------------|
| Low | Unlikely to occur. Strong preventive controls exist or exploitation requires exceptional circumstances. |
| Medium | Could occur under certain conditions. Existing controls reduce but do not eliminate the possibility. |
| High | Likely to occur or has been observed previously. Significant exposure or limited mitigating controls exist. |

---

# Business Impact Ratings

| Rating | Description |
|---------|-------------|
| Low | Minor operational disruption with limited business impact. |
| Medium | Noticeable disruption affecting business operations or customers. |
| High | Significant financial, operational, legal, regulatory, or reputational impact. |

---

# Risk Matrix

|               | **Low Impact** | **Medium Impact** | **High Impact** |
|---------------|----------------|-------------------|-----------------|
| **High Likelihood** | Medium | High | High |
| **Medium Likelihood** | Low | Medium | High |
| **Low Likelihood** | Low | Low | Medium |

---

# Risk Priority

| Risk Rating | Priority | Typical Response |
|--------------|----------|------------------|
| High | Immediate | Mitigate as soon as practical |
| Medium | Planned | Reduce risk through scheduled improvements |
| Low | Monitor | Accept or monitor based on business requirements |

---

# Risk Evaluation Criteria

The following factors should be considered when assigning likelihood and impact.

### Likelihood

- Ease of exploitation
- Exposure to attackers
- Existing security controls
- Historical incidents
- Threat intelligence

### Business Impact

- Service availability
- Data confidentiality
- Data integrity
- Financial impact
- Regulatory impact
- Reputational impact
- Customer impact

---

# Risk Acceptance

Residual risks may be accepted where:

- The remaining risk is within the organization's risk appetite.
- Additional controls are not cost-effective.
- Business requirements justify acceptance.
- Executive or risk owner approval has been obtained.

Accepted risks should be documented and reviewed periodically.

---

# Risk Review

Risk ratings should be reviewed when:

- Significant infrastructure changes occur.
- New threats or vulnerabilities are identified.
- Security incidents occur.
- New regulatory requirements are introduced.
- The threat model is updated.

---

# Relationship to Threat Modelling

The Risk Matrix supports:

- Threat Register
- Risk Register
- Risk Treatment Planning
- Security Control Prioritization

---

# Related Documents

- 01-Risk_Register.md
- 03-Risk_Treatment.md
- ../05-Threat-Analysis/05-Threat_Register.md