---
type: Phase 003 Project Record
title: 003-B — Candidate Identity and Operational Principles
description: Provisional concept identity tests, archetypal operational principles, rivals, and falsification criteria.
tags: [phase-003, candidate-identity, operational-principles]
sources:
  - id: phase-003-a
    resource: 003-a-project-start-gate.md
    title: Independently cleared 003-A start gate
  - id: phase-002-e
    resource: ../002/002-e-bounded-convergence.md
    title: Phase 002 candidate dispositions
  - id: purpose
    resource: ../../canonical/purpose/purpose-model.md
    title: Canonical provisional purposes
  - id: contract
    resource: concept-specification-contract.md
    title: Representation-independent specification contract
---
# 003-B — Candidate Identity and Operational Principles

**Status: IDENTITY AND OP ANALYSIS DRAFT; independent review pending. No concept promoted, rejected as final, or implementation selected.**

## Evidence posture and screening rules

This record tests C2, C3 and C6 from the [sponsor-accepted Phase 002 exit](../002/002-f-exit-assessment.md). It does not claim user interviews, real-world validation, measured adoption, independent provider verification or clearance of historical S-40 HOLD. Phase 001 [P01–P06](../../canonical/purpose/purpose-model.md) are the purpose authority. C1 is a quarantined S-81/PR #1-like control, C4 a recovery lens, and C5 a deferred federation hypothesis. An archetypal operational principle (OP) must explain **what the person can meaningfully accomplish and why**, without defining storage, APIs, UI, workflow, services or distributed orchestration. One OP is not a use-case catalog or proof of completeness.

Identity tests: a candidate has a distinct user mental model; a single coherent purpose; a recognizable before/action/after archetype; observable consequences even if the implementation changes; and a plausible ability to be specified independently. Its name is not evidence. Where purpose coverage is protective rather than intrinsic, say so. Retained here means **admitted for abstract specification challenge**, not a stable canonical identity.

## C2 — Living inquiry

**Provisional purpose:** Enable a maintainer or independent reviewer to sustain a challengeable question about whether a particular change is adequately supported by applicable observations as the change and objections evolve (P01, P05; P06 is a related outcome boundary).

**Mental model:** A question can remain open, be challenged, and be revisited with changed observations. It is not simply a case folder with a status label.

**OP C2-1 — Revising a contested answer.** A maintainer asks whether a proposed change is supported. Available observations support a provisional answer. An independent reviewer raises an objection to one observation; the inquiry now explicitly carries that unresolved challenge rather than presenting the prior answer as settled. When the change is revised, the old observations cease to justify the new revision without renewed applicability. The maintainer can distinguish what remains known, what is disputed and what requires renewed evaluation. This is a semantic sequence, not a screen flow or an evaluation engine.

**Candidate intrinsic behavior:** Maintain an answerable question and the distinction between supporting grounds, unresolved challenges and revision applicability; expose whether the answer is still justified. It must not itself grant sponsor authorization, perform a review, or claim the work completed. Whether one inquiry may cover multiple revisions is deliberately left for 003-C to test.

**Disqualifying probes:** If removing a generic container/receipt leaves no recognizable inquiry behavior, C2 is merely C1 or B07; if a change revision silently preserves a previously justified answer, P01 fails; if objections can disappear without challengeable disposition, P05 fails; if the inquiry's answer becomes permission, P02 fails. **Alternative:** C6 might communicate the same information without owning an inquiry, or C1 might separately track facts. Identity is **plausible, unproven**.

## C3 — Permissions and obligations

**Provisional purpose:** Enable an accountable actor to know which decision remains theirs, what obligations are unmet, and whether a particular bounded authorization has actually been given under the applicable project's authority (P02, P04). P03/P05 and P01 are protective constraints, not extra independent purposes.

**Mental model:** Permission is an actor's explicit scoped commitment, not a computed consequence of green checks. Unmet obligations remain visible even if a technical assessment is favorable.

