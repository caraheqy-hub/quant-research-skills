---
name: project-craft
description: Use for substantial software projects and meaningful feature work that need an initial design, skill and open-source research, clear minimal code, and reviewable delivery. Skip for tiny edits and purely informational requests.
---

# Project craft

Work toward the user's actual deliverable. Scale the process to the task; do not turn this skill into an approval gate or a reason to leave authorized work unfinished.

1. **Start from the project decision.** Read the existing project and constraints. Reuse a `project-start` launch note when one exists; otherwise sketch the intended outcome, main components, data flow, and largest uncertainty. Revise the design when evidence changes.
2. **Check implementation choices.** Reuse the initial survey instead of repeating it. For a new or consequential technical choice, inspect current primary documentation and maintained code before committing to an architecture. Compare fitness, maintenance, license, dependencies, and hidden complexity. Use `skill-garden` only when choosing or improving a skill is itself needed. Keep one-off project facts in that project's instructions.
3. **Build the smallest coherent slice.** Prefer a direct data flow, clear names, standard library and existing dependencies, and small functions with one purpose. Add abstraction after a second real use case or a concrete reason. Put error checks at real input, boundary, and risk points; avoid speculative layers, broad exception handling, duplicated configuration, and tests that merely echo implementation.
4. **Verify what matters.** Run the smallest meaningful end-to-end path, then test timing, data provenance, external interfaces, and observed failure cases that could change the conclusion. Read outputs before claiming success. For financial research, keep publication time, signal time, execution time, universe history, fees, and holdout selection explicit.
   When a bug appears, use `debug-ledger`: search relevant past cases, reproduce and trace the present failure, then record the observed case after verification. Keep unresolved cases labelled as such; do not promote an untested guess into a rule.
5. **Leave a readable project.** Keep code and directories easy to navigate. Explain usage in plain language for the reader, record the source and limits of claims, and distinguish a working example from a faithful reproduction or production-ready system. For a public release, check tracked files for credentials, personal paths, restricted data, and third-party license terms before pushing. Summarize what changed, how it was checked, and what remains uncertain.

At completion, use `skill-garden` if an observed lesson may recur across projects; otherwise leave the finding in the project.

Useful public guidance: [Python PEP 20](https://peps.python.org/pep-0020/) on readability and simplicity; [Google's small changes guide](https://google.github.io/eng-practices/review/developer/small-cls.html) on keeping changes self-contained. These are principles, not a required ceremony.
