# Plan — 4 August to 26 October 2026

Replaces `CURRICULUM.md` and `SPRINT_0.md`. Twelve weeks, dated. Roadmap
stages 5–7 stay directional and get no calendar until this completes.

**Governing constraint:** every phase ends with software in supervised use by a
real person, an entry in `EVIDENCE.md`, and one published write-up. A phase
ending in documents or understanding alone has not ended.

---

## Method

**Build first, explain after.** Attempt cold, hit the wall, then go deep on the
wall. Fundamentals are taught as the *delta* from existing .NET, C#, SQL and
Azure knowledge — never from first principles.

**Progression is demonstrated, never timed.** No learning item completes
because a period elapsed. It completes when an independent checkpoint is
passed: implementing and debugging without assistance, then examined cold.

**Teaching and examination are separated.** The coach that teaches a concept
does not assess it. A coach cannot reliably detect the gaps it created.

**Coaching disputes are settled by evidence.** Where the coaches disagree,
build the smallest thing that discriminates between the two positions. Working
software and measurement decide — not whichever assistant sounds more certain.

**Evaluation is a design activity before it is a tooling activity.** Tooling
belongs to Phase 2. Deciding what correct means, what ambiguous means, when the
system should abstain, and what each error type costs happens *before* the
first build. A classifier built without that produces something untestable.

**Two tracks, different clocks.**

- *Fast track* — this plan. Dated, gated on shipping, non-negotiable.
- *Depth track* — 2–3 hours weekly. Undated, no deliverables, one substantial
  thing at a time. **The depth track never blocks the fast track.**

**Ambiguity drills.** One 48-hour prototype every fortnight from a deliberately
underspecified brief and messy real input.

**Writing is a deliverable, not a byproduct.** See `WRITING.md`.

---

## Publishing rule

*Carried forward from `CURRICULUM.md` v1 — this rule survives its parent file.*

Public sharing is selected **after** the work exists. Nothing confidential,
employer-specific, client-identifying, or weakly understood is published. A
repository update, case study, diagram, article or post may satisfy the
sharing step; no channel is ever mandatory.

Extension for the public-repo era: **do not publish a claim that cannot be
defended in an interview.** Claims are classified before publication as
defendable, conditional (fixable by precision) or unsupported. Conditional
claims are rewritten, not deleted.

---

## Data boundary

Binding for the whole programme.

- No real client email, personal information, financial identifiers, tax file
  numbers, credentials, or production configuration enters this repository or
  any public artefact. Fixtures are synthetic.
- **Logs record identifiers, categories, confidence scores and rule paths.
  Never message body text.** Diagnosing a misclassification must be possible
  without storing the content that caused it.
- Client written agreement is obtained before any client data is processed,
  covering: what leaves their environment, which provider and region processes
  it, retention settings, and deletion on request.
- The client has obligations to their own customers. This tool inherits them.

---

## Week 0 — 28 July to 3 August

Setup only. No learning content.

- [ ] Push `TARGET_ROLE.md`, `EVIDENCE.md`, `PLAN.md`, `WRITING.md`
- [ ] Update charter Roles section, `AGENTS.md` and README in the same commit —
      the repository must not describe two different operating models
- [ ] Retire `CURRICULUM.md` and `SPRINT_0.md`
- [ ] `.private/` created and gitignored
- [ ] Sprint 1 issue rewritten; old issue closed
- [ ] Client conversation: scope, consent, data handling agreed in writing
- [ ] **Classification spec written** (see Phase 1 pre-build gate)
- [ ] 90-minute independent checkpoint attempted cold and examined
- [ ] Five postings pasted into `TARGET_ROLE.md`; gap scored personally
- [ ] Article 1 drafted

---

## Phase 1 — 4 to 24 August: ship one real LLM service

**Goal:** an email triage and classification service running as a **supervised
pilot** at a client practice — read-only input, human approval on every
outcome, safe failure, auditable decisions, immediate rollback.

Not "in production." Supervised pilot is the honest description and the
defendable claim.

**Requirements:** R1, R2, R7

### Pre-build gate — the classification spec

No code until this exists. One page, living in the build repository.

- The category set, and what each category means at its boundary
- What counts as ambiguous, and what the system does when it is
- Abstention: when the system declines to classify rather than guessing
- **Error cost asymmetry.** In accounting email these costs differ by orders
  of magnitude — a missed statutory deadline notice is severe; a newsletter
  wrongly queued for review costs seconds. This asymmetry drives thresholds,
  abstention behaviour, and what may never be auto-filed.
