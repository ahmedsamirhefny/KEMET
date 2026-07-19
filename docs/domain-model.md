# KEMET Domain Model

> The Domain Model defines the core business concepts of KEMET.

It is the foundation of the entire platform.

Everything inside the system revolves around these domain objects.

---

# Philosophy

KEMET is not built around AI models.

KEMET is built around investment management.

Artificial Intelligence is only a tool used to achieve investment objectives.

The Account Owner defines business goals.

The Portfolio Manager Agent is responsible for achieving them.

All other AI Agents act as domain experts that provide recommendations.

They never own business goals.

---

# Domain Overview

```
Account Owner
        │
        ▼
Investment Objective
        │
        ▼
Portfolio Manager Agent
        │
        ▼
Trading Plan
        │
        ▼
Execution
        │
        ▼
Position
        │
        ▼
Trade Lifecycle
```

Expert Agents continuously support the Portfolio Manager Agent through recommendations.

---

# Core Domains

## Identity Domain

Responsible for system users.

### Entities

- Account Owner
- User
- Workspace
- Roles
- Permissions

---

## Investment Domain

Responsible for investment goals.

### Entities

- Investment Objective
- Portfolio
- Portfolio Manager Agent
- Capital
- Risk Profile
- Daily Target
- Weekly Target
- Monthly Target

### Responsibilities

The Portfolio Manager Agent is the only component responsible for achieving the investment objective.

It continuously evaluates progress and decides whether new trading opportunities are required.

No other agent is aware of the investment objective.

---

## Intelligence Domain

Responsible for market analysis.

### Entities

- Agent
- Recommendation
- Confidence
- Evidence
- Knowledge
- Knowledge Card
- Mentor Agent

### Responsibilities

Expert Agents analyze only their own domain.

They publish recommendations.

They never execute trades.

They never communicate directly with the Account Owner.

---

## Trading Domain

Responsible for execution.

### Entities

- Trading Plan
- Order
- Position
- Position Manager Agent
- Execution Engine
- Trade Lifecycle

### Responsibilities

The Position Manager Agent manages only active positions.

Responsibilities include:

- Stop Loss adjustments
- Take Profit adjustments
- Partial Close
- Position Scaling
- Position Protection
- Trade Closing

The Position Manager Agent never opens new trades.

---

## Learning Domain

Responsible for continuous improvement.

### Entities

- Experience
- Reward
- Feedback
- Memory
- Learning Session
- Performance

### Responsibilities

Agents learn from previous trading results.

Knowledge is shared with other agents through the Knowledge Bus.

---

## Infrastructure Domain

Responsible for platform services.

### Components

- Event Bus
- Configuration Manager
- Plugin Loader
- Notification System
- Audit Logs
- Background Jobs
- Storage
- Logging

---

# Ownership Rules

## Account Owner

Owns:

- Capital
- Investment Objective
- Risk Preferences

Does NOT analyze markets.

---

## Portfolio Manager Agent

Owns:

- Investment Objective
- Trading Strategy
- Daily Progress
- Capital Allocation
- Final Trading Plan

The Portfolio Manager Agent is the only AI component allowed to convert recommendations into trading decisions.

---

## Expert Agents

Own:

- Domain Knowledge

Produce:

- Recommendations

Never:

- Open trades
- Close trades
- Know investment objectives
- Interact with the Account Owner

---

## Position Manager Agent

Owns:

- Open Positions

Responsibilities:

- Protect profits
- Reduce losses
- Manage risk after execution
- Optimize exits

Never creates new positions.

---

# Domain Communication

```
Expert Agents

↓

Recommendations

↓

Portfolio Manager Agent

↓

Trading Plan

↓

Execution Engine

↓

Position Manager Agent

↓

Trade Lifecycle

↓

Learning System
```

---

# Guiding Principle

Every component has exactly one responsibility.

Business objectives belong only to the Portfolio Manager Agent.

Market expertise belongs to Expert Agents.

Trade management belongs to the Position Manager Agent.

Learning belongs to the Learning Domain.

This separation keeps the platform modular, scalable, and explainable.
