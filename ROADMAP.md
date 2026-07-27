# Roadmap v1

This roadmap describes capability progression, not a fixed calendar. Advancement depends on evidence from completed work.

## Stage 0 — Establish the operating system

**Outcome:** Project Forge has a clear mission, working agreements, definitions of done, a small backlog, and a ready first sprint.

**Evidence:** The Sprint 0 foundation is committed and the first learning sprint is ready.

## Stages 1–4 — Current twelve-week fast track

The dated sequence, milestones and gates are maintained only in [PLAN.md](PLAN.md). In summary:

1. **Supervised email-classification pilot** — define correctness and risk boundaries first; build a deterministic baseline and then a structured LLM service; keep all outcomes human-approved.
2. **Evaluation and data** — build the client-side golden dataset, measure category-specific errors, catch regressions in CI, and instrument cost and latency.
3. **Bounded agent and deployment** — add autonomy only where justified, with approvals, auditability, Azure deployment and observability.

These stages develop production Python, Pydantic, FastAPI, pytest, structured outputs, data handling, evaluations and deployment through one real client problem. The previous Automation Opportunity Scorer direction is retired.

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

Only the twelve-week fast track is dated. Stages 5–7 remain directional until its evidence gates are complete.

