# ADR-001: Adopt Modular Monolith Architecture

**Status:** Accepted  
**Date:** 2025-10-10  
**Version:** 1.0  
**Author:** Tom Grout

---

## Context
The Complaint Management System (CMS) needs to support multiple tenants (banks, telecoms) with strict data isolation, high maintainability, and future extensibility (e.g., chatbot integration).  
A modular approach is needed to balance agility, separation of concerns, and manageable deployment complexity.

## Decision
Adopt a **Modular Monolith** architecture using clearly defined domain modules (Consumer, Helpdesk, Support, Admin, Analytics) within a single deployable unit.

## Alternatives Considered
- **Microservices:** offers stronger isolation but adds heavy operational complexity, latency, and deployment overhead not justified for MVP/prototype.
- **Layered Monolith:** simpler but creates tight coupling and weak boundaries, reducing scalability and modularity.

## Consequences
+ Clear internal boundaries supporting DDD-style modularity.
+ Easier to deploy and test as a single artefact.
- Requires disciplined code organisation and clear internal APIs to prevent coupling.

## Rationale & References
Aligns with scalability (NFR-1), maintainability (NFR-5), and extensibility (NFR-6).  
Supports proof-of-concept within Azure Container Apps while remaining future-ready for service decomposition.  
References: C4Model.com, Fowler’s “Modular Monoliths” (2021).
