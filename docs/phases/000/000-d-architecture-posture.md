# 000-D — Architecture inheritance and neutrality
Status: COMPLETED as inventory, not architecture approval.
## Existing proposals
Linear as work/dependency tracker; GitHub as source/review/CI provenance; shared coordinator for provider selection, review reconciliation and evidence; repository adapters for local policies; shadow-mode migration; deterministic replay and exact-head binding.
## Classification
External or sponsor-mandated controls: explicit merge authorization; no unauthorized AWS/Terraform apply; no security-exit waiver; per-repository privilege boundaries. Existing behavior: TreatFlow controller/review flows and aws-backbone verification gates, subject to exact-code inspection. Proposals: ReviewReceipt, ReviewEnvelope, DecisionReceipt, schemas, shared dispatcher, randomized provider selection, repository extraction and orchestration runtime. Unknown: stable interfaces, tenancy model, failure recovery, audit retention, provider independence criteria, and authority of future status writes.
## Gap rule
Each future design phase must map proposed architecture to purpose, semantics, authority and failure cases. Missing justification is a gap, not implicit approval. S-81 draft PR #1 remains noncanonical architecture until reviewed after appropriate concept-design gates.
