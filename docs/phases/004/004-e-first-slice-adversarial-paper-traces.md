---
type: Phase Design Record
title: 004-E — First Bounded Adversarial Paper Traces
description: Source-linked counterexample execution on paper against provisional C2, C3 and R-06; no executable or empirical validation.
tags: [phase-004, adversarial, provisional, paper-traces]
sources:
  - id: c2
    resource: ../../canonical/concepts/c2-living-inquiry.md
    title: C2 provisional conceptual actions and boundaries
  - id: c3
    resource: ../../canonical/concepts/c3-scoped-authorization.md
    title: C3 provisional exact-scope authorization
  - id: r06
    resource: ../../canonical/concepts/r06-work-outcome-accountability.md
    title: R-06 provisional actions, invariants and inspection
  - id: phase3
    resource: ../003/003-c-r06-completion-behavior-return.md
    title: Phase 003 R-06 action guards and invariants
  - id: entry
    resource: 004-e-adversarial-entry-gate.md
    title: Admitted 004-E bounded trace scope
---

# 004-E — Three adversarial paper traces against current concept contracts

**Evidence class:** Three **reasoned specification-level traces**, not executable tests, empirical participant observations, or independent reviewer verdicts. Baseline: merged 004-D documents at `main` `2f2c224d378eff860c9aacd5beafcd35ea9a5e69`. These probe the *existing* provisional concepts, not a new generic-case algebra; prior 004-D RD-14 probes remain separate and RD-14 stays open. The sequence descriptions below are paper instantiations of documented actions; an action called *rejected* is an expected guard result, not a claim that software ran.

## T1 — Stale revision must not regain present substantiation or permission

