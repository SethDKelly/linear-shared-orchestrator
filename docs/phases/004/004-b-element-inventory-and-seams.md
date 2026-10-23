---
type: Phase Design Record
title: 004-B — Purpose, Behavioral Element Inventory and Seam Classification
description: Bounded inventory and preliminary ownership classification of Phase 003 concepts; no modularity or boundary verdict.
tags: [phase-004, modularity, inventory, seam-classification, provisional]
sources:
  - id: phase-004-entry
    resource: 004-a-project-start-gate.md
    title: Independently reviewed 004-A plan
  - id: canonical-purpose
    resource: ../../canonical/purpose/purpose-model.md
    title: Canonical purpose model
  - id: phase-003-behavior
    resource: ../003/003-c-abstract-behavior-specifications.md
    title: C2 and C3 abstract behavior
  - id: r06-behavior
    resource: ../003/003-c-r06-completion-behavior-return.md
    title: R-06 abstract behavior
---

# 004-B — Purpose, Element Inventory and Seam Classification

**Status: in progress; no independent verdict.** The 004-A exact-head review at `5f5b355` permits 004-B inventory and seam classification only. It does **not** admit 004-C, decide completeness, close RD-14, promote C1 or finalize boundaries.

## Scope and recording discipline

The [canonical purpose model](../../canonical/purpose/purpose-model.md) and [Phase 003-F handoff](../003/003-f-independent-exit-assessment.md) are the current inputs. The tables below enumerate named state, action, guard, query, output and invariants at the level currently visible in canonical owners. Each grouped row is an **index to the individual elements named in that row**, not evidence that each element has already been independently challenged. Missing intrinsic semantics must be recorded as **unknown**, not invented.

Seam classes: **I** intrinsic to the current concept hypothesis; **S** potential Phase 005 synchronization; **X** extrinsic Phase 006 inclusion/dependence; **U** unresolved ownership. These are preliminary classifications for challenge, not authoritative modularity decisions.

## Purpose and candidate disposition inventory

| Purpose | Incoming behavior / candidate | Preliminary question and status |
|---|---|---|
| P01 | C2 inquiry | Does unsettled inquiry deliver independent value apart from P05 contested-ground correction? **U** |
| P02 | C3 scoped authorization | Permission must be explicit, local, scoped and revocable; obligation claims remain external **I / S** |
| P03 | C4 recovery lens, no promoted standalone owner | Which intrinsic C2/C3/R-06 correction actions cover recovery, and what residual purpose remains unowned? **U** |
| P04 | C3 local scope; C5 federation deferred | Cross-project permission must not be inferred from local permission. **I / X**, C5 deferred |
| P05 | C2 challenged grounds, rebase and query | Distinguish from P01; contested ground is not settled. **U** |
| P06 | R-06 outcome accountability; C6 narrative unpromoted | Work outcome is not a narrative or proof of execution; representation deferred to Phase 007 **I / S** |

C1 generic case remains a **non-promoted comparator** under RD-14/E-301/E-305; no collapse or distinctness verdict is made. C4 is a recovery lens, C5 deferred federation, and C6 not retained as a standalone concept. E-305 governs these dispositions. E-306 forbids treating Phase 005 synchronization, Phase 007 representation or security validation as intrinsic actions.

## Element inventory: C2 living inquiry

| Element(s) from canonical owner | Kind | Preliminary owner / seam | Open challenge |
|---|---|---|---|
| Inquiry identity, current revision, inquiry question, grounds and their applicability, challenges, answer proposals, historical record | State / inputs / history | C2 **I**; ground source **U** | P01/P05 separability; revision-qualified ground credibility |
| OpenInquiry | Action / existence guard | C2 **I** | Creation does not imply settled ground |
| OfferGround | Action / proposed ground input | C2 **I**; external ground origin **U** | Ground authority/credibility is not established by offering |
| ChallengeGround | Action / contested-ground effect | C2 **I** | Challenge must remain visible |
| AddressChallenge | Action / resolution attempt | C2 **I** | No silent challenge erasure |
| RebaseInquiry | Action / new revision and applicability effect | C2 **I** | New revision invalidates inherited applicability |
| ProposeAnswer | Action / unsettled answer | C2 **I** | Answer does not authorize or prove execution |
| InspectInquiry | Query / result | C2 **I** | Expose unresolved challenges and revision context |
| Contested ground never silently settled; history preserved; answer not permission or completion | Invariants | C2 **I**; C3/R-06 **S** only if application synchronizes | No cross-concept authority implied |

## Element inventory: C3 scoped authorization

