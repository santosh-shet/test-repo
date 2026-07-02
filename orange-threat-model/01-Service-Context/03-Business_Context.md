# 03 – Business Context

## Purpose

This document describes the business context of the Orange Infrastructure Services used to host and operate Tieto Banktech applications. It explains why the service exists, the business capabilities it supports, and the importance of the service from a security and operational perspective.

This information provides the business foundation for the subsequent threat modelling activities.

---

# Business Overview

Tieto Banktech delivers banking solutions and services to financial institutions. The applications are hosted on infrastructure managed by Orange Infrastructure Services.

Orange provides managed infrastructure capabilities, enabling Tieto Banktech to deliver secure, reliable, and highly available banking services without managing the underlying infrastructure components.

The service supports production and non-production environments and provides the infrastructure platform required to operate critical banking applications.

---

# Business Objectives

The primary business objectives of the service include:

- Provide secure hosting for Tieto Banktech applications.
- Ensure high availability of banking services.
- Protect customer and business information.
- Support regulatory and contractual requirements.
- Maintain business continuity and disaster recovery capabilities.
- Enable scalable and reliable infrastructure services.
- Support secure operations through monitoring, logging, and security services.

---

# Business Drivers

The service is implemented to support the following business drivers:

- Reliable delivery of banking applications.
- Operational stability.
- Information security.
- Regulatory compliance.
- Business continuity.
- Disaster recovery preparedness.
- Centralized infrastructure management.
- Managed operational support.
- Secure administration of infrastructure resources.

---

# Business Services Supported

The infrastructure supports multiple business services, including:

- Banking applications
- API services
- Authentication services
- Business processing services
- Integration services
- Administrative portals
- Monitoring and operational services

---

# Critical Business Functions

The hosted environment enables several critical business functions, including:

- Customer access to banking services
- Business transaction processing
- Authentication and authorization
- Application availability
- Secure administration
- Operational monitoring
- Incident response
- Backup and recovery
- Audit logging

---

# Business Assets

The following business assets are considered valuable and require protection.

| Asset | Description |
|---------|-------------|
| Banking Applications | Core business applications delivered by Tieto Banktech |
| Customer Information | Customer-related business data processed by applications |
| Business Transactions | Banking and financial transactions |
| Application Services | APIs and application functionality |
| Infrastructure Services | Compute, storage, networking and supporting services |
| Audit Logs | Operational and security logs |
| Backup Data | Business continuity and disaster recovery data |
| Administrative Access | Privileged administrative interfaces |

---

# Business Stakeholders

The following stakeholders have an interest in the service.

| Stakeholder | Responsibility |
|-------------|----------------|
| Tieto Banktech | Owns and manages banking applications |
| Orange Infrastructure Services | Operates and manages infrastructure services |
| Customers | Consume banking services |
| Operations Teams | Service operations and monitoring |
| Security Teams | Security monitoring and incident response |
| Infrastructure Administrators | Platform administration |
| Business Owners | Service ownership and business decisions |

---

# Business Dependencies

Successful delivery of the service depends on several supporting capabilities.

Internal dependencies include:

- Orange Infrastructure Services
- Network connectivity
- Compute platform
- Storage platform
- Backup services
- Logging platform
- Security services

External dependencies include:

- DNS services
- NTP services
- PKI / Certificate Authority
- Identity Provider
- External vendor repositories

---

# Availability Requirements

The service is expected to provide:

- High availability
- Infrastructure resilience
- Fault tolerance where applicable
- Disaster recovery capabilities
- Backup and restore capabilities
- Continuous operational monitoring

Specific service level agreements (SLAs) are managed separately and are outside the scope of this document.

---

# Information Security Objectives

The infrastructure should support the following security objectives.

## Confidentiality

Protect customer, business, and operational information against unauthorized disclosure.

## Integrity

Protect systems and information against unauthorized modification.

## Availability

Ensure banking services remain available to authorized users.

## Accountability

Provide sufficient logging and auditing to support investigations and compliance.

---

# Regulatory and Compliance Considerations

The service may support compliance with applicable regulatory, contractual, and organizational requirements, including:

- ISO/IEC 27001
- DORA
- NIS2
- GDPR
- Customer contractual security requirements
- Internal Tieto Banktech security policies

The applicable requirements depend on the specific banking services hosted on the platform.

---

# Business Impact

Loss or compromise of the service could result in:

- Service disruption
- Loss of customer confidence
- Financial impact
- Regulatory non-compliance
- Operational disruption
- Security incidents
- Reputational damage

---

# Threat Modelling Relevance

Understanding the business context enables threat modelling activities to:

- Identify critical assets.
- Prioritize threat scenarios.
- Evaluate business impact.
- Support risk assessment.
- Select appropriate security controls.
- Focus mitigation efforts on business-critical services.

---

# Related Documents

- 01-Service_Scope.md
- 02-Architecture_Overview.md
- ../02-System-Model/Assets.md
- ../03-Trust-Boundaries/Trust_Boundaries.md
- ../04-Data-Flows/Data_Flows.md
- ../05-Threat-Analysis/Threat_Scenarios.md