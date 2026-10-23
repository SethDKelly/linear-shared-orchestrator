---
type: Phase 003 Project Record
title: 003-C — Abstract Behavior Specifications
description: Independent concept-level state and action hypotheses and identity falsification.
tags: [phase-003, abstract-state, actions, identity-tests]
sources:
  - id: identity
    resource: 003-b-candidate-identity-operational-principles.md
    title: Independently reviewed 003-B identities and operational principles
  - id: contract
    resource: concept-specification-contract.md
    title: Phase 003 specification contract
  - id: purpose
    resource: ../../canonical/purpose/purpose-model.md
    title: Purpose authority
---
# 003-C — Abstract behavior specifications

**Status: INDEPENDENT PASS at 321bbf0; 003-E reconciliation admitted. Separate 003-D evidence remains independently owned.** These are representation-independent hypotheses, not canonical concepts, executable models, APIs, workflow definitions or application architecture.

## C2 — Living inquiry

**Purpose/OP:** A person can maintain a challengeable answer about the applicability of observations to a change. [003-B](003-b-candidate-identity-operational-principles.md) describes objection and revision invalidating previously applicable grounds.

**Abstract domains:** Inquiry, ChangeRevision, Ground, Challenge, Participant, Claim. Identities are opaque and not external concept types. Ground applicability and independent credibility are *assertions to challenge*, not computed trust.

**Minimum memory hypothesis:** For each inquiry, its question and currently referenced change revision; the set of grounds asserted applicable to that revision; challenges and their dispositions with supersession relations; and any provisional answer with the grounds/revision on which it depends. Historical links are necessary only insofar as they prevent a prior answer being misrepresented as current or silently erasing an objection. No reviewer, receipt, issue or provider type is intrinsic.

**Conceptual actions:**
- **OpenInquiry(question, revision):** establishes an unsettled question for a specified revision.
- **OfferGround(inquiry, ground, claimedRevision):** makes a contestable assertion; does not establish independent verification.
- **ChallengeGround(inquiry, ground, reason):** marks an applicable ground disputed; does not automatically settle the entire question.
- **AddressChallenge(inquiry, challenge, disposition, rationale):** records an accountable disposition; never deletes the existence of a prior challenge.
- **RebaseInquiry(inquiry, newRevision):** changes the relevant revision and removes the *presumption* that previous grounds or answer apply; applicability must be reasserted or established.
- **ProposeAnswer(inquiry, claim, citedGrounds):** records an answer with explicit revision and grounding, never a sponsor permission or final verification.
- **InspectInquiry(inquiry):** returns the question, current revision, asserted grounds, unresolved challenges and answer applicability without mutating them.

**Guards/effects/invariants:** Actions referring to an inquiry require that it exists. Challenges require a referenced asserted ground. A ground disputed without a resolved challenge cannot be silently treated as unchallenged. Rebase does not erase historical grounds, but previous revision grounds do not by themselves justify the new revision. An answer's justification is revision-qualified; unsupported answers remain claims, not validated conclusions. The concept does not evaluate providers or authenticate participants.

**Initial/history/under-specification:** Initially no inquiries. Inquiry may remain unsettled indefinitely; there is no invented timeout or automatic closure. Ordering among independent grounds is unspecified. The criteria for independent ground credibility, access to evidence, and whether a question may span multiple revisions are open design questions, not falsely solved by an invented algorithm.

**C1 falsification:** Remove any generic container or review receipt. The residual semantics of *challenge, revision-qualified justification, and preservation of contested answers* remain describable. Whether that difference is valuable enough for an independent concept is **not proved** and is for 003-D/003-E to test.

## C3 — Scoped permission, with obligations under test

**Purpose/OP:** An accountable decision-maker can explicitly withhold or grant bounded authorization despite favorable technical review, while seeing unmet obligations without mistaking them for permission.

**Abstract domains:** DecisionScope, Actor, Authorization, ObligationClaim, EvidenceClaim. These are abstract parameters, not a project-specific role hierarchy, policy engine, review receipt or shared provider.

**Minimum memory hypothesis:** For a scope, explicit authorization assertions including actor, scope and current validity/supersession; withdrawals; and references to obligation claims *only if* the concept's own behavior requires preserving an actor's declared basis for decision. Obligations are initially modeled as **abstract externally asserted inputs**, not intrinsically owned lifecycle or a universal policy catalog.

**Conceptual actions:**
- **ConsiderScope(scope, obligations):** presents a bounded decision and asserted unmet obligations without creating permission.
- **Withhold(scope, actor, rationale):** explicitly records that permission was not granted; review evidence is irrelevant to the fact of authorization.
- **Authorize(scope, actor, basis):** establishes an explicit, actor-attributed authorization for exactly the scope; valid only under an assumed project-local authority predicate, which is a required guard, not implemented policy.
- **Withdraw(scope, actor, authorization):** revokes or supersedes a prior authorization under an applicable authority guard.
- **InspectPermission(scope):** returns whether explicit current authorization exists, its scope and actor, and the known unresolved obligation claims without converting those claims into approvals.

