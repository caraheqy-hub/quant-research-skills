---
name: ai-system-evaluation
description: Measure quality and efficiency of AI agents, large language models, and related applications across real tasks. Use when comparative evaluation, latency, cost, resource use, or net human productivity is the main deliverable; exclude a one-off benchmark mention during ordinary implementation.
---

# AI system evaluation

Start with the decision the experiment must support and the unit of comparison: model, agent framework, prompt, tool setup, application, or human workflow. Keep other variables fixed or state their confounding effects.

- Build a task set that represents actual use, with success criteria and scoring decided before testing. Include normal, difficult and failure cases; preserve all attempts, timeouts and quota failures. Keep a holdout for later decisions.
- Record versions, prompts, tools, data snapshot, hardware, concurrency, sampling settings and run dates. Use paired tasks and repeated runs when stochastic variation matters.
- Measure completion quality and error types alongside latency distribution, token or compute use, and money cost. For tool-using agents, inspect traces and consequential actions, not only final text. For personal productivity, use `agent-output-system` to measure preparation, review, rework, adoption, and net human time saved.
- Prefer deterministic checks for objective outcomes; calibrate human or model judges on examples before relying on their scores. Report uncertainty, sample size, exclusions and limitations. Do not tune on the final holdout.
- Save the task set, protocol, raw run records, scoring code and a concise result table when rights permit. Explain which conclusion follows from the observed setting and which remains a hypothesis.

Use `agent-development` to fix an agent, `llm-finetuning` to train weights, and `project-craft` to build the evaluation harness. A dedicated subskill is warranted only when a recurring task family needs distinct scoring or instrumentation.
