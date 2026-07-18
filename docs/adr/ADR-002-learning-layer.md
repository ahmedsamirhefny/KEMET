# ADR-002

## Title

Adopt a centralized Continuous Learning Layer.

---

## Status

Accepted

---

## Context

Allowing every AI agent to update itself independently would make system behavior difficult to reproduce and debug.

---

## Decision

Learning responsibilities are centralized inside the Continuous Learning Layer.

Agents collect experience but never modify themselves directly.

---

## Consequences

Pros

- Stable architecture.
- Reproducible results.
- Easier evaluation.
- Safer deployments.

Cons

- More engineering effort.
- Additional infrastructure.