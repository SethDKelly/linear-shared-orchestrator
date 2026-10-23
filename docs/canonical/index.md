# Canonical Design Knowledge

This directory contains the **current authoritative design state** for a project created from Base. Phase records explain how conclusions were reached; canonical documents state what the design currently means.

## Current project knowledge

- [Canonical project intake](project/intake.md) — provisional project framing, evidence classifications and unresolved questions. Phase 000 exit was accepted by sponsor on 2026-10-22.

- [Current provisional purpose model](purpose/purpose-model.md) — Phase 001 needs and success framing; Phase 001 exit is sponsor-accepted with explicit carry-forwards; Phase 002 exit was sponsor-accepted; Phase 003-A independently passed. Phase 003 exit was sponsor-accepted with carry-forwards on 2026-10-22; provisional canonical concept specification owners are listed below and remain fully revisable in Phase 004.

## Typical knowledge families

A cloned project should create only the families its design actually needs. Common families may include:

- `project/` — current intake definition, context, actors, boundaries, constraints, assumptions, and unresolved project questions;
- `purpose/` — human purposes, needs, burdens, desired improvements, success framing, and purpose tensions;
- `concepts/` — concept definitions, operational principles, state, actions, invariants, and independence boundaries;
- `synchronizations/` — explicit cross-concept interactions;
- `dependencies/` — concept inclusion dependencies and product-family relationships;
- `authority/` — actors, protected decisions, authority seams, and non-substitutable responsibilities;
- `experience/` — mappings from concepts into user-visible behavior and experience contracts;
- `principles/` — project-specific design principles, accepted constraints, and durable policy;
- `decisions/` — durable design decisions not naturally owned elsewhere;
- `open-questions/` — unresolved design questions that remain current.

These are suggested knowledge families, not a mandatory taxonomy.

## Authority and documentation discipline

When a conclusion becomes durable, promote its stable meaning here rather than forcing future readers to reconstruct current truth from phase history. Prefer updating an existing natural owner and linking to it over creating duplicative canonical documents.

See [Canonical and Historical Knowledge Authority](../methodology/knowledge-authority.md) and [Documentation Integrity & OKF Governance](../methodology/documentation-governance.md).

## Navigation

- [Bundle root](../)
- [Phase records](../phases/)
- [Methodology](../methodology/)

## Provisional concept specifications (not final concept acceptance)

- [C2 — Living inquiry](concepts/c2-living-inquiry.md) — revision-qualified, challengeable inquiry (P01/P05).
- [C3 — Scoped authorization](concepts/c3-scoped-authorization.md) — explicit bounded permission with project-local authority (P02/P04).
- [R-06 — Work outcome accountability](concepts/r06-work-outcome-accountability.md) — accountable attempted-work and substantiated-outcome distinctions (P06).

These are current specification owners only. **Phase 004 may revise, split, merge, generalize or reject any or all of them.** C1 remains a comparator, C4 a recovery lens, C5 deferred federation, and C6 not retained as a standalone narrative concept. Phase 003 exit was sponsor-accepted and PR #2 merged as `82b6a9f`. Phase 004-A is under independent review; no Phase 004-B admission, implementation, or AWS authorization is implied.
