# 004-E — Adversarial modularity: bounded entry gate

Status: **admitted for design-only adversarial qualification**, not Phase 004 exit or implementation. Linear: S-136. Baseline: merged Phase 004 documentation in `main` at `2f2c224d378eff860c9aacd5beafcd35ea9a5e69` (PR #3 and PR #5). Sponsor accepted 004-D design with explicit carry-forwards.

## Purpose and qualification boundary
Challenge existing Phase 003 purpose, concept identities, behavioral contracts and Phase 004 provisional boundaries against concrete counterexamples. Preserve C2/C3/R-06 as provisional; RD-14 open/indeterminate, RD-15 credibility/actor eligibility open, and P05/R-06 disposition under S-141. Neither missing assignee nor an optional technical document evaluator is a new veto. The TPO owns admission, dependency routing and closure; independent reviewers assess evidence, not author the decision.

## First bounded slice: three falsifiable paper traces
1. **Stale revision / reidentification:** An apparently valid permission or completion assertion refers to an obsolete revision. Trace the exact existing guards, participant-visible rejection and history; classify any gap as intrinsic defect, verification failure or deferred enhancement.
2. **Contested evidence / silence:** Two independently supported contradictory claims and a silent challenged party must remain visibly contested. Show that timeout, absence of reply and a favorable assessment cannot silently settle a challenge.
3. **False completion / unauthorized disposition:** A bare assertion or `verified=true` must not create work completion or convert a generic reply into C2 `AddressChallenge` or an invented R-06 `AddressOutcomeChallenge`. Preserve request/acknowledgment/attempt distinctions.

For each trace record canonical source/line or section, initial state, ordered actions, expected guards/effects, counterexample, observation, classification, and bounded disposition. Do not change canonical behavior as part of the entry gate.

## Success and exit criteria
A coherent three-trace evidence table, explicit negative controls and cross-reference to existing Phase 003 contract; any real intrinsic contradiction routes to the qualified canonical owner (material identity change reopens Phase 003; proven RD-14 collapse routes to Phase 002-C). A broken test is repaired as verification work rather than used to reject a sound concept. Later-phase composition (005), extrinsic dependence (006), reuse (008) remain deferred. Independent exact-head design review, documented carry-forwards and TPO exit decision precede 004-E closure. No speculative extra review cycles or mandatory R-06 challenge resolution.

## Execution controls
One small PR per qualified slice; keep exact-head evidence and reviewer provenance, use existing Cursor/Codex review receipts without duplication. S-140 eight-domain design remains non-authoritative and is not canonized here. S-40 security HOLD remains: no implementation, AWS/IAM/STS/Terraform or production changes. Phase 012 is the endpoint; no Phase 013.