- What the system is never permitted to do autonomously
- How a wrong classification is noticed, and by whom

This document makes Phase 2 largely mechanical. Skipping it makes Phase 2
impossible.

### Learning, in the order it becomes necessary

- Python delta from C#: dynamic and duck typing, truthiness, comprehensions,
  context managers, decorators, the import and module model
- Environment and packaging: virtualenv, dependency pinning, project layout.
  Where .NET habits mislead most
- Pydantic: validation, model design, why it matters for LLM output
- FastAPI: routing, dependency injection, request lifecycle
- pytest: fixtures, parametrisation, structure
- Structured LLM outputs: schema design, failure modes, retry and fallback
- Secrets, configuration, and privacy-preserving logging

**Gate on the Python delta:** the 90-minute independent checkpoint passed and
examined cold. Not a weekend elapsed.

### Milestones

| Date | Milestone |
|------|-----------|
| 3 Aug | Classification spec complete; checkpoint passed |
| 10 Aug | Deterministic baseline classifying a synthetic corpus, tests passing |
| 17 Aug | **Supervised pilot live with the client** |
| 24 Aug | Hardened; `EVIDENCE.md` entry; **Article 2 published** |

### Gate

- Running as a supervised pilot for at least five working days
- Every misclassification observed is captured — this becomes the Phase 2
  golden dataset and is the most valuable output of the phase
- Teach-back on structured outputs and their failure modes
- One extension built independently, without AI assistance
- Evidence entry complete including "what I got wrong"
- Re-score `TARGET_ROLE.md`

---

## Phase 2 — 25 August to 21 September: evals and data

**Goal:** prove the Phase 1 service works, with a suite that catches it when it
stops working. The classification spec becomes the specification the evals test
against.

The differentiating phase. Most self-taught portfolios contain a demo and no
evidence it functions.

**Requirements:** R2, R3, R4

### Learning

- Golden dataset construction: sampling, labelling, edge case selection
- Eval design against asymmetric error costs — why aggregate accuracy misleads
  when one error type is catastrophic and the other trivial
- Regression testing for non-deterministic output
- LLM-as-judge: where it works, where it fails, validating the judge
- Cost and latency instrumentation
- Data engineering: SQL at speed against unfamiliar schemas, messy data
  wrangling, pipeline basics. Conceptual exposure to Spark, Airflow, dbt

### Milestones

| Date | Milestone |
|------|-----------|
| 31 Aug | Golden dataset built and labelled from real pilot misclassifications |
| 7 Sep | Eval suite running locally, baseline recorded |
| 14 Sep | Evals in CI, failing the build on regression |
| 21 Sep | Cost/latency instrumented; evidence entry; **Article 3 published** |

### Gate

- A deliberately introduced regression is caught by the suite
- Teach-back on why aggregate accuracy is the wrong headline metric here
- Baseline and current numbers recorded and explainable
- Timed SQL exercise against an unfamiliar schema
- Re-score `TARGET_ROLE.md`

---

## Phase 3 — 22 September to 26 October: bounded agent, deployed

**Goal:** an agent with real autonomy inside real constraints — deployed,
observable, written up with measured before and after.

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
this design. Make it explicit in the write-up.

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
algorithm drills.

Applications begin once at least two evidence entries are publicly verifiable.

---

## Rules

1. **One active build.** New ideas go to `BACKLOG.md`.
2. **Shipping beats understanding.** Understanding follows shipping; the
   reverse order was tried and produced documents.
3. **No new governance documents.** This file, the charter, the backlog, the
   journey log, the evidence ledger and the writing pipeline are sufficient.
   Build-specific artefacts — specs, ADRs — live in the build repository.
4. **Gates are negotiable on date, never on evidence.**
5. **If two weeks pass with no commits containing code, the plan has failed**
   and gets diagnosed rather than rewritten.
6. **Writing never substitutes for building.**
7. **Claims match reality.** "Supervised pilot" is not "production." "Reduced
   processing time" requires a measurement. Precision in the repository is
   practice for precision in an interview.

---

## Review

End of each phase: what shipped, what the evidence shows, what the re-score
says, whether the next phase still makes sense. Recorded in `JOURNEY.md`.
