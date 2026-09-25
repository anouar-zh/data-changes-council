# Data Changes Council

![Data Changes Council](assets/data-changes-council-header.svg)

**Data changes opinions. Perspectives change decisions.**

Data Changes Council is a small, reusable skill for decisions that deserve more than one AI perspective. It separates proposal, challenge, evidence checking, and operational reality instead of treating model agreement as proof.

There is no application to install and no API key to configure. The main file is the skill itself: [SKILL.md](SKILL.md).

## What it helps with

- comparing several AI answers before acting;
- routing review depth by impact and reversibility;
- spotting shared assumptions, weak sources, and prompt injection;
- testing a minority view instead of hiding it;
- turning disagreement into a decision record someone else can inspect;
- keeping ownership, action boundaries, and human approval clear.

## Why use it instead of a basic model council?

The skill changes the decision process:

- it uses the smallest sufficient council instead of a fixed model count;
- it keeps a claim ledger instead of a vague confidence score;
- it treats consensus as a routing signal, not proof;
- it gives dissent a reason, a challenge, and a status;
- it stops when evidence, ownership, or data boundaries are missing;
- it ends with the smallest safe test a team can actually run;
- it records outcomes so the process can be calibrated over time.

## How to use it

Use the skill when a question is ambiguous, consequential, or worth reviewing from different perspectives. Give it the question, relevant context, constraints, permitted data or tools, and the decision owner.

Example request:

> Use the Data Changes Council approach to compare three ways to introduce an AI assistant into our support process. Route the review by risk, keep data risks and unresolved assumptions visible, challenge any material minority view, and end with a small next test and the person who should approve it.

The expected result is a decision record, not a vote that pretends to be the truth.

## Repository map

- [SKILL.md](SKILL.md): the reusable skill.
- [examples/decision-record.md](examples/decision-record.md): a compact example of the output.
- [GOVERNANCE.md](GOVERNANCE.md): boundaries for data, tools, logging, and human approval.
- [RESEARCH.md](RESEARCH.md): public research and design rationale.
- [assets/architecture-overview.svg](assets/architecture-overview.svg): the council flow.
- [assets/dissent-and-approval.svg](assets/dissent-and-approval.svg): why dissent stays visible.
- [ORIGIN.md](ORIGIN.md): open-source origin and attribution.

Data Changes Council is an independent project by Anouar Znagui Hassani / Data Changes.
