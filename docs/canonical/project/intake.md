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
