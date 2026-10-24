---
type: Non-Authoritative Methodology Proposal
title: Qualification-Contract-Governed Agentic Implementation and Independent Verification (Proposal)
description: Proposed downstream engineering method for shared meaning, bounded delegation, focused PRs, evidence provenance, and independent final verification; not implementation admission.
tags: [proposal, qualification-contract, agentic-delivery, verification, review, downstream]
sources:
  - id: lifecycle
    resource: phase-lifecycle.md
    title: Phase lifecycle and admission gates
  - id: agent-governance
    resource: agentic-development-governance.md
    title: Shared agentic development governance
  - id: design-only
    resource: design-only-guardrails.md
    title: Design-only guardrails and downstream execution boundary
  - id: knowledge-authority
    resource: knowledge-authority.md
    title: Current versus provisional knowledge authority
---

# Qualification-contract-governed delivery — proposal, not an adopted process

**Authority and lifecycle:** This is a review candidate for a *separately authorized downstream engineering process*. It is not current methodology authority, a Phase 004 concept-boundary decision, an implementation admission, or a change to Phase 011/012 readiness rules. Phases 000–011 remain design-only. Phase 012 is pre-implementation preparation and does not authorize feature implementation. Any adoption requires a separately qualified decision after applicable lifecycle gates; no Phase 013 is part of the currently authorized program. The [existing agentic governance](agentic-development-governance.md), [phase lifecycle](phase-lifecycle.md), and [design-only guardrails](design-only-guardrails.md) remain governing. **This PR's review does not supersede them.** Only a later, separately qualified and explicitly authorized methodology-adoption decision can replace any of those contracts.

## Principle and gate-scoped shared reference

**A shared definition is a shared meaning. Define together; build independently; verify independently; reconcile against the shared definition.**

For each admitted downstream implementation gate, one **approved, versioned qualification contract** is the central organizing artifact. It describes *what* behavior is authorized, what is excluded, and what independent evidence will qualify completion. It does not prescribe implementation mechanisms where the source design leaves them open. The contract is derived from current canonical knowledge and must cite its owner revisions; it cannot silently rewrite concepts or bypass protected human authority. **Canonical concept and methodology owners outrank the gate-scoped qualification contract.** Under the [knowledge-authority hierarchy](knowledge-authority.md), a conflicting contract is invalid for execution until its source owner is changed through the authorized concept-design lifecycle and the gate is requalified. Contract requalification alone cannot revise or replace a canonical owner. The contract is the shared *reference*, not an assumption that reviewers must agree with it: independent agents must be able to challenge contradictions, missing cases, or unsafe criteria.

### Minimum qualification contract

| Field | Obligation |
|---|---|
| Identity and provenance | Stable contract ID, version/revision and immutable digest, gate ID, canonical owner links and source revisions, accountable approver and admission date. |
| Intent and boundaries | One coherent build purpose, in-scope and out-of-scope behaviors, explicit non-behaviors, protected authority, dependencies, unresolved assumptions and non-goals. |
| Behavioral semantics | Inputs/outputs, state transitions, invariants, guards, failures, unknown states, revision/history semantics, interfaces and observable outcomes; distinguish concept meaning from architecture choices. |
| Verification obligations | Traceable positive, negative, boundary, adversarial, integration and regression obligations, plus security/accessibility/privacy checks when applicable. Define expected observations and unacceptable false positives. |
| Delegation contract | Named owners of implementation, independent test design, integration/CI/fixtures, documentation and gate adjudication; interface handoffs, shared fixtures and branch ownership. Shared fixtures, expected outcomes and test oracles must be derived from the approved contract and canonical owner sources, never implementation internals; an integration agent cannot silently redefine the oracle. |
| Exit evidence | Required CI/checks, coverage evidence, independent reviewer identities and scopes, evidence-ledger links, release/rollback concerns if relevant, exact candidate SHA, and explicit PASS / PASS WITH CARRY-FORWARD / HOLD decision authority, including which obligations may not be carried. |
| Change control | Which changes are editorial versus material, who can requalify a revision, which downstream artifacts must be refreshed, and how invalidated reviews/tests are marked. |

A contract revision is **not** an approved revision merely because a coding agent changes it. If meaning, guards, exclusions, acceptance behavior, security boundaries or test obligations change, stop affected work, seek owner clarification and requalify before proceeding. An editorial correction may avoid reopening semantics but must still receive the exact-head reviews required by the applicable merge policy.

## Gate-aligned execution and delegation

