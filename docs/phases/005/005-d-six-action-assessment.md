---
type: Phase Design Candidate
title: 005-D — Six-Action Source-First Exposure and Scope/Work Seam Assessment
description: Bounded paper-trace assessment of C3 and R-06; two direct conceptual actions accepted in 005-D1, no synchronization accepted.
tags: [phase-005, composition, application-actions, six-action-tranche, partial-accepted-work]
---

# 005-D — Six-action source-first assessment

**Status: PARTIALLY ACCEPTED — 005-D1 direct conceptual exposure of C3 `ConsiderScope` and R-06 `RequestWork` only.** Independent Cursor exact-head semantic PASS and separate Codex no-major-findings review on [PR #26](https://github.com/SethDKelly/linear-shared-orchestrator/pull/26) at `fcfd6ecf421609d8ec72adecf5bcfaafb3f90316`; protected `develop` squash merge `18de9b0ae3b458ad52c5bbe41dfe5175cae28225`; **separate TPO acceptance** recorded in [S-145](https://linear.app/s-kelly/issue/S-145) on 2026-10-29. The other four actions and all proposed synchronizations remain unaccepted. CI UNKNOWN, historical public disclosure audit INCOMPLETE; no Phase 005-D exit, implementation, or Phase 006 admission. This follows the [independently qualified, TPO-admitted entry](005-d-entry-assessment.md), [S-145](https://linear.app/s-kelly/issue/S-145), the [Phase 005 composition contract](composition-synchronization-contract.md), [C3](../../canonical/concepts/c3-scoped-authorization.md), [R-06](../../canonical/concepts/r06-work-outcome-accountability.md), and [Phase 000 intake](../../canonical/project/intake.md). Source-owned intrinsic guards are unchanged. The six-action table below preserves the **initial candidate snapshot**. The later 005-D1 decision controls accepted status: only `ConsiderScope` and `RequestWork` are direct conceptual actions; the other four remain conditional/HOLD. None grants project-local authority.

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

## 005-D1 — Source-qualified exposure decision (independently reviewed; TPO accepted)

**Accepted narrow decision:** Following the exact-head review, protected merge and separate TPO acceptance linked above, qualify only **C3 `ConsiderScope`** and **R-06 `RequestWork`** as conceptually direct application actions. Their source-owned meanings are independently complete: [C3](../../canonical/concepts/c3-scoped-authorization.md) presents a decision scope and external obligation claims without creating permission; [R-06](../../canonical/concepts/r06-work-outcome-accountability.md) records an actor-attributed bounded unit/revision request without attempt, completion or permission. This is accepted conceptual application-action *availability*, **not** a grant to an arbitrary actor, a UI/API decision, a system trigger, or a project-local policy waiver. Any concrete invocation must still satisfy source guards and applicable local access/security authority.

**Negative controls:** A review PASS, obligation claim or `ConsiderScope` never triggers `Authorize`. `RequestWork(U,r1,actor)` does not imply `AcknowledgeRequest`, `RecordAttempt`, `SubstantiateOutcome`, or permission to execute; missing actor attribution or bounded unit/revision fails the source contract. Neither direct action requires the other, and no synchronization edge is proposed.

**Explicit non-decisions for the other four actions:**

| Action | Disposition until attributable source/authority evidence | Exact reopening evidence |
| --- | --- | --- |
| C3 `Withhold` | **Conditional direct candidate**, not accepted: a consequential actor-attributed withholding must honor local eligibility. | Qualified project-local permission-decision actor predicate and attributable source-owner confirmation of direct exposure. |
| C3 `Authorize` | **HOLD**, not accepted: explicit grant changes bounded permission and cannot follow from review or work state. | Qualified local authority predicate for actor/scope/basis and independently reviewed exposure decision. |
| C3 `InspectPermission` | **Conditional direct inspection candidate**, not accepted: concept-valid inspection does not establish who may view obligation or actor evidence. | Qualified project-local evidence visibility/access rule and source-owner confirmation that exposure preserves current vs historical permission. |
| R-06 `InspectOutcome` | **Conditional direct inspection candidate**, not accepted: unit-exists guard and contest/safety/history remain mandatory. | Qualified project-local evidence visibility/access rule and R-06 source-owner confirmation of full canonical inspection semantics. |

**Accountability:** TPO routes these source-owner/authority questions using [Phase 004 F1/F2](../004/004-f2-obligation-navigation-crosswalk.md) and [S-145](https://linear.app/s-kelly/issue/S-145). GitHub authorship is contributor provenance, not proof of an accountable human owner. A missing Linear assignee is metadata debt, not a veto on the two non-permission-creating candidate actions. No new project-local authority or privacy rule is inferred.

**Acceptance gate disposition:** The required independent exact-head semantic review, separate Codex receipt, protected merge and separate TPO accepted-work decision have been recorded for **these two actions only**. This does not accept any other action, authorize execution, close 005-D/005, or admit Phase 006. Preserve CF-1 C2 exclusion, RD-15, frozen Q4/Q5, safety contest/history, separate S-40 HOLD and non-authoritative S-140.

## C3 scope ↔ R-06 work-unit synchronization test

**Candidate application promise:** A person can distinguish whether a bounded work request exists from whether an accountable actor explicitly permitted execution of the work within a particular scope. This is a *visibility and distinction* promise; the intake does not presently require that creating a request grants permission or triggers a permission decision.

**Proposed participants:** C3 `InspectPermission(scope)` and R-06 `RequestWork(unit, revision, actor)` / `InspectOutcome(unit)` are independently meaningful. A mandatory synchronized action would require an application-owned, source-supported mapping `unit@revision -> decisionScope`, applicable actor authority and a demonstrated need for coordinated occurrence. Neither concept currently produces that mapping or guarantees that the two actions share a decision scope. **No such synchronization is accepted.**

**Valid independent paper trace:** An actor requests unit U at revision r1 using `RequestWork`. R-06 inspection reports requested only. C3 inspection of separately identified scope S reports no current authorization. The application does not claim execution is permitted or completion substantiated. If an eligible accountable actor later explicitly authorizes S, that permission applies only to S and does not retroactively prove an attempt, assessment or completed work. This trace fulfills the distinction without a mandatory cross-concept trigger.

**Invalid over-coupled trace:** `RequestWork(U,r1)` automatically invokes `Authorize(S)`, or `Authorize(S)` automatically creates an R-06 request. This fabricates actor authority, scope correspondence and a user purpose; **REJECT** both mandatory pairings.

**Under-coupling falsifier / reopening trigger:** An authoritative application promise explicitly requires an action to request work *and* record an attributable permission decision for the *same* bounded scope, and an owner-qualified semantic binding from U/r1 to S plus applicable actor predicate exists. In that case, independent-only behavior might fail the promise; reopen a narrow synchronization candidate and test participant preconditions, history and invalid states. Do not infer this promise from current workflow convention or from an S-140 proposal.

**Revision/history:** `ReidentifyWork` does not automatically withdraw unrelated C3 permission; C3 `Withdraw` does not erase R-06 request/outcome history. Any shared revision/scope applicability must be justified separately. No blanket cascade, implicit completion, automatic challenge pairing, or inferred C2 ground.

## Disposition and remaining gates

- **Accepted only in 005-D1:** C3 `ConsiderScope` and R-06 `RequestWork` are directly available conceptual application actions with existing intrinsic guards; no mandatory synchronization edge accepted. The other four exposure classifications and the scope/work seam trace remain candidate/conditional and are not final 005-D exit decisions.
- **HOLD for authority/source evidence:** direct C3 `Authorize` exposure, access constraints for inspection, exact project-local scope/work identity policy and any positive multi-action synchronization. Route to attributable qualified purpose/authority owner; do not infer human identity from a shared contributor account.
- **Preserve:** RD-15, frozen Q4/Q5, CF-1 C2 exclusion, R-06 contest/safety/history, separate S-40 HOLD, and non-authoritative S-140. Phase 006 inclusion, Phase 007 mapping, Phase 008 reuse, implementation and release are not admitted.
- **Phase 005 exit sufficiency:** the separate purpose-to-capability sufficiency check must trace the entire Phase 000/001 purpose baseline. This six-action assessment does **not** establish completeness for work admission/prioritization, reviewer recovery, cross-repository coordination, evidence reconciliation or release coordination.
- **Assurance:** PR #26 has independent exact-head Cursor semantic PASS and separate Codex no-major-findings receipt for the two-action decision; TPO acceptance is separately recorded. New exposure or synchronization decisions require their own qualified evidence and independent review. CI UNKNOWN unless independently verified; historical public disclosure audit INCOMPLETE. No automatic phase progression.
