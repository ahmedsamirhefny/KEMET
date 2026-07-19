# KEMET Glossary

> Official terminology used across the KEMET platform.

---

## Account Owner

The only human actor in the platform.

Defines investment objectives, risk preferences, and execution permissions.

---

## Portfolio Manager Agent

The only AI agent responsible for achieving the Account Owner's investment objectives.

It evaluates all expert recommendations, manages portfolio risk, and produces the final trading decision.

---

## Expert Agent

A specialized AI agent responsible for a single domain of expertise.

Examples:

- Technical Analysis
- News Analysis
- Economic Analysis
- Risk Analysis
- TradingView Analysis
- Market Regime Analysis
- Sentiment Analysis

Expert Agents never execute trades and never know investment objectives.

---

## Recommendation

A structured opinion produced by an Expert Agent.

Recommendations contain analysis, confidence, reasoning, evidence, and risk assessment.

Recommendations are the universal communication language inside KEMET.

---

## Recommendation Event

A standardized event used to publish Recommendations through the Event Bus.

The Event transports the Recommendation without modifying it.

---

## Event Bus

The communication layer responsible for delivering events between AI agents.

Agents never communicate directly.

---

## Knowledge

Validated experience or information that can be shared between agents.

Knowledge may originate from historical trading, market behavior, or other expert agents.

---

## Mentor Agent

An AI agent responsible for improving other agents by sharing validated knowledge and historical experience.

The Mentor Agent never makes trading decisions.

---

## Portfolio

Represents the managed trading capital and its current investment state.

---

## Investment Objective

Defines what the Account Owner expects to achieve.

Examples:

- Daily Profit Target
- Weekly Profit Target
- Monthly Profit Target
- Maximum Drawdown

---

## Position Management

Responsible for managing open positions after execution.

Examples include:

- Trailing Stop
- Stop Loss adjustment
- Take Profit optimization
- Partial Close

---

## Execution Strategy

Defines how approved trading decisions are delivered.

Execution may occur through:

- Notification
- Manual confirmation
- MT5 integration
- Broker API

---

## Learning

The continuous improvement process of the platform.

Learning is based on historical outcomes, agent feedback, and validated trading experience.

---

## Confidence

A numerical estimation representing how strongly an agent believes in its Recommendation.

---

## Evidence

The supporting facts behind a Recommendation.

Examples include technical indicators, economic events, market structure, and volatility metrics.

---

## AI Committee

The collection of Expert Agents collaborating under the Portfolio Manager Agent.

The committee models the decision-making process of a professional investment team.