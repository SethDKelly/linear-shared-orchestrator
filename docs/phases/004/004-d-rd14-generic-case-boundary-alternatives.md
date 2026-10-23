---
type: Phase Design Record
title: 004-D — RD-14 Generic-Case Comparison and Boundary Alternatives (Review Candidate)
description: Bounded falsification of C2 and R-06 distinctness against the unpromoted C1 control; no final factoring decision.
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
---

# 004-D — RD-14 generic-case comparison and boundary alternatives

**Status: review candidate, NOT an independent 004-D verdict.** 004-C's independent PASS WITH CARRY-FORWARD at `fba7b20`, followed by the PR #3 documentation reconciliation review at `77a2ffb` (Cursor PASS WITH CARRY-FORWARD; Codex code review completed without major findings), admits **only** RD-14 generic-case comparison and boundary alternatives. This record neither closes RD-14 nor approves any boundary. PR #3 remains unmerged; root and Phase 003 index wording about "boundary alternatives" remains a documentation carry-forward.

## Authority and the comparator

Phase 002-C calls **C1 "Distinct civic actions"**, a control decomposition separating inspection, contestation, authorization and completion reporting; Phase 002-E did **not** retain it as a new independent concept because it resembled incumbent receipt/decision/progress modules. "Generic case" here is a **falsification hypothesis** for C2 and R-06, not an accepted canonical C1 case specification or permission to resurrect an implementation container. A proposed generic case must state its own purpose, state, actions, guards, effects, revision semantics and independently useful operational principle before it can displace an owner. Naming all facts "case events" does not prove behavioral equivalence.

RD-14 / E-301 asks whether C2 and R-06 retain intrinsic, user-observable semantics not subsumed by the control/generic-case alternative. **Demonstrated intrinsic collapse returns to Phase 002-C for renewed alternatives and independent review; it does not auto-promote C1.** The separate RD-15 abstract-survival ruling is available context, not an extra prerequisite to recognizing collapse. Concrete R-06 basis credibility and actor eligibility remain open.

## Source-linked behavior to discriminate

| Probe | C2 intrinsic promise (P01/P05) | R-06 intrinsic promise (P06) | Generic-case counterhypothesis and falsifier |
|---|---|---|---|
| Initial value | `OpenInquiry(question, revision)` creates an unsettled, inspectable question without a challenge or work request | `RequestWork(unit, revision, actor)` creates a bounded request without claiming progress | A generic case that requires a request to ask a question, or a question to request work, loses independent value. If both are merely optional labels, show its actual guards and inspection contract. |
| Contestation | `ChallengeGround` disputes an offered ground; `AddressChallenge` retains objection history; `ProposeAnswer` stays provisional | `ChallengeOutcome` contests an accountable outcome assertion; `SubstantiateOutcome` requires applicable support and no unresolved disqualifying challenge | A shared `challenge` verb is not equivalence: test whether it can preserve the **different targets, effects and resolution conditions** without importing one concept's semantics into the other. |
| Revision | `RebaseInquiry` removes presumed applicability of grounds and provisional answers | `ReidentifyWork` removes presumed applicability of prior assessments, claims and bases while retaining history | If a single generic revision action cannot express both effects without a domain-specific discriminator, a mere shared history store does not establish collapse. |
| Status truth | `InspectInquiry` exposes question, grounds, disputes and answer applicability | `InspectOutcome` exposes request, acknowledgment, attempt, assessment, claim, substantiation, dispute and invalidation; missing remains unknown | A generic `status=done` or favorable assessment falsely collapses outcome distinctions. A generic model may survive only by faithfully reproducing these invariants without turning into an unbounded union. |
| Support and eligibility | Offered grounds are contestable applicability assertions, not independently verified truth | Completed-outcome substantiation needs attributable, revision-applicable, challengeable support and abstract actor eligibility; `verified=true` is insufficient | Do not equate C2 grounds with R-06 completion proof, or smuggle IAM/actor policy into the generic case. Concrete credibility and eligibility are still unresolved, not evidence of identity collapse. |

These are **specification-level falsification probes**, not completed user studies, executable tests or a finding that C1 is invalid. The shared vocabulary of claims, grounds, challenge and revision creates a real genericity hypothesis. The different observable purposes, states, guard/effect rules and substantiation requirements are counterevidence that must be challenged independently.

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

1. **Question without work:** C2 must permit an unsettled inquiry and revised ground even if no bounded work unit exists. If a generic case cannot do so, it fails to subsume C2.
2. **Work without question:** R-06 must preserve requested, attempted, assessed, claimed and substantiated distinctions without a C2 inquiry. A generic case that turns an assessment into completion fails P06.
3. **Two challenges, different objects:** challenge a C2 ground and independently challenge an R-06 assertion; confirm that resolution of one does not automatically settle the other.
4. **Two revisions, different invalidation:** rebase inquiry and reidentify work separately; verify stale grounds, assessments, claims and bases are not inherited as current.
5. **False evidence:** favorable review, `verified=true`, silence, quota and timeout cannot create permission or substantiated completion. C3 authority and S-40 remain separate.
6. **Strongest collapse hypothesis:** propose a parameterized generic state/action algebra reproducing *all* C2 and R-06 guards, effects, inspections and histories. If that algebra has a coherent independently valuable purpose rather than an unbounded union, record the exact equivalence and **reopen 002-C** before choosing a replacement.

## Preliminary analysis and review boundary

**No RD-14 resolution yet.** The first five probes reveal nontrivial distinct intrinsic semantics, while probe 6 remains the strongest untested collapse alternative. The current evidence supports **continuing** adversarial comparison, not declaring C2/R-06 permanently independent or declaring a generic-case collapse. A reviewer must challenge the counterexamples and request missing behavior-level equivalence evidence. If a collapse is established, stop 004-D boundary promotion and return to Phase 002-C; otherwise preserve unresolved alternatives for 004-E rather than fabricating a final choice.

C1 remains an unpromoted control; C3 scoped permission is a negative control, **not** a 004-D authorization to decide C3's final boundary. C4 stays a recovery lens, C5 deferred, C6 unpromoted. P05 ownership remains open. R-06 basis credibility, actor eligibility and C2-ground synchronization remain open; Phase 005 composition, Phase 006 inclusion, Phase 007 presentation and later empirical/security validation are not specified here. E-301–E-306, G01–G14, E-001–E-004 and S-40 HOLD remain binding.

**Requested independent verdict:** PASS / PASS WITH CARRY-FORWARD / HOLD on the *bounded comparison quality*, specifically whether the C1 control is represented accurately, alternatives are genuine and falsifiable, RD-14 collapse/reopening is not prejudged, and no Phase 004 exit, canonical-owner mutation, implementation, AWS/IAM, or Phase 005 work is authorized.