**Purpose / source:** P01/P03/P06 current-versus-historical truth. [R-06 conceptual actions and invariants](../../canonical/concepts/r06-work-outcome-accountability.md#conceptual-actions-and-guards), [Phase 003 R-06 invariants 2, 3 and 5](../003/003-c-r06-completion-behavior-return.md#invariants-and-temporal-behavior), [C2 conceptual actions](../../canonical/concepts/c2-living-inquiry.md#conceptual-actions), [C3 conceptual actions](../../canonical/concepts/c3-scoped-authorization.md#conceptual-actions).

**Initial state:** No work request, inquiry or permission. Choose existing unit `u` at `r0`, inquiry `i` and authorization scope `s0`; `r1 != r0`, `s1 != s0`. All bases and actors are abstract; no concrete eligibility policy is assumed.

| Step | Guard-valid paper action | Expected observable state / counterexample check |
| --- | --- | --- |
| 1 | `RequestWork(u,r0,A)`; `RecordAttempt(u,r0,B,reportedResult)`; `AssertOutcome(u,r0,C,completed,[b0])` | Request, attempt and completed *assertion* remain distinct; neither attempt nor assertion proves completion. A cited basis is not automatically independently credible. |
| 2 | **Conditional** `SubstantiateOutcome(u,assertion,b0)`, only if `b0` really supports the claim, applies to `r0`, is attributable and no disqualifying contest or safety review is active | Current substantiation can be shown for `r0` *only if all abstract guards hold*. This is a conditional branch, not a finding that `b0` passed RD-15. |
| 3 | `ReidentifyWork(u,r1)`; `InspectOutcome(u)` | Historical `r0` request/attempt/claim/substantiation retained, but **not** current `r1` substantiation. Reject a purported carry-forward of `b0` merely because `r1` is called “minor.” Missing `r1` evidence is unknown. |
| 4 | `OpenInquiry(question,r0)`; `OfferGround(i,g0,r0)`; `ProposeAnswer(i,claim,[g0])`; `RebaseInquiry(i,r1)`; `InspectInquiry(i)` | The existing inquiry is unsettled or its old answer stale; old `g0` and answer history is visible but not presumed current at `r1`. No work request or permission is inferred from inquiry. |
| 5 | `ConsiderScope(s0,obligations)`; **conditional** `Authorize(s0,localActor,basis)` only if the project-local authority predicate is satisfied; then inspect `s1` | Even if explicit permission exists for `s0`, it does **not** authorize `s1`. No actual permission is granted by this paper trace; S-40 remains binding. |

**Falsifier:** Any source-permitted transition that marks an `r0` basis as currently substantiating `r1` without renewed applicability, or an `s0` authorization as applicable to `s1`, contradicts the cited invariants. **Paper result:** The documented guards and inspection rules reject both; no intrinsic contradiction established. **Class:** bounded design check **PASS ON PAPER**, not executable verification. **Carry-forward:** Concrete basis credibility/actor eligibility (RD-15) and evidence-access/privacy rules need a separately qualified owner; not a new 004-E blocker.

## T2 — Competing grounds, nonmaterial objection and safety suspicion must remain distinguishable

**Purpose / source:** P05/P06 contest observability. [C2 challenge/disposition](../../canonical/concepts/c2-living-inquiry.md#conceptual-actions), [R-06 ChallengeOutcome / InspectOutcome](../../canonical/concepts/r06-work-outcome-accountability.md#conceptual-actions-and-guards), [R-06 invariants](../../canonical/concepts/r06-work-outcome-accountability.md#invariants-lifecycle-and-deliberate-open-questions).

**Initial state:** An existing `u,r0` and attributable completed assertion `a` with a potentially supporting `b`; any initial substantiation is **conditional** on source guards. An existing C2 inquiry `i` with offered ground `g`. Each row below is a **fork from this initial state**, not an impossible sequence where mutually exclusive statuses are conflated.

| Fork | Guard-valid paper action | Required inspection / rejected shortcut |
| --- | --- | --- |
| A — Nonmaterial | `ChallengeOutcome(u,a,X,reason,restatement,groundsWithoutMaterialDifference)` with existing `a` and identified `X` | Retain attributed **NOT SUBSTANTIATED** objection/history; it is not an active material contest, does not prove `a`, and by itself does not withdraw otherwise valid current substantiation. New material grounds can reopen qualification. |
| B — Material | `ChallengeOutcome(u,a,Y,reason,competingOutcome,statedMaterialGrounds)` | Show **CONTESTED**; if material and disqualifying, withdraw affected *current* substantiation immediately while preserving historical substantiation. Silence, timeout and favorable assessment do not resolve it. |
| C — Credible safety/evidence suspicion | `ChallengeOutcome(u,a,Z,reason,credibleSuspicion,availableGrounds)`, with a credible integrity suspicion whose detailed evidence is still being investigated | Show **CONTESTED — SAFETY REVIEW PENDING** and suspend affected current substantiation. No new/restored substantiation while separately qualified review remains pending. Do not infer that every unsupported objection is credible: concrete credibility policy remains RD-15. |
| D — Contradictory supported assertions | Record another attributable outcome assertion `a2` for the **same** unit/revision with support such that `a` and `a2` cannot both hold | `InspectOutcome(u)` must expose **CONTESTED** even with **no** explicit `ChallengeOutcome`. Neither a “latest wins” policy nor silent success is source-permitted. |
| E — Inquiry challenge | `ChallengeGround(i,g,reason)`; `AddressChallenge(i,challenge,disposition,rationale)` with an existing challenge | C2 preserves challenge plus attributed disposition. It does **not** authorize `u`, settle an R-06 outcome challenge, or invent `AddressOutcomeChallenge`. |

**Falsifier:** A source-compliant inspection that hides supported contradictions, erases a NOT SUBSTANTIATED objection, treats silence as challenge disposition, or restores a safety-suspended outcome without separately qualified evidence would violate the current contract. **Paper result:** Explicit provisional inspection/guard rules reject those shortcuts; no intrinsic defect established. **Class:** bounded design check **PASS ON PAPER**. **Carry-forward:** S-141 source-owner choice on P05/R-06 disposition is intentionally open, not mandatory resolution; independently investigate credible suspicion; materiality/eligibility and privacy of grounds require later qualification.

## T3 — Favorable review, bare assertion and generic reply must not become completed or authorized work

**Purpose / source:** P02/P04/P06 false-positive protection. [Phase 003 R-06 guards](../003/003-c-r06-completion-behavior-return.md#conceptual-actions-and-semantics), [R-06 conceptual actions](../../canonical/concepts/r06-work-outcome-accountability.md#conceptual-actions-and-guards), [C2 actions](../../canonical/concepts/c2-living-inquiry.md#conceptual-actions), [C3 actions](../../canonical/concepts/c3-scoped-authorization.md#conceptual-actions).

**Initial state:** No work requested, no inquiry and no scoped permission.

| Step | Paper action / adversarial attempt | Expected guard or observation |
| --- | --- | --- |
| 1 | Attempt `AcknowledgeRequest(u,r0,A)` and `RecordAttempt(u,r0,B,unknown)` before a request | **Reject**: both require a request for that revision. This is an expected negative-control guard failure, not an executed failed test. |
| 2 | `RequestWork(u,r0,A)`; `AcknowledgeRequest(u,r0,B)`; `RecordAssessment(u,r0,C,favorable)`; `InspectOutcome(u)` | Acknowledged and assessed, but **no attempt** and no completed-outcome substantiation. Assessment can be recorded without implying execution. |
| 3 | On another requested unit `v,r0`, `RecordAttempt(v,r0,D,unknown)` without acknowledgment; inspect | Attempt exists, acknowledgment absent; unknown is not completed. This demonstrates the converse independence. |
| 4 | `AssertOutcome(u,r0,E,completed,[])`; attempt `SubstantiateOutcome(u,assertion,verified=true)` | Claim is attributable but unsubstantiated; **reject** bare `verified=true` without independently meaningful, same-revision supporting basis. A claim is not completion. |
| 5 | `OpenInquiry(q,r0)`; `OfferGround(i,g,r0)`; `ChallengeGround(i,g,reason)`; attempt a generic “reply” as if it were `AddressChallenge` | **Reject as disposition** unless the actual C2 `AddressChallenge(i,existingChallenge,disposition,rationale)` action is invoked with attributable disposition. Even valid C2 disposition never implies R-06 completion. |
| 6 | `ConsiderScope(s,externalObligations)`; `Withhold(s,localActor,rationale)`; inspect | No permission. Neither favorable assessment, C2 answer, `verified=true`, nor issue status grants `Authorize`. An actual `Authorize` still requires explicit project-local actor authority and exact scope; S-40 is not waived. |

**Falsifier:** A guard-valid source rule that promotes assessment, `verified=true`, an arbitrary reply or a withhold/consideration into substantiated completion or permission would defeat the separation. **Paper result:** The specified action guards and negative controls reject the promotions; no intrinsic contradiction established. **Class:** bounded design check **PASS ON PAPER**; expected guard rejections are paper negative controls, not implementation failures. **Carry-forward:** The actor eligibility predicate and basis quality remain open RD-15 inputs, not a fabricated universal validator.

## Disposition and next bounded gate

**Finding classes:** (i) **Intrinsic in-scope defect:** none demonstrated by these paper traces; if independently substantiated, route to provisional canonical owner and qualified Phase 003 reopening for material behavior/identity change, or Phase 002-C for demonstrated RD-14 collapse. (ii) **Broken verification/test:** none executed; no automated test pass/fail claimed. (iii) **Later-phase improvement:** privacy/accessibility of evidence display, concrete actor/basis qualification and cross-concept synchronization remain explicit owner/trigger carry-forwards, not mandatory additions to this slice.

**Decision scope:** These three traces provide a falsifiable first 004-E review candidate only; they do **not** prove universal concept independence, empirical participant success, RD-14 resolution, 004-E exit or Phase 005 admission. C2/C3/R-06 remain provisional. S-141 outcome challenge-disposition source-owner question stays open; NOT SUBSTANTIATED history, credible-suspicion investigation and visible contested outcomes are preserved. No implementation, AWS/IAM/STS/Terraform, security bypass, release or production authority. S-40 HOLD persists; Phase 012 is the program endpoint.

**Review request:** Independent exact-head reviewer should check the three sequences against linked canonical action guards, including conditional basis/actor eligibility, C2 challenge preconditions, contradictory supported outcomes and the C3 scope/authority negative control. Return bounded PASS, PASS WITH CARRY-FORWARD or a precise intrinsic HOLD; separate documentation/verification errors from real conceptual defects. No self-certified independent verdict.
