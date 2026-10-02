# Nexora Documentation

This directory is the source of truth for Nexora V1 product decisions, requirements, research/trading behavior, safety rules, and the implementation plan. Keep it current as decisions are made.

## Current phase

**Documentation + Brainstorming.** Do not begin application implementation until the user explicitly says implementation is ready.

## Reading order

1. [Project instructions](PROJECT_INSTRUCTIONS.md) — charter, scope, and working principles.
2. [Product vision and V1 scope](01-product-vision-and-scope.md)
3. [V1 user workflow](02-user-workflow.md)
4. [V1 features and requirements](03-features-and-requirements.md)
5. [Research and trading logic](04-research-and-trading-logic.md)
6. [Risk and safety rules](05-risk-and-safety.md)
7. [V1 architecture and build plan](06-architecture-and-build-plan.md)

Work through one numbered document at a time. The active document is **01 — Product Vision and V1 Scope**. The other numbered documents are starting outlines and should be completed in order.

## Decision status

Use these labels consistently in every document:

- **CONFIRMED** — explicitly approved by the user.
- **PROPOSED** — a candidate decision awaiting approval.
- **OPEN** — a question or decision not yet resolved.
- **LATER / V2** — intentionally outside the current V1 scope.

Never present a proposal or assumption as confirmed. Record meaningful decisions in the relevant document and update cross-references when needed.

## Documentation conventions

- Use Markdown, descriptive headings, and relative links within this directory.
- Keep content concise, specific, and testable. Avoid duplicating long explanations; link to the canonical section instead.
- Distinguish product intent from implementation choices.
- For requirements, assign stable IDs (for example, `FR-001`, `NFR-001`, `RISK-001`) and include acceptance criteria when useful.
- Record unresolved choices under **OPEN**; do not silently decide them.
- Add a short change history to each numbered document when substantive decisions are made.
- Keep implementation code out of scope until the user explicitly authorizes the implementation phase.

## Document template

Use this structure for numbered documents, adapting sections where they do not apply:

1. Purpose
2. Status and scope
3. Confirmed decisions
4. Proposed decisions
5. Open questions
6. Main content
7. Later / V2 ideas
8. Related documents
9. Change history

