---
type: Canonical Concept Specification
title: R-06 — Work Outcome Accountability (Provisional)
description: Current revision-qualified request, attempt and outcome-accountability semantics.
tags: [canonical, concept, provisional, r06, phase-004]
sources:
  - id: identity
    resource: ../../phases/003/003-b-completion-identity-return.md
    title: R-06 operational principle
  - id: behavior
    resource: ../../phases/003/003-c-r06-completion-behavior-return.md
    title: R-06 abstract behavior
  - id: challenge
    resource: ../../phases/003/003-d-r06-completion-adversarial-return.md
    title: Independent adversarial tests
  - id: reconciliation
    resource: ../../phases/003/003-e-r06-corrective-reconciliation.md
    title: P06 behavioral reconciliation
---
# R-06 — Work outcome accountability

**Authority:** Provisional canonical owner of current P06 completion semantics. Phase 004 may **revise, split, merge, generalize or reject** this concept, including merging it into a generic case if its independent identity fails. Canonical location does not certify independent validity, completion, authorization or implementation readiness.

## Purpose and operational principle
P06: a contributor or downstream receiver distinguishes requested, acknowledged, attempted, assessed, asserted and substantiated outcomes of bounded work. **OP R06-1:** A requested unit is acknowledged and attempted while evaluation is pending; a later evaluation is not itself completion. Only an accountable completed-outcome assertion with grounds applicable to the current revision can be currently substantiated. Invalidation withdraws current substantiation while preserving history.

## Abstract identity and state
Parameters: WorkUnit, Revision, Actor, Attempt, Acknowledgment, Assessment, OutcomeClaim, Basis. Per bounded unit/revision, retain the request, separately attributable acknowledgments and attempts (either may exist without the other), evaluations, outcome assertions, cited bases, challenges, dispositions, invalidations and revision/supersession history sufficient to distinguish old from current. No native C2 inquiry, C3 authorization, receipt, controller, provider or workflow type.

## Conceptual actions and guards
| Action | Conceptual effect |
|---|---|
| RequestWork(unit, revision, actor) | Establish bounded request, not progress |
| AcknowledgeRequest(unit, revision, actor) | Record acknowledgment only; request must exist |
| RecordAttempt(unit, revision, actor, reportedResult) | Record attributed attempt and reported result (including failure/unknown); request must exist; does not imply acknowledgment |
| RecordAssessment(unit, revision, actor, assessmentClaim) | Record revision-attributed evaluation, not actual completion |
| AssertOutcome(unit, revision, actor, outcome, bases) | Record accountable outcome assertion, not automatically substantiated |
| ChallengeOutcome(unit, assertion, reason) | Mark assertion contested and retain objection |
| SubstantiateOutcome(unit, assertion, applicableBasis) | Require attributable assertion, same-current-revision applicable supporting basis and no unresolved disqualifying challenge; never authorize |
| InvalidateBasis(unit, basis, reason) | Remove current substantiation dependent on basis; retain historical claim |
| ReidentifyWork(unit, newRevision) | Preserve history; prior bases/claims do not automatically apply to new revision |
| InspectOutcome(unit) | Expose distinct requested/acknowledged/attempted/assessed/claimed/substantiated/disputed/invalidated facts; missing is unknown |

## Invariants, lifecycle and deliberate open questions
None of request, acknowledgment, attempt, favorable assessment, authorization or outcome assertion implies substantiated completion. Only a supported, revision-applicable, uncontested completed-outcome assertion can be described as **currently substantiated**, and contradictory supported outcomes remain contested. `verified=true` without independently meaningful basis is not proof. A new revision drops inherited applicability even if called immaterial. Challenges, invalidation and supersession preserve historical facts. Initially no work is requested; no automatic closure, timeout, retry or workflow is implied.

Ground credibility, eligibility of actors to assert/substantiate, evidence access/retention, privacy and empirical user need remain open. Phase 004 must run **RD-14** (generic-case collapse) and **RD-15** (unverifiable-basis input) and may return to Phase 002-C if independence fails. C2 may provide challengeable grounds as an abstract input, but cannot substitute for work-attempt facts. C3 permission cannot substitute for completion or waive project-local security, including S-40 HOLD. C6 prose remains unpromoted. No merge/release authority, API, UI, schema, orchestration, provider or deployment is established.
