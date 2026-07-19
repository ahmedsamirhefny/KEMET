# ADR-004: Recommendation-Based Event Communication

## Status

Accepted

## Date

2026-07-19

---

## Context

KEMET consists of multiple AI Agents working independently.

Agents must collaborate without being tightly coupled.

Direct communication between agents increases dependencies and reduces scalability.

---

## Decision

Agents never communicate directly.

Every Expert Agent publishes a Recommendation.

Recommendations are delivered through the Event Bus using a standardized Event Envelope.

The Recommendation is a Domain Object.

The Event is only the transport mechanism.

---

## Event Envelope

```json
{
  "event_id": "...",
  "event_type": "recommendation.published",
  "timestamp": "...",
  "producer": "...",
  "payload": { ... }
}
```

---

## Consequences

Advantages

- Loose coupling
- Scalable architecture
- Easy integration of new agents
- Event replay capability
- Audit-friendly design

Disadvantages

- Eventual consistency
- More infrastructure complexity

---

## Related Documents

- architecture.md
- domain-model.md