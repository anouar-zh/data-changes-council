# Architecture direction

Data Changes Council is built around a small, inspectable deliberation loop.

1. **Context and policy check**. Classify the input, apply workspace rules, and reject data that the selected provider is not allowed to receive.
2. **Independent answers**. Ask selected providers in parallel. Each response keeps its model identifier, version, timestamp, sources, and latency.
3. **Structured review**. Review answers against a task specific rubric. Scores must include reasons and may include an abstention.
4. **Synthesis**. Produce a recommendation that distinguishes evidence, inference, uncertainty, and dissent.
5. **Human approval**. Hold any external action until an identified person approves it.

Consensus is a signal for routing. It is not a truth score. The session record should make it possible to see when all models depended on the same weak source.

## First implementation boundary

The first release returns a decision record. It does not send messages, change production systems, make purchases, or claim legal, medical, financial, or employment authority.
