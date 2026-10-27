---
okf_version: "0.2"
---

# Shared Orchestrator Knowledge Bundle

This directory is the Open Knowledge Format (OKF) v0.2 knowledge bundle for this project, adopting [Base methodology at commit 3078410](https://github.com/SethDKelly/Base/tree/3078410da427351bb9d139b8881c31a960072a7a). It guides this project from project intake through completed Jackson-aligned software concept design, then through a post-closure pre-implementation repository preparation phase before downstream engineering begins.

## Start here

- [Methodology](methodology/) — design authority, lifecycle, documentation/knowledge governance, design-only guardrails, and agentic development governance.
- [Lifecycle phases](phases/) — Phases 000–011 for concept design plus Phase 012 for post-closure pre-implementation preparation.
- [Canonical knowledge](canonical/) — the sponsor-accepted Phase 000 intake and Phase 001 purpose model (PASS WITH CARRY-FORWARD, 2026-10-22); Phase 002 exit was sponsor-accepted on 2026-10-22; Phase 003 exit was sponsor-accepted with carry-forwards; PR #2 merged. Phase 004-A/B/C received bounded independent reviews and PR #3 subsequently merged as `e20258bdcfac794c7b6375d347db3f8080c4fe53`. Sponsor S-135 froze 004-D Q4/Q5; RD-14 remains OPEN/INDETERMINATE and concrete RD-15 OPEN. Bounded 004-E review and exit documents merged in PRs #7–#9, 004-F entry in PR #10 and F1/F2 in PRs #11/#12. [F3 independent exit evidence](phases/004/004-f3-independent-exit-evidence.md) remains a review candidate. C2/C3/R-06 remain provisional, S-40 security HOLD persists, and Phase 004 sponsor exit was separately accepted as **PASS WITH CARRY-FORWARD** on 2026-10-27 ([S-137](https://linear.app/s-kelly/issue/S-137)); **Phase 005 admission has not occurred**.

## Governing contracts

- [Concept Design Methodology Authority](methodology/authority.md) — methodological authority and interpretation rules.
- [Jackson-Aligned Concept Design Lifecycle](methodology/concept-design-lifecycle.md) — reviewed high-level concept-design lifecycle and its boundary with Phase 012.
- [Phase Lifecycle Contract](methodology/phase-lifecycle.md) — mandatory start gate, dynamic subphase derivation, exit review, reopening, and handoff structure.
- [Documentation Integrity & OKF Governance Contract](methodology/documentation-governance.md) — OKF conformance, progressive disclosure, freshness/staleness discipline, cross-linking, anti-duplication, and drift control.
- [Canonical and Historical Knowledge Authority](methodology/knowledge-authority.md) — current truth versus phase evidence.
- [Design-Only Guardrails](methodology/design-only-guardrails.md) — implementation prohibition and readiness/execution states.
- [Agentic Development Governance](methodology/agentic-development-governance.md) — shared Claude/Cursor/Codex behavior for consuming and maintaining the OKF-grounded repository.

## Knowledge model

Durable current design meaning belongs under [canonical knowledge](canonical/). Chronological discovery, alternatives, reviews, validation, audits, and handoffs belong under [phase records](phases/). Phase records are evidence, not automatically current truth.

Documents should link to existing authoritative knowledge rather than restating it. Directory indexes provide progressive disclosure; ordinary concept documents carry OKF frontmatter and form a traversable graph through standard Markdown links.

## Lifecycle invariant

Until successful Phase 011 concept-design closure:

- **Implementation readiness:** not ready
- **Implementation execution:** not started
- **Implementation authorization:** not yet

Successful Phase 011 closure may change readiness to **ready** while execution remains **not started**.

Phase 012 then performs repository/OKF audit, stale-document reconciliation, README polish, agentic-rule preparation, and engineering-handoff hardening. Phase 012 does not itself begin feature implementation or grant implementation execution authorization.
