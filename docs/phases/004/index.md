# Phase 004 — Concept Modularity, Boundary, Specificity, Completeness & Independence

Phase 004 audits and corrects the factoring of behavior into concepts so each retained concept serves one coherent purpose, minimally fulfills it, stands independently, and uses genericity where needed before composition begins.

## Phase contract

- [Phase definition](phase-definition.md) — methodological intention, boundaries, neighboring-phase distinctions, entry/exit criteria, and implementation state.
- [004-A — Modularity Audit Scope, Boundary Risk, Genericity Pressure & Subphase Planning](004-a-start-gate.md) — mandatory start gate that derives project-specific modularity and boundary-refinement work.
- [Concept Modularity & Boundary Refinement Contract](modularity-boundary-contract.md) — specificity, completeness, independence, genericity, boundary corrections, re-specification, counterexample, and documentation rules.
- [Exit Review & Phase 005 Handoff Template](exit-review-template.md) — reusable closure test used by the dynamically selected final Phase 004 subphase.

## Project Phase 004 start gate

- [004-A project start-gate preparation](004-a-project-start-gate.md) — sponsor-accepted Phase 003 baseline, modularity risk inventory, proposed B–F workstreams, and independent review entry criteria. **Independent PASS WITH CARRY-FORWARD at `5f5b355`; 004-B inventory only admitted.**

- [004-B purpose, element inventory and seam classification](004-b-element-inventory-and-seams.md) — bounded 004-A-authorized inventory; **independent 004-B PASS WITH CARRY-FORWARD at `50c6938`; bounded 004-C admitted.**

- [004-C specificity, minimal completeness and RD-15 survival](004-c-specificity-rd15-survival.md) — independent **004-C PASS WITH CARRY-FORWARD at `fba7b20`**; RD-15 abstract survival ruling permits 004-D *RD-14 comparison and alternatives only*. RD-14 remains open.

- [004-D RD-14 generic-case comparison and boundary alternatives](004-d-rd14-generic-case-boundary-alternatives.md) — **review candidate only**, with historical C1 civic-actions control kept separate from a hypothetical generic-case algebra. Initial Cursor HOLD was lifted by independent **PASS WITH CARRY-FORWARD at `231af23`**; Codex code review found no major issues at that head but is not a semantic verdict. The stronger B1 candidate at `4fed559` received independent **Cursor HOLD** (two exact-head verdicts) and Codex code-review findings: its typed guard table is a disguised union and omits canonical behavior-changing guards. Corrective candidate `5942eb1` records B1's tagged-union failure and restores explicit source guards; **fresh exact-head review is required**. B1's failure does not close RD-14, establish permanent C2/R-06 independence, reopen Phase 002-C, select a final boundary, admit 004-E, or exit Phase 004.

## Refinement status

**Refined.**

Project-specific substantive subphases remain dynamically derived by `004-A`; Base does not prescribe a fixed scorecard, concept count, or B–X sequence.

## Navigation

- [Previous phase](../003/)
- [Next phase](../005/)
- [All phases](../)
- [Canonical knowledge](../../canonical/)
