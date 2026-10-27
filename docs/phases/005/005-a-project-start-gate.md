---
type: Phase Start Gate Assessment
title: 005-A — Project Composition Entry and Dependency-Safe Work Plan
description: Source-linked bounded Phase 005-A concept-design start-gate candidate, with falsifiable composition planning and independent qualification boundary.
tags: [phase-005, start-gate, composition, planning, review-candidate]
---

# 005-A — Project composition entry and work plan

**Status: REVIEW CANDIDATE; 005-A independent gate verdict pending.** Sponsor explicitly authorized **Option A** for bounded Phase 005 concept-design entry on [Linear S-110](https://linear.app/s-kelly/issue/S-110) on 2026-10-27, then granted standing *conditional* phase-start authority for Phases 005–011 on [S-98](https://linear.app/s-kelly/issue/S-98). This authorizes 005-A planning, **not** automatic 005-B–F admission, canonical synchronization promotion, implementation, merge or security waiver. Phase 004 exit was sponsor-accepted **PASS WITH CARRY-FORWARD** on [S-137](https://linear.app/s-kelly/issue/S-137); [F3](../004/004-f3-independent-exit-evidence.md) remains a historical independent-exit *candidate*, not an independently certified PASS. [The prior 005-A eligibility assessment](005-a-initial-eligibility-assessment.md) passed independent review as an **eligibility assessment only** in merged [PR #15](https://github.com/SethDKelly/linear-shared-orchestrator/pull/15).

## 1. Baseline and governing authority

Use the [Phase 005 start-gate contract](005-a-start-gate.md), [phase definition](phase-definition.md), [composition contract](composition-synchronization-contract.md), and [Phase 004 F1](../004/004-f1-owner-disposition-reconciliation.md)/[F2](../004/004-f2-obligation-navigation-crosswalk.md) for the bounded handoff. The **provisional** current concept owners are [C2 living inquiry](../../canonical/concepts/c2-living-inquiry.md) (P01/P05), [C3 scoped authorization](../../canonical/concepts/c3-scoped-authorization.md) (P02/P04), and [R-06 work outcome accountability](../../canonical/concepts/r06-work-outcome-accountability.md) (P06). These links, not this phase plan, own intrinsic actions, preconditions, effects, history, authority and revision semantics.

- **C2:** `OpenInquiry`, `OfferGround`, `ChallengeGround`, `AddressChallenge`, `RebaseInquiry`, `ProposeAnswer`, `InspectInquiry`. A proposed answer is neither authorization nor completed work; rebase invalidates presumed applicability of old grounds.
- **C3:** `ConsiderScope`, `Withhold`, `Authorize`, `Withdraw`, `InspectPermission`. External obligation assertions and favorable review never create permission; authorization remains explicit, actor-attributed and scope-guarded.
- **R-06:** `RequestWork`, `AcknowledgeRequest`, `RecordAttempt`, `RecordAssessment`, `AssertOutcome`, `ChallengeOutcome`, `SubstantiateOutcome`, `InvalidateBasis`, `ReidentifyWork`, `InspectOutcome`. An assertion or attempt is not substantiation. Preserve revision applicability, contested and **NOT SUBSTANTIATED** history, and independent credible-suspicion investigation; do not invent a mandatory challenge-resolution action.

C1 remains an unpromoted historical comparator; C4 a recovery lens; C5 cross-project federation deferred; C6 not retained as a standalone concept. [S-135](https://linear.app/s-kelly/issue/S-135) Q4/Q5 are frozen absent material intrinsic evidence. **RD-14** generic-case collapse and **RD-15** independently credible basis/materiality/actor eligibility remain open with F2 owners and triggers. Demonstrated source-complete RD-14 collapse returns **first to Phase 002-C**; intrinsic specification or factoring defects return to their qualified Phase 003/004 owners, not to a synchronization workaround. The separate AWS Backbone S-40 security HOLD persists.

## 2. Obligation triage and candidate seams — questions, not edges

| ID | Purpose-linked question | Candidate action seam to investigate | First falsifier / guard | Accountable route |
| --- | --- | --- | --- | --- |
| CO-1 | Does an inquiry's supported/contested answer ever inform a work-outcome assessment without becoming proof of completion? | C2 `ProposeAnswer` or `InspectInquiry` ↔ R-06 `RecordAssessment` or `AssertOutcome` | No same-current-revision applicable evidence, or a contested inquiry treated as substantiated; **no edge admitted** | TPO → C2/R-06 source owners |
| CO-2 | Does a bounded work request require explicit project-local permission, without treating review as authorization? | C3 `Authorize`/`InspectPermission` ↔ R-06 `RequestWork` | A review/assessment/obligation assertion is used to grant C3 permission, or authority guard fails; **no edge admitted** | TPO → C3/R-06 source owners |
| CO-3 | Are correction, withdrawal and re-identification visible across independently valid histories when the application promises it? | C2 `RebaseInquiry`, C3 `Withdraw`, R-06 `ReidentifyWork`/`InvalidateBasis` | Prior-revision evidence silently becomes current, or independent lifecycle action is wrongly made mandatory; **no edge admitted** | TPO → affected concept source owners |
| CO-4 | Does a material challenge require application-level awareness without adding an intrinsic R-06 adjudication action? | C2 `ChallengeGround` ↔ R-06 `ChallengeOutcome`/`InspectOutcome` | `NOT SUBSTANTIATED` erased, safety-review pending treated as PASS, or a new mandatory resolution action invented; **no edge admitted** | TPO → R-06 policy/source owner (RD-15) |

These are *candidate* cross-concept questions, not a declaration that any pair must synchronize. For each, first test whether the promised behavior is actually concept-local, already covered by an existing action, or unsupported by product purpose. Record **reject/no synchronization** as a valid outcome. Do not use this table as a substitute for independently qualified purpose-to-action evidence.

## 3. Deliberate application action surface

005-B must classify each relevant intrinsic action as **directly exposed**, **composition-only**, **system-triggered**, **intentionally not exposed**, or **unresolved**. No class is pre-assigned by this plan. Specifically test whether C3 `Authorize` should ever be directly available under its own authority guard, whether R-06 `SubstantiateOutcome` must remain protected from unsupported application invocation, and whether C2 inspection/challenge can remain independently useful. A one-action exposure is allowed when meaningful; no UI, endpoint, webhook, event bus or transport decisions are made here.

## 4. Dependency-safe candidate subphases and evidence

| Candidate | Scope and source | Depends on | Minimum sufficient review evidence and handoff |
| --- | --- | --- | --- |
| **005-B — Baseline/action-surface inventory** | F1/F2 and current C2/C3/R-06 purposes, actions, guards, revision/authority semantics; exposure/non-exposure candidate classification | Independent 005-A entry PASS/PASS WITH CARRY-FORWARD | Source-linked action and purpose coverage, explicit unknowns, intrinsic-defect return triggers; **no synchronization design** |
| **005-C — Obligation/seam qualification** | CO-1–CO-4 and any separately evidenced purpose-linked seam; concept-local vs cross-concept vs unsupported | Accepted B baseline | For each candidate, supported application purpose, participating actions, semantic value availability, counterexample, accept/reject/hold; no inferred permission |
| **005-D — Deliberate exposure and bounded synchronization** | Qualified C seams only; direct/combined/hidden application actions; conceptual trigger, bindings, conditions and chained effects | C qualified seams and B exposure inventory | Paper traces for both valid and invalid states, authority/guard/revision/contested-history negative tests; over/under-synchronization challenged |
| **005-E — Automation, synergy and surface regression** | Accepted D composition only; non-exposure, chain cycles, genuine additional benefit vs mere feature aggregation | D accepted semantic composition | Purpose-linked positive/negative paper traces, explicitly supported or rejected synergy, Phase 006/007 deferrals |
| **005-F — Independent exit and Phase 006 handoff** | Accepted B–E work or explicit dispositions, canonical/index reconciliation and open obligations | All admitted Phase 005 work dispositioned | Independent exact-head semantic exit verdict, documentation/OKF audit, explicit carry-forward owner/trigger, separate Phase 006 start eligibility |

This sequence is **proposed, not automatically admitted**. The independent 005-A reviewer may require a narrower dependency-safe decomposition. Do not create B–F Linear issues or begin D synchronization until 005-A is independently qualified and the TPO admits the next bounded subphase. Keep reviewer/WIP capacity and current active version eligibility as hard prerequisites, not as a reason to promote future-version work.

## 5. Qualification tests, ownership and exclusions

The 005-A reviewer should falsify the **plan** (not require completed composition): (1) every cited current concept action and source resolves and its stated semantics match; (2) CO-1–CO-4 remain questions, not preapproved syncs; (3) C3 authorization cannot be inferred from C2 or R-06 evidence; (4) R-06 contested, safety-review-pending and NOT SUBSTANTIATED remain distinguishable; (5) revision changes cannot silently reuse old evidence; (6) application exposure is determined before synchronization design; (7) RD-14/15 and Q4/Q5 return triggers survive; (8) Phase 006 inclusion/dependence, Phase 007 representation, Phase 008 reuse and all implementation are excluded; (9) each candidate subphase has a predecessor, falsifier, evidence and owner route; (10) canonical navigation resolves.

**Authority and writers:** canonical concept source owners control intrinsic semantics; a future qualified composition owner controls only application-level synchronization and exposure, not the underlying concepts. TPO owns admission/dependencies and routes unassigned work; missing Linear assignee is metadata debt. Independent Cursor/Codex review of the **exact PR head/base** is required for gate qualification; Codex no-major-code-findings alone is not a semantic PASS. GitHub owns CI/PR/merge evidence, Linear work state, repository docs canonical meaning, and SHA-bound ledger historical review events. Conflicts are recorded with provenance, not resolved by last-writer-wins. S-140 eight-domain architecture and merged methodology proposals remain **non-authoritative**, not new gate criteria.

**Gate request:** independent reviewer return **PASS**, **PASS WITH CARRY-FORWARD** (named owner/trigger), or precise **HOLD** for an in-scope missing baseline, invalid purpose/action seam, unsafe dependency order, broken source or authority conflict. No self-certification. Phase 005-A may close only after independently supported gate outcome and canonical navigation reconciliation. **Implementation readiness: not ready; execution: not started; authorization: not granted.**