1. **Qualification entry:** Verify prerequisites, scope, canonical source versions, exclusions, measurable observations, test obligations, authority, risks, and review plan. Outcome: admitted contract revision or HOLD. An unqualified work item is preparation only.
2. **Parallel bounded workstreams (future process only, after separate downstream implementation admission):** An implementation agent realizes only admitted behavior. A separate test-design agent derives cases directly from the approved contract, including adversarial and negative controls, without relying on implementation internals as its oracle. An integration agent prepares compatible fixtures, interfaces, checks and dependency wiring. A documentation agent maintains traceability and expected operational handoff. Workstream owners must use the **same contract ID and revision** and must declare deviations, not silently resolve semantic disagreements.
3. **Iteration within one focused PR/gate:** Prefer one primary qualified behavior package per PR, with clear exclusions and a stable interface. During iteration use fast local checks, static analysis, focused unit tests and targeted reviewer questions. These are diagnostic, **not** substitutes for independent gate reviews. Do not defer known blocking security/correctness findings.
4. **Integration candidate freeze:** Reconcile workstreams and test obligations, run required CI and relevant unit/integration suites, check contract-to-code and contract-to-test coverage, freeze an immutable candidate SHA and ledger snapshot. Any uncovered obligation is explicit HOLD or authorized carry-forward, never implied PASS.
5. **Independent final verification:** Cursor and Codex independently review the exact frozen HEAD with explicit scopes (deep code, architecture, security, semantics as qualified). Independent testing executes behavioral, adversarial, integration and regression cases with evidence; test authors and implementers cannot self-certify the gate. A Codex automated code-review receipt is not automatically independent semantic approval. Reviewers may challenge the qualification contract itself.
6. **Reconciliation and exit:** Triage each finding by severity, correct defects in coherent batches, invalidate affected evidence on HEAD or contract changes, re-freeze and repeat required exact-head reviews and tests. PASS or PASS WITH CARRY-FORWARD requires all mandatory gates, required independent approvals, branch protections and CI; otherwise HOLD. **PASS WITH CARRY-FORWARD is permissible only for explicitly authorized nonblocking obligations with an owner, trigger and due gate; blocking security or correctness findings, protected human authority, the S-40 security HOLD, and unresolved C2/C3/R-06 boundary authority cannot be carried forward to authorize execution or merge.** Merge only with existing authorization and verified exact HEAD, then synchronize Linear, documentation and the next admitted gate.

## Stable, auditable review-evidence ledger

Use **one gate-scoped evidence ledger per gate**, not a competing canonical-knowledge owner or independent prose timelines duplicated across documents. **Historical review, test, HOLD, finding, invalidation, supersession and requalification events MUST be immutable and append-only.** Record a correction or invalidation as a new event citing the earlier event/evidence; never overwrite or delete the historical event. A replaceable current-state summary is a derived convenience, **not** independent review evidence or an authoritative verdict. Never retroactively assign a previous SHA's PASS to a newer SHA. The future authorized implementation must separately choose and enforce the storage/immutability mechanism; this proposal does not grant that authority.

Minimum event fields: timestamp, gate and contract revision/digest, commit SHA, review or test identity, reviewer/agent and independence role, reviewed scope, tool and evidence link, PASS/PASS WITH CARRY-FORWARD/HOLD or diagnostic-only outcome, finding IDs/severity, remediation SHA, superseded/invalidated evidence, carry-forward owner/trigger, and gate decision authority. Keep exact-head evidence separate from source-design acceptance and from PR mergeability. Ledger changes must not themselves imply a new independent verdict.

**Review batching rule:** Batch coherent changes at a meaningful candidate boundary and request deep exact-head reviews after freeze. Cheap checks can run frequently; a material semantic change or finding with security consequences is handled immediately. Avoid repeated provenance-only commit/review loops by maintaining the ledger as the review record and updating navigational summaries at controlled checkpoints. If repository policy requires a new exact-head review after a ledger-only commit, comply rather than transferring an older verdict.

## Parallelism without authority leakage

**Parallel preparation of implementation contracts, test plans, architecture sketches or fixtures is a proposed capability for a future separately admitted downstream process only. It is not admitted during Phases 000–012.** Within the current phases, only explicitly gate-qualified concept-design and non-authoritative methodology-proposal work is permitted. No agent may begin feature implementation before separately authorized downstream execution admission; a prepared contract, test plan or architecture sketch is not admission. Agents must not alter provisional [C2 living inquiry](../canonical/concepts/c2-living-inquiry.md), [C3 scoped authorization](../canonical/concepts/c3-scoped-authorization.md), or [R-06 work-outcome accountability](../canonical/concepts/r06-work-outcome-accountability.md) boundaries; synthesize missing R-06 challenge disposition; invent the concrete **RD-15 unverifiable-basis input** and actor-eligibility outcomes described in [003-F E-302](../phases/003/003-f-independent-exit-assessment.md); bypass the historical [S-40 security HOLD](../phases/003/003-d-r06-completion-adversarial-return.md) ([live Linear gate](https://linear.app/s-kelly/issue/S-40)); or infer AWS/IAM authorization from a design or PR approval. Contract-driven downstream engineering remains subject to those canonical owners and any later supersession.

**Adoption tests for this proposal:** independently review that the proposed gate is unambiguous, contract versions can be traced to source owners, reviewers can identify invalidated evidence, parallel test design remains independent, the final review is exact-head, and no process text grants unauthorized implementation or protected actions. Any downstream process must separately decide the exact enforcement mechanisms and ownership before this proposal becomes authoritative.
