# 06 – Out of Scope

## Purpose

This document defines the areas, systems, processes, and responsibilities that are explicitly excluded from this threat modelling exercise.

Clearly identifying out-of-scope items helps establish the boundaries of the assessment and prevents assumptions regarding responsibilities that are outside the Orange Infrastructure Services supporting Tieto Banktech applications.

---

# Scope Boundary

This threat model focuses on the infrastructure services provided by Orange to support Tieto Banktech applications.

Activities, systems, and services outside this defined service boundary are not analysed unless they directly affect the hosted infrastructure.

---

# Excluded Business Processes

The following business processes are outside the scope of this threat model.

- Customer business operations
- Banking product functionality
- Financial transaction business logic
- Customer onboarding processes
- Internal operational procedures not related to infrastructure

---

# Excluded Applications

The following are outside the scope unless specifically hosted or managed within the assessed environment.

- Customer-developed applications
- Third-party SaaS platforms
- Office productivity applications
- End-user desktop software
- Mobile applications
- Application source code
- Application development lifecycle

---

# Excluded End User Devices

The following devices are excluded.

- Customer devices
- Personal devices
- Employee workstations
- Mobile phones
- Home networks

The security posture of these devices is not assessed within this threat model.

---

# Excluded Infrastructure

Unless specifically included within the Orange managed service scope, the following infrastructure is excluded.

- Customer-owned infrastructure
- Customer-managed data centres
- Internet backbone infrastructure
- Telecommunications provider infrastructure
- Public cloud services not managed by Orange
- Third-party hosting providers

---

# Excluded Physical Security

This assessment does not include detailed evaluation of:

- Building security
- Visitor management
- CCTV
- Environmental controls
- Power infrastructure
- Fire suppression systems

These may be covered through separate physical security assessments.

---

# Excluded Organizational Processes

The following organizational activities are outside the scope.

- Human Resources processes
- Procurement processes
- Legal processes
- Vendor contracting
- Financial management
- Corporate governance

---

# Excluded Security Assessments

The following are not performed as part of this threat model.

- Penetration testing
- Vulnerability scanning
- Secure code review
- Red team exercises
- Configuration compliance assessments
- Digital forensic investigations

The results of these activities may be used as inputs to future updates of the threat model.

---

# Excluded Threats

The following threats are not analysed in detail unless they directly affect the Orange managed infrastructure.

- Physical theft of customer devices
- Social engineering of customers
- Insider threats outside the assessed environment
- Internet-wide denial-of-service attacks
- Nation-state threat intelligence
- Supply chain risks unrelated to Orange Infrastructure Services

---

# Excluded Responsibilities

The following responsibilities remain outside the Orange Infrastructure Services threat model.

## Tieto Banktech

- Application development
- Business logic
- Application configuration
- User management within applications
- Application release management

## Customers

- End-user security
- Endpoint protection
- Local device configuration
- Customer network security
- User awareness

## Third Parties

- External DNS providers
- External Certificate Authorities
- Identity providers not managed by Orange
- Vendor software repositories

---

# Future Scope

The following areas may be included in future versions of the threat model.

- Application-level threat modelling
- API threat modelling
- Secure software development lifecycle
- Container security
- Kubernetes platform security
- Identity and Access Management architecture
- Zero Trust architecture
- Cloud-native services
- Supply chain security

---

# Scope Review

This document should be reviewed whenever:

- Orange service scope changes.
- New infrastructure services are introduced.
- Responsibilities change between Orange and Tieto Banktech.
- New third-party services are integrated.
- Major architectural changes occur.

---

# Related Documents

- 01-Service_Scope.md
- 02-Architecture_Overview.md
- 03-Business_Context.md
- 04-Service_Dependencies.md
- 05-Service_Assumptions.md
- ../02-System-Model/Assets.md