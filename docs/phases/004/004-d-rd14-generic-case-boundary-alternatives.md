---
type: Phase Design Record
title: 004-D — RD-14 Generic-Case Comparison and Boundary Alternatives (Review Candidate)
description: Bounded C1 civic-actions control and parameterized generic-case comparison against C2 and R-06; no final factoring decision.
tags: [phase-004, rd-14, boundary-alternatives, provisional, review-candidate]
sources:
  - id: accepted-exit
    resource: ../003/003-f-independent-exit-assessment.md
    title: Sponsor-accepted Phase 003 exit and RD-14 return trigger
  - id: alternative-control
    resource: ../002/002-c-alternative-decompositions.md
    title: Phase 002 competing decompositions including C1
  - id: control-disposition
    resource: ../002/002-e-bounded-convergence.md
    title: C1 control-only disposition
  - id: c2
    resource: ../../canonical/concepts/c2-living-inquiry.md
    title: Provisional C2 behavior owner
  - id: r06
    resource: ../../canonical/concepts/r06-work-outcome-accountability.md
    title: Provisional R-06 behavior owner
  - id: rd15
    resource: 004-c-specificity-rd15-survival.md
    title: Reviewed bounded RD-15 abstract survival
  - id: rd14-challenge
    resource: ../003/003-d-r06-completion-adversarial-return.md
    title: 003-D RD-14 generic-case collapse and RD-12 local security HOLD
---

# 004-D — RD-14 generic-case comparison and boundary alternatives

**Status: review candidate, NOT an independent 004-D verdict.** 004-C's independent PASS WITH CARRY-FORWARD at `fba7b20`, followed by the PR #3 documentation reconciliation review at `77a2ffb` (Cursor PASS WITH CARRY-FORWARD; Codex code review completed without major findings), admits **only** RD-14 generic-case comparison and boundary alternatives. This record neither closes RD-14 nor approves any boundary. PR #3 remains unmerged; root and Phase 003 index wording about "boundary alternatives" remains a documentation carry-forward.

## Authority and the comparator

Phase 002-C calls **C1 "Distinct civic actions"**, a control decomposition separating inspection, contestation, authorization and completion reporting; Phase 002-E did **not** retain it as a new independent concept because it resembled incumbent receipt/decision/progress modules. "Generic case" here is a **falsification hypothesis** for C2 and R-06, not an accepted canonical C1 case specification or permission to resurrect an implementation container. A proposed generic case must state its own purpose, state, actions, guards, effects, revision semantics and independently useful operational principle before it can displace an owner. Naming all facts "case events" does not prove behavioral equivalence.

RD-14 / E-301 asks whether C2 and R-06 retain intrinsic, user-observable semantics under **two separately tested alternatives**: the historical C1 civic-actions control and a newly hypothesized generic-case algebra. The 003-D R-06 adversarial return records RD-14 as the arbitrary-label generic-case collapse challenge and RD-12 as the historical aws-backbone S-40 HOLD. **Demonstrated intrinsic collapse returns to Phase 002-C for renewed alternatives and independent review; it does not auto-promote C1.** The separate RD-15 abstract-survival ruling is available context, not an extra prerequisite to recognizing collapse. Concrete R-06 basis credibility and actor eligibility remain open.

## Two noninterchangeable comparators

