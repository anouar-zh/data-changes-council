# Repository instructions

## Scope

Data Changes Council is a portable Agent Skills workflow. The repository is intentionally documentation-first. It does not contain an application, provider integrations, API routes, model keys, installation scripts, or a test suite.

## Canonical skill

- Keep the reusable workflow in the root `SKILL.md`.
- Keep the YAML front matter valid, with a focused `name` and a clear `description`.
- Keep the skill provider-neutral so it can be used with Codex, ChatGPT Skills, Claude Code, or as uploaded project context.
- Preserve the distinction between advice, drafting, and execution.
- Do not turn model agreement into a truth score.
- Keep risk routing, claim evidence, dissent, human approval, and stop rules explicit.

## Supporting files

- Update `README.md` when the installation or usage flow changes.
- Keep `examples/decision-record.md` aligned with the output fields in `SKILL.md`.
- Keep `GOVERNANCE.md` and `DISCLAIMER.md` consistent with the human approval and liability boundaries.
- Keep `RESEARCH.md` factual, dated, and linked to public sources.
- Preserve `ORIGIN.md` and `LICENSE` when modifying material derived from the upstream project.
- Assets are explanatory or repository presentation material. They must not imply that an application or model orchestration engine exists.

## Validation

Before publishing changes:

1. Check the YAML front matter and required sections in `SKILL.md`.
2. Run `git diff --check`.
3. Confirm there are no API keys, provider credentials, customer data, invented claims, or stale references to the removed application.
4. Review links and examples.
5. Commit and push only the intended documentation and asset changes.
