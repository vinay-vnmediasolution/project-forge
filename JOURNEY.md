# Project Forge Journey

This is the concise chronological record of progress, changes in understanding, and evidence. Detailed explanations belong in `learning/`; executable work belongs in issues and project files.

## 2026-07-25 — Sprint 0 foundation

### Completed

- Established the Project Forge mission, charter, roadmap, curriculum, backlog, and definitions of done.
- Recorded the learner baseline and available capacity.
- Created and closed the Sprint 0 milestone.

### Evidence

- `PROJECT_CHARTER.md`
- `SPRINT_0.md`
- GitHub Issues #1–#3

## 2026-07-27 — Learning-first reset

### What we learned

The initial Sprint 1 approach moved from a short API explanation directly into product and contract design. That made the application project drive the curriculum and left the learner without a sufficiently clear foundation.

### Decision

- Teach theory and fundamentals before project application.
- Use visual models, plain-language explanations, .NET comparisons, knowledge checks, and isolated exercises.
- Treat understanding as the gate before implementation.
- Store curated lesson notes under `learning/`.
- Use GitHub issues for meaningful learning units and separate build outcomes.
- Keep teach-backs and personal reflections in Vinay's own words.

### Next

Restart Sprint 1 with Lesson 01: How Python Executes Programs.

## 2026-07-27 — Lesson 01 completed

### Learned

- How CPython parses source, compiles it into bytecode, and executes it using the Python virtual machine
- The relationship between names, objects, values, identity, and types
- Assignment as name binding or rebinding
- Conversion as creation of an object of the target type
- The difference between dynamic and strong typing
- Why supported operations depend on the involved types

### Practised

- Predicted execution without running code first
- Traced name bindings and types
- Diagnosed incorrect predictions about string operations and division
- Wrote a small independent program that converted ticket-count text and calculated monthly tickets

### What became clearer

CPython performs both compilation and interpretation. Names do not carry permanent types; they bind to objects, and the objects have types.

### Evidence

- `learning/01-python-foundations/lessons/01-how-python-runs.md`
- GitHub Issue #4
