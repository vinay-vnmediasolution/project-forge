# Evidence Ledger

The portfolio record. If someone reads one file in this repository, it should
be this one.

**Rule:** an entry is created only for a completed, independently inspectable increment. Its status must say whether it is a checkpoint, prototype, supervised pilot, production deployment or retired system. A prototype may evidence a narrow skill, but it cannot satisfy a phase gate that requires real use. Nothing merely planned belongs here; `BACKLOG.md` holds intent.

**Second rule:** every entry must survive *"defend this for twenty minutes."*

**Where the uncomfortable part lives:** each entry has a private counterpart in
`.private/gaps.md` (gitignored) recording what I could **not** defend about
that build. That file is interview preparation, not content, and never
publishes.

---

## Entry template

```
### [Title]

| | |
|---|---|
| **Date** | |
| **Requirements** | R1, R3, ... |
| **Status** | Checkpoint / Prototype / Supervised pilot / Production / Retired |
| **Artefact** | repo / URL |
| **Published as** | article or write-up link, or "not published" |

**Problem** — one sentence. The problem, not the solution.

**Users** — who used it, by role. "Nobody yet" is valid for a checkpoint or prototype and must not be presented as adoption.

**Built** — three sentences. What it does, how it works.

**Measured** — observed change, before and after. "Not measured" stated
explicitly where true; an unmeasured build is weaker but still honest.

**Key trade-off** — the decision that could reasonably have gone the other
way, and why it didn't.

**What I got wrong** — what broke, surprised me, or had to be rebuilt.
Entries without this read as marketing. This is also the most publishable
material in the repository.
```

---

## Entries

*None yet. First entry due 24 August 2026.*

---

## Planned

Sequencing only — not evidence until built.

| # | Working title | Phase | Reqs | Target |
|---|--------------|-------|------|--------|
| 1 | Email triage and classification service | 1 | R1, R2, R7 | 24 Aug |
| 2 | Eval suite and regression harness | 2 | R2, R3 | 21 Sep |
| 3 | Bounded agent with human-in-the-loop approvals | 3 | R1, R2, R5, R6 | 19 Oct |
| 4 | Deployment and operations write-up | 3 | R5, R8 | 26 Oct |
| 5 | Sanitised agent-governance pattern brief | Parallel | R8, R10 | TBC |

---

## Coverage

Updated after each entry. Empty rows are where interview questions will land
hardest.

| Req | Capability | Entries |
|-----|-----------|---------|
| R1 | Production engineering | — |
| R2 | LLM / agentic systems | — |
| R3 | Eval-driven thinking | — |
| R4 | Data engineering | — |
| R5 | Full-stack breadth | — |
| R6 | Prototyping under ambiguity | — |
| R7 | Customer-facing ownership | — |
| R8 | Regulated delivery | — |
| R9 | Enterprise systems | — |
| R10 | Disposition / ownership | — |

---

## Confidentiality

Client and employer material appears only in abstracted form: no names, email content, identifying metadata, internal system details or real figures without written permission. Where a
client outcome is quoted, permission is obtained first and noted against the
entry. See the publishing rule in `PLAN.md`.
