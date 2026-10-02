---
name: debug-ledger
description: Diagnose software, SDK, data-pipeline, and backtest failures using evidence; keep a reusable bug ledger and consult relevant past cases before fixing a similar failure.
---

# Debug ledger

When a program fails or produces an unexpected result, read the error and reproduce the smallest failing path before changing code. Identify the executable, package version, inputs, last known working state, and the point where observed behavior first diverges. Trace the cause through the data flow; do not infer the cause from a closing dialog or a final symptom alone.

Consult only the matching entries in [cases](references/cases.md) (search by tool, error string, or domain). A past case is a hypothesis, not proof that today's failure has the same cause. After fixing a bug, record one concise case: **symptom → evidence → root cause or unresolved status → minimal fix → verification → recurrence guard**. Record actual failures even when unresolved. Distinguish observed facts from inferences and code-review findings. Avoid tokens, personal paths, account IDs, full logs, and raw private data. Merge duplicate cases and move project-specific details into that project's own issue/test notes.

For a general development project, use `project-craft` for design and delivery. For an A-share factor/backtest error, also use `factor-mining` to check data time, sample selection, and tradeability. For GM SDK calls, verify the current API and run the exact intended Python interpreter; a third-party skill example does not establish current SDK behavior.

Before claiming a fix, rerun the original failing path and the narrow regression check. If the observed symptom is gone but its cause remains unknown, report the uncertainty and keep the case marked unresolved.
