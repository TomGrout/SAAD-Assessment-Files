# ADR-003: Implement Multi-Tenant Data Isolation

**Status:** Accepted  
**Date:** 2025-10-12
**Version:** 1.0  
**Author:** Tom Grout

---

## Context
CMS will be used by multiple organisations (e.g., NatWest, Vodafone). Each tenant’s data must be securely isolated per legal and contractual obligations (GDPR/UK DPA).

## Decision
Use **schema-per-tenant** model with strict tenancy identifiers at the data access layer, enforced through middleware and repository pattern.

## Alternatives Considered
- **Shared schema with tenant ID column:** simple but high risk of data leakage.
- **Separate database per tenant:** strongest isolation but poor scalability and maintenance burden.

## Consequences
+ Meets GDPR and contractual isolation requirements.
+ Simplifies audit and logging per tenant.
- Slightly increased overhead in schema management.

## Rationale & References
Supports NFR-3 (Security/Privacy) and aligns with ABC Ltd’s scalability goal of onboarding multiple large clients.  
Ref: Azure SaaS Patterns, Microsoft Cloud Architecture Center.
