# Decisions

## Project

- Project Name: KEMET
- Type: Finance Intelligence Platform

---

## Technology

- Python
- Flet
- FastAPI
- PostgreSQL
- Docker
- uv
- VS Code
- CachyOS

---

## Architecture

- Multi-Agent Architecture
- Three-Layer Design
- AI Orchestrator
- Learning Layer
- Risk First

---

## Development Rules

- Documentation before implementation.
- Feature Branch Workflow.
- Conventional Commits.
- Testable Code.
- Modular Design.

# Decisions

> This document records the major architectural and technical decisions made during the KEMET project.
>
> Once accepted, decisions should not be modified without creating a new decision.

---

# Decision #001

Project name is **KEMET**.

Reason:
Represents the ancient Egyptian identity of the platform.

---

# Decision #002

KEMET is an **AI Finance Intelligence Platform**, not a trading bot.

---

# Decision #003

The initial supported market is **XAUUSD (Gold)**.

Other markets will be added later.

---

# Decision #004

Frontend will be built using **Flet**.

The platform must support:

- Desktop
- Web
- Mobile

From a single codebase.

---

# Decision #005

Backend APIs will be implemented using **FastAPI**.

---

# Decision #006

The project follows **Clean Architecture**.

Business logic must remain independent from frameworks.

---

# Decision #007

Communication between components follows an **Event-Driven Architecture**.

---

# Decision #008

The platform follows a **Multi-Agent Architecture**.

Each AI Agent has exactly one responsibility.

---

# Decision #009

AI Agents collaborate using recommendations rather than direct commands.

---

# Decision #010

Learning is implemented as a dedicated domain.

Knowledge is shared between agents.

Agents improve through accumulated experience.

---

# Decision #011

Risk Management has higher priority than Profit Generation.

Every trading decision must satisfy risk constraints before execution.

---

# Decision #012

Portfolio Manager Agent is the only component responsible for achieving Investment Objectives.

---

# Decision #013

Expert Agents never know business objectives.

---

# Decision #014

Recommendations are Domain Objects.

---

# Decision #015

Events transport Recommendations.

---

# Decision #016

All Events follow a standardized Event Envelope.

---

# Decision #017

The Account Owner is the only human actor in the system.

# Decision #018

Every completed session must produce tangible project artifacts.

Each session should end with:

- Updated documentation
- Architecture review (if needed)
- Decisions review
- ADR review (if needed)
- Session journal
- Git commit message
- Next session plan

No session is considered complete until its documentation is synchronized with the project state.