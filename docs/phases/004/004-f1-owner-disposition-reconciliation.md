---
type: Phase Design Record
title: 004-F1 — Provisional Owner and Candidate-Disposition Reconciliation
description: Source-linked Phase 004-F1 owner/disposition candidate; no final factoring or Phase 004 exit.
tags: [phase-004, reconciliation, provisional, owner-disposition, review-candidate]
sources:
  - id: plan
    resource: 004-a-project-start-gate.md
    title: Accepted Phase 004 workstream and return routes
  - id: entry
    resource: 004-f-reconciliation-entry-gate.md
    title: Admitted bounded F1 closure criteria
  - id: phase003
    resource: ../003/003-f-independent-exit-assessment.md
    title: Sponsor-accepted provisional Phase 003 concept dispositions
  - id: purpose
    resource: ../../canonical/purpose/purpose-model.md
    title: P01–P06 purpose obligations
---

# 004-F1 — Provisional owner and candidate disposition reconciliation

**Status: review candidate, not F1 PASS or Phase 004 exit.** Source baseline: merged `main` `14a4e730e78e8f1e4b248473a5b76526cd3e8451` (Phase 004-F entry PR #10). This record reconciles existing authority and explicitly avoids promoting a concept, changing behavior, or closing RD-14/RD-15. It is a *disposition inventory* rather than a new canonical specification.

## Candidate identities, disposition and accountable specification locations

| Candidate | Purpose / current disposition | Existing source of behavior or disposition | F1 reconciliation / falsifier |
| --- | --- | --- | --- |
| **C1** historical distinct civic actions / generic-case hypothesis | Comparator only; **not promoted**. The historical four-action control is distinct from a proposed generic-case algebra; neither has demonstrated source-complete collapse. | [004-D comparator and alternatives](004-d-rd14-generic-case-boundary-alternatives.md); [004-A risk inventory](004-a-project-start-gate.md) | Do not call C1 canonical or close RD-14. Proven intrinsic collapse returns **first to Phase 002-C**, without automatic C1 promotion. |
| **C2** living inquiry | **Provisional canonical specification owner**, P01/P05; not an accepted independent factoring verdict. | [C2 canonical specification](../../canonical/concepts/c2-living-inquiry.md) | Question, ground, challenge, attributed disposition, rebase and provisional answer remain distinct from authorization and completion. A challenge cannot disappear by silence. |
| **C3** scoped authorization | **Provisional canonical specification owner**, P02/P04; project-local permission, not a universal obligation-policy engine. | [C3 canonical specification](../../canonical/concepts/c3-scoped-authorization.md) | Withholding and scoped grant/withdrawal remain explicit; favorable review, external obligation assertions and completion do not grant permission. S-40 still blocks independent security activity. |
| **C4** reviewer recovery | P03 recovery **lens**, not an independently retained concept. | [Phase 003 exit disposition](../003/003-f-independent-exit-assessment.md); [004-A C4 risk](004-a-project-start-gate.md) | Silence or missing independent review remains **unknown/pending**, never implied PASS; later recovery behavior requires separate qualified owner if proposed. |
| **C5** federation | P04 cross-project authority **deferred**, not accepted. | [Phase 003 exit disposition](../003/003-f-independent-exit-assessment.md); [004-A C5 risk](004-a-project-start-gate.md) | No shared authority or cross-project admission inferred. Rediscover only on cross-project evidence demonstrating independent authority and affected-party need, as required by the Phase 003 exit and 004-B; project-specific evidence alone is insufficient. |
| **C6** change narrative | P06 narrative presentation **not retained as a standalone concept**. | [Phase 003 exit disposition](../003/003-f-independent-exit-assessment.md); [004-A C6 risk](004-a-project-start-gate.md) | Narrative cannot substitute for R-06 completion evidence; Phase 007 representation deferred. Independent authored-account evidence would require qualified rediscovery. |
| **R-06** work outcome accountability | **Provisional canonical specification owner**, P06; not independently certified against generic-case challenge. | [R-06 canonical specification](../../canonical/concepts/r06-work-outcome-accountability.md) | Request, acknowledgment, attempt, assessment, assertion and current substantiation remain separate; no new `AddressOutcomeChallenge` action is invented. RD-15 basis credibility/actor eligibility remains open. |

The [purpose model](../../canonical/purpose/purpose-model.md) supplies P01 current state, P02 bounded sponsor authorization, P03 honest blocked/pending review, P04 local authority, P05 independently challengeable findings and P06 truthful completion. **P01/P05 are jointly served by C2 but not equated**: revision-applicable observations and the ability to challenge them are separately testable. **P03 is covered by an honest pending/unknown observation across existing concepts and coordination, not an unowned automatic recovery action.** P04's local-authority obligation is protected by C3 and the separate S-40 hold; C5 is not required to supply it. P06 is behaviorally owned by R-06, not C6 prose. This is purpose-to-owner traceability, not empirical proof of sufficiency.

## Non-negotiable behavioral negative controls

1. **Challenge truth:** C2 `AddressChallenge` is an attributed inquiry-ground disposition, preserving the objection. R-06 `ChallengeOutcome` retains **NOT SUBSTANTIATED** history for unsupported objections; materially supported contradictions remain visibly **CONTESTED**; credible safety/evidence-integrity suspicion permits independent investigation and **CONTESTED — SAFETY REVIEW PENDING** with current substantiation suspended. An unresolved R-06 challenge is not forced to resolve.
2. **Completion truth:** R-06 historical substantiation remains inspectable after `InvalidateBasis` or material challenge withdraws **current** substantiation. A new revision cannot inherit old bases. No acknowledgment, attempt, favorable assessment, bare outcome claim, `verified=true`, timeout or silence establishes completed work.
3. **Permission truth:** Neither C2 provisional answer nor R-06 outcome, review PASS, missing obligation data, or an actor's mere assertion creates C3 permission. Authorization is scoped, actor-attributed and project-local; no security waiver.
4. **Boundary return:** Localized boundary edits must re-satisfy the entire Phase 003 behavioral contract inside Phase 004; material identity/behavior changes reopen Phase 003. **Demonstrated RD-14 collapse returns first to Phase 002-C**; Phase 003 reopening is not a substitute.

## Open decisions, authority and closure test

- **RD-14/E-301:** OPEN/INDETERMINATE under frozen S-135 Q4/Q5 sponsor decisions; C1 remains an unpromoted comparator. Only demonstrated source-complete intrinsic collapse returns first to Phase 002-C; no automatic C1 promotion. **E-305:** continues to govern the C1 comparator alongside the settled C4 recovery lens and deferred C5 federation disposition; each retains the distinct existing rediscovery/return triggers documented above and in 004-A/004-B. E-305 is not itself a single OPEN collapse-only decision.
- **RD-15/E-302:** concrete independently credible R-06 basis, materiality and actor eligibility remain open for a qualified policy/source owner; do not fabricate rules. C3 obligation truth is a separate boundary.
- **S-141:** P05/R-06 outcome challenge-disposition source-owner question stays explicitly separate; it is **not** a mandatory R-06 resolution action or F1 exit veto.
- **E-303/E-304/E-306, G01–G14, E-001–E-004:** remain in their existing historical destinations; F2 must reconcile exact owner/trigger/status and navigation rather than silently mark them complete. Phase 005 composition, 006 extrinsic inclusion, 007 representation, 008 reuse remain deferred; Phase 012 is endpoint.
- **S-40:** independent security HOLD; no implementation, AWS/IAM/STS/Terraform or production. S-140 eight-domain orchestration and version eligibility proposal remains **NON-AUTHORITATIVE**, for a separate methodology gate.

**F1 qualification:** Independently compare each row with linked canonical/Phase 003/004 sources. HOLD only on an unsupported owner promotion, omitted P01–P06 purpose, missing material negative control, contradictory disposition or broken authoritative source reference. A reviewer PASS WITH CARRY-FORWARD qualifies this bounded inventory, not final canonical promotion or Phase 004 exit. TPO records a separate accepted-work decision; CI/protection and review assurance are separately checked for merge readiness. Shared GitHub commit identity identifies a contributor account, not the accountable TPO, human owner or independent reviewer.
