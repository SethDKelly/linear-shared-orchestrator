# S-81 — Portable orchestration contract baseline

Status: design-only proposal; not an active enforcement controller.

## Authorities and isolation

- Linear owns work identity, dependencies, and eligibility; GitHub owns commit/PR/CI evidence and protected merge controls.
- Repository policies own authorization, security-exit gates, required checks, and release gates. Shared logic cannot weaken them.
- Every evaluation is scoped by installation/repository, PR number, exact head SHA, policy version, and execution attempt.
- Never share credentials, caches, or provider tokens across repositories. Default to read-only access.
- TreatFlow remains operational during shadow validation; aws-backbone stays read-only; SYNGAN is the next onboarding target.

## Proposed versioned contracts

1. **ReviewRequest**: repository identity, PR, base/head SHA, diff fingerprint, policy version, review class, dispatch attempt, provider constraints, and expiry.
2. **ProviderStatus**: provider identity, capabilities, availability, quota/rate-limit state, retry eligibility, and observation timestamp.
3. **ReviewReceipt**: request identity, provider, reviewer independence, observed SHA, findings, verdict (PASS/HOLD/INSUFFICIENT_EVIDENCE), provenance, and evidence timestamp.
4. **FindingLedger**: stable finding identity, original report, affected scope, remediation commit, disposition, and independent verification; no automatic clearing from comment resolution.
5. **EvidenceEnvelope**: exact-head CI results, immutable source links, checksums, qualification and freshness, with explicit missing/invalid states.
6. **RepositoryPolicy**: required providers/checks, fallback strategy, privilege boundaries, security-exit requirements, and explicit sponsor approval class.
7. **DecisionReceipt**: input fingerprints, policy version, provider selection reason, cumulative finding reconciliation, decision, and audit trail.

## Decision invariants

- Quota exhaustion, timeout, unavailable reviewers, stale head, missing CI, or ambiguous provenance never become approval.
- Bugbot can be the default Cursor review provider; targeted @cursoragent and Codex are separate independently qualified options. Switching/randomization is deterministic from an auditable seed and eligible-provider set; never select an unavailable provider as a passing result.
- Re-review is required after material head changes; previously resolved findings remain traceable.
- A shared PASS is advisory and never authorizes merge, deployment, Terraform apply, privileged AWS access, or security-exit acceptance.
- Shadow mode must not write to PR state, trigger providers, or mutate Linear status; compare decisions only.

## Implementation boundaries

Initial implementation: pure policy evaluation, schema validation, deterministic replay, and read-only fixtures. Defer live dispatch, credentials, persistent orchestration, automated cutover, and privileged actions until independently reviewed.

## Qualification scenarios

- Exact-head review PASS with current CI and separately recorded sponsor authorization.
- Stale review after head change -> HOLD.
- Codex quota exhaustion + Cursor DOCS-HOLD -> HOLD, not fallback approval.
- Unresolved cumulative P1/P2 finding -> HOLD.
- Cross-repository identity mismatch -> reject.
- TreatFlow shadow disagreement -> report divergence without enforcement.
- aws-backbone PR #10 historical replay -> S-40 HOLD preserved; no AWS action.
- SYNGAN phase/package gates -> repository-specific policy preserved.

## Next gates

S-81 contract and dependency reconciliation -> S-83 sanitized read-only replay in parallel with TreatFlow adapter design -> S-82 shadow validation -> S-84 SYNGAN onboarding -> S-85 independent release-authority decision. No production cutover without separate approval.