**OP C3-1 — Review passes, permission remains withheld.** A review of a change returns a favorable technical assessment, while a local project obligation remains unmet and the sponsor has not authorized the change. The accountable sponsor sees the difference and withholds permission. After the obligation is addressed, the sponsor may explicitly authorize the bounded change; a subsequent materially different change cannot inherit that permission merely because it shares a project or issue. This does not decide authentication, roles, or policy machinery.

**Candidate intrinsic behavior:** Distinguish proposed/withheld/granted/withdrawn or superseded authorization as conceptual meanings, the scope and actor of an authorization, and independently unmet obligations. It must not infer authorization from review status, issue status, narrative, or provider availability. Whether obligations are part of C3 or external facts consumed abstractly is an explicit Phase 004 factoring question.

**Disqualifying probes:** If a PASS automatically grants permission, P02 fails; if shared coordination overrides a stricter local rule, P04 fails; if C3 requires a specific review receipt/provider/controller type to exist, independence fails; if it becomes an application-wide role/policy engine without a bounded actor-facing purpose, specificity fails; if an unresolved reviewer objection is reduced to a checkbox, P05 protection fails. **Alternative:** C5's local commitments might make permission intelligible without a universal permission concept; C1 may record a decision without establishing C3's independent semantics. Identity is **plausible, unproven**.

## C6 — Human-readable change narrative

**Provisional purpose:** Enable a contributor, maintainer or affected downstream party to understand what materially changed, why its claimed state is warranted, what remains disputed or incomplete, and what should be revisited (P01, P06; P05 is protective and may be intrinsic if the explanation itself supports challenge).

**Mental model:** A change has an accountable explanation that can be corrected and challenged, not merely a latest green summary or a progress dashboard.

**OP C6-1 — Correcting a misleading completion account.** A contributor reports that a review was requested and work was acknowledged. The account initially sounds complete, but an affected maintainer challenges the claim: the review has not returned and the change has not been verified. The explanation is corrected to distinguish request, attempt, acknowledgment, verification and actual completion; it preserves the challenged prior claim and explains what remains unknown. A downstream reader can understand the current account without being told that persuasive prose constitutes independent evidence.

**Candidate intrinsic behavior:** Preserve a revisable explanation of consequential changes, distinguish assertions from independently checkable grounds and explicitly unknown/disputed outcomes, and allow correction without laundering the prior claim. It must not itself create evidence, approve a change, or certify completion. Whether the narrative is intrinsically independent of C2's answer is a key open identity question.

**Disqualifying probes:** If C6 only formats C2/C3 state, it is a presentation mapping for Phase 007, not a separate concept; if unsupported prose is accepted as evidence, P01/P05 fail; if acknowledgment becomes completion, P06 fails; if confidential evidence is exposed to make a story readable, the affected-party harm boundary fails. **Alternative:** C2 could be the owner of the question and explanation; C4 could provide a recovery account without a general narrative concept. Identity is **most exposed to overlap and presentation-mapping risk**.

## Independent identity comparison

| Probe | C2 living inquiry | C3 permissions and obligations | C6 change narrative |
|---|---|---|---|
| Characteristic user question | “What do we know about this change, and can it be challenged?” | “Who may decide what, and what is still owed?” | “What happened, why does it matter, and what is still uncertain?” |
| Distinctive before/after | Justification becomes contested, revised or renewed | Authorization remains withheld, is explicitly granted or invalidated | A misleading account becomes corrected and comprehensible |
| Core meaning not borrowed | Challengeable question and applicable grounds | Scoped decision authority and obligations | Accountable explanation and correction |
| Most dangerous conflation | Evidence answer → permission | Technical PASS → sponsor authority | Narrative → evidence or completion |
| Closest alternative | C6; C1 container | C5; C1 decision record | C2; C4 recovery lens |
| Current identity disposition | **Retain provisionally for 003-C/D** | **Retain provisionally for 003-C/D** | **Conditional retention for 003-C/D**, explicitly test if merely mapping |
| Independent concept established? | No | No | No |

**No forced fusion:** C2's justified answer, C3's explicit permission, and C6's corrected explanation could coexist, but none may automatically trigger another. If C6 cannot explain a distinct user-facing semantic action beyond restating C2, 003-E must reject standalone ownership or return to discovery rather than invent an artificial state. If C3's obligation tracking is too broad, 003-E must separate authority from obligations without assuming a policy engine.

