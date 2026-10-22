# 000-C — Actors, context and desired outcomes
Status: COMPLETED provisionally.
## Actors
Sponsor/owner: defines purpose, accepts risk, explicitly approves merges and sensitive actions. Project maintainers: own repository-specific policies and releases. Reviewers: independent evaluators with bounded scope. Delivery agents: execute scoped changes without granting their own approval. Provider operators: supply review/agent capability with variable quota and availability. Downstream users/operators of TreatFlow, SYNGAN and aws-backbone: affected indirectly by reliability, security and release quality.
## Desired improvements (stakeholder assertions)
Reusable, explainable review and delivery coordination across repositories; fewer manual status checks and lost findings; safe bounded parallel work; accurate evidence-based gates; graceful provider unavailability; lower duplicated maintenance; portable onboarding without eroding local project authority.
## Harms to avoid
Unauthorized merges, security-exit waivers, privileged AWS actions, credential leakage, stale-head acceptance, quota treated as approval, false completion, circular self-review, and review cost amplification.
## Uncertainty
Expected operators beyond the sponsor, scale, acceptable latency/cost and support model are not established. Carry into Phase 001.
