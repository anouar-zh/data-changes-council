# CouncilForge roadmap

## Phase 1: make the foundation honest

- Replace placeholder provider responses with a typed provider adapter interface.
- Remove unsupported claims that agreement automatically improves accuracy.
- Align package metadata with the repository license.
- Add a session schema for model version, prompt policy, rubric, evidence, dissent, cost, and approval state.

## Phase 2: build the deliberation loop

- Run independent responses concurrently with timeouts.
- Redact or block inputs by data classification before provider calls.
- Review answers against a configurable rubric instead of a single generic score.
- Keep source references and unresolved claims in the final result.
- Synthesize without hiding minority views.

## Phase 3: evaluate it

- Create a small, versioned task set from real but anonymised work patterns.
- Compare single model, fast council, and full council on correctness, completeness, cost, latency, and reviewer effort.
- Track false consensus and cases where the dissenting answer was better.
- Publish evaluation limits with every release.

## Phase 4: make it usable in organisations

- Add role based access and workspace level provider policies.
- Add retention controls, audit export, and incident records.
- Add a review queue for high impact or low consensus sessions.
- Add Dutch and English output policies.
- Add optional integrations only behind explicit approval gates.