| Comparator | Independently testable action/purpose boundary | Disqualifier and evidence needed | Disposition |
|---|---|---|---|
| **A — Historical C1: Distinct civic actions (control only)** | Four distinct accountable civic actions, **inspect evidence**, **contest findings**, **authorize actions**, **report completion**, with a separately accountable actor for each even when concerning one change. Map each against C2 inquiry and R-06 outcome, not against a hypothetical case container. | E-001: resembles S-81/PR #1 receipt/decision/progress architecture, not an established independent user-valued concept. A completion *report* can be mistaken for work *completed*. C1 authorization is a historical control action and neither defines nor grants C3 scoped permission. To displace an owner, demonstrate intrinsic equivalent guards/effects and history, not familiar module names. | **Open control comparison; C1 not promoted** |
| **B — Hypothetical generic case (new, not C1)** | Proposed single purpose: maintain a revisable, challengeable account of a bounded subject. Candidate abstract state: subject, revision, actor-attributed events, claims, grounds, objections, applicability and inspectable history. Candidate actions: open, record, challenge, address, revise, inspect; the explicit B1 typed mapping below tests these actions and reveals domain-dependent guards rather than a proven generic principle. | A coherent single purpose and parameterized guard/effect table must reproduce C2 question/ground/challenge-disposition and R-06 request/acknowledgment/attempt/assessment/outcome/substantiation/invalidation without `status=done`, invented proof or a disguised union. Specify every precondition, effect, unknown and independent operational principle before equivalence can be judged. | **Open falsification hypothesis; no new owner** |

**Separate falsification tracks:** A is challenged for its four civic actor boundaries and the E-001 recordkeeping/completion confusion. B is challenged for whether one coherent generic purpose and guard/effect algebra can actually reproduce both concepts. A favorable result on either track cannot be substituted for evidence on the other.

## Source-linked behavior to discriminate

| Probe | C2 intrinsic promise (P01/P05) | R-06 intrinsic promise (P06) | Generic-case counterhypothesis and falsifier |
|---|---|---|---|
| Initial value | `OpenInquiry(question, revision)` creates an unsettled, inspectable question without a challenge or work request | `RequestWork(unit, revision, actor)` creates a bounded request without claiming progress | A generic case that requires a request to ask a question, or a question to request work, loses independent value. If both are merely optional labels, show its actual guards and inspection contract. |
| Contestation | `ChallengeGround` disputes an offered ground; `AddressChallenge` records an **attributed disposition and rationale while preserving the objection**; `ProposeAnswer` remains provisional, **not sponsor permission or proof of execution** | `ChallengeOutcome` marks an existing outcome assertion disputed and retains objection; **R-06 has no challenge-disposition action**. `SubstantiateOutcome` requires an attributable assertion, same-current-revision applicable supporting basis, and no unresolved disqualifying challenge; **never authorizes** | Test a C2 objection that receives a disposition while an R-06 assertion remains disputed. A generic `resolveChallenge` must not invent an R-06 disposition or turn C2 explanation into C3 authorization. |
| Revision and invalidation | `RebaseInquiry` removes presumed applicability of grounds and provisional answers, retaining inspectable old history | `InvalidateBasis` **withdraws current substantiation on the same revision** while retaining the historical assertion; separately `ReidentifyWork` **changes revision**, dropping inherited assessments, claims and bases while preserving their history | A single generic `revise` cannot conflate basis withdrawal on the same revision with a new work identity/revision; stale facts remain inspectable but not currently applicable. |
| Status truth | `InspectInquiry` exposes question, grounds, unresolved challenges and answer applicability, including old history | `InspectOutcome` separately exposes request, acknowledgment, attempt, assessment, claim, substantiation, dispute and invalidation; **missing facts remain unknown**. `AcknowledgeRequest` without `RecordAttempt` is valid; `RecordAttempt` without acknowledgment is also valid. | A generic `status=done`, acknowledgment or favorable assessment falsely collapses outcome distinctions. Test both acknowledgment-without-attempt and attempt-without-acknowledgment, retaining inspectable revision history and unknown facts. |
| Support and eligibility | Offered grounds are contestable applicability assertions, not independently verified truth | Completed-outcome substantiation needs attributable, revision-applicable, challengeable support and abstract actor eligibility; `verified=true` is insufficient | Do not equate C2 grounds with R-06 completion proof, or smuggle IAM/actor policy into the generic case. Concrete credibility and eligibility are still unresolved, not evidence of identity collapse. |

These are **specification-level falsification probes**, not completed user studies, executable tests or a finding that C1 is invalid. Comparator A must also be tested as four distinct actor-accountable civic actions, not as the generic case in comparator B. The shared vocabulary of claims, grounds, challenge and revision creates a real genericity hypothesis. The different observable purposes, states, guard/effect rules and substantiation requirements are counterevidence that must be challenged independently.

