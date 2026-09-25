# Example decision record

## Decision question

Should a support team use an AI assistant to draft replies to common customer questions?

## Context, constraints, and action boundary

The team wants faster first drafts. Customer messages may contain personal data. The assistant may advise and draft, but it may not send, edit the source system, or make a customer decision. A support lead owns the decision.

## Risk class and routing used

**Review.** The pilot is limited and reversible, but source quality and personal data make a claim check necessary. Builder, Skeptic, Evidence auditor, Operator, and a minority challenge were used.

## Options considered

1. Do nothing and keep manual drafting.
2. Run a narrow pilot for low-risk questions using approved source material.
3. Run a broad pilot across all support categories.

## Option comparison

| Option | Evidence and unknowns | Reversibility and exposure | Operational fit | Trade-off |
|---|---|---|---|---|
| Do nothing | Known process, no new source gap | Low change, no new model exposure | Easy to maintain | No learning or drafting benefit |
| Narrow pilot | Source coverage still unknown | Reversible and limited to low-risk questions | Manageable for one support lead | Requires a measured test |
| Broad pilot | Source coverage is unverified | Larger data and quality exposure | Harder to review consistently | Faster reach, higher downside |

## Agreement with supporting claims

- Start with a limited set of low-risk questions.
- Use approved source material rather than open-ended model knowledge.
- Keep the draft separate from the send action.
- Measure correction time as well as drafting time.

## Dissent, minority challenge, and separating assumption

One perspective recommends a broad pilot. The other perspectives recommend a narrow pilot because the quality of the source material is not yet known. The broad-pilot view depends on the assumption that source coverage is already adequate. That assumption is untested, so the minority view is retained and the broad pilot is blocked.

## Claim ledger and source gaps

| Claim | Status | Source or observation | Date and freshness | Independence | Impact | Next check |
|---|---|---|---|---|---|---|
| Source coverage is sufficient | unknown | no measured coverage yet | not available | unclear | high | sample 50 questions |
| A human can approve every draft | proposed control | support lead process | current process | observed | high | confirm workflow |
| The pilot will save time | predicted | no result yet | not available | none | medium | measure correction time |

## Decision status

**Proposed.** The support lead has not yet approved the pilot.

## Recommendation and stop rule

Run a two-week test on one category of low-risk questions. The assistant may draft, but cannot send. Stop expansion if personal data cannot be minimised, source coverage is inadequate, or reviewers cannot check drafts in time.

## Human approval needed from

The support lead approves the category, source set, acceptance criteria, and test result before expansion.

## Smallest next test

Prepare 50 anonymised questions, define acceptance criteria, and measure accepted, corrected, and rejected drafts.

## Record metadata

Timestamp: 2026-09-25
Models or passes: four independent role passes plus one minority challenge
Sources: approved support material, to be listed before the pilot
Rounds: 1
Decision status: proposed
Material cost or latency: not measured yet
