# Writing Pipeline

Public writing is a deliverable of this programme, not a byproduct of it.

---

## Audience

**Not beginners.** Every bootcamp graduate is publishing a learning journey and
that genre is saturated.

The audience is **senior enterprise practitioners retooling into applied AI**:
architects, delivery leads, engineering managers and consultants with fifteen
or twenty years behind them who can already reason about systems, and who want
to know what actually transfers and what doesn't. Almost nobody is writing for
them. It happens to be the same audience that buys consulting.

Secondary readers: hiring managers for FDE and applied-AI roles, who will read
this as evidence.

---

## The standard

1. **No article without a shipped artefact behind it.** Writing follows
   building. An essay about work not yet done does not publish.
2. **Lead with what went wrong.** The `EVIDENCE.md` "what I got wrong" field is
   the most publishable material in this repository. A post about a thing that
   worked first time is a post nobody needed.
3. **Show the artefact.** Link the repo, the eval output, the diagram, the
   number. Assertion without artefact reads as content marketing.
4. **Never publish an undefendable claim.** Anything written publicly becomes a
   question a hiring panel is entitled to ask. Write to that bar.
5. **No confidential material.** Publishing rule in `PLAN.md` governs. Employer
   abstracted to "a tier-1 Australian bank" or "a large regulated enterprise";
   client to "an accounting practice." Client outcomes quoted only with
   written permission.
6. **Concrete over conceptual.** "Here is the eval that caught my classifier
   degrading, here is the data" beats "reflections on evaluation."

---

## Cadence

- **One substantial article per phase.** Four across the twelve weeks.
- **Short journal entries** as they occur, in `JOURNEY.md`. Some become
  articles; most don't, and that's the point of separating them.
- Drafting is time-boxed. If an article takes more than three hours it is
  competing with the build and gets cut back or deferred.

---

## Backlog

Working titles. Sequenced against the plan. Cut freely — this is a backlog,
not a commitment.

| # | Working title | Ships after | Angle |
|---|--------------|-------------|-------|
| 1 | I threw out my AI learning plan three weeks in | Week 0 | An AI coach built me a curriculum that taught Python from first principles to someone with twenty years of .NET. Why that happens, and what I replaced it with. Honest, contrarian, publishable now. |
| 2 | What actually transfers from twenty years of .NET to Python | Phase 1 | The real delta. Packaging, typing model, idioms. What senior enterprise habits actively mislead. Scarce and concrete. |
| 3 | Your AI demo works. Prove it still works next Tuesday. | Phase 2 | Evals explained for enterprise architects, using a real suite catching a real regression, with the data shown. |
| 4 | When an agent is justified, and when it's just overhead | Phase 3 | Autonomy boundaries and risk-tiered approvals, drawing on governance experience most AI builders don't have. |
| 5 | Case study: a bounded agent in production | Phase 3 | The full engagement — problem, build, deployment, measured before and after. The cornerstone piece. |
| — | Agent governance in a regulated enterprise | Parallel | Sanitised pattern brief. Highest-value asset; requires the redaction pass and a policy check before publication. |
| — | Accuracy is the wrong headline metric | Spare | Split from #3 if it runs long. |
| — | What a hiring panel actually screens for | Spare | The `TARGET_ROLE.md` research, written up. |

---

## Pre-publish checklist

Run on every piece before it goes out.

- [ ] Artefact exists and is linked
- [ ] Every claim defendable under twenty minutes of questioning
- [ ] No employer name, internal system, client identity, or real internal
      figure
- [ ] Contains at least one thing that went wrong
- [ ] Someone with twenty years of experience would learn something
- [ ] Would still stand behind this in an interview in six months
- [ ] Cross-linked from `EVIDENCE.md` ("Published as")

---

## Distribution

Primary: LinkedIn, under own name. The repository is the artefact each article
points back to.

Not doing yet, and deliberately: newsletter, blog platform, video, community.
The charter's out-of-scope list rules these out until the core programme has
momentum. Revisit no earlier than November.
