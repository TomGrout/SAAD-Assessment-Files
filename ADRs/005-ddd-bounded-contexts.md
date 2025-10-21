# ADR-005: Domain-Driven Design (DDD) and Bounded Contexts

**Status:** Accepted  
**Date:** 2025-10-21  
**Version:** 1.0  
**Author:** Tom Grout

---

## Context
The Complaint Management System (CMS) must support multiple functional domains—complaint lifecycle, user management, communication, analytics—while maintaining clear separation of concerns.  
Given the modular monolith and hexagonal architecture, strong domain boundaries are essential to prevent coupling between modules, enable testability, and support future service extraction if the platform scales beyond the proof of concept.

## Decision
Adopt **Domain-Driven Design (DDD)** principles and implement **Bounded Contexts** for the major domains:
- **Complaints** – core domain managing lifecycle and workflow.  
- **Users and Roles** – authentication, authorisation, and tenant context.  
- **Communications** – notifications and events.  
- **Reporting** – read models and analytics.  
- **Administration** – configuration and tenancy management.  

Each bounded context will define its own domain model, repositories, and adapters. Cross-context interaction will occur only through **domain events** or **application service interfaces**.

## Alternatives Considered
- **Single shared domain model:** rejected due to tight coupling and reduced flexibility.  
- **Microservices per context:** rejected for the PoC phase because of operational complexity and time constraints.  

## Consequences
**Positive**  
- Enforces modularity within the monolith.  
- Facilitates independent evolution and testing of domains.  
- Provides a clear path to microservice decomposition later.  

**Negative**  
- Requires disciplined modelling and communication patterns between contexts.  
- Initial overhead in defining aggregates and event contracts.

## Rationale & References
Aligns with maintainability (NFR-5), scalability (NFR-1), and extensibility (NFR-6).  
Supports the modular monolith and hexagonal architecture decisions (ADR-001).  
Reference: [https://c4model.com](https://c4model.com)