## Strongest generic-case collapse candidate B1 — constructed comparison, not a verdict

**B1's proposed single purpose** is to preserve a bounded subject's attributable, revisable, contestable assertions and their current applicability. Candidate state consists of subject, revision, typed actor-attributed events, grounds/bases, challenges, supersession and inspectable history. Its abstract operations are `record(kind,...)`, `challenge(target,...)`, `address(challenge,...)`, `changeRevision(...)`, `invalidate(basis,...)`, `markSupported(assertion,...)` and `inspect(view)`. A **single parameterized guard/effect table**, rather than one generic action or `status=done`, must preserve the full source behavior. Typed rules below are a *hypothesis*, not a new canonical specification; the risk is that B1 is merely a tagged union of two distinct concepts.

| Source action | B1 typed guard / effect and adversarial obligation (not a validated common rule) |
|---|---|
| C2 `OpenInquiry` | `record(question)`: supplied revision; create an unsettled inquiry. Initial state has **no inquiries**; no work request, answer or challenge inferred. |
| C2 `OfferGround` | `record(ground, claimedRevision)`: existing inquiry and referenced facts; retain the ground's **claimedRevision** as a contestable assertion of applicability, never verified truth. |
| C2 `ChallengeGround` | `challenge(ground)`: existing inquiry and ground; preserve an attributed dispute. A contested ground cannot silently become uncontested justification. |
| C2 `AddressChallenge` | `address(groundChallenge)`: existing C2 challenge; record attributed disposition and rationale while preserving the challenge. **No corresponding R-06 disposition action exists.** |
| C2 `RebaseInquiry` | `changeRevision(inquiry)`: retain prior inquiry history but withdraw presumed current applicability of old grounds and provisional answers; do not inherit an answer into a new revision. |
| C2 `ProposeAnswer` | `record(answer)`: existing inquiry, referenced grounds and revision-qualified claim; contested grounds cannot silently justify an uncontested answer. Provisional only; neither sponsor permission nor proof of execution. |
| C2 `InspectInquiry` | `inspect(inquiryView)`: expose question, grounds, disputes, dispositions, answer applicability and retained historical facts, including unknown/missing facts; an inquiry can remain unsettled indefinitely. |
| R-06 `RequestWork` | `record(request)`: bounded unit, revision and attributable actor; initial state has **no requested work**. Establish request only, not acknowledgment, attempt, progress or completion. |
| R-06 `AcknowledgeRequest` | `record(ack)`: an existing request **for that work revision** and attributable actor; acknowledgment is neither an attempt nor progress/completion. No attempt prerequisite. |
| R-06 `RecordAttempt` | `record(attempt)`: existing request for identified revision and attributable actor; reported result may be failure, unknown or apparent success. No acknowledgment prerequisite; attempt implies neither assessment nor completed work. |
| R-06 `RecordAssessment` | `record(assessment)`: identified revision and attributed evaluation claim; even a favorable assessment is not execution or completion. |
| R-06 `AssertOutcome` | `record(outcomeClaim)`: attributable unit/revision, outcome and cited bases; permitted claims include **completed, incomplete, failed, unknown**. Assertion is not substantiation and does not itself establish completion. |
| R-06 `ChallengeOutcome` | `challenge(outcomeClaim)`: existing assertion; mark it disputed and retain objection. No invented `AddressOutcomeChallenge`/resolution transition; disposition ownership remains an open 004-B completeness question. |
| R-06 `SubstantiateOutcome` | `markSupported(outcomeClaim,basis)`: existing attributable assertion, **basis supporting that specific claimed outcome**, applicable to the same current revision, with no unresolved disqualifying challenge. Only a supported, current, uncontested **completed** assertion is currently substantiated completion. **RD-08:** contradictory supported outcomes remain contested; never silently select a winner. Later invalidation may withdraw substantiation. `verified=true` alone is insufficient. Never authorize. |
| R-06 `InvalidateBasis` | `invalidate(basis)`: identified basis; withdraw all dependent **current** substantiation on the same revision, preserving the assertion, invalidation and history. |
| R-06 `ReidentifyWork` | `changeRevision(workUnit)`: new revision; old assessments, claims and bases lose inherited current applicability even if change is called immaterial, while historical facts remain inspectable. |
| R-06 `InspectOutcome` | `inspect(outcomeView)`: distinguish request, acknowledgment, attempt, assessment, assertion, substantiation, dispute, invalidation, revision applicability and retained history; absent facts are **unknown**, never implied success. |
**Reasoned adverse checks, not empirical execution:** The expanded B1 rows expose required inquiry-without-work and work-without-inquiry cases, acknowledgment without attempt and attempt without acknowledgment, attributed C2 disposition versus unresolved R-06 challenge, same-revision basis invalidation versus work reidentification, and **RD-08 contradictory supported outcomes remaining contested**. These checks expose the model's typed dependencies; they do not establish a single coherent generic concept. It cannot legitimately create an R-06 `AddressOutcomeChallenge` transition: the absence is an **open R-06 completeness/ownership question** from 004-B, not distinctness evidence. B1's type-specific guards are essential to these outcomes; a generic label, timeout, favorable review or `verified=true` cannot substitute for them. Actor eligibility and basis credibility remain unvalidated RD-15 inputs.

