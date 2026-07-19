# Session 002

Date: 2026-07-19

---

## Goals

- Continue domain design
- Define Investment Domain
- Define Intelligence Domain
- Finalize communication model

---

## Decisions Made

### Investment Domain

- Portfolio Manager Agent is the only AI Agent responsible for achieving Investment Objectives.

- Expert Agents are unaware of business objectives.

- Account Owner is the only human actor.

---

### Intelligence Domain

- Recommendation is the universal language between agents.

- Knowledge is persistent.

- Recommendation is temporary.

- Events transport Recommendations.

---

### Event Architecture

Recommendation

↓

RecommendationPublished Event

↓

Event Bus

↓

Subscribers

---

## Architecture Decisions

- Recommendation is a Domain Object.

- Events are transport only.

- Event payload contains Recommendation data.

- Event Envelope is standardized.

---

## Next Session

- Design Recommendation Domain Object.

- Define Recommendation lifecycle.

- Design Knowledge Domain.

- Start Domain implementation.