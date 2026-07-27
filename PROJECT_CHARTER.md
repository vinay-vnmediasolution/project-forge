# Project Charter

## Mission

Develop Vinay into an elite Forward Deployed AI Engineer who can turn ambiguous enterprise problems into secure, useful, production-quality AI systems—and create credible evidence of that capability.

## Why Project Forge exists

Vinay already brings enterprise architecture, integration, Azure, delivery, stakeholder, consulting, and product-thinking experience. Project Forge converts those strengths into deeper modern software engineering and applied AI capability through deliberate practice and real delivery.

This is not a collection of tutorials. It is a learning-and-shipping system.

## North star

Consistently discover a meaningful problem, choose a proportionate solution, build it well, deploy it safely, measure the result, and explain the work clearly to both technical and business audiences.

## In scope

- Software engineering fundamentals and professional practice
- Python and TypeScript where they serve real builds
- APIs, data, testing, security, observability, and system design
- Cloud delivery, initially with Azure
- AI and machine-learning fundamentals required for sound decisions
- LLM, retrieval, tool-use, agent, and evaluation engineering
- Product discovery, workflow mapping, ROI, adoption, and consulting
- Enterprise AI governance and operational readiness
- Architecture diagrams, decision records, reflections, and selected public evidence

## Out of scope

- Unrelated personal programmes such as investing, language learning, and fitness
- Confidential employer or client information
- Building multiple showcase products simultaneously
- Websites, visual branding, communities, newsletters, or extra publishing channels before the core programme has momentum
- Chasing every new AI framework
- Creating repositories before a standalone, useful project justifies one
- Activity presented as progress without evidence of understanding or delivery

Other initiatives may offer safe use cases or benefit from Project Forge skills. Cross-pollination is welcome; shared execution and blurred ownership are not.

## Working principles

1. **Ship each phase.** Produce working, reviewable evidence, not theory alone.
2. **One active build.** New ideas go to the parking lot unless they replace current scope deliberately.
3. **Finish before expanding.** Meet the definition of done before starting the next major build.
4. **Learn just in time, then go deeper.** Alternate explanation, implementation, feedback, and improvement.
5. **Solve real problems.** Prefer small, useful systems over large demonstrations with invented value.
6. **Evidence over confidence.** Use working behaviour, tests, decisions, explanations, and user outcomes.
7. **Safety by design.** Protect secrets, privacy, client information, and production systems.
8. **Durable source of truth.** Material decisions and progress belong in the repository, not only in chat.

## Roles

### Learner and builder — Vinay

- Protect focused time.
- Attempt the work first and ask specific questions.
- Explain decisions in his own words.
- Reflect honestly on gaps, surprises, and mistakes.
- Decide what is safe and worthwhile to publish.
- Resolve coaching disagreements with evidence, not preference.

### Primary coach — teaching, design review, code review

- Teach as a delta from existing .NET, Azure, integration and delivery
  experience. Never from first principles.
- Review design and code; challenge decisions.
- Hold the programme against stated priorities and flag drift.
- Does not assess what it has taught.

### Examiner — independent assessment and second opinion

- Sets independent checkpoints completed without AI assistance.
- Examines teach-backs cold and probes for gaps.
- Provides a genuinely independent architectural opinion, including
  disagreement with the primary coach.
- Examines public claims as directly evidenced, defendable with attribution,
  conditional and requiring qualification, or unsupported.
- Interrogates drafts as a hostile hiring panel would and identifies claims
  Vinay cannot yet defend.
- Does not ghostwrite articles or allow drafting to replace shipping.
- Runs interview simulation from November.
- Does not generate curriculum, plans, or repository structure.

### Engineering agents — Codex and Claude Code

- Work from repository issues and written acceptance criteria.
- Implement, test, review, and document within agreed scope.
- Explain material design choices rather than hiding them behind generated
  code.
- Never replace the learner's understanding or reflection.

### Separation principle

Teaching and assessment are held by different parties. A coach cannot reliably
detect the gaps it created. Where coaches disagree, build the smallest thing
that discriminates between the positions; working software and measurement
decide.


## Definition of done

### Independent learning checkpoint

A checkpoint is done when Vinay has attempted it without AI assistance, can explain and debug the result under cold examination, and has identified where documentation or prior knowledge was insufficient. Elapsed time, completed notes and assisted code do not satisfy this gate.

### Project increment

A project increment is done when:

- the agreed behaviour works and proportionate automated checks pass;
- configuration and diagnostics respect the data boundary;
- setup, operation, failure handling and rollback are understood;
- material trade-offs are recorded without creating unnecessary governance;
- Vinay can demonstrate, explain and modify the increment;
- user value is measured where the claim depends on measurement.

A prototype, supervised pilot and production deployment are different states and must be described accurately.

### Phase

A phase is done only when the gate in `PLAN.md` is met, the evidence is recorded in `EVIDENCE.md`, and any public write-up has passed the standards in `WRITING.md`. Incomplete work is split, returned to the backlog or dropped explicitly.

## Governance

- `PLAN.md` governs the dated fast track; `ROADMAP.md` is directional.
- GitHub issues hold executable work. Build-specific specifications and decisions live with the build.
- No new governance document is added unless an existing source of truth cannot hold the decision.
- Dates may move; evidence gates do not weaken.
- When capacity is constrained, reduce scope before reducing safety or evidence quality.
- “Parking lot” remains a valid way to stop premature expansion.