| Element(s) from canonical owner | Kind | Preliminary owner / seam | Open challenge |
|---|---|---|---|
| DecisionScope, Actor, Authorization, ObligationClaim, EvidenceClaim; revision and permission applicability | State / abstract inputs | C3 permission **I**; obligation/evidence claims **U / S** | Claims are not an intrinsic obligation lifecycle |
| ConsiderScope | Action / scope consideration | C3 **I** | Consideration is not permission |
| Withhold | Action / no permission effect | C3 **I** | Favorable review does not override withholding |
| Authorize | Action / project-local authority predicate guard | C3 **I** | Actor eligibility and scope must not be inferred from reviewer PASS |
| Withdraw | Action / revoke permission effect | C3 **I** | Changed scope loses inherited applicability |
| InspectPermission | Query / result | C3 **I** | Silence, issue status and narrative are not permission |
| Permission requires explicit authority; scope changes invalidate inherited permission; S-40 HOLD | Invariants / external authority | C3 **I**; external security authority **U** | No AWS authorization; no obligation/receipt substitution |

## Element inventory: R-06 work outcome accountability

| Element(s) from canonical owner | Kind | Preliminary owner / seam | Open challenge |
|---|---|---|---|
| Work request, subject revision, acknowledgment, attempt, evaluation, outcome assertion, supporting basis, substantiation, challenges and historical record | State / abstract inputs / history | R-06 **I**; basis source and actor eligibility **U** | RD-15: basis independently credible and attributable? |
| RequestWork | Action / request existence guard | R-06 **I** | No attempt or completion inferred |
| AcknowledgeWork | Action | R-06 **I** | Acknowledgment is not attempt |
| RecordAttempt | Action | R-06 **I** | Attempt is not outcome |
| RecordEvaluation | Action | R-06 **I** | Favorable evaluation is not completion |
| AssertOutcome | Action | R-06 **I** | Assertion is not substantiation |
| OfferBasis | Action / supporting basis input | R-06 **I**; external basis source **U** | Basis credibility not presumed |
| ChallengeOutcome | Action / contestation | R-06 **I** | Preserve unresolved disqualifying challenge |
| AddressOutcomeChallenge | Action / challenge handling | R-06 **I** | No silent proof creation |
| SubstantiateOutcome | Action / same-revision attributable basis and no unresolved disqualifying challenge guard | R-06 **I**; basis credibility **U** | `verified=true` is not proof |
| InspectOutcome | Query / result | R-06 **I** | Preserve six independent facts and historical challenge |
| Acknowledgment/attempt/evaluation/assertion/substantiation are distinct; revision freshness; contradictions contested; S-40 HOLD | Invariants / history | R-06 **I** | New revision loses inherited applicability even if called immaterial |

## Cross-boundary seam classification (preliminary)

| Interaction pressure | Class | Rationale / next challenge |
|---|---|---|
| C2 grounds as an abstract input to R-06 outcome basis | **U / S** | Ground credibility is not automatically inherited; determine whether this is only a Phase 005 synchronization or an unowned intrinsic basis rule in RD-15 |
| C3 permission versus R-06 attempt/completion | **S** | Permission and accountable outcome remain different facts; a possible Phase 005 interaction must not imply either from the other |
| C3 obligation claims versus authorization | **U / S** | C3 has no obligation lifecycle; E-302 must not be confused with RD-15 |
| P03 reviewer recovery across C2 challenge, C3 withdrawal and R-06 correction | **U / S** | Recovery lens is not automatically a standalone concept; trace residual uncovered P03 |
| P04 cross-project federation versus local C3 permission | **X / U** | C5 remains deferred absent evidence; no cross-project authority assumption |
| P06 C6 narrative presentation of R-06 facts | **S** (representation deferred) | Phase 007 owns presentation; no standalone C6 promotion |
| C1 generic case versus C2/R-06 | **U** | RD-14 stays open until RD-15 basis/actor survival test; actual collapse returns to Phase 002-C |

## Required hypothesis and evidence queue (not decisions)

| Pressure | Alternatives to challenge | Discriminating evidence required |
|---|---|---|
| C2 P01/P05 | Retain; split contested-ground handling; generalize to C1 | Counterexample of valuable inquiry without challenge and challenge without independent inquiry |
| R-06 versus C1 | Retain; merge into generic case; reframe outcome basis | RD-15 credible-basis and actor-eligibility survival plus counterexample showing intrinsic outcome distinctions |
| C3 obligation/evidence claims | Retain external claims; split obligation owner; reduce C3 to permission | Demonstrate whether obligation semantics are actually intrinsic to permission |
| P03 C4 lens | Retain lens; generalize correction; introduce owner only with independent purpose evidence | Recovery scenario unfulfilled by C2/C3/R-06 intrinsic actions |
| C5 federation | Defer; revisit only on cross-project evidence | Independent authority and affected-party need; no assumption of adoption |
| C6 narrative | Defer to Phase 007; reopen only with independently authored account evidence | Distinct value beyond representation of R-06 facts |

## Exit conditions for this bounded 004-B record

Before any 004-C work: verify every named element against the full canonical sources and record any omitted guard/effect explicitly; independently challenge seam classifications and P01/P05/P03 coverage; preserve RD-14 open pending RD-15; obtain **fresh exact-head independent review** and reconcile its verdict. A PASS on this inventory is not a completeness or modularity PASS. G01–G14, E-001–E-004 and E-301–E-306 remain open. S-40 HOLD is unchanged. No implementation or AWS activity is authorized.
