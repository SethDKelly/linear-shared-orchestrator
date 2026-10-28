---
type: Phase Design Candidate
title: 005-B — Current Concept Action and Application Surface Inventory
description: Source-linked, provisional exposure classification for independently retained concepts; no synchronization admitted.
tags: [phase-005, action-surface, source-inventory, review-candidate]
---

# 005-B — Source-linked action and application-surface inventory

**Status: REVIEW CANDIDATE, not an independently accepted 005-B verdict.** Scope is the bounded [005-A project plan](005-a-project-start-gate.md), independently reviewed on the exact PR head and merged into `develop`. [S-143](https://linear.app/s-kelly/issue/S-143) is the admitted 005-B work item; the [phase definition](phase-definition.md) and [composition contract](composition-synchronization-contract.md) govern. This inventory does **not** admit a synchronization edge, a new intrinsic concept action, or Phase 005-C. The canonical concept documents below own action meaning, not this inventory.

## Purpose and source baseline

| Provisional source owner | Purpose | Source authority | Action coverage |
| --- | --- | --- | --- |
| C2 — Living inquiry | P01/P05: maintain a challengeable, revision-qualified inquiry and distinguish disputed/stale grounds from current provisional answers | [C2](../../canonical/concepts/c2-living-inquiry.md) | 7 / 7 |
| C3 — Scoped authorization | P02/P04: explicitly distinguish project-local bounded permission from review or external obligation assertions | [C3](../../canonical/concepts/c3-scoped-authorization.md) | 5 / 5 |
| R-06 — Work outcome accountability | P06: distinguish request, attempt, assessment, assertion, current substantiation, contest and history | [R-06](../../canonical/concepts/r06-work-outcome-accountability.md) | 10 / 10 |

**Exposure notation is provisional, not permission.** `D?` = possible directly exposed application action, subject to purpose/actor/guard validation; `N?` = possible intentional non-exposure until independently qualified policy; `U` = unresolved. Composition-only and system-triggered classifications are **not inferred** before Phase 005-C seam qualification; they remain available outcomes in later analysis. A direct candidate is not a UI control, endpoint, service or authorization. An intrinsic action may be concept-valid but deliberately absent from the application.

## Action inventory (22 current intrinsic actions)

| Source | Intrinsic action | Candidate exposure | Current guard, distinction or falsifier (source-owned) |
| --- | --- | --- | --- |
| C2 | `OpenInquiry` | D? | New unsettled inquiry for a revision; does not create permission. |
| C2 | `OfferGround` | D? | Referenced inquiry exists; offered applicability is an assertion, not verified truth. |
| C2 | `ChallengeGround` | D? | Referenced ground exists; objection is retained, not erased. |
| C2 | `AddressChallenge` | U | Attributed disposition preserves challenge history; actor eligibility not invented here. |
| C2 | `RebaseInquiry` | D? | New revision invalidates presumed applicability of old grounds/answers. |
| C2 | `ProposeAnswer` | D? | Revision-qualified provisional claim, not permission or completed work. |
| C2 | `InspectInquiry` | D? | Exposes question, current revision, grounds, unresolved challenges and current provisional-answer applicability; contested/stale grounds remain visible, not automatically credible. |
| C3 | `ConsiderScope` | D? | External obligation assertions do not create permission. |
| C3 | `Withhold` | D? | Actor-attributed withholding; silence is not a grant. |
| C3 | `Authorize` | U | Explicit project-local authority predicate and exact scope; never inferred from review, C2 or R-06. |
| C3 | `Withdraw` | U | Authorized withdrawal/supersession of applicable prior permission, with history. |
| C3 | `InspectPermission` | D? | Shows current explicit permission and unresolved assertions without converting them to approval. |
| R-06 | `RequestWork` | D? | Bounded unit/revision request; not progress. |
| R-06 | `AcknowledgeRequest` | D? | Existing request required; acknowledgment does not imply attempt. |
| R-06 | `RecordAttempt` | D? | Existing request; reported failure/unknown possible; no automatic acknowledgment. |
| R-06 | `RecordAssessment` | D? | Evaluation is not completion. |
| R-06 | `AssertOutcome` | D? | Accountable claim with bases is not automatically substantiated. |
| R-06 | `ChallengeOutcome` | U | Existing assertion and identified actor/objection; materiality/eligibility remain RD-15. |
| R-06 | `SubstantiateOutcome` | N? | Same-current-revision applicable basis, no material disqualifying contest or active safety-review hold; never infer from assessment. |
| R-06 | `InvalidateBasis` | U | Withdraw current substantiation dependent on invalid basis, preserve history. |
| R-06 | `ReidentifyWork` | D? | New revision preserves history but does not inherit prior evidence applicability. |
| R-06 | `InspectOutcome` | D? | Separate requested/attempted/assessed/asserted/current vs historical substantiation; contested and unknown visible. |

**Source verification contract:** names and distinctions above are read from the three linked current canonical files, not reconstructed from historic PR descriptions. Each row is a candidate *application exposure*, not an accepted application action. For `N?`, a later qualified owner may reject non-exposure; it is not a new intrinsic prohibition. No new concept action, precondition or actor eligibility rule is added.

## Negative and boundary tests before exposure acceptance

1. **Authorization isolation:** C2 `ProposeAnswer`, R-06 `RecordAssessment` and `AssertOutcome`, a favorable independent review, or an external obligation assertion cannot produce C3 `Authorize`; explicit project-local authority and scope are required.
2. **Outcome truth:** Request, acknowledgment, attempt, assessment, assertion and substantiation are distinct. A `NOT SUBSTANTIATED` challenge is recorded but not proof for either side. A supported material contradiction remains `CONTESTED`, even without an explicit challenge.
3. **Credible suspicion:** `CONTESTED — SAFETY REVIEW PENDING` suspends *current* affected substantiation; no later invocation restores it without separate qualified safety/evidence disposition. Independent credible-suspicion investigation remains available.
4. **History and revision:** C2 `RebaseInquiry`, R-06 `ReidentifyWork` and `InvalidateBasis` preserve historical records while removing presumed current applicability. A new revision does not silently inherit prior grounds or completed-outcome bases.
5. **No invented adjudication:** C2 `AddressChallenge` is a source-owned inquiry-ground disposition; R-06 has **no mandatory challenge-resolution action**. A material R-06 challenge can remain visibly unresolved.
6. **Application purpose falsification:** For each `D?`, ask whether P01–P06 actually requires direct invocation by an eligible actor. If not, mark `U` or `N?`; do not create a one-action synchronization merely because the concept action exists.
7. **Intrinsic-defect return:** A demonstrable C2/C3/R-06 intrinsic guard, purpose or independence defect returns to its qualified Phase 003/004 owner; do not repair it by Phase 005 composition. RD-14 source-complete generic-case collapse returns first to Phase 002-C.

## Decision ledger and handoff

- **CF-1 C2 `InspectInquiry` source-alignment candidate:** The corrected row enumerates the complete [canonical C2 inspection surface](../../canonical/concepts/c2-living-inquiry.md) rather than only disputed/stale grounds. This is an inventory correction, **not** an intrinsic C2 action change or an accepted direct application exposure. TPO must obtain attributable provisional C2 source-owner semantic confirmation **before** using this row as a Phase 005-D guard or accepting direct exposure; independent exact-head review remains separate. The `D?` classification remains provisional; no permission or synchronization edge follows. See [005-C1](005-c1-source-first-composition-reassessment.md) for the trigger and negative controls.
- **Unresolved exposure:** C2 `AddressChallenge`; C3 `Authorize`/`Withdraw`; R-06 `ChallengeOutcome`/`InvalidateBasis`. TPO routes source-owner/authority evidence; a missing assignee is metadata debt, not independent proof of unsound semantics.
- **Non-exposure hypothesis:** R-06 `SubstantiateOutcome` is a protected candidate pending independently qualified policy; do not infer that it must be directly invokable or system-triggered.
- **RD-14/RD-15:** Remain open with [F2 owner/trigger routing](../004/004-f2-obligation-navigation-crosswalk.md); [F1 provisional owner dispositions](../004/004-f1-owner-disposition-reconciliation.md) remain in force. S-135 Q4/Q5 frozen absent material intrinsic evidence. No silent owner promotion.
- **Next gate, not admitted:** 005-C may qualify CO-1–CO-4 as concept-local, cross-concept, unsupported or HOLD, with a purpose source and falsifying counterexample. No edge is approved by this inventory. Phase 006 dependence, Phase 007 representation, Phase 008 reuse, implementation and AWS remain excluded; S-40 security HOLD persists.
- **Assurance:** Independent exact-head semantic review must check all 22 action names, source guard accuracy, provisional exposure rationale and negative controls. A Codex no-major-findings receipt is distinct from semantic PASS. Applicable GitHub CI/protection/publication gates and separate merge readiness remain mandatory; absent CI is UNKNOWN, not PASS. Public historical all-ref/commit/PR-discussion/Actions disclosure audit remains **INCOMPLETE**, not certified clean.

**Gate request:** PASS / PASS WITH CARRY-FORWARD (owner + trigger) / precise HOLD for demonstrably missing current action, incorrect intrinsic semantics, unsafe exposure, broken source or lost negative control. No implementation, new synchronization, release, AWS, or unqualified next-subphase admission.
