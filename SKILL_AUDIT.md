# Skill boundaries and cleanup

Updated 2026-10-02. This repository contains eleven self-authored skills. The cleanup makes their triggers and handoffs distinct while keeping project-specific facts out of reusable instructions.

## Workflow boundaries

| Question | Lead skill | Handoff |
| --- | --- | --- |
| What should this new project be, what already exists, and which domain fits? | `project-start` | Reuse its launch note during implementation. |
| How should a substantial software artifact be built and verified? | `project-craft` | Check new technical choices; do not repeat the launch survey. |
| Which skill belongs to a task, or where should a verified lesson live? | `skill-garden` | It manages the skill library, not the project design. |
| Does a topic need a broad evidence survey? | `source-research` | Return a source-grounded evidence map to the project. |
| Is the central question quantitative finance? | `quant-projects` | Use `factor-mining` for factor methodology and a platform skill only for a chosen platform. |
| Is the deliverable an agent, tuned model, or comparative measurement? | `agent-development`, `llm-finetuning`, or `ai-system-evaluation` | Pick by the primary deliverable; use the others only for concrete subtasks. |

The `quant-projects` entrypoint no longer restates the factor experiment protocol in `factor-mining`. `ai-system-evaluation` covers system comparisons; the separate local `agent-output-system` covers personal workflow adoption and net human time saved.

## External local skills

- `juejinquant` is based on the third-party [fadewalk project](https://github.com/fadewalk/juejinquant-skill). It is a platform reference for GM/MyQuant/GoldMiner, not a generic trigger for all quant work. Confirm changing API details in official documentation. Its source and bundled examples are not copied into this public repository.
- `jupyter-notebooks` is an external installed skill for notebook artifacts, not a domain workflow. Its local references to unavailable data tools should be conditional on tools actually present.
- `agent-output-system` is maintained with its own project. Use it when the outcome is personal net productivity rather than a model or agent benchmark.

## What remains project-specific

Data licenses, model versions, compute limits, experiment settings, platform accounts, and observed results belong in the project. A new domain or subskill is justified only when repeated projects require a distinct method or validation path. A single new topic, asset, or SDK does not by itself justify another skill.
