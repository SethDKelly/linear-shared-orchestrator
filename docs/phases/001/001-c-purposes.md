---
type: Phase 001 Project Record
title: 001-C — Purpose obligations
description: Need-focused and solution-neutral purpose decomposition.
tags: [phase-001, purpose, evidence]
sources:
  - id: needs
    resource: 001-b-needs.md
    title: Provisional affected-party needs
---
# 001-C — Need-focused purpose obligations
Status: ANALYSIS COMPLETE; hypotheses require Phase 001 exit scrutiny.
| ID | Need-focused purpose | Failure counterexample |
|---|---|---|
| P01 | A maintainer can determine the current trustworthy state of a change without reconstructing scattered evidence | A stale review appears current |
| P02 | A sponsor can make a bounded authorization decision with explicit unresolved risks | Review PASS silently implies merge authority |
| P03 | An operator can recognize reviewer unavailability and preserve an honest blocked or pending decision state without treating missing independent evaluation as clearance | Quota exhaustion becomes automatic clearance |
| P04 | Different projects can preserve their own acceptance/security boundaries regardless of how work is coordinated | Shared defaults override a stricter local gate |
| P05 | A reviewer can identify prior findings and independently challenge their disposition | A resolved label substitutes for evidence |
| P06 | Contributors can distinguish genuine completed work from pending or failed work across handoffs | An acknowledged request is reported as finished |

P01 concerns applicability of evidence to the current change; P05 concerns challengeability of finding history; P06 concerns truthful progress state. These are separately testable, though empirical validation remains outstanding. Delivery-agent stop conditions are a candidate need to examine in 001-B, not a prematurely fixed concept. This need provisionally relates to P06 (truthful progress and stop state) and P02 (protected decisions remain sponsor-controlled), but its distinctness and operational evidence remain unvalidated.

Broad avoidance of downstream harm is an overall product-level protective purpose, not a seventh discriminating obligation. These are provisional purposes, not candidate software concepts or product KPIs.
