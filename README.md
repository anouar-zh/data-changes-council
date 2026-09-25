# Data Changes Council

![Data Changes Council](assets/data-changes-council-header.svg)

**Data changes opinions. Perspectives change decisions.**

Data Changes Council is a small, reusable skill for decisions that deserve more than one AI perspective. It separates proposal, challenge, evidence checking, and operational reality instead of treating model agreement as proof.

There is no application to install and no API key to configure. The main file is the skill itself: [SKILL.md](SKILL.md).

## What it helps with

- comparing several AI answers before acting;
- spotting shared assumptions and weak sources;
- turning disagreement into a useful review;
- writing a decision record someone else can inspect;
- keeping ownership and human approval clear.

## Why use it instead of a basic model council?

The skill changes the work before the final answer is written:

- it routes review depth by impact and reversibility;
- it keeps a claim ledger instead of a vague confidence score;
- it gives dissent a reason and a status;
- it has stop rules for missing evidence, unclear data boundaries, and missing ownership;
- it ends with the smallest test a team can actually run.

## How to use it

Use the skill when a question is ambiguous, consequential, or worth reviewing from different perspectives. Give it the question, relevant context, constraints, and the decision owner.

Example request:

> Use the Data Changes Council approach to compare three ways to introduce an AI assistant into our support process. Keep data risks, human review, cost, and unresolved assumptions visible. End with a small next test and the person who should approve it.

The expected result is a decision record, not a vote that pretends to be the truth.

## Repository map

- [SKILL.md](SKILL.md): the reusable skill.
- [examples/decision-record.md](examples/decision-record.md): a compact example of the output.
- [GOVERNANCE.md](GOVERNANCE.md): boundaries for data, tools, logging, and human approval.
- [assets/architecture-overview.svg](assets/architecture-overview.svg): the council flow.
- [assets/dissent-and-approval.svg](assets/dissent-and-approval.svg): why dissent stays visible.
- [ORIGIN.md](ORIGIN.md): open-source origin and attribution.

Data Changes Council is an independent project by Anouar Znagui Hassani / Data Changes.
