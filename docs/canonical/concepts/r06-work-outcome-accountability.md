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
| ChallengeOutcome(unit, assertion, reason) | Record the attributable challenge, its proposed materially different proposition or outcome, and why the difference matters, preserving its basis and history. If no material difference is substantiated, classify the challenge **NOT SUBSTANTIATED** without marking the outcome actively contested or validating the underlying assertion. A credibly safety-significant objection is not dismissed solely for imperfect framing. If materially differentiated and substantiated as a contest, mark the assertion **contested** and preserve that status for inspection. |
| SubstantiateOutcome(unit, assertion, applicableBasis) | Require attributable assertion, same-current-revision applicable supporting basis and no unresolved material disqualifying challenge; a NOT SUBSTANTIATED challenge is not evidence for the assertion and never itself establishes completion; never authorize |
| InvalidateBasis(unit, basis, reason) | Remove current substantiation dependent on basis; retain historical claim |
| ReidentifyWork(unit, newRevision) | Preserve history; prior bases/claims do not automatically apply to new revision |
| InspectOutcome(unit) | Expose distinct requested/acknowledged/attempted/assessed/claimed/substantiated/disputed/invalidated facts; missing is unknown |

## Invariants, lifecycle and deliberate open questions
None of request, acknowledgment, attempt, favorable assessment, authorization or outcome assertion implies substantiated completion. Only a supported, revision-applicable completed-outcome assertion without an unresolved material disqualifying challenge can be described as **currently substantiated**, and materially contradictory supported outcomes remain contested. The challenger bears the burden of identifying and supporting a decision-relevant difference; differences of phrasing alone do not constitute a material contest. An adjudicator may question propositions and validity, investigate evidence on credible suspicion, and reject unsupported propositions, without manufacturing a contest or routinely rebuilding the parties' evidence. A recorded NOT SUBSTANTIATED challenge is neither an active contest nor proof of the challenged claim. A materially contested outcome remains observably contested and cannot silently become success, verification, acceptance or resolution. `verified=true` without independently meaningful basis is not proof. A new revision drops inherited applicability even if called immaterial. Challenges (including NOT SUBSTANTIATED objections), invalidation and supersession preserve attributable historical facts and may be revisited on genuinely new material evidence. R-06 does not intrinsically require an adjudication action or resolution of every challenge; an unresolved challenge remains inspectable. Any external adjudication, settlement or cross-concept synchronization requires separately qualified ownership in later design phases. No silence, timeout, favorable assessment or unreasoned closure silently clears a material disqualifying challenge. Initially no work is requested; no automatic closure, timeout, retry or workflow is implied.

Ground credibility, eligibility of actors to assert/substantiate, evidence access/retention, privacy and empirical user need remain open. Phase 004 must run **RD-14** (generic-case collapse) and **RD-15** (unverifiable-basis input) and may return to Phase 002-C if independence fails. C2 may provide challengeable grounds as an abstract input, but cannot substitute for work-attempt facts. C3 permission cannot substitute for completion or waive project-local security, including S-40 HOLD. C6 prose remains unpromoted. No merge/release authority, API, UI, schema, orchestration, provider or deployment is established.
