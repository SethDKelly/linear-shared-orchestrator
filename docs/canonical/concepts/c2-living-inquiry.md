---
type: Canonical Concept Specification
title: C2 — Living Inquiry (Provisional)
description: Current abstract inquiry behavior; factoring and independent identity remain subject to Phase 004.
tags: [canonical, concept, provisional, c2, phase-004]
sources:
  - id: identity
    resource: ../../phases/003/003-b-candidate-identity-operational-principles.md
    title: C2 purpose and operational principle
  - id: behavior
    resource: ../../phases/003/003-c-abstract-behavior-specifications.md
    title: C2 state and action specification
  - id: reconciliation
    resource: ../../phases/003/003-e-behavioral-reconciliation.md
    title: C2 boundary reconciliation
---
# C2 — Living inquiry

**Authority:** Provisional canonical owner of current C2 behavioral meaning, not final acceptance of C2 as an independent concept. Phase 004 may **revise, split, merge, generalize or reject** this boundary. No implementation or sponsor exit decision is implied.

## Purpose and operational principle
P01/P05: enable a maintainer or independent reviewer to maintain a challengeable, revision-qualified question about whether observations support a change. **OP C2-1:** A question receives a provisional answer grounded in observations; a reviewer challenges a ground, leaving the answer contested; a change revision invalidates inherited applicability until grounds are renewed. The person can inspect what is known, disputed and stale.

## Abstract identity and memory
Parameters: Inquiry, ChangeRevision, Ground, Challenge, Participant, Claim. State for each inquiry: question; current revision; offered grounds with asserted applicability; challenges and attributed dispositions; provisional answers with supporting grounds and revision; supersession/history sufficient to avoid erasing objection or presenting stale answers as current. No native review receipt, provider, authorization, work-attempt or controller type.

## Conceptual actions
- **OpenInquiry(question, revision):** create an unsettled inquiry for a revision.
- **OfferGround(inquiry, ground, claimedRevision):** add a contestable applicability assertion, not verified truth.
- **ChallengeGround(inquiry, ground, reason):** register dispute; do not silently erase it.
- **AddressChallenge(inquiry, challenge, disposition, rationale):** attribute disposition and preserve prior challenge.
- **RebaseInquiry(inquiry, newRevision):** change current revision; earlier grounds and answers lose presumed applicability.
- **ProposeAnswer(inquiry, claim, citedGrounds):** record revision-qualified provisional answer, not permission or proof of execution.
- **InspectInquiry(inquiry):** expose question, revision, grounds, unresolved challenges and current answer applicability.

Actions referencing inquiries or grounds require the referenced fact to exist. Initial state contains no inquiries. An inquiry may remain unsettled indefinitely. Challenge disposition does not retroactively erase the challenge. A contested ground cannot silently count as uncontested justification; a new revision does not inherit a prior answer. Independent credibility, participant eligibility, evidence access, retention and multi-revision inquiry behavior are open validation/design questions. Ground order, timeout and automatic closure are deliberately unspecified.

## Boundaries and required challenges
C2 answers **what grounds support a question**; it does not authorize (C3), record attributable execution outcome (R-06), perform a review, or create a narrative concept (C6). A generic case (C1) may subsume its behavior: Phase 004 must attempt that falsification. P03 silence stays unknown; P04 local authority remains external. No S-81 architecture, API, schema, UI or workflow is selected.
