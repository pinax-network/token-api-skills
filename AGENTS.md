# AGENTS.md

Repository-wide conventions for building Token API agent skills.

## Purpose

This repository is a catalog of task-focused agent skills for the Token API.

Use:

- per-skill `SKILL.md` files for agent behavior and workflow
- per-skill `agents/openai.yaml` files for UI metadata
- shared references for reusable API knowledge

Do not use this file as a replacement for `SKILL.md`. This file defines the
standards that all skills in this repository should follow.

## Repository Layout

- `skills/<skill-name>/SKILL.md`: task-specific instructions
- `skills/<skill-name>/agents/openai.yaml`: display metadata
- `shared/references/*.md`: reusable API and domain references

## Skill Design Rules

- Organize top-level skills by user task, not by endpoint family.
- Keep skills narrow enough to be composable.
- Put chain-specific and endpoint-specific details in shared references when
  they are likely to be reused.
- Prefer EVM, SVM, and TVM routing guidance over hard-coding a single chain
  model into every skill.

## Writing `SKILL.md`

Each `SKILL.md` should include:

- clear trigger conditions in frontmatter `name` and `description`
- a short workflow that tells the agent how to approach the task
- references to shared docs when detailed API context is needed
- an output section describing what a good response should contain

Keep `SKILL.md` concise. Avoid copying large endpoint lists into every skill.

## Writing `agents/openai.yaml`

Each metadata file should include:

- `display_name`
- `short_description`
- `default_prompt`

The metadata should match the `SKILL.md` purpose closely. If the skill changes,
update both files together.

## Shared References

Use `shared/references/` for:

- auth and pagination rules
- network and identifier conventions
- reusable query patterns
- cross-skill API summaries

When new API coverage is added, prefer updating shared references before
duplicating details inside multiple skills.

## Quality Bar

New skills should:

- solve a distinct user-facing task
- state assumptions clearly
- separate direct API observations from inferred conclusions
- mention ambiguity when inputs are incomplete
- avoid overstating what token, holder, transfer, or swap data can prove
