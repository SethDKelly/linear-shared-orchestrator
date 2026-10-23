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

- [004-D RD-14 generic-case comparison and boundary alternatives](004-d-rd14-generic-case-boundary-alternatives.md) — **review candidate only**, with historical C1 civic-actions control kept separate from a hypothetical generic-case algebra. Initial Cursor HOLD was lifted by independent **PASS WITH CARRY-FORWARD at `231af23`**; Codex code review found no major issues at that head but is not a semantic verdict. The stronger B1 candidate at `4fed559` received independent **Cursor HOLD** (two exact-head verdicts) and Codex code-review findings: its typed guard table is a disguised union and omits canonical behavior-changing guards. Corrective candidate `5942eb1` records B1's tagged-union failure and restores explicit source guards; independent **Cursor PASS WITH CARRY-FORWARD at exact head `2381196`** lifted the previous `4fed559` HOLD for this bounded comparison, **without resolving RD-14 or admitting 004-E**. Codex's code review at `2381196` identified a remaining **P1 inspect-subject existence-guard omission**, not a semantic approval. Subsequent documentation correction `7ab6237` restores C2/R-06 inspect-existence preconditions and addresses the Cursor carry-forwards; independent **Cursor PASS at exact head `025ab4a`** verifies that limited correction, without RD-14 closure. **Codex code review at `025ab4a` nevertheless identified two additional P1 omissions**: `RebaseInquiry` must reference an existing inquiry, and `InvalidateBasis` must reference an existing recorded basis. Documentation correction `7a188d8` explicitly restores both existence guards. **At exact head `833e4bf8b908e7a2c22ebb6c63e07a3878b5d73d`, independent Cursor semantic review returned PASS, and Codex code review reported no major issues (not an independent semantic design verdict).** Both `RebaseInquiry` and `InvalidateBasis` existence guards were verified on that head. This is clearance of the bounded B1 comparison correction, **not** an RD-14 resolution, 004-D exit decision, final concept factoring, or admission of 004-E. The subsequent index-only reconciliation at **exact head `7c2964b4b51a61f7ade249c182b6ede7f39828e8` received independent Cursor semantic PASS**; Codex code review at that head reported no major issues but is not a semantic verdict. A later bounded **004-D evidence-sufficiency and gate-preparation ledger** at `1398af4b` records unresolved C1 control equivalence, RD-15 concrete credibility/eligibility, P05 challenge ownership, and the need for separately admitted wider 004-D work; **independent Cursor PASS WITH CARRY-FORWARD at exact head `ec16b9fe8966275abee01b9175990a04feeab1e1`** verified its five obligation rows; Codex code review at that head reported no major issues (not a semantic verdict). Cursor identified one review-provenance error: guard corrections were cleared at `833e4bf`, whereas `7c2964b` cleared the index-only reconciliation. The 004-D record corrects this attribution and adds the bounded **historical C1 four-action source-linked paper counterexample trace** (inspection, contestation, authorization, completion reporting). **These new changes await independent exact-head review**; the paper trace is not empirical validation, RD-14 closure, 004-D exit or 004-E admission. B1's failure does not close RD-14, establish permanent C2/R-06 independence, reopen Phase 002-C, select a final boundary, admit 004-E, or exit Phase 004.

## Refinement status

**Refined.**

Project-specific substantive subphases remain dynamically derived by `004-A`; Base does not prescribe a fixed scorecard, concept count, or B–X sequence.

## Navigation

- [Previous phase](../003/)
- [Next phase](../005/)
- [All phases](../)
- [Canonical knowledge](../../canonical/)
