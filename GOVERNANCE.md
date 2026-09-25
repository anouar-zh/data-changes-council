# Governance boundaries

Data Changes Council is decision support. It is not an autonomous decision maker.

## Required controls

- Do not send confidential or personal data to a provider unless the organisation has approved that data flow.
- Keep provider credentials server side and outside the repository.
- Record the model, version, prompt policy, rubric version, sources, timestamp, cost, and reviewer.
- Keep disagreement visible when models do not reach a stable conclusion.
- Require a human approval step before sending messages, changing production systems, making purchases, or taking other external actions.
- Escalate legal, medical, employment, financial, and safety related decisions to a qualified person.
- Make it possible to delete or redact stored session data.

## Confidence language

Consensus is a routing signal, not a truth score. The UI should say what the models agreed on, what they did not check, and what a person still needs to verify.
