---
type: Methodology Design Proposal
title: Closure-oriented planning, priority admission and scope conservation — review candidate
description: Non-authoritative proposal for backlog preparation and milestone closure without expanding approved scope.
tags: [methodology-proposal, planning, prioritization, scope-control, review-candidate]
---

# Closure-oriented planning and admission — independent design candidate

**Status: NON-AUTHORITATIVE, NOT ADOPTED.** **Coordination identity: [PR #16](https://github.com/SethDKelly/linear-shared-orchestrator/pull/16)**; do not use Linear S-140 as this proposal's owner. [Linear S-140](https://linear.app/s-kelly/issue/S-140) currently coordinates [PR #6's separate qualification-contract proposal](qualification-contract-delivery-proposal.md). Phase 004's *eight-domain responsibilities / source-of-truth and writer / version admission / WIP* S-140 gloss is related **non-authoritative design context**, not a fourth adopted meaning of that issue. This document proposes only the **planning, scope classification, priority, and admission-decision boundary**, not an implementation or a new controller.

Authority: [methodology authority](authority.md), [phase lifecycle](phase-lifecycle.md), [canonical knowledge](knowledge-authority.md), [design-only guardrails](design-only-guardrails.md). Phase 000–011 remain concept design; Phase 012 is pre-implementation preparation and the current program endpoint. There is **no admitted Phase 013 or downstream implementation gate**. Phase 005-A is an assessment, not admission. S-40 remains a separate security HOLD; provisional C2/C3/R-06 and RD-14/RD-15 are not silently resolved.

## Distinct responsibilities and source ownership

| Responsibility | Permitted decision | Explicitly excluded |
|---|---|---|
| Approved plan/phase/version authority | Approves objective, scope, acceptance criteria, dependencies, milestone/version eligibility and plan changes | Delegation to a queue score or Linear field mutation |
| Project Planner | Observes backlog; classifies work, identifies minimal gaps, prepares readiness proposals and closure paths | Changes canonical acceptance, approves gap or execution |
| Priority & Admission function | Ranks eligible work, applies WIP/backpressure, proposes a gate decision to the actual authorizer | Grants plan-change, security, independent-review or downstream implementation authority |
| Delivery Orchestrator | Acts only on still-valid admitted, revision-bound work; produces closure evidence | Converts ready proposals into admitted work |
| Evidence/synchronization function | Records source-linked observations, reconciles GitHub/Linear, preserves append-only decisions and retries idempotently | Self-certifies PASS or rewrites historical evidence |
| Independent reviewer | Independently falsifies the qualified candidate at the required exact head | Is assumed to be the planner, contributor or evidence author |

These are **responsibility labels**, not proof of distinct human/agent identities. The planner, proposer, executor and evidence author are **not** the plan authority or the independent reviewer by role. Contributor, accountable owner, approver and reviewer remain distinct; missing Linear assignee is metadata debt, not an automatic exit veto.

Canonical phase/plan documents own approved scope; Linear owns work-item status, relationships and accountable ownership **as observations**, not unilateral scope changes; GitHub owns exact commit, checks, reviews, PR/merge events; the PR #6 proposal, if later adopted, would own a separate gate-scoped qualification contract and review-evidence ledger. Only the designated writer changes its source of truth. Conflicts between systems are flagged for owner reconciliation; downstream synchronization is not plan approval.

## Intake and falsifiable scope conservation

**ACTIVE** means a work item explicitly admitted to the currently authorized work/phase gate, not every backlog issue or proposal. An ACTIVE item must continue to trace to the *same approved plan obligation/revision* or a separately **plan-authority-approved** minimum necessary gap; its scope, source revision and gate conditions must still hold. A parent link is necessary for traceability but **never sufficient** to prove scope.

Classify each candidate **before** prioritizing:
- **PLANNED:** Exact current approved obligation, unchanged behavior and acceptance; decomposition may only split the same requirement.
- **NECESSARY GAP:** Quote the exact already-approved acceptance sentence and source revision; provide an observation showing that sentence is already false or unprovable under the approved verification obligations; demonstrate the smallest repair that introduces **no new user-visible behavior or criterion beyond that sentence**; identify exclusions, negative control and accountable *plan-authority* approval. A missing negative test is a gap only when the original requirement or governing test obligation already requires it. Otherwise propose a plan change.
- **EXPANSION:** New feature, new objective, changed acceptance, or an asserted gap that fails the quoted-sentence test. Quarantine for separate plan authority; no execution admission even with a convenient parent.
- **DUPLICATE / SUPERSEDED:** Compare the merged evidence **and all residual acceptance text** to the canonical plan revision, plus other open PRs/dependencies citing the issue. Only close as duplicate when no distinct obligation or active dependent work remains. Otherwise preserve unmatched content as insufficient evidence or proposed expansion.
- **INSUFFICIENT EVIDENCE:** Missing or disputed source/approval; keep in preparation or HOLD, never promote to ACTIVE.

A proposed security containment may immediately **HOLD/isolate the affected surface and escalate to the named security/sponsor authority**. It does not authorize remediation, readiness promotion on that surface, branch-policy bypass or unrelated work. Unaffected, separately qualified work can continue only after scope isolation is evidenced.

## Readiness, revocation and priority

**DISCOVERED → CLASSIFIED → PREPARED → READY FOR ADMISSION REVIEW → ADMITTED (only after a separately authorized gate) → IN PROGRESS → QUALIFIED FOR CLOSURE → CLOSED**. HOLD/DEFER/REVOKED are explicit side states. Readiness is not approval. Revoke READY/ADMITTED immediately when a **material** scope classification, source-owner revision, exact execution HEAD, qualification-contract revision, authority, security condition or required gate changes. Requalify before resuming. A purely editorial canonical edit with no semantic/source-owner impact does not revoke work; record the unchanged semantic revision. A named source/plan authority may lodge a material dispute; ordinary unsubstantiated comments cannot indefinitely freeze a train.

**Hard gates precede priority**: version-train admission, scope class, security, phase authority, dependencies, required independent assurance and execution capacity. Among eligible work use lexicographic classes, never a blended score:
- **P0:** verified safety/authority containment or explicit HOLD, under its own authority.
- **P1:** qualified current-milestone closure **and qualified critical-path prerequisites that directly unlock that closure**; prioritize by demonstrated milestone exit impact, then readiness, constrained reviewer capacity and stable work ID. A noncritical P1 task does not outrank an unlocking prerequisite merely because it is already ready.
- **P2:** other necessary approved current-milestone dependencies and bounded remediation.
- **P3:** next **approved** milestone **offline preparation only**, requiring named preparation authority, separate WIP cap and no diversion from unfinished current-train critical path.
- **P4:** unapproved future versions and expansions; no admission.

Unused capacity does **not** admit a lower class while a higher-priority closure path is blocked or under-resourced. Suspend previously admitted lower-train work if it now threatens the current train; finish-first applies **only** to still-in-scope, still-qualified active work. Explicit sponsor reordering is a recorded plan/admission decision, not a silent scheduling exception.

WIP counts **admitted execution packages/PRs**, while reviewer WIP counts simultaneous independent reviews; a separate bounded **ready-queue depth** counts prepared but unadmitted packets. Set actual numerical caps and cadence only through later authorized operations design; do not invent them here. Throttle when assurance capacity is exhausted; no extra review spam.

## Planner and controller cycle

1. Read fresh approved phase/version scope and source revision, Linear issues/dependencies, GitHub exact-head review/CI/merge state, reviewer capacity and holds. If a source is unavailable, label the affected decision INSUFFICIENT EVIDENCE and do not invent freshness.
2. Reconcile actual completed/superseded items first. Before closing a Linear duplicate or dropping a dependency, compare against canonical scope and any active PR references; a removed Linear link **is not** an authorized dependency change. Replan only after source/plan-authority change.
3. Classify new and changed requests with the quoted-sentence test; revoke stale admissions; derive the shortest legitimate current-milestone exit path, including unlocking prerequisites.
4. Prepare a **readiness pointer**, not a second qualification contract: obligation ID and canonical source revision, scope-class evidence, existing gate/contract reference *if one actually exists*, exclusions by reference, blockers, authority, WIP lane and closure evidence links. Do not restate independent acceptance or test oracles in competing planner prose.
5. Choose **one** primary qualified closure target and at most **one** separately authorized, non-competing preparation task. Emit close/finish/unblock/prepare/defer/HOLD decisions with owner, reason and event-based recheck. Do not treat poll-only or documentation-only status logs as delivery.
6. Re-evaluate at bounded schedule and on actual merge/closure, material new intake, gate verdict, source-owner change, security event or capacity shift. Debounce unchanged events; preserve blocker age and explicit 2-cycle tactic change/3-cycle STOP–EXECUTE ALTERNATIVE/AWAIT DECISION/PAUSE.
7. Produce a small derived **PlanningDecision** with stable decision ID, source revisions, classified candidates, disposition, named authority, reasons, previous decision link and next trigger. It is **not** an independent review receipt or PASS/HOLD verdict. An **admission proposal and qualification-contract ID/revision exist only for an actual separately authorized downstream admission request**; omit them in design-only, documentation and ordinary planning cycles.

Decision equivalence ignores observation timestamp when the authoritative inputs and decisions are unchanged. Stable tie-break uses immutable work ID. Synchronization writes use idempotency key **decision ID + target + operation**, compare source revision before write, and record a new event only on material state change. Retries must not create duplicate issues, reviews or approval claims. Historical evidence stays append-only.

## Adversarial falsification obligations

1. Dependency-free v2 appears with v1 unfinished and idle capacity: no v2 admission or unapproved preparation.
2. Two eligible items compete for one lane: an unlocking critical-path prerequisite beats an off-path ready closure item; formal protected-branch gates still hold.
3. Existing PR loses its approved parent or source/HEAD/contract revision changes: revoke readiness/admission despite sunk effort.
4. Decorative parent link or missing negative test with no pre-existing quoted criterion: classify expansion, not gap.
5. Necessary negative test already entailed by approved requirement: approve minimal verification gap through plan authority, without new behavior.
6. Merged PR and duplicate Linear issue with extra acceptance text or another active PR: preserve unmatched obligation; no false close.
7. Linear dependency is silently removed: retain canonical dependency until authorized owner revision; orphaned work loses eligibility.
8. Reviewer unavailable: throttle review lane; no invented PASS or unauthorized future preparation.
9. S-40 or another security HOLD: isolate affected surface; no readiness promotion or privileged remediation without authority.
10. Phase 005-A is in assessment: no 005-B admission, implementation or Phase 013.
11. Same evidence reobserved across cycles or retried sync: stable decision, no duplicate review/issue, no priority thrash.
12. Planner proposes omitting an acceptance clause or weakening exit criteria: plan-change gate, not admission.
13. Pure editorial canonical revision versus material owner dispute: only material authorized dispute holds; record provenance.
14. Scope expansion labeled P0 without incident evidence: do not smuggle feature work through containment.
15. Ready-queue fills while reviewer WIP is saturated: backpressure prevents backlog inflation and new speculative packages.

## Review and adoption boundary

Review this candidate independently for gap-test sufficiency, authority separation, prerequisite priority, revocation, idempotency and case falsification. The [PR #6 proposal](qualification-contract-delivery-proposal.md) remains independent and non-authoritative; no duplicate execution contract or evidence ledger is created here. No automatic controller deployment, Phase 005 admission, AWS IAM/STS/Terraform, production action, security waiver, or new program phase is authorized. If later accepted, the plan owner must explicitly choose the canonical methodology location and update navigation; this PR alone does not make it governing.