## P01–P06 and affected-party challenge matrix

| Purpose | Positive probe | Required negative counterexample / affected party |
|---|---|---|
| P01 | C2 applicable grounds; C6 evidence-qualified explanation; C3 cannot obscure freshness | Maintainer misled by stale exact-head review after revision |
| P02 | C3 explicit scoped sponsor decision, visible separately from C2/C6 | Sponsor is bypassed by favorable evaluation or narrative |
| P03 | C2/C3/C6 represent unavailable review as unresolved, C4 recovery lens | Operator mistakes quota exhaustion or silence for clearance |
| P04 | C3's permission is constrained by project-local authority; C5 comparator | Local security owner loses stricter project gate |
| P05 | C2 contestable grounds; C6 correctable claims; C3 cannot erase objections | Independent reviewer sees a finding silently closed or reclassified |
| P06 | C6 explains actual outcome vs request/attempt; C2 must not claim completion | Contributor or downstream user sees acknowledgment presented as completion |

Cross-cutting affected parties include evidence subjects (privacy, access, retention), asynchronous and accessibility-constrained users, independent reviewers, sponsors, project security owners, operators, and downstream consumers. These harms are **not** evidence that P07 exists. Empirical interviews, security and cost baselines, provider independence, and cross-project identity remain open. No scenario is an observed study.

## Numbered findings, decisions and return triggers

- **B-001 (C2 vs C1):** The inquiry must have a semantic contest/revision behavior independent of a container or review receipt. **Disposition:** retain provisionally, require 003-C minimal-state test; return to 002-C if no such behavior survives.
- **B-002 (C3 specificity):** Permission is meaningful; “obligations” may create an overloaded policy concept. **Disposition:** retain provisionally; 003-C must test whether obligations are intrinsic or an abstract input, and 003-D must preserve P02/P04.
- **B-003 (C6 vs C2 / Phase 007):** Narrative may be merely a representation of inquiry. **Disposition:** conditional retention only; 003-C must identify independent semantic memory/action or recommend no standalone concept, and 003-D must test persuasive-prose harm.
- **B-004 (authority separation):** No candidate may infer permission from evidence, reviewer response, progress or narration. **Disposition:** explicit cross-candidate disqualifier, not a synchronization design.
- **B-005 (recovery and federation):** C4 remains a bounded recovery lens; C5 remains deferred pending cross-project evidence; neither silently promoted. **Disposition:** revisit 002-C/002-D only if independent user-facing behavior or new affected-party evidence materially changes the decomposition.
- **B-006 (evidence limitations):** G01–G14, E-001–E-004, S-40 HOLD, missing stakeholder interviews, accessibility, privacy/retention, and quantitative baselines remain unverified. **Disposition:** hand to 003-D and later validation; no inferred clearance.

## 003-C / 003-D conditional handoff

**003-C abstract behavior specification:** For C2 and C3, and **C6 only as a falsifiable independent-identity test**, derive minimum necessary abstract memory, meaningful actions, guards/effects, conceptual history and query semantics. If C6's entire behavior is a pure rendering of C2, record that result instead of manufacturing state. Test C3 obligation/permission split. No schema, API, UI, storage, provider, workflow or inter-concept synchronization.

**003-D independent adversarial evaluation:** Challenge all six purposes, sponsor/local authority, independent reviewer objections, exact-head freshness, nonresponse and interrupted work, privacy/accessibility/evidence-subject harm, historical S-40 HOLD and cross-project claims. Specifically attempt to falsify C2's inquiry independence, C3's boundedness and C6's non-mapping identity. Maintain separate evidence ownership; 003-C and 003-D may proceed in parallel only after **independent 003-B PASS**.

**Proposed 003-B verdict: READY FOR INDEPENDENT REVIEW.** Candidate identities remain *provisional*, and none has been canonicalized. Any review HOLD blocks both 003-C and 003-D. Phase 003 exit, PR #2 merge, implementation and sponsor concept selection remain unauthorized.
