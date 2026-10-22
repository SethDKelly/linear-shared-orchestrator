---
type: Phase 002 Project Record
title: 002-A — Project discovery start gate
description: Phase 002 project-specific start-gate assessment and discovery workstream plan.
tags: [phase-002, start-gate, planning]
sources:
  - id: phase-001-exit
    resource: ../001/001-f-exit.md
    title: Sponsor-accepted Phase 001 exit
  - id: canonical-purpose
    resource: ../../canonical/purpose/purpose-model.md
    title: Current provisional purpose model
---
# 002-A — Project discovery start gate

**Status: READY TO BEGIN PHASE 002 SUBPHASES — project start-gate recommendation; independent review pending.**

## Entry authorization
On 2026-10-22, sponsor explicitly accepted Phase 001 PASS WITH CARRY-FORWARD and authorized transition to Phase 002. This admits the [mandatory 002-A start gate](002-a-start-gate.md), not substantive candidate discovery or implementation. Phase 001 [exit evidence and carry-forwards](../001/001-f-exit.md) remain authoritative.

## Baseline and safeguards
Use [canonical purpose](../../canonical/purpose/purpose-model.md), [Phase 000 intake](../../canonical/project/intake.md), [Phase 001 needs](../001/001-b-needs.md), [purposes](../001/001-c-purposes.md), [tensions](../001/001-d-context-tensions.md), and [success cases](../001/001-e-success.md). P01–P06 are provisional purpose obligations; broad harm protection is contextual. Historical architecture (including S-81/PR #1), providers, controller, schemas, services, and integrations are non-authoritative candidate prompts only.

## Entry and uncertainty assessment

Phase 001 sponsor acceptance and independently reviewed P01–P06 purpose baseline meet entry prerequisites. Unvalidated needs, G01–G14 and unknown quantitative targets do not preclude **divergent hypotheses** if explicitly qualified. They do prevent treating any candidate as selected architecture, proving benefits, or finalizing security semantics.

## Anchoring and decomposition risks
- **High:** S-81/PR #1 portable contracts, ReviewReceipt, controller, agent/provider roles and repository policy adapter are inherited proposals, not concept boundaries. Start with user-visible purpose and counterfactuals, not module names.
- **High:** conflating approval with review outcome, provider availability with evidence sufficiency, and Linear status with canonical truth. Challenge separately against P01, P02, P03, P05 and P06.
- **High:** shared multi-repository service assumptions may hide tenant/security boundaries and local authority (P04, G05/G06/G13).
- **Medium:** bias toward the most recent TreatFlow experience; historical examples from SYNGAN and aws-backbone are not validated common requirements.
- **Medium:** feature lists, issue titles and technical nouns becoming candidate concepts by naming alone.

## Divergence strategy and breadth
Explore independent purpose-first seeds (P01–P06), affected-party and harm counterfactuals, failure situations, cross-project differences, analogy to familiar review/authorization/record-keeping constructs, and deliberately contrary decompositions (unified versus separate review/decision/progress meanings). Keep separate idea generation from evaluation; do not set an arbitrary candidate quota. A materially distinct alternative must change behavioral responsibility, authority or user mental model—not merely name or provider.

## Candidate evaluation and provenance
During divergence record tentative purpose association, user mental model, behavior sketch, source confidence, alternative boundary and unknowns; do not reject on incomplete Phase 003 details. During convergence assess purposive, user-facing, semantic, end-to-end, plausibly independent, familiar and reusable behavior and evidence of meaningful alternative decomposition. Retain only plausible hypotheses for Phase 003, not final concept authority. Record why alternatives were reframed/deferred/rejected. Do not infer proof from LLM brainstorming or stakeholder preference.

## Carry-forward allocation
| Carry-forward | Destination / trigger |
|---|---|
| G01 (provider independence/quota versus review quality), G03 (freshness), G04 (sponsor authority), G10 (Linear versus canonical truth) | 002-B seeds, 002-C alternative decomposition, 002-E convergence; recheck before retained candidate claims |
| G02, G05, G12; durable workflow, shared engine and incumbent architecture | 002-C and 002-D; challenge inherited decomposition before convergence |
| G06, G13; sensitive evidence, tenant identity and secrets | 002-D candidate harm/security challenge; later security/behavioral specification; no secrets collected |
| G07–G09; TreatFlow, aws-backbone S-40 HOLD / PR #10 historical state, SYNGAN variance | 002-D comparative counterfactuals; never reinterpret aws-backbone S-40 HOLD as cleared; verify live evidence before operational claims |
| G11; Phase 012+ orchestrator dogfooding | Deferred to Phase 012; no Phase 002 architecture dependency |
| G14; users, service levels, cost and baselines | 002-B needs and 002-E evaluation caveats; obtain empirical evidence before performance claims |
| Interviews, accessibility and downstream impact | 002-B and 002-D; revisit before favoring candidates affecting underrepresented parties |
| Privacy/retention and project authority constraints | 002-D and 002-E; block any unsafe authority assumption |

## Project-specific subphase plan and dependencies
| Subphase | Mode and purpose | Dependencies | Expected evidence / completion |
|---|---|---|---|
| 002-B — Purpose-first candidate seeds and affected-party counterfactuals | Divergent; gather independent seeds from P01–P06 and needs, without selection | 002-A | Source-qualified seed inventory; each purpose considered; harms and missing evidence explicit |
| 002-C — Materially alternative concept decompositions | Divergent; challenge unified/split boundaries, authority and evidence meaning | 002-B | At least two materially different *structures where relevant*, with rationale; no numeric quota |
| 002-D — Cross-context, harm, familiarity and anchoring challenge | Divergent/adversarial; test seeds and decompositions against privacy, local policy, historical examples and unfamiliar affected parties | 002-B; may overlap 002-C | Counterexamples, alternative inspirations and constraint register; unresolved evidence qualified |
| 002-E — Concept-likeness screening and bounded convergence | Convergent; distinguish user-facing behavioral candidates from technical fragments | 002-C and 002-D | Purpose coverage matrix; retained/deferred/reframed/rejected candidate dispositions; Phase 003 uncertainty list |
| 002-F — Canonical consolidation, independent exit and Phase 003 handoff | Exit; documentation/OKF, canonical navigation, adversarial review and sponsor decision | 002-E | Coherent provisional retained candidate baseline, independent review, explicit carry-forwards and separate exit acceptance |

**Return-to-divergence mechanism:** If 002-E identifies missing purpose coverage, an untested alternative, an affected-party omission, or evidence that changes a candidate boundary, record a numbered convergence finding and reopen the relevant 002-B seed inventory and/or 002-C decomposition and 002-D challenge records. Re-run the affected comparison and resume 002-E only after documenting its disposition. This is an iterative review loop within the existing workstreams, not a circular Linear blocking relation; 002-F remains blocked until 002-E closes all material reopened findings.

**Per-workstream boundary:** 002-B takes Phase 001 canonical purpose and needs, excludes selection, and hands off qualified seeds and uncertainties; 002-C takes B and excludes architecture or Phase 003 specification, handing off competing decompositions; 002-D takes B and cross-context cautions, excludes assertions of verified historical outcomes, and hands off harm/anchoring counterexamples; 002-E takes C and D, excludes final concept approval, and hands off provisional dispositions plus reopened questions; 002-F takes E and excludes implementation or sponsor-acceptance inference, handing off independently reviewed provisional canonical knowledge and unresolved questions.

**Dependency rationale:** B generates unconstrained evidence-qualified seeds; C and D can progress in parallel after B because C studies decomposition and D studies external constraints; E waits for both to avoid premature convergence; F independently reconciles the complete result. Separate files and distinct issue scopes minimize overlap.

## Linear planning mirror

Parent [S-95](https://linear.app/s-kelly/issue/S-95), start gate [S-107](https://linear.app/s-kelly/issue/S-107), and derived workstreams: [002-B S-123](https://linear.app/s-kelly/issue/S-123), [002-C S-124](https://linear.app/s-kelly/issue/S-124), [002-D S-125](https://linear.app/s-kelly/issue/S-125), [002-E S-126](https://linear.app/s-kelly/issue/S-126), [002-F S-127](https://linear.app/s-kelly/issue/S-127). Blocking relations mirror B → C/D → E → F. The repository remains the design authority.

## Documentation and Phase 003 handoff
Use project-specific `docs/phases/002/002-b-*.md` through `002-f-*.md` as phase evidence. The [canonical purpose model](../../canonical/purpose/purpose-model.md) stays authoritative for purpose. Promote only stable retained semantic candidates into provisional canonical concept knowledge; rejected seeds stay in phase records. Update Phase 002 and canonical indexes only for actual promoted knowledge. Phase 003 must receive candidate-to-purpose associations, behavior/mental-model sketches, alternative decomposition history, provisional boundaries, provenance and explicit unresolved specification questions. Reopen Phase 001 if a purpose proves defective.

## Start-gate decision and boundaries

**READY TO BEGIN PHASE 002 SUBPHASES (recommended).** Planned B–F workstreams and dependency sequence above satisfy the 002-A planning contract. This is a project start-gate readiness recommendation, not Phase 002 exit, concept approval, or implementation approval. Independent review of this new exact head is requested before treating the plan as review-cleared. Linear issues are the planning mirror, not canonical design authority.
