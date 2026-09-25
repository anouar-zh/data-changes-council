---
name: data-changes-council
description: Use when a decision benefits from several independent AI perspectives, visible disagreement, evidence checks, and human approval before action.
---

# Data Changes Council

Use this skill when a decision deserves independent perspectives, evidence checks, visible disagreement, and a human approval step. The goal is a better decision record, not a vote that pretends to be truth.

## What makes this council different

It does not simply ask several models for an answer and count agreement. It separates four jobs:

- **Builder** proposes a workable option.
- **Skeptic** looks for missing constraints, failure modes, and cheaper alternatives.
- **Evidence auditor** checks which claims are sourced, stale, inferred, or unsupported.
- **Operator** tests whether a real team can adopt and maintain the option.

Use independent passes when several models are available. If only one model is available, run the four jobs as separate, context-preserving passes and label them as simulated perspectives.

## Risk based routing

Classify the decision before choosing the depth of review:

- **Quick**: reversible, low impact, no sensitive data. One answer plus a short skeptic pass.
- **Review**: meaningful cost, cross-team effect, or ambiguous evidence. Three independent perspectives, source ledger, and a dissent check.
- **High impact**: legal, medical, employment, financial, security, safety, personal data, production changes, or irreversible action. Four perspectives, current sources, explicit human owner, and no external action without approval.

Never increase confidence merely because more models agree. Increase review depth when the cost of being wrong increases.

## Council protocol

1. **Write the decision contract.** State the decision question, desired outcome, constraints, deadline, reversibility, affected people, data sensitivity, and named owner.
2. **Collect independent proposals.** Give every perspective the same context. Require assumptions, recommendation, evidence needed, and a failure condition.
3. **Run adversarial review.** Ask the Skeptic and Evidence auditor to challenge the proposals without averaging them together. Ask the Operator to identify the first practical test.
4. **Build a claim ledger.** For each material claim, record source, publication or observation date, freshness, whether it is fact or inference, and what remains unknown.
5. **Resolve or preserve dissent.** State what changed after review. If a disagreement remains, keep both positions and the assumption that separates them.
6. **Synthesize with a stop rule.** Recommend an option only when the evidence and owner are sufficient for the risk level. Otherwise recommend a smaller test, more evidence, or escalation.
7. **Gate action.** A human owner approves before messages are sent, production systems change, money is spent, or people are materially affected.

## Evidence rules

- Cite sources when the decision depends on current, legal, financial, medical, security, or organisational facts.
- Treat model agreement as a routing signal, not proof.
- If all perspectives use the same weak or outdated source, flag possible shared error.
- Never invent a customer case, result, certification, source, or personal experience.
- Keep costs, latency, model names and versions, timestamps, and the rubric version visible when they affect the decision.

Stop and escalate when a material source conflict is unresolved, the data boundary is unclear, the human owner is missing, or the requested action is outside the stated approval.

## Output format

Return a short decision record with:

- **Decision question**
- **Context and constraints**
- **Risk level and routing used**
- **What the perspectives agree on**
- **Dissent and the assumption behind it**
- **Claim ledger and source gaps**
- **Recommendation, safer alternative, and stop rule**
- **Human approval needed from**
- **Smallest next test or action**

For a simple, low-impact question, use one model and a quick check. Use a larger council only when ambiguity, impact, or the cost of a mistake justifies it.
