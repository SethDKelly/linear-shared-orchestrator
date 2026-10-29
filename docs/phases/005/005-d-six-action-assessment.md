---
type: Phase Design Candidate
title: 005-D — Six-Action Source-First Exposure and Scope/Work Seam Assessment
description: Bounded paper-trace assessment of C3 and R-06 application actions; no synchronization or exposure accepted.
tags: [phase-005, composition, application-actions, six-action-tranche, review-candidate]
---

# 005-D — Six-action source-first assessment

**Status: DESIGN CANDIDATE FOR INDEPENDENT REVIEW; no action exposure or synchronization edge accepted.** This follows the [independently qualified, TPO-admitted entry](005-d-entry-assessment.md), [S-145](https://linear.app/s-kelly/issue/S-145), the [Phase 005 composition contract](composition-synchronization-contract.md), [C3](../../canonical/concepts/c3-scoped-authorization.md), [R-06](../../canonical/concepts/r06-work-outcome-accountability.md), and [Phase 000 intake](../../canonical/project/intake.md). Source-owned intrinsic guards are unchanged. The classifications below are *proposals*, not project-local authorization.

## Deliberate six-action application surface

| Source action | Provisional treatment | Source purpose and guard | Negative / falsifying trace |
| --- | --- | --- | --- |
| C3 `ConsiderScope` | **Direct candidate** | P02/P04: consider a bounded decision scope and external obligation claims without granting permission. | Presenting a favorable review or unmet obligation must not create `Authorize`. |
| C3 `Withhold` | **Direct candidate** | Accountable actor explicitly withholds permission for a scope; actor eligibility is project-local. | No response or reviewer unavailability is not an attributed withholding or grant. |
| C3 `Authorize` | **Unresolved exposure** pending qualified project-local authority predicate; not automatically available | Explicit actor-attributed permission exactly for scope; review and R-06 work facts cannot authorize. | A request for work, technical PASS or favorable assessment must not create permission; a different scope cannot inherit it. |
| C3 `InspectPermission` | **Direct inspection candidate**, subject to evidence visibility/access policy | Shows explicit current permission, actor/scope and external obligation assertions without laundering them into permission. | A missing grant must not display as approved; history must not appear as current permission. |
| R-06 `RequestWork` | **Direct candidate** | P06: create bounded unit/revision request with attributable requesting actor; no attempt or completion implied. | A request without permission to execute must remain a request; no attempt or authorization is inferred. |
| R-06 `InspectOutcome` | **Direct inspection candidate**, subject to evidence visibility/access policy | Unit must exist; distinguish requested, acknowledged, attempted, assessed, asserted, current/historical substantiation, contested, unknown and revision. | A favorable assessment or `NOT SUBSTANTIATED` objection cannot be displayed as verified completion; safety-review suspension remains visible. |

A **direct candidate** is conceptual exposure only, not a UI/API/role implementation or accepted action. No `system-triggered` or `composition-only` classification is supported by the current source for this tranche. C2 `InspectInquiry` is **excluded** pending CF-1 attributable source-owner confirmation.

## C3 scope ↔ R-06 work-unit synchronization test

**Candidate application promise:** A person can distinguish whether a bounded work request exists from whether an accountable actor explicitly permitted execution of the work within a particular scope. This is a *visibility and distinction* promise; the intake does not presently require that creating a request grants permission or triggers a permission decision.

**Proposed participants:** C3 `InspectPermission(scope)` and R-06 `RequestWork(unit, revision, actor)` / `InspectOutcome(unit)` are independently meaningful. A mandatory synchronized action would require an application-owned, source-supported mapping `unit@revision -> decisionScope`, applicable actor authority and a demonstrated need for coordinated occurrence. Neither concept currently produces that mapping or guarantees that the two actions share a decision scope. **No such synchronization is accepted.**

**Valid independent paper trace:** An actor requests unit U at revision r1 using `RequestWork`. R-06 inspection reports requested only. C3 inspection of separately identified scope S reports no current authorization. The application does not claim execution is permitted or completion substantiated. If an eligible accountable actor later explicitly authorizes S, that permission applies only to S and does not retroactively prove an attempt, assessment or completed work. This trace fulfills the distinction without a mandatory cross-concept trigger.

**Invalid over-coupled trace:** `RequestWork(U,r1)` automatically invokes `Authorize(S)`, or `Authorize(S)` automatically creates an R-06 request. This fabricates actor authority, scope correspondence and a user purpose; **REJECT** both mandatory pairings.

**Under-coupling falsifier / reopening trigger:** An authoritative application promise explicitly requires an action to request work *and* record an attributable permission decision for the *same* bounded scope, and an owner-qualified semantic binding from U/r1 to S plus applicable actor predicate exists. In that case, independent-only behavior might fail the promise; reopen a narrow synchronization candidate and test participant preconditions, history and invalid states. Do not infer this promise from current workflow convention or from an S-140 proposal.

**Revision/history:** `ReidentifyWork` does not automatically withdraw unrelated C3 permission; C3 `Withdraw` does not erase R-06 request/outcome history. Any shared revision/scope applicability must be justified separately. No blanket cascade, implicit completion, automatic challenge pairing, or inferred C2 ground.

## Disposition and remaining gates

- **Qualified for further independent review:** six provisional exposure classifications and a documented **no-mandatory-sync** conclusion for this specific scope/request pair, with explicit counterexample and reopening condition. These are not final 005-D exit decisions.
- **HOLD for authority/source evidence:** direct C3 `Authorize` exposure, access constraints for inspection, exact project-local scope/work identity policy and any positive multi-action synchronization. Route to attributable qualified purpose/authority owner; do not infer human identity from a shared contributor account.
- **Preserve:** RD-15, frozen Q4/Q5, CF-1 C2 exclusion, R-06 contest/safety/history, separate S-40 HOLD, and non-authoritative S-140. Phase 006 inclusion, Phase 007 mapping, Phase 008 reuse, implementation and release are not admitted.
- **Phase 005 exit sufficiency:** the separate purpose-to-capability sufficiency check must trace the entire Phase 000/001 purpose baseline. This six-action assessment does **not** establish completeness for work admission/prioritization, reviewer recovery, cross-repository coordination, evidence reconciliation or release coordination.
- **Assurance:** obtain independent exact-head semantic verdict and separate code/document review receipt before treating these proposed exposure decisions as accepted. CI UNKNOWN unless independently verified; historical public disclosure audit INCOMPLETE. No automatic merge or phase progression.
