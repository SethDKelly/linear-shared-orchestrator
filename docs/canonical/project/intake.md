---
type: Canonical Project Intake
title: Shared Agentic Delivery and Review Orchestration — Intake
description: Current provisional project framing and uncertainties, reconciled from Phase 000.
tags: [canonical, intake, shared-orchestration]
---
# Shared Agentic Delivery & Review Orchestration
## Contemplated capability
A reusable cross-repository capability for coordinating bounded agentic delivery and independent review while preserving exact-source evidence, project-specific policy authority, explicit sponsor authorization and explainable decisions.
## Motivation
TreatFlow and aws-backbone review cycles reveal duplicated coordination, stale-head risks, inconsistent provider availability, cumulative-finding reconciliation needs and complex approval boundaries. SYNGAN is the next intended consumer.
## Affected parties
Sponsor, maintainers, delivery agents, independent reviewers, service/provider operators, and downstream users of adopting repositories.
## Intended outcomes
Reliable, auditable, low-friction cross-repository delivery/review coordination; safe recovery from unavailable reviewers; preserved local security/release authority; portable onboarding.
## Boundaries
No automatic merge, security-exit waiver, AWS/Terraform apply, credential sharing or promotion of unavailable/quota-blocked reviews to approval. TreatFlow remains unblocked and current controller authoritative pending separate migration approval. aws-backbone retains infrastructure authority. Base integration of Linear/orchestrator is deferred until the orchestrator is completed and dogfooding validates the pattern.
## Evidence and uncertainty
Prior conversations are attributed stakeholder/history context, not runtime verification. S-81 PR #1 and shared architecture are proposals. Current gaps G01–G14 are tracked in docs/phases/000/000-f-gaps.md. Concept decomposition, API schemas, persistence, provider selection and runtime architecture remain open.

## Evidence classifications
- **Stakeholder assertions:** desired cross-project reuse; TreatFlow as proving ground; SYNGAN as next intended consumer; human sponsor approval preference.
- **Observed repository evidence:** [draft PR #1](https://github.com/SethDKelly/linear-shared-orchestrator/pull/1) proposes contract shapes; [draft PR #2](https://github.com/SethDKelly/linear-shared-orchestrator/pull/2) contains intake records. Neither is an accepted architecture.
- **Planning evidence:** [Linear P-S-3](https://linear.app/s-kelly/project/shared-agentic-delivery-and-review-orchestration-3be70452c5e3), [S-81](https://linear.app/s-kelly/issue/S-81)–[S-85](https://linear.app/s-kelly/issue/S-85).
- **External constraints requiring verification:** platform permissions, provider APIs and review policy, security requirements and any regulatory obligations.
- **Assumptions:** shared coordination can reduce duplicated work; repository policies can remain autonomous; provider evidence can be compared. These are hypotheses for later phases.
- **Proposals:** exact-head receipt formats, dispatcher, policy adapter, randomized provider selection and shadow mode are not approved design commitments.
- **Current open questions:** [G01–G14 gap register](../../phases/000/000-f-gaps.md), including operator needs, independence, security, retention, reliability and costs.
- **Historical evidence caution:** TreatFlow qualification is not established complete; aws-backbone PR #10 status is unverified; S-40 is a distinct HOLD/security-exit track.
