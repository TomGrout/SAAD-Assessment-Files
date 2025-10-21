# ADR-002: Use C4 Model for Architecture Documentation

**Status:** Accepted  
**Date:** 2025-10-10
**Version:** 1.0  
**Author:** Tom Grout

---

## Context
The CMS architecture must be clearly communicated to technical and non-technical stakeholders and meet assessment criteria requiring C4 representation.

## Decision
Adopt the **C4 Model** to represent the system across four abstraction levels (Context, Container, Component, Code).

## Alternatives Considered
- **UML only:** powerful but overly detailed for early architectural communication.
- **Custom ad hoc diagrams:** less standardised and harder to maintain.

## Consequences
- ✅ Improves traceability between design levels.
- ✅ Simplifies peer and tutor feedback.
- ⚠️ Requires consistent notation and clear legends across diagrams.

## Rationale & References
C4 is explicitly recommended in the SHU brief and aligns with professional documentation standards.  
Reference: [https://c4model.com]
