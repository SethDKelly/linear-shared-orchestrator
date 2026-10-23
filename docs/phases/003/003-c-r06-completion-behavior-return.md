---
type: Phase 003 Project Record
title: 003-C Corrective Return — R-06 Completion Behavior
description: Abstract, representation-independent work outcome accountability semantics.
tags: [phase-003, correction, completion, abstract-behavior]
sources:
  - id: identity
    resource: 003-b-completion-identity-return.md
    title: Independently passed R-06 identity return
  - id: contract
    resource: concept-specification-contract.md
    title: Phase 003 specification contract
  - id: purpose
    resource: ../../canonical/purpose/purpose-model.md
    title: Canonical P06 purpose
---
# 003-C corrective return — R-06 abstract completion behavior

**Status: BOUNDED SPECIFICATION independently PASS at `75e3f41` ([review](https://github.com/SethDKelly/linear-shared-orchestrator/pull/2#issuecomment-6356088541)); corrective 003-E subsequently PASS at `e313539`. Phase 003-F exit NOT READY pending canonical ownership and navigation remediation.** This record owns only R-06 behavior. It does not revise C2/C3, revive C6, or choose an execution workflow.

## Identity, purpose and domains
**R-06 — Work outcome accountability:** A contributor or downstream receiver can distinguish what has been requested, acknowledged, attempted, evaluated, claimed as an outcome, and substantiated as completed for a bounded unit of work (P06). P01/P03 protect freshness and unknown results; P02/P04 protect sponsor and project-local authority.

Abstract parameters: WorkUnit, Revision, Actor, Attempt, Acknowledgment, Assessment, OutcomeClaim, Basis. No native types from C2/C3, review receipts, providers, controllers, issues or project authorization engines. WorkUnit identity is an abstract scope; Revision is the version of that scope to which evidence must apply.

## Minimum necessary state
For each WorkUnit and current Revision, retain the request fact and its attribution, a set of separately attributable acknowledgments, a set of attempts with their reported results or unknown outcomes, separately attributable assessment claims with their subject revisions, accountable outcome assertions with their cited bases, and any explicit challenge, withdrawal or invalidation of an assertion/basis. Historical relation to superseded revisions is retained only to avoid treating old facts as currently applicable. No ordered workflow, scheduling, queue, receipt, provider rotation, UI, persistence model or exhaustive audit store is implied. Acknowledgment and attempt are **distinct facts**: either may exist without the other, and neither is an outcome.

## Conceptual actions and semantics
| Action | Guard | Effect / observable meaning |
|---|---|---|
| RequestWork(unit, revision, actor) | Bounded subject and revision supplied | Establishes requested work, not acknowledgment or progress |
| AcknowledgeRequest(unit, revision, actor) | Request exists for revision | Adds acknowledgment only; never attempt or completion |
| RecordAttempt(unit, revision, actor, reportedResult) | Request exists; actor attribution available | Adds attempt and reported result (including unknown/failed); does not imply acknowledgment, assessment or completion |
| RecordAssessment(unit, revision, actor, assessmentClaim) | Subject revision identified | Adds attributed evaluation claim; favorable evaluation does not establish actual execution or completion |
| AssertOutcome(unit, revision, actor, outcome, bases) | Subject identified and claim attributable | Adds an explicit claimed result, which may be completed, incomplete, failed or unknown; the claim is not automatically substantiated |
| ChallengeOutcome(unit, assertion, reason) | Referenced assertion exists | Marks the assertion disputed and preserves the objection |
| SubstantiateOutcome(unit, assertion, applicableBasis) | Accountable assertion exists; basis specifically applies to the same current revision and supports that outcome; no unresolved disqualifying challenge | Marks the claim as currently substantiated, subject to subsequent invalidation; does not grant authorization |
| InvalidateBasis(unit, basis, reason) | Referenced basis exists | Revokes present substantiation that depends on it without erasing the historical claim |
| ReidentifyWork(unit, newRevision) | New revision differs from previous | Preserves history, but prior assessments/bases/claims are not current substantiation without new applicability |
| InspectOutcome(unit) | Unit exists | Returns independently distinguishable requested, acknowledged, attempted, assessed, claimed, substantiated, disputed and invalidated facts; missing evidence is unknown, not success |

An actor's eligibility to make a completion assertion or substantiate a basis is an **abstract authority predicate** to validate later; it cannot be assumed from provider responses, issue state or a shared coordinator. The difference between a report of a result and proof that it actually occurred is explicit. Substantiation is a claim with an applicable basis, not metaphysical certainty.

## Invariants and temporal behavior
1. Requested ≠ acknowledged ≠ attempted ≠ assessed ≠ outcome-asserted ≠ substantiated; none of the first five implies the last.
2. Completion is displayed as **currently substantiated** only if an attributable completed-outcome assertion exists, at least one applicable supporting basis is present, and no unresolved disqualifying challenge or invalidation defeats that basis. A reported attempt, favorable review or sponsor permission alone cannot satisfy this condition.
3. A basis and its substantiation are **revision-qualified**; new exact subject revision invalidates inherited applicability even if a person calls the change immaterial.
4. Failure, partial outcome and unknown remain distinct from substantiated completion. Nonresponse, timeout or quota do not create a result.
5. Correction, supersession, challenge and invalidation do not erase historical assertions, attempts or assessments; current read behavior distinguishes current validity from prior history.
6. Project-local security/acceptance authority remains separate. Substantiated completion is not permission to merge, release or waive an S-40 HOLD.
7. Contradictory supported outcome assertions or unresolved competing challenges leave current outcome **contested**, not silently choose a winner.

Initially there is no requested work. There is no automatic timeout, closure or escalation. Multiple attempts may occur; their order is retained only if required to distinguish correction/supersession. Whether a completed outcome can be later reversed is modeled through invalidation, not by silently deleting history. Criteria for independently verifying a basis, evidence access/retention and actor eligibility are **open validation questions** rather than assumed algorithms.

## Minimality and independent-identity falsification
Remove C2 and C3 native state. R-06 still has a coherent behavioral promise: an acknowledgment is not an attempt, an attempt is not a result, a favorable evaluation is not execution, and an attributable supported result can become contested or stale. C2 might evaluate a question about those facts, but it does not intrinsically own the facts of attempted work. C3 may authorize a bounded action, but authorization is not evidence that it occurred.

**Falsification:** If independent reviewers conclude the above can be fully represented by a generic case with arbitrary status labels and no distinct outcome-accountability invariant, R-06 must return to Phase 002-C rather than be canonized. The abstract `Basis` input must not become a hidden C2 or provider dependency. A genuine completion claim still requires a meaningful basis; an invented “verified=true” input is insufficient without independent challenge.

## 003-D challenge handoff
Independently test acknowledgment without attempt, attempt without acknowledgment, positive assessment without execution, authorized-but-unexecuted, completion claim without basis, basis for a prior revision, contradictory outcomes, reviewer silence, evidence withdrawal, privacy/access, historical S-40 HOLD and cross-project local authority. 003-D does not adopt this record as clearance. 003-E HOLD and 003-F block remain until separate independent review and renewed reconciliation.
