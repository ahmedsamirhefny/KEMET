# KEMET

> Production-grade Multi-Agent Finance Intelligence Platform built with Python.

KEMET is a Multi-Agent Finance Intelligence Platform that models how professional traders and portfolio managers make investment decisions using collaborative artificial intelligence.

Instead of relying on a single AI model, KEMET decomposes the investment process into a team of specialized AI agents. Each agent is responsible for a single domain of expertise and publishes structured recommendations. A Portfolio Manager Agent evaluates these recommendations and produces the final investment decision.

KEMET is designed to be explainable, modular, scalable, and production-ready.

---

# Why KEMET?

Most AI trading systems rely on a single model making a single decision.

Professional investment teams work differently.

Technical analysts, economists, news analysts, and risk managers collaborate before any investment decision is made.

KEMET models this collaborative decision-making process using specialized AI Agents.

This architecture provides:

- Explainable Decisions
- Domain Expertise
- Modular Design
- Collective Intelligence
- Continuous Improvement

---

# Vision

Professional traders never rely on a single indicator or one source of information.

They combine:

- Technical Analysis
- Fundamental Analysis
- Market News
- Economic Events
- Risk Management
- Capital Allocation
- Experience

Professional investing is a collaborative decision-making process.

KEMET models that collaboration using AI Agents.

---

# Philosophy

KEMET is **not** a trading bot.

KEMET is a Finance Intelligence Platform.

Its purpose is to replicate the structured thinking process of professional traders and portfolio managers.

Artificial Intelligence is the implementation technology—not the architecture.

The architecture is inspired by real investment teams.

KEMET separates domain expertise from decision making.

---

# Actors

KEMET has only one human actor.

- Account Owner

The Account Owner defines:

- Investment Objectives
- Risk Preferences
- Execution Permissions

All remaining components are autonomous AI Agents collaborating to achieve those objectives.

---

# Architecture Overview

```text
                     Market
                        │
                        ▼
               Data Collection
                        │
                        ▼
          Specialized AI Agents
                        │
                        ▼
              Recommendations
                        │
                        ▼
          Recommendation Events
                        │
                        ▼
          Portfolio Manager Agent
                        │
                        ▼
              Final Decision
                        │
                        ▼
             Execution Engine
                        │
             ┌──────────┴──────────┐
             ▼                     ▼
        Monitoring            Audit Logs
             │                     │
             └──────────┬──────────┘
                        ▼
               Knowledge Sharing
                        │
                        ▼
                 Agents Improve
```

---

# Core Principles

- Multi-Agent Architecture
- Domain-Driven Design
- Event-Driven Communication
- Recommendation-Based Collaboration
- Explainable AI
- Risk-First Design
- Human-in-the-Loop
- Knowledge Sharing
- Production-Ready Engineering
- Continuous Learning

---

# Expert Agents

Current planned agents include:

- Portfolio Manager Agent
- News Agent
- Economic Calendar Agent
- Technical Analysis Agent
- Market Regime Agent
- Risk Management Agent
- Portfolio Agent
- Sentiment Agent
- TradingView Agent
- Monitoring Agent
- Mentor Agent
- Audit Agent

The platform is designed to support additional agents through a plugin-based architecture.

---

# Knowledge Sharing

Agents never control each other.

Agents never execute trades independently.

Every Expert Agent publishes structured Recommendations.

Recommendations are transported through Recommendation Events over the internal Event Bus.

The Portfolio Manager Agent evaluates every recommendation before producing the final investment decision.

This architecture enables Collective Intelligence while preserving the independence of every agent.

---

# Technology Stack

## Backend

- Python
- FastAPI
- SQLAlchemy
- PostgreSQL

## Desktop Application

- Flet

## Infrastructure

- Docker
- Nginx
- Linux
- GitHub Actions

## LLM Providers

- OpenAI
- Ollama
- Hugging Face

## AI Frameworks

- LangChain
- MCP

---

# Project Structure

```text
docs/
src/
tests/
scripts/
docker/
configs/
```

---

# Project Status

Current Sprint

✅ Sprint 0 — Foundation & Architecture

Next Sprint

🚀 Sprint 1 — Core Domain Implementation

---

# Roadmap

- Sprint 0 — Foundation & Architecture
- Sprint 1 — Core Domain
- Sprint 2 — Application Layer
- Sprint 3 — Expert Agents
- Sprint 4 — Portfolio Manager
- Sprint 5 — Knowledge Sharing
- Sprint 6 — Learning System
- Sprint 7 — Execution Engine
- Sprint 8 — Desktop Platform
- Sprint 9 — Monitoring & Audit
- Sprint 10 — Cloud Deployment
- Sprint 11 — Production Release

More details are available in **docs/roadmap.md**

---

# Goals

- Build a production-grade AI Finance Platform.
- Demonstrate advanced Python architecture.
- Showcase AI Engineering best practices.
- Build an extensible Multi-Agent Framework.
- Apply Domain-Driven Design and Event-Driven Architecture.
- Model professional investment decision making using collaborative AI.

---

# Documentation

Project documentation is available under the `docs/` directory.

Key documents include:

- Vision
- Roadmap
- Architecture
- Domain Model
- Decisions
- ADRs
- Glossary
- Session Journal

---

# License

License selection is postponed until the first public release.

---

# Author

Designed and developed by

**Ahmed Samir**

GitHub:

https://github.com/ahmedsamirhefny

---

> KEMET does not attempt to replace traders.

> It attempts to model the structured thinking process of professional traders and portfolio managers using collaborative artificial intelligence.