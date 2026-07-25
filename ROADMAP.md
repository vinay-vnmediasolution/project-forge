# Roadmap v1

This roadmap describes capability progression, not a fixed calendar. Advancement depends on evidence from completed work.

## Stage 0 — Establish the operating system

**Outcome:** Project Forge has a clear mission, working agreements, definitions of done, a small backlog, and a ready first sprint.

**Evidence:** The Sprint 0 foundation is committed and the first learning sprint is ready.

## Stage 1 — Engineering foundations through a useful API

**Capability:** Build and explain a production-minded Python service.

Topics include:

- Python fundamentals and type hints
- HTTP and REST API design
- validation, error handling, configuration, and logging
- SQL and persistence
- unit and integration testing
- Git workflow and code review
- containers and basic delivery

**Anchor to prior experience:** Translate familiar enterprise integration, API, release, and Azure concepts into the Python ecosystem.

**Initial build:** A small, useful **Automation Opportunity Scorer API** that captures a workflow problem and produces a transparent, rules-based opportunity score. AI is intentionally not required in the first increment.

## Stage 2 — System design and dependable delivery

**Capability:** Design a service that remains understandable and operable as requirements grow.

Topics include:

- modular and hexagonal design
- domain modelling and boundaries
- authentication and authorization
- asynchronous work, messaging, and idempotency
- observability and failure handling
- CI/CD and Azure deployment
- architecture decision records

**Build evolution:** Turn the scorer into a deployable service with persistence, identity, auditability, and operational evidence.

## Stage 3 — Data and AI foundations

**Capability:** Make informed AI design choices rather than treating models as magic.

Topics include:

- probability, evaluation, and data quality
- tokens, embeddings, attention, and transformers
- model limitations, latency, cost, and privacy
- structured outputs and tool calling
- responsible use and threat modelling

**Build evolution:** Add an evidence-based AI-assisted analysis behind a clear interface and compare it with the deterministic baseline.

## Stage 4 — LLM application engineering

**Capability:** Build grounded, testable LLM applications.

Topics include:

- prompt and context design
- retrieval pipelines and source attribution
- structured outputs and tool integration
- model selection and routing
- caching, cost, latency, and resilience
- evaluation datasets and regression testing

**Showcase direction:** An AI Discovery Consultant that analyses sanitised process material and produces traceable opportunities, questions, risks, and next steps.

## Stage 5 — Agent and workflow engineering

**Capability:** Decide when an agent is justified and build one with bounded autonomy.

Topics include:

- workflows versus agents
- state, planning, memory, and tool use
- MCP and integration contracts
- approvals and human-in-the-loop design
- multi-agent trade-offs
- agent evaluation and observability

**Build evolution:** Add controlled research or workflow tools only where they create measurable value.

## Stage 6 — Forward deployment

**Capability:** Own the path from discovery to adoption.

Topics include:

- stakeholder interviews and workflow mapping
- problem framing and opportunity scoring
- prototype strategy
- ROI and success metrics
- deployment, change management, and adoption
- executive communication and technical handover

**Capstone:** Run a sanitised end-to-end engagement from discovery through measured pilot and retrospective.

## Stage 7 — Enterprise AI leadership

**Capability:** Lead safe, scalable AI delivery across an organisation.

Topics include:

- identity, privacy, governance, and compliance
- auditability and model risk
- platform patterns and reusable accelerators
- operating models and portfolio prioritisation
- build/buy/partner decisions
- coaching teams and communicating strategy

## Review gates

At the end of each stage:

1. Demonstrate the working system.
2. Explain the architecture and trade-offs.
3. Complete a practical assessment without agent-generated answers.
4. Review business value and user evidence.
5. Decide whether to deepen, remediate, or advance.

Only Stage 1 should be planned in detail during Sprint 0. Later stages remain direction, not active scope.

