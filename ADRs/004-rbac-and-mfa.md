# ADR-004: OIDC/SAML with MFA; RBAC + ABAC

**Status:** Accepted  
**Date:** 2025-10-20  
**Version:** 1.0  
**Author:** Tom Grout

---

## Context
Enterprise tenants such as banks and telecoms will often already have their own identity providers and compliance requirements for strong authentication and least-privilege access.  
The Complaint Management System (CMS) must support single sign-on (SSO) and multi-factor authentication (MFA) for security, while enabling flexible role and attribute-based authorisation for internal users across multiple tenants.

## Decision
Adopt **OpenID Connect (OIDC)** and **SAML 2.0** for federated authentication through tenant identity providers (e.g., Microsoft Entra ID).  
Access control within the CMS will use a combination of:
- **Role-Based Access Control (RBAC)** for standard permissions (e.g., Consumer, Agent, Support, Manager, Administrator).  
- **Attribute-Based Access Control (ABAC)** for dynamic policies (e.g., tenant, complaint type, SLA level).

Short-lived **JWT tokens** will carry tenant and role claims. MFA will be required for all privileged roles.

## Alternatives Considered
- **Custom authentication system:** rejected due to high security risk and maintenance cost.  
- **RBAC only:** rejected because static roles cannot cover tenant-specific or contextual policies.  
- **Third-party IDaaS only:** rejected to avoid vendor lock-in and maintain flexibility for client-side IdPs.

## Consequences
**Positive**
- Supports SSO for enterprise tenants.  
- Strong authentication with MFA improves compliance (GDPR, UK DPA).  
- Enables fine-grained authorisation and audit logging.  

**Negative**
- Requires configuration for each tenant IdP.  
- Policy definition and evaluation add operational overhead.  
- JWT management introduces token lifecycle complexity.

## Rationale & References
Supports security and privacy NFRs (NFR-3), auditability, and maintainability.  
Aligns with enterprise integration expectations and modern identity standards.  
Reference: [https://c4model.com](https://c4model.com)
