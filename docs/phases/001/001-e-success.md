# 001-E — Representative success situations
Status: ANALYSIS COMPLETE; candidate evaluation situations, not validated thresholds.
| Purpose | Representative success situation | Disqualifying observation |
|---|---|---|
| P01 | After a head changes, maintainer can identify which evidence remains applicable | Earlier commit's review silently counts |
| P02 | Sponsor sees outstanding findings and precise authorization scope before acting | Merge proceeds from technical PASS alone |
| P03 | Review provider unavailable; operator sees a blocked or alternate independently qualified path | Quota/timeout yields green state |
| P04 | SYNGAN and TreatFlow differ in local gates; each retains its own required exit evidence | One project's gate is weakened by reuse |
| P05 | Reviewer can reconstruct each material finding's original evidence and disposition | Finding disappears without explanation |
| P06 | Review acknowledged but incomplete; contributor sees pending, not completed | Acknowledgment represented as review PASS |
| P07 | A risky change is withheld despite apparently successful superficial metrics | Completion KPI masks harmful outcome |
Evaluation plan: replay historical counterexamples; ask independent reviewers to challenge evidence; test comprehensibility with real maintainers; compare missed findings, false advancement, recovery burden and decision time. Baselines and numeric thresholds must be established later with real evidence. No implementation or mechanism chosen.
