# AGENTS.md

This file guides coding agents working in this repository.

## Mission

Help Vinay develop demonstrable Forward Deployed AI Engineering capability through focused learning, useful builds, explicit trade-offs, and completed increments.

## Source of truth

Read these before making substantive changes:

1. `PROJECT_CHARTER.md`
2. `PLAN.md`
3. The active GitHub issue and its acceptance criteria
4. Any build-specific specification or decision record referenced by that issue
5. `TARGET_ROLE.md` and `EVIDENCE.md` when the work claims portfolio value

If chat instructions conflict with committed project decisions, identify the conflict instead of silently choosing. `PLAN.md` governs programme sequencing; the active issue governs implementation scope.

## Working rules

- Inspect the repository before editing.
- Work on one clearly scoped issue at a time.
- Preserve existing user changes and unrelated work.
- Prefer the smallest useful vertical slice.
- Explain material design decisions and trade-offs.
- Add proportionate tests and documentation.
- Keep configuration external and never commit secrets.
- Use sanitised examples; do not invent or expose confidential employer or client details.
- Update durable project files when a decision or learning must survive the chat.
- Place new ideas in the backlog or parking lot rather than implementing them opportunistically.

## Learning guardrails

Agents accelerate implementation without replacing learning:

- Teach only the delta from Vinay's existing .NET, Azure, SQL, integration and delivery experience.
- Let the current build expose the learning need; do not generate a parallel curriculum.
- Ask Vinay to explain material choices and failure modes in his own words.
- Keep generated code small enough to inspect, test and modify independently.
- Do not write Vinay's teach-back, reflection, evidence claim or public article for him.
- Curated notes under `learning/` are optional review aids, not gates or an active course sequence.
- Independent checkpoints are completed without AI assistance; agents must not solve or rehearse them.

## Current scope

Phase 1 is the email-triage and classification service described in `PLAN.md`.

Before client-build code begins, verify that:

- the classification specification defines category boundaries, ambiguity, abstention and asymmetric error costs;
- written client agreement covers data scope, provider and processing region, retention and deletion;
- fixtures are synthetic and the real corpus remains client-side.

The pilot is read-only, requires human approval for every outcome, fails safely, is auditable and can be rolled back immediately. Do not describe it as autonomous or production-ready.

Do not add a website, branding, community channels, parallel products or new repositories.

## Completion

Before declaring work complete:

- verify the acceptance criteria;
- run relevant checks;
- inspect the final diff;
- report exactly what changed;
- name any remaining blocker or unverified assumption.

## Roles and separation

Role definitions live in `PROJECT_CHARTER.md` under "Roles". Teaching and
assessment are deliberately separated; see the separation principle there.

Engineering agents work only from issues with written acceptance criteria.
Where an issue conflicts with `PLAN.md`, `PLAN.md` wins and the issue is
corrected.

## Data boundary

Binding on all agents. No real client email, personal information, financial
identifiers, credentials, or production configuration in this repository.
Fixtures are synthetic. Logs use opaque correlation IDs and record categories, confidence scores and generic rule codes. They never record sender, recipient, subject, body, attachment content, extracted financial entities, raw prompts, raw model responses or credentials.