**B1-specific result: tagged union, not one operational principle.** The mapped operations require an inquiry/work type discriminator to choose different guard and effect families: `address` applies only to ground challenges, `markSupported` and `invalidate` only to outcomes, `changeRevision` discards different facts for inquiries versus work, and acknowledgment/attempt are not generic applicability assertions. B1's proposed purpose therefore fails to explain these operations as one inseparable intrinsic behavior; it is a typed union of two action sets, not demonstrated conceptual collapse. The detailed rows document the failure rather than rescuing B1 through a broader label. **RD-14 as a whole remains INDETERMINATE and OPEN:** failure of this B1 is neither a permanent C2/R-06 independence ruling nor grounds to reopen Phase 002-C. A genuinely new, independently valuable single-purpose algebra would require fresh adversarial comparison and exact-head review before any Phase 002-C return. C1 remains an unpromoted historical control. No RD-14 closure, boundary selection, 004-E admission, canonical-owner change, implementation or AWS/IAM authorization follows.

## Boundary alternatives and discriminating tests

| Alternative | Potential advantage | Decisive adverse case / evidence required | Provisional disposition |
|---|---|---|---|
| Retain C2 and R-06 separately | Distinct inquiry truth and outcome-accountability promises; no implicit work from an inquiry | Show a participant who can use either concept with all peer concepts absent; challenge whether distinct guards are merely one parameterized generic action | **Open**; current specification baseline, not final acceptance |
| Combine into one generic case | Common revision, challenge and history mechanics could simplify conceptual identity | A question with no work request and a failed attempt with no inquiry must both remain meaningful; generic guards cannot silently equate answers and completion | **Open**, not promoted; requires new complete concept specification |
| Split shared challenge/ground semantics into a third concept | May clarify P05 independently from P01/P06 | Demonstrate a standalone affected-party need and independent operational principle; otherwise this is a reusable mechanism or Phase 005 seam | **Open**, no new concept authorized |
| Reframe/generalize C2 or R-06 parameters | Abstract identity may remove avoidable application-specific coupling | Permutation/renaming test must preserve revision applicability, contestability and completion substantiation, not erase domain-relevant meaning | **Open**, only if source semantics survive |
| Reduce or reject an owner | Avoid duplicate purpose or an inert fragment | Must exhibit an actual behavioral redundancy and provide a named destination for P01/P05 or P06 obligations; a generic container alone is insufficient | **Open**, requires Phase 002-C return on genuine RD-14 collapse |
| Expand an owner for completeness | Could restore an intrinsic missing guard or correction behavior | Must show a purpose-critical behavior absent from canonical actions; cannot import C3 permission, external evidence policy, Phase 005 synchronization or infrastructure | **Open**, no new behavior invented |

