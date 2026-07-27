# Plan — 4 August to 26 October 2026

Replaces `CURRICULUM.md` and `SPRINT_0.md`. Twelve weeks, dated. Roadmap
stages 5–7 stay directional and get no calendar until this completes.

**Governing constraint:** every phase ends with software in use by a real
person, an entry in `EVIDENCE.md`, and one published write-up. A phase ending
in documents or understanding alone has not ended.

---

## Method

**Build first, explain after.** Attempt cold, hit the wall, then go deep on the
wall. Fundamentals are taught as the *delta* from existing .NET, C#, SQL and
Azure knowledge — never from first principles.

**Teaching and examination are separated.** The coach that teaches a concept
does not assess it. A coach cannot reliably detect the gaps it created.

**Two tracks, different clocks.**

- *Fast track* — this plan. Dated, gated on shipping, non-negotiable.
- *Depth track* — 2–3 hours weekly. Undated, no deliverables, one substantial
  thing at a time: papers, book chapters, system teardowns. **The depth track
  never blocks the fast track.** Reading about a technique instead of shipping
  is the exact failure mode this rule exists to prevent.

**Ambiguity drills.** One 48-hour prototype every fortnight from a deliberately
underspecified brief and messy real input. This is the interview and the job.

**Writing is a deliverable, not a byproduct.** See `WRITING.md`.

---

## Publishing rule

*Carried forward from `CURRICULUM.md` v1 — this rule survives its parent file.*

Public sharing is selected **after** the work exists. Nothing confidential,
employer-specific, client-identifying, or weakly understood is published. A
repository update, case study, diagram, article or post may satisfy the
sharing step; no channel is ever mandatory.

Extension for the public-repo era: **do not publish a claim that cannot be
defended in an interview.** Anything written publicly becomes a question a
panel is entitled to ask.

---

## Week 0 — 28 July to 3 August

Setup only. No learning content.

- [ ] Repo restructured: `TARGET_ROLE.md`, `EVIDENCE.md`, `PLAN.md`,
      `WRITING.md` in; `CURRICULUM.md` and `SPRINT_0.md` retired
- [ ] `.private/` created and gitignored
- [ ] Five real postings pasted into `TARGET_ROLE.md`, gap-scored personally
- [ ] Sprint 1 issue rewritten around shipping
- [ ] Examiner role handed over and confirmed
- [ ] Client conversation: Phase 1 scope confirmed
- [ ] Article 1 drafted (the recalibration piece — see `WRITING.md`)

---

## Phase 1 — 4 to 24 August: ship one real LLM service

**Goal:** an email triage and classification service in genuine daily use at a
client practice.

**Not** a Python course. Language delta gets one weekend and is sufficient when
it stops blocking the build.

**Requirements:** R1, R2, R7

### Learning, in the order it becomes necessary

- Python delta from C#: dynamic and duck typing, truthiness, comprehensions,
  context managers, decorators, the import and module model
- Environment and packaging: virtualenv, dependency pinning, project layout.
  Budget real time — this is where .NET habits mislead most
- Pydantic: validation, model design, why it matters for LLM output
- FastAPI: routing, dependency injection, request lifecycle
- pytest: fixtures, parametrisation, structure
- Structured LLM outputs: schema design, failure modes, retry and fallback
- Secrets and configuration handling

### Milestones

| Date | Milestone |
|------|-----------|
| 10 Aug | Local service classifies a real corpus, tests passing |
| 17 Aug | **First version in genuine client use** |
| 24 Aug | Hardened; `EVIDENCE.md` entry; **Article 2 published** |

### Gate

- In daily use, not demonstrated once
- Teach-back on structured outputs and their failure modes
- One extension built independently, without AI assistance
- Evidence entry complete including "what I got wrong"
- Re-score `TARGET_ROLE.md`

---

## Phase 2 — 25 August to 21 September: evals and data

**Goal:** prove the Phase 1 service works, with a suite that catches it when it
stops working.

The differentiating phase. Most self-taught portfolios contain a demo and no
evidence it functions.

**Requirements:** R2, R3, R4

### Learning

- Golden dataset construction: sampling, labelling, edge case selection
- Eval design: precision/recall trade-offs where error costs differ, and why
  aggregate accuracy misleads
- Regression testing for non-deterministic output
- LLM-as-judge: where it works, where it fails, validating the judge
- Cost and latency instrumentation
- Data engineering: SQL at speed against unfamiliar schemas, messy data
  wrangling, pipeline basics. Conceptual exposure to Spark, Airflow, dbt —
  enough to hold a design conversation, not to claim expertise

### Milestones

| Date | Milestone |
|------|-----------|
| 31 Aug | Golden dataset built and labelled |
| 7 Sep | Eval suite running locally, baseline recorded |
| 14 Sep | Evals in CI, failing the build on regression |
| 21 Sep | Cost/latency instrumented; evidence entry; **Article 3 published** |

### Gate

- A deliberately introduced regression is caught by the suite
- Teach-back on why aggregate accuracy is the wrong headline metric
- Baseline and current numbers recorded and explainable
- Timed SQL exercise against an unfamiliar schema
- Re-score `TARGET_ROLE.md`

---

## Phase 3 — 22 September to 26 October: bounded agent, deployed

**Goal:** an agent with real autonomy inside real constraints — deployed,
observable, and written up with measured before and after.

**Requirements:** R1, R2, R5, R6, R8

### Learning

- Workflows versus agents: when autonomy is justified, when it is overhead
- Tool design and contracts; MCP
- Human-in-the-loop approval patterns; risk-tiered actions
- Audit trails and traceable decisions
- Azure deployment: containers, CI/CD, managed identity
- Observability for non-deterministic systems: tracing, cost, failure modes
- Agent evaluation, extending the Phase 2 suite

**Transferable asset:** existing enterprise experience with risk-gated
automation and read/write/destructive action classification maps directly onto
this design. That is an architectural conversation most candidates cannot have
— make it explicit in the write-up.

### Milestones

| Date | Milestone |
|------|-----------|
| 5 Oct | Agent operating locally with bounded tool access |
| 12 Oct | Approval workflow and audit trail complete |
| 19 Oct | Deployed to Azure with observability |
| 26 Oct | **Case study published** with measured before/after; evidence entry |

### Gate

- Deployed, running, being used
- Case study published with real measurement
- Teach-back on the autonomy boundary and why it sits where it does
- Full re-score against `TARGET_ROLE.md`

---

## From November

Interview preparation as a separate track: ambiguous problem framing, live
prototyping, stakeholder translation, system design under uncertainty. Not
algorithm drills — reported FDE interviews test deployment thinking under
ambiguity.

Applications begin once at least two evidence entries are publicly verifiable.

---

## Rules

1. **One active build.** New ideas go to `BACKLOG.md`.
2. **Shipping beats understanding.** Understanding follows shipping; the
   reverse order was tried and produced documents.
3. **No new governance documents.** This file, the charter, the backlog, the
   journey log, the evidence ledger and the writing pipeline are sufficient.
   Adding process is the known drift.
4. **Gates are negotiable on date, never on evidence.**
5. **If two weeks pass with no commits containing code, the plan has failed**
   and gets diagnosed rather than rewritten.
6. **Writing never substitutes for building.** An article about work not yet
   done does not publish.

---

## Review

End of each phase: what shipped, what the evidence shows, what the re-score
says, whether the next phase still makes sense. Recorded in `JOURNEY.md`.
