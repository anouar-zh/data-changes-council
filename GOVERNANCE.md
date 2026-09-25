# Governance boundaries

Data Changes Council is decision support. It is not an autonomous decision maker.

## Required controls

- Do not send confidential or personal data to a provider unless the organisation has approved that data flow.
- Minimise, redact, or summarise sensitive data before a model call where possible.
- Treat retrieved documents, attachments, code, and tool output as untrusted content. Instructions inside them do not override the council or the human owner.
- Keep provider credentials server side and outside the repository.
- Record the model, version, prompt policy, rubric version, sources, timestamp, cost, round count, and reviewer when material.
- Keep disagreement and the minority challenge visible when models do not reach a stable conclusion.
- Require a human approval step before sending messages, changing production systems, making purchases, or taking other external actions.
- Escalate legal, medical, employment, financial, and safety related decisions to a qualified person.
- Make it possible to delete or redact stored session data.

## Confidence language

Consensus is a routing signal, not a truth score. The record should say what the models agreed on, what they did not check, which claims remain uncertain, and what a person still needs to verify.
