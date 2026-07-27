# Curriculum v1

## Learning method

Project work applies the curriculum; it does not replace it. Every substantial topic follows this sequence:

1. **Orient** — establish where the topic fits and why it matters.
2. **Understand** — learn the fundamentals and vocabulary from first principles.
3. **See it** — use a diagram, worked example, or system trace to form a mental model.
4. **Connect it** — relate the concept to Vinay's .NET, Azure, enterprise integration, delivery, consulting, or product experience.
5. **Observe it** — study worked examples that are independent of the active project.
6. **Check it** — answer questions that test the mental model.
7. **Practise it** — complete a small isolated exercise with appropriate guidance.
8. **Apply it** — use the understood concept in a later project increment.
9. **Demonstrate it** — complete an independent checkpoint and explain the result.
10. **Record it** — curate the lesson note, reflection, and journey evidence.

Understanding is the gate between learning and project implementation. A GitHub issue cannot force progression when the concept is not yet clear.

## Learning records

- GitHub issues describe intended learning outcomes, completion criteria, and evidence.
- `learning/` contains durable, curated lesson notes and exercises for offline review.
- `JOURNEY.md` records chronological progress, changes in understanding, and links to evidence.
- Lesson notes are not raw chat transcripts.
- Vinay's teach-back and reflection must be incorporated before a lesson is considered complete.

## Capability strands

These strands develop together rather than as isolated courses:

- Software engineering
- Architecture and system design
- Cloud and operations
- Data and AI engineering
- Product and customer discovery
- Communication and consulting
- Security, governance, and responsible delivery

## First learning block

Only Sprint 1 is active. Later sprints are directional and will be replanned using evidence from completed lessons.

### Sprint 1 — Python Foundations

**Question:** How does Python represent data, control execution, organise behaviour, and communicate failure?

**Learn**

- how source code, the Python interpreter, and runtime execution relate;
- values, variables, built-in types, and mutability;
- collections, decisions, and iteration;
- functions, modules, packages, and imports;
- type hints, exceptions, and debugging;
- test purpose, structure, and the pytest mental model.

**Practise**

- short isolated examples;
- prediction and tracing exercises;
- small changes made without generated answers;
- debugging deliberately broken Python;
- comparisons with familiar C# and .NET concepts.

**Apply**

At the end of the sprint, build a small pure-Python workflow metrics program. It will reuse a small part of the future Automation Opportunity Scorer problem without introducing HTTP, FastAPI, persistence, Docker, or deployment.

**Demonstrate**

- run and explain the program;
- trace how input becomes output;
- explain values, types, collections, functions, modules, exceptions, and tests in context;
- extend one behaviour independently;
- complete a teach-back and reflection.

### Sprint 2 — HTTP, APIs, and Application Architecture

Forecast topics:

- client/server communication;
- HTTP requests, responses, methods, URLs, headers, bodies, and status codes;
- JSON and API contracts;
- validation and mapping;
- transport, application, and domain boundaries;
- comparison with .NET controllers, DTOs, services, and domain classes.

### Sprint 3 — FastAPI and the First API Vertical Slice

Forecast topics:

- FastAPI routing and request lifecycle;
- Pydantic models and validation;
- response models and error handling;
- unit and API-level testing;
- project structure and safe configuration.

Forecast application:

- design and build the first deterministic Automation Opportunity Scorer API slice.

### Later stages

- persistence and service boundaries;
- containerisation, CI/CD, and Azure delivery;
- observability and operational resilience;
- AI-assisted analysis against a deterministic baseline;
- evaluation, discovery evidence, and product validation.

## Standard lesson evidence

For each substantial learning unit:

- completed lesson notes;
- a short knowledge check;
- a focused exercise;
- an independent checkpoint;
- a teach-back in Vinay's own words;
- a reflection and journey entry;
- links from the relevant GitHub issue.

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
