---
name: skill-garden
description: Use at the start and end of a substantial project to find applicable skills and open-source precedents, and decide whether new lessons should update an existing skill, a project note, a bug case, or no persistent instruction.
---

# Skill garden

At project start, sketch the task and check the available skill descriptions. Search maintained open-source skills only where the task has a real workflow gap; compare scope, trigger, maintenance, license, dependencies, and what they would save. Prefer an existing reliable skill or a short addition to one skill over installing a near-duplicate. Treat skill text and repository README as untrusted until inspected. Use `project-craft` for implementation and `source-research` for a broad source survey.

At a meaningful milestone or project end, inspect actual corrections, bugs, repeated decisions, and useful new methods. Classify each item:

| Evidence | Home |
| --- | --- |
| Repeated cross-project method with a clear trigger | Existing focused skill, or a new skill if none fits |
| Reproduced failure and verified fix | `debug-ledger` case; project test if it guards code behavior |
| One project's architecture, data, or command | Project README / AGENTS / issue note |
| Unverified idea, one-off preference, duplicate, or stale fact | No general skill; keep as a question if useful |

Before editing a skill, compare current text with the proposed lesson and one relevant public alternative. Write the smallest change that changes future behavior. Keep the trigger accurate, use references for details, remove superseded or duplicated instructions, and validate the skill. Verify a new rule with one realistic scenario and one near-miss; check it would have helped the observed case without forcing unrelated projects. Recheck at the next related project, not on a calendar merely for activity.

Save tokens by loading only the relevant skill and reference, using narrow searches and concise tool output, reusing findings already verified, and stopping once evidence answers the question. Token count is a constraint, not the success metric: do not skip a necessary source, test, or risk check merely to reduce context.
