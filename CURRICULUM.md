# Curriculum v1

## Learning method

Each topic uses a repeatable cycle:

1. **See it** — a visual model, worked example, or system trace.
2. **Understand it** — the essential theory and vocabulary.
3. **Connect it** — relate it to Vinay's enterprise, Azure, integration, delivery, consulting, or product experience.
4. **Build it** — implement a small vertical slice.
5. **Test it** — verify behaviour and explore failure cases.
6. **Explain it** — teach it back in plain language.
7. **Reflect and reuse** — capture lessons and extract a reusable asset where justified.

## Capability strands

These strands develop together rather than as isolated courses:

- Software engineering
- Architecture and system design
- Cloud and operations
- Data and AI engineering
- Product and customer discovery
- Communication and consulting
- Security, governance, and responsible delivery

## First learning block: four two-week sprints

Only Sprint 1 is considered ready after Sprint 0. Sprints 2–4 are forecast and will be replanned using evidence.

### Sprint 1 — A useful Python API

**Question:** How does a professional Python API differ from a script or a demo?

**Learn**

- Python project structure, functions, classes, type hints, and dependency management
- HTTP requests, responses, status codes, and REST resource design
- validation, error handling, automated tests, and safe configuration
- the difference between domain rules and transport code

**Build**

The first vertical slice of an Automation Opportunity Scorer API:

- accept a sanitised workflow description and measurable pain indicators;
- validate the request;
- calculate a transparent deterministic score;
- return the score, contributing factors, and suggested next discovery questions;
- include unit tests and API-level tests.

**Relate**

- Compare Python typing and project structure with familiar .NET patterns.
- Connect API contracts to enterprise integration experience.
- Connect repeatable tests to release and automation disciplines.

**Demonstrate**

- run the API and tests;
- explain the request path from endpoint to domain rule and back;
- explain one design decision and one rejected alternative.

### Sprint 2 — Persistence and service boundaries

**Question:** How do we preserve useful data without coupling every concern?

Forecast topics:

- relational modelling and SQL
- repository boundaries and migrations
- configuration and structured logging
- integration tests and test isolation

Forecast increment:

- persist assessments and retrieve their history;
- record score-version information so results remain explainable.

### Sprint 3 — Delivery and operability

**Question:** What changes when software must run reliably for someone else?

Forecast topics:

- containers
- CI checks
- health and readiness
- logging, metrics, and failure modes
- initial Azure deployment options

Forecast increment:

- package and deploy the service with a reproducible path and basic operational evidence.

### Sprint 4 — Discovery and product evidence

**Question:** Does the system help someone make a better decision?

Forecast topics:

- discovery interviews
- workflow mapping
- outcome metrics
- usability feedback
- architecture communication

Forecast increment:

- test the service against safe, realistic scenarios;
- refine the score and questions using feedback;
- produce the first compact case study and learning review.

## Standard lesson evidence

For each substantial topic:

- a short teach-back;
- a working change or focused exercise;
- tests or another proportionate verification;
- one architecture or trade-off note;
- a reflection linked from the relevant issue.

## Assessment

Assessment combines:

- **Explain:** clear teach-back without copied wording.
- **Apply:** complete a small change with decreasing scaffolding.
- **Diagnose:** find and explain a defect or design weakness.
- **Design:** compare options and defend a choice.
- **Deliver:** produce a usable, verified increment.
- **Reflect:** identify what was learned and what remains uncertain.

Self-ratings may guide planning, but advancement is based on evidence.

## Publishing rule

Public sharing is selected after the work exists. Nothing confidential, employer-specific, client-identifying, or weakly understood is published. A useful repository update, case study, diagram, article, or post may satisfy the sharing step; every channel is never required.

