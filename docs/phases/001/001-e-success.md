---
type: Phase 001 Project Record
title: 001-E — Success situations
description: Hypothetical, evaluable purpose success and failure cases.
tags: [phase-001, success, evidence]
sources:
  - id: purposes
    resource: 001-c-purposes.md
    title: Purpose obligations
---
# 001-E — Representative success situations
Status: ANALYSIS COMPLETE; candidate evaluation situations, not validated thresholds.
| Purpose | Representative success situation | Disqualifying observation |
|---|---|---|
| P01 | After a head changes, maintainer can identify which evidence remains applicable | Earlier commit's review silently counts |
| P02 | Sponsor sees outstanding findings and precise authorization scope before acting | Merge proceeds from technical PASS alone |
| P03 | Review provider unavailable; operator sees an honest pending or blocked state until independent evidence is available | Quota/timeout yields green state |
| P04 | In a hypothetical future comparison, two adopting projects impose different local gates; each retains its own required exit evidence | One project's gate is weakened by reuse |
| P05 | Reviewer can reconstruct each material finding's original evidence and disposition | Finding disappears without explanation |
| P06 | Review acknowledged but incomplete; contributor sees pending, not completed | Acknowledgment represented as review PASS |

Broad downstream-harm avoidance is evaluated as a product-level guardrail across all six cases, not an independently discriminating P07. Evidence-subject exposure should be challenged explicitly in future evaluations.

Evaluation plan: replay historical counterexamples; ask independent reviewers to challenge evidence; test comprehensibility with real maintainers; compare missed findings, false advancement, recovery burden and decision time. Baselines and numeric thresholds must be established later with real evidence. No implementation or mechanism chosen.
