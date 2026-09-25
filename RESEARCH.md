# Research basis

Data Changes Council was compared with public council implementations and governance guidance on 25 September 2026. The aim was to understand what a reusable council skill should keep, and where it should be stricter.

## Patterns found

Public council skills commonly use independent answers, peer review, adversarial debate, and a final synthesis. Some require a fixed number of models or a fixed three-stage flow. Others focus on provider orchestration, model selection, or raw transcript visibility.

That pattern is useful for generating alternatives. It does not, by itself, establish source quality, operational ownership, safe action boundaries, or whether agreement comes from genuinely independent evidence.

## Design choices in this project

Data Changes Council keeps the useful parts and adds:

- risk based routing instead of a fixed number of models;
- four explicit jobs: Builder, Skeptic, Evidence auditor, and Operator;
- a claim ledger that marks facts, inferences, predictions, unknowns, freshness, and source independence;
- a minority challenge so a correct minority view is not dismissed by a majority;
- bounded rounds and a smallest sufficient council to control cost and latency;
- prompt injection handling for retrieved documents and tool output;
- explicit action boundaries and human approval before external or high impact actions;
- outcome review so routing and dissent handling can be calibrated over time.

These are operating rules for decision quality. They are not a claim that a council is always more accurate than one model.

## Sources reviewed

- [DAIR AI LLM Council skill](https://github.com/dair-ai/dair-academy-plugins/blob/main/plugins/llm-council/skills/llm-council/SKILL.md)
- [MugenGH AI Council](https://github.com/mugenGH/ai-council/blob/main/SKILL.md)
- [NGMeyer Council Review](https://github.com/ngmeyer/council-review/blob/main/SKILL.md)
- [Tsenart Council Skill](https://github.com/tsenart/council-skill)
- [Thevgavini GHCP LLM Council](https://github.com/thevgavini/ghcp-llm-council)
- [OliWoods LLM Council](https://github.com/OliWoods-Org/llm-council)
- [NIST AI Risk Management Framework](https://www.nist.gov/itl/ai-risk-management-framework)
- [NIST Generative AI Profile](https://nvlpubs.nist.gov/nistpubs/ai/NIST.AI.600-1.pdf)
- [NIST Govern Playbook](https://airc.nist.gov/airmf-resources/playbook/govern/)
- [Minority Sentinel research](https://arxiv.org/abs/2606.29270)

The sources informed the design. They do not endorse this repository.

## Installation references checked

- [OpenAI Skills in ChatGPT](https://help.openai.com/en/articles/20001066-skills-in-chatgpt): upload flow, scanning, and workspace permissions.
- [OpenAI Skills guide](https://developers.openai.com/api/docs/guides/tools-skills): skill bundle format, `SKILL.md`, and discovery requirements.
- [OpenAI plugin skills](https://developers.openai.com/plugins/concepts/skills): skill structure and use with ChatGPT and Codex.
- [Anthropic Agent Skills](https://platform.claude.com/docs/en/managed-agents/skills): `.claude/skills/<skill-name>/SKILL.md` discovery for Claude Code and managed agents.
- [Anthropic Claude Code CLI reference](https://docs.anthropic.com/en/docs/claude-code/cli-usage): terminal product and CLI behavior.
- [Anthropic Projects](https://support.anthropic.com/en/articles/9519177-how-can-i-create-and-manage-projects): project knowledge and project instructions.

Product surfaces change. The repository distinguishes native skill installation from uploading `SKILL.md` as project or chat context, because those are different mechanisms.