**Guards/effects/invariants:** An authorization must be explicit, attributable, scoped and currently applicable. A review PASS, issue state, favorable narrative or absence of objections cannot create permission. Permission for scope A does not imply permission for a materially changed scope B. Project-local authority guards may forbid actions even when shared coordination would allow them. The relationship between a permission and a declared obligation is deliberately not reduced to a universal rule: the actor's decision is distinct from the truth of the obligation claim.

**Initial/history/under-specification:** Initially no permission; a missing authorization is not approval. Withdrawal and changed scope preserve the historical fact of prior authorization but do not grant present permission. Exact actor eligibility and local policy evaluation are open inputs for later design/security validation; no authentication mechanism, RBAC, tokens or storage is chosen.

**Overload falsification:** If removing the externally supplied obligation claims leaves the same coherent scoped-authority behavior, C3's intrinsic identity is **permission**, not a bundled obligation-management engine. The provisional name remains historical; a rename/split may be necessary in 003-E. If permission is just a record of another actor's decision without meaningful guarded effects, independent concept status remains questionable.

## C6 — Correctable account (conditional identity test)

**Purpose/OP:** A contributor can correct a misleading account of work so downstream people can distinguish attempt, acknowledgment, verified result and completion without treating the explanation as independent evidence.

**Hypothesis A — Pure rendering:** If the narrative is entirely a view over C2 claims and C3 decisions, its meaning is derivable from other concepts. No intrinsic state or action remains, so **C6 should not become a standalone concept**; defer user-facing mapping to Phase 007.

**Hypothesis B — Independent accountable assertion:** A distinct actor-authored account can itself be asserted, challenged, corrected and historically attributed even when the underlying change observations are unchanged. Abstract domains: Account, Assertion, Author, Correction, BasisReference. Minimal memory would be authored assertions, their attribution, contested/corrected relations and stated basis. Actions would be **AssertAccount**, **ChallengeAssertion**, **CorrectAssertion**, **InspectAccount**. Correction preserves the prior claim and identifies the corrected meaning; it never verifies the underlying work or authorizes it.

**Identity discriminator:** Can two independent accounts about the *same* change and identical C2/C3 state be meaningfully different because of accountable authorship, contest and correction? If yes, B has semantic behavior beyond formatting; if no, A is more parsimonious. This is a conceptual counterfactual, **not empirical evidence** that users need a separate concept. The risk of duplicating C2's challenge/history semantics remains material; 003-D must try to collapse B into C2 before 003-E decides.

**Invariant and limits under B:** A correction does not erase the challenged prior assertion. Unverified prose cannot become verification, a requested review cannot become completed review, and a narrative cannot grant permission. Initially no accounts. Narrative structure, writing style, visibility, access and retention are not specified. Do not invent persistent state merely to preserve C6.

## Cross-candidate sufficiency and separation

| Concern | C2 | C3 | C6 |
|---|---|---|---|
| Current evidence applicability | Inquiry grounds and revision | No intrinsic evidence verdict | Claims can cite, not establish, applicability |
| Authorization | Never grants | Explicit, scoped actor decision | Never grants |
| Reviewer silence/unavailability | Unresolved ground/question | No inferred permission | Honest unknown/incomplete explanation |
| Challenge and correction | Contest grounds/answers | Reconsider explicit authorization | Contest authored assertions *only if B survives* |
| Completion | Never self-certifies | Permission is not completion | Distinguishes reported and verified completion |
| Cross-project autonomy | No policy engine | Local authority guard, not global override | No forced sharing or visibility |

No concept invokes another's actions or stores another's native types. Cross-concept synchronization, visibility mapping and security infrastructure remain Phase 005/007/later design. P01–P06 remain test obligations; these specifications do not certify stakeholder fit.

## 003-C open findings for independent challenge
- **C-001:** Does C2's contest/rebase memory provide independent user value, or is it an ordinary case record? Reopen 002-C if no independent characteristic behavior survives.
- **C-002:** C3's intrinsic identity may be scoped permission only; obligation claims may belong elsewhere. Test specificity and project-local authority.
- **C-003:** C6 Hypothesis B might duplicate C2; prefer Hypothesis A if no distinct accountable-assertion behavior survives. No artificial state.
- **C-004:** Validity of grounds, actor authority, retention/privacy, temporal relevance and stakeholder demand are unverified. 003-D and later phases own adversarial/empirical challenges.

**Handoff:** This record is an independent 003-C workstream draft. 003-D's evidence must not be silently incorporated or treated as clearance. Both need independent review before 003-E reconciliation; Phase 003 exit and implementation remain unauthorized.
