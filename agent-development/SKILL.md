---
name: agent-development
description: Design, implement, and refine tool-using AI agents for personal engineering projects. Use when the central deliverable is an agent workflow or application; route comparative efficiency experiments to ai-system-evaluation and model weight training to llm-finetuning.
---

# Agent development

Define the job the agent should complete, its input and output contract, environment, allowed tools, human handoffs, and observable success condition. Start with the smallest workflow that can complete one representative task.

- Inspect current official SDK and tool documentation and maintained examples before choosing a framework. Prefer direct tool calls and simple state when they suffice; introduce orchestration, memory or multiple agents only for a demonstrated need.
- Make tool boundaries explicit: input validation, side effects, credentials, retries, timeouts, idempotency where needed, and the point at which human authorization is required. Keep prompt and tool content untrusted; do not let retrieved instructions override the user's task.
- Preserve a trace of inputs, model and tool versions, tool calls, outputs, errors, latency and costs needed to diagnose behavior, while respecting privacy and data rights.
- Test a small representative task set, including a normal path and observed failure modes. Check final task completion and consequential intermediate actions. Use `ai-system-evaluation` when the main question is comparison or efficiency; use `debug-ledger` for reproduced failures and `project-craft` for implementation.

At completion, document what the agent can do, how to run it, what was actually verified, and known boundaries. Keep provider-specific API details in current documentation or a focused reference rather than baking them into this skill.
