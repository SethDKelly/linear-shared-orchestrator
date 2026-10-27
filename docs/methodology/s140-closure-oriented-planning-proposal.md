---
type: Methodology Design Proposal
title: S-140 — Closure-oriented planning, prioritization and scope conservation
description: Non-authoritative design candidate for backlog preparation, admission control and periodic reprioritization.
tags: [s-140, methodology-proposal, planning, prioritization, scope-control, review-candidate]
---

# S-140 — Closure-oriented planning and admission control

**Status:** NON-AUTHORITATIVE DESIGN PROPOSAL. This is an evaluation candidate, not a controller deployment, phase admission, methodology adoption, or new project scope. Existing phase, canonical, repository security, independent-review and sponsor authorities remain governing. [S-140](https://linear.app/s-kelly/issue/S-140) is the coordination issue; this document is a bounded candidate for further concept-design refinement.

## Design problem and desired outcome

The delivery orchestrator can execute a qualified work package yet cannot safely infer *which* backlog item should be prepared or admitted. A queue that rewards available work, review activity, or task creation can expand scope and postpone milestone closure. The proposed planning loop must preserve an approved milestone/phase plan as the authority for **what**, while periodically deciding **when**, **how to prepare**, **how much work to admit**, and **what to close**.

## Responsibility boundaries

| Responsibility | Owns | Must not do |
|---|---|---|
| Approved plan / milestone authority | Scope, objectives, exit criteria, version train, explicit plan changes | Be silently rewritten by backlog activity |
| Project Planner | Dependency and readiness analysis, in-scope gap evidence, candidate work packages, backlog disposition and closure-path proposal | Admit implementation, invent features, weaken exit criteria |
| Priority & Admission Controller | Capacity-aware ordering, WIP limits, version-train eligibility, pause/resume/defer decisions, qualified admission proposals | Promote unapproved scope or waive security/review |
| Delivery Orchestrator | Execute admitted, revision-bound qualification contracts; coordinate tests, reviews, evidence, PR closure | Treat an easy unplanned task as authority to start |
| Evidence / Replanning | Append-only observations, closure and blocker signals, provenance, re-evaluation triggers | Rewrite historical evidence or self-certify success |

Linear is the work/dependency/ownership system of record; GitHub is the source for branch, exact-head PR, review, checks and merge evidence. Canonical phase/methodology documents define accepted scope. Synchronization is idempotent and provenance-linked; no system infers a phase acceptance or approval from another system's status alone.

## Scope conservation invariant

**An active work item must trace to a current approved plan obligation, or to a documented necessary gap for fulfilling that obligation.** A gap needs: parent obligation and source revision; observable failure without the gap; minimum sufficient remediation; evidence/acceptance impact; exclusions; accountable approver; and a reviewable decision. This is **not** a license to add new features. New objectives, capabilities or materially changed acceptance criteria are **scope expansion**, requiring a separately authorized plan-change gate.

Classify intake before prioritization:
1. **Planned** — already approved; optionally split into coherent, independently closable packages without changing its behavior.
2. **Necessary in-scope gap** — demonstrably required to satisfy existing approved behavior; qualify with minimum-sufficient repair and provenance.
3. **Scope expansion** — unapproved feature, objective, version, or changed success criterion; quarantine as a proposal pending separate plan authority.
4. **Duplicate/superseded/obsolete** — link to canonical owner or completion evidence; close or archive without manufacturing replacement work.
5. **Insufficient evidence** — keep in discovery/preparation, not admitted delivery.

A security or correctness defect may require immediate containment or a HOLD even when the remediation plan is not yet admitted; it does not authorize unrelated expansion or privileged actions.

## Planner cycle: backlog to ready

At a bounded cadence and on material events:
1. Read current accepted phase/version train, exit criteria, dependency graph, Linear work status, GitHub exact-head evidence, capacity and security holds.
2. Reconcile already-closed/merged/superseded items first; detect missing source-of-truth synchronization, stale review and duplicates.
3. Identify the shortest legitimate remaining path to the current milestone exit; surface blockers, unqualified dependencies, and the smallest necessary in-scope gaps.
4. For each candidate prepare a **readiness packet**: plan/requirement link, version train, scope classification, acceptance observations, non-goals, dependency and authority gates, canonical source revision, test/review expectations, estimate/capacity class, and closure evidence.
5. Distinguish **READY FOR ADMISSION REVIEW** from **ADMITTED FOR EXECUTION**. A ready packet is never implementation authority. Future-version preparation is allowed only when separately qualified and capacity-bounded.
6. Produce a small disposition set: close now, finish active, unblock, prepare next, defer, HOLD, or propose plan change.

## Priority and admission cycle

Re-evaluate on an explicit scheduled cadence and after: PR merge/closure, gate PASS/HOLD, dependency change, security event, newly eligible work, version-train change, or material capacity change. Debounce repeated unchanged events; persist decision inputs and reason for a stable ordering.

Priority classes:
- **P0 safety/authority** — contain or HOLD affected work; remediate only with applicable authorization.
- **P1 current admitted milestone closure** — work directly needed to meet its unchanged exit criteria.
- **P2 P1 critical-path dependency** — qualified prerequisite to closing P1.
- **P3 next *approved* milestone preparation** — bounded readiness work, not automatic implementation admission.
- **P4 future version/unapproved expansion** — defer unless a separate sponsor decision authorizes a bounded exception.

Within a class, weigh closure impact, dependency criticality, readiness, evidence freshness, size/uncertainty, reviewer capacity and WIP. No opaque score may override a hard gate. A dependency-free v2 item cannot displace unfinished admitted v1 simply because it is available. Apply WIP caps per workstream and review lane, reserve capacity for remediation and independent assurance, and prefer finishing a qualified active PR over starting several new ones.

## Required decisions and audit receipts

For each cycle emit a compact, provenance-linked **PlanningDecision**:
- Plan/milestone/version and source revision; observation time; Linear and GitHub evidence snapshots; active holds.
- Candidates with scope class, parent obligation, readiness, dependency/critical path, capacity, chosen disposition and reason.
- Exact items to close, finish, unblock, prepare, defer, or request explicit scope change; owner and next recheck trigger.
- Admission proposal with qualification contract ID/revision, approval authority and remaining gate conditions.
- Previous decision linkage; record changed priorities and why. Historical receipts remain append-only; current queue order is derived state.

No change to an existing plan's scope, milestone criteria, independent review or security authority is implied by a PlanningDecision. Failure to fetch fresh authoritative state produces an explicit **INSUFFICIENT EVIDENCE / HOLD**, not speculative reprioritization.

## Concept-design falsification cases

1. Easy dependency-free v2 task appears during unfinished v1: remain P4 or bounded P3 preparation; no implementation displacement.
2. Current milestone PR becomes exact-head merge-ready: close/finish outranks starting an unrelated ready task, subject to protection gates.
3. Reviewer unavailable/quota exhausted: do not infer PASS; throttle affected lane, prepare independent non-mutating work if permitted.
4. New request lacks a parent plan obligation: scope expansion proposal, not a delivery story.
5. A missing negative test is necessary to meet an existing requirement: qualify minimum-sufficient in-scope gap with evidence, not a new feature.
6. Duplicate Linear story and merged GitHub PR: reconcile provenance and close duplicate; no new implementation.
7. A purported dependency is removed: re-evaluate critical path without expanding the milestone.
8. Security HOLD on a repo: isolate the affected work; no develop/main branch change waives it.
9. Phase 005 start gate is only under assessment: do not admit 005-B work from readiness alone.
10. Multiple priority events with unchanged evidence: idempotent decision, no thrashing or repeated review requests.
11. Planner proposes relaxing exit criteria to close faster: reject as unauthorized plan change.
12. Stale canonical revision or disputed ownership: hold admission until reconciled; preserve history.

## Refinement questions for independent design review

- Which plan/phase authority owns the approved backlog boundary when Linear issue descriptions drift?
- How are necessary gaps falsified against the original acceptance criteria without creating a perverse incentive to label expansion a gap?
- Which readiness fields are required versus optional for design-only, documentation, and implementation work?
- How do P0 containment and urgent defect remediation work without bypassing independent security and sponsor gates?
- What bounded cadence and event-debounce policy prevents churn while responding quickly to true critical-path changes?
- How should WIP/reviewer capacity and age of unresolved blockers be exposed without turning them into a superficial score?
- Which minimal canonical owner should adopt this after S-140 review, without duplicating PR #6's qualification-contract and evidence-ledger responsibilities?

## Qualification and adoption boundary

Review this proposal for missing invariants, over-specification, conceptual overlap, and adversarial counterexamples. Revise as needed. **Do not** mark this design authoritative or deploy a scheduler/controller without a separate methodology-adoption decision and the applicable downstream lifecycle gates. PR #6 remains a separate non-authoritative execution-contract proposal; Phase 005-A composition eligibility remains a separate concept-design gate.
