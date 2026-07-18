# ADR-001

## Title

Use Flet as the primary UI framework.

---

## Status

Accepted

---

## Context

The platform must support Desktop, Web, and Mobile while maintaining a single Python codebase.

---

## Decision

KEMET will use Flet for all user interfaces.

FastAPI will provide backend APIs integrated within the same application architecture.

---

## Consequences

Pros

- Single language (Python).
- Faster development.
- Cross-platform.
- Shared components.

Cons

- Smaller ecosystem than React.
- Some advanced web features may require custom implementations.