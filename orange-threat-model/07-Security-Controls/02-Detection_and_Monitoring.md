# 02 – Detection and Monitoring

## Purpose

This document describes the monitoring and detection capabilities supporting the Orange Infrastructure Services hosting Tieto Banktech applications.

The objective is to ensure security events are identified, investigated, and responded to in a timely manner, reducing the likelihood and impact of security incidents.

---

# Overview

Security monitoring provides continuous visibility into infrastructure, applications, administrative activities, and supporting services.

Detection capabilities should identify abnormal behaviour, policy violations, malicious activity, and operational failures that may affect the confidentiality, integrity, or availability of the environment.

---

# Monitoring Objectives

The monitoring strategy aims to:

- Detect unauthorized access.
- Detect suspicious administrative activity.
- Detect infrastructure compromise.
- Detect service disruption.
- Detect configuration changes.
- Detect malicious software.
- Support incident investigation.
- Support compliance and audit requirements.

---

# Monitoring Scope

Monitoring should include the following components.

| Component | Monitoring Objective |
|-----------|----------------------|
| Tieto Banktech Applications | Application availability, authentication failures, application errors |
| Compute | Resource utilization, operating system events, configuration changes |
| Storage | Capacity, integrity, unauthorized access |
| Network | Connectivity, firewall events, unusual traffic |
| Logging Platform | Log collection, integrity, availability |
| Backup & Disaster Recovery | Backup success, restore failures, backup integrity |
| Security Services | Alert generation, detection coverage |
| Administrative Activities | Privileged access, configuration changes, failed administrative logins |

---

# Security Events

The following events should be monitored.

## Authentication

- Failed logins
- Successful administrative logins
- Multiple authentication failures
- Privileged account usage
- Account lockouts

---

## Authorization

- Privilege changes
- Role modifications
- Unauthorized access attempts
- Permission changes

---

## Infrastructure

- Server restarts
- Unexpected configuration changes
- Service failures
- Operating system errors
- Resource exhaustion

---

## Network

- Firewall events
- Network scanning
- Unusual traffic patterns
- Denial-of-Service indicators
- Unexpected outbound connections

---

## Logging

- Logging failures
- Log deletion
- Log modification
- Missing log sources
- Time synchronization issues

---

## Backup

- Backup failures
- Restore failures
- Backup integrity issues
- Unexpected backup deletion

---

## Security

- Malware detection
- Endpoint protection alerts
- Vulnerability discoveries
- Security policy violations
- Threat detection alerts

---

# Detection Methods

Typical detection methods include:

- Centralized logging
- Security Information and Event Management (SIEM)
- Infrastructure monitoring
- Endpoint protection
- Vulnerability management
- Alert correlation
- Manual security reviews

---

# Alert Prioritization

| Severity | Description |
|----------|-------------|
| Critical | Immediate response required due to significant business impact or active compromise. |
| High | High-risk security event requiring prompt investigation. |
| Medium | Security event requiring investigation during normal operations. |
| Low | Informational event requiring monitoring or periodic review. |

---

# Incident Response

Detected security events should follow the organization's incident response process, including:

- Event validation
- Initial triage
- Investigation
- Containment
- Eradication
- Recovery
- Lessons learned

---

# Monitoring Review

Monitoring effectiveness should be reviewed periodically to ensure:

- Critical systems remain covered.
- New infrastructure is monitored.
- Alert thresholds remain appropriate.
- Detection rules are updated based on emerging threats.
- Monitoring aligns with organizational security requirements.

---

# Relationship to Threat Modelling

Monitoring and detection capabilities support:

- STRIDE threat detection
- MITRE ATT&CK technique detection
- PASTA attack simulation
- Risk monitoring
- Incident response

---

# Related Documents

- 01-Security_Controls.md
- 03-Control_Validation.md
- ../05-Threat-Analysis/03-MITRE_ATTACK.md
- ../06-Risk-Assessment/01-Risk_Register.md