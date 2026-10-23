---
type: Canonical Concept Specification
title: C3 — Scoped Authorization (Provisional)
description: Current explicit permission semantics with project-local authority and external obligation claims.
tags: [canonical, concept, provisional, c3, phase-004]
sources:
  - id: identity
    resource: ../../phases/003/003-b-candidate-identity-operational-principles.md
    title: C3 operational principle
  - id: behavior
    resource: ../../phases/003/003-c-abstract-behavior-specifications.md
    title: C3 state and actions
  - id: reconciliation
    resource: ../../phases/003/003-e-behavioral-reconciliation.md
    title: Scoped permission reconciliation
---
# C3 — Scoped authorization

**Authority:** Provisional canonical owner of current C3 permission behavior; Phase 004 may **revise, split, merge, generalize or reject** it. This owner does not grant any actual sponsor or project authorization.

## Purpose and operational principle
P02/P04: an accountable actor distinguishes explicit bounded permission from favorable review and sees asserted unmet obligations without confusing them with authorization. **OP C3-1:** Technical review passes but local obligations remain unmet, so sponsor withholds authorization; later the sponsor may authorize a specific bounded scope, which a materially different scope cannot inherit.

## Abstract identity and memory
Parameters: DecisionScope, Actor, Authorization, ObligationClaim, EvidenceClaim. For each scope retain explicit actor-attributed authorizations, validity/supersession, withholdings and withdrawals; optionally retain references to externally asserted obligation claims if needed to explain the decision. No intrinsic obligation-management lifecycle, universal policy catalog, identity provider or shared policy engine.

## Conceptual actions
- **ConsiderScope(scope, obligations):** present decision scope and external obligation assertions; no permission is created.
- **Withhold(scope, actor, rationale):** explicitly record permission withheld.
- **Authorize(scope, actor, basis):** record explicit actor-attributed authorization exactly for scope, guarded by a project-local authority predicate.
- **Withdraw(scope, actor, authorization):** revoke/supersede an applicable prior permission under the authority guard.
- **InspectPermission(scope):** expose current explicit authorization, scope, actor and unresolved external obligation assertions, never transform assertions into approval.

Initially no permission; silence and missing authorization do not grant it. Review PASS, issue status, narrative and favorable outcome do not imply permission. Scope changes remove inherited applicability. History of withdrawal is preserved without current permission. Exact actor eligibility and local policy rules remain unverified abstract guards, not algorithms. Obligation truth is separate from a decision-maker's permission; their relation is deliberately not universally resolved.

## Boundaries and required challenges
C2's evidence answer and R-06's substantiated completion never automatically authorize. Project-local security can still block an action; **S-40 HOLD remains**. Phase 004 must test whether scoped permission warrants an independent concept and whether obligation claims should be factored elsewhere. No merge, release, implementation, cross-project authority or provider architecture is authorized.