## Adversarial discriminators for independent review

0. **C1 four-action control, not generic case:** On one change, have different actors inspect evidence, contest findings, authorize an action and report completion. Test whether those are merely S-81/PR #1 receipt/decision/progress records (E-001), whether reporting completion is falsely equated with executed work, and whether a C1 authorization label would improperly stand in for C3 scoped authority. Map each C1 action against C2 inquiry and R-06 outcome semantics; do not promote C1 or infer C3 permission.
1. **Question without work:** C2 must permit an unsettled inquiry and revised ground even if no bounded work unit exists. If a generic case cannot do so, it fails to subsume C2.
2. **Work without question:** R-06 must preserve requested, **acknowledged**, attempted, assessed, claimed, disputed, invalidated and substantiated distinctions without a C2 inquiry. Test acknowledgment without attempt, attempt without acknowledgment, failed/unknown reported result, and a favorable assessment without completed work. A generic case that turns any of these into completion fails P06.
3. **Two challenges, different objects:** challenge a C2 ground and use `AddressChallenge` to record its attributed disposition while preserving history; independently `ChallengeOutcome` on an R-06 assertion must mark it disputed without inventing an R-06 disposition. `SubstantiateOutcome` must reject absent, stale or disqualifyingly challenged support and never authorize; `ProposeAnswer` must not grant sponsor permission or prove execution.
4. **Two revisions, different invalidation:** rebase inquiry and reidentify work separately; verify stale grounds, assessments, claims and bases are not inherited as current. Also call `InvalidateBasis` on the *same* work revision: dependent substantiation is withdrawn while the historical claim remains inspectable. Unknown missing facts cannot be silently promoted to favorable results.
5. **False evidence:** favorable review, `verified=true`, silence, quota and timeout cannot create permission or substantiated completion. C3 authority and S-40 remain separate.
6. **Strongest collapse hypothesis (B1 tested and rejected as a tagged union):** the B1 table above maps all named C2 and R-06 actions but depends on separate typed guard/effect families and fails to demonstrate one independently valuable operational principle. A later genuinely unified algebra must preserve *all* guards, effects, inspections and histories, not just shared event mechanics. Only a demonstrated intrinsic equivalence would trigger independently reviewed **Phase 002-C reopening** before choosing a replacement.

## Preliminary analysis and review boundary

**No RD-14 resolution yet.** Probes 0–5 are **proposed falsification tests**, not executed tests or established evidence that independence survives. Probe 6 now has a constructed B1 mapping and explicit **tagged-union failure** under the current purpose/guard test; it does not demonstrate intrinsic equivalence, and no permanent independence verdict follows. The current evidence supports **continuing** adversarial comparison, not declaring C2/R-06 permanently independent or declaring a generic-case collapse. A reviewer must challenge the counterexamples and request missing behavior-level equivalence evidence. If a collapse is established, stop 004-D boundary promotion and return to Phase 002-C; otherwise preserve unresolved alternatives for 004-E rather than fabricating a final choice.

C1 remains an unpromoted control; C3 scoped permission is a negative control, **not** a 004-D authorization to decide C3's final boundary. C4 stays a recovery lens, C5 deferred, C6 unpromoted. P05 ownership remains open. R-06 basis credibility, actor eligibility and C2-ground synchronization remain open; Phase 005 composition, Phase 006 inclusion, Phase 007 presentation and later empirical/security validation are not specified here. E-301–E-306, G01–G14, E-001–E-004 and the historical aws-backbone **S-40 HOLD (003-D RD-12)** remain binding; neither a favorable review nor a shared coordinator may clear local security authority.

**Requested independent verdict:** PASS / PASS WITH CARRY-FORWARD / HOLD on the *bounded comparison quality*, specifically whether the C1 control is represented accurately, alternatives are genuine and falsifiable, RD-14 collapse/reopening is not prejudged, and no Phase 004 exit, canonical-owner mutation, implementation, AWS/IAM, or Phase 005 work is authorized.
