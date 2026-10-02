---
name: llm-finetuning
description: Plan and run personal large-language-model fine-tuning projects, including dataset preparation, training, evaluation, and model comparison. Use when the project changes model weights or adapters; exclude prompt-only agent development and evaluation-only studies.
---

# LLM fine-tuning

State the target behavior, base model and license, deployment constraints, available compute, and a measurable reason to train. First establish a base-model or prompt baseline on representative held-out tasks.

1. **Data:** Record origin, rights, consent or privacy constraints, transformations, format, deduplication, and train/validation/test separation. Inspect examples and label quality. Prevent near duplicates and benchmark answers from leaking into training.
2. **Method:** Select the least costly method that can test the hypothesis, such as supervised fine-tuning or an adapter when appropriate. Confirm current model, tokenizer, chat template, framework and hardware compatibility against official documentation. Fix seeds where feasible and record all settings and package versions.
3. **Run:** Start with a small end-to-end smoke run that saves and reloads a checkpoint. Log data version, token counts, loss, wall time, memory and compute use. Diagnose training instability before scaling.
4. **Evaluate:** Compare the tuned model with the same base baseline on untouched tasks and deployment conditions. Measure task quality plus latency, memory and inference cost when relevant; inspect regressions and error categories. Distinguish training loss from useful behavior.
5. **Deliver:** Preserve reproducible configuration and evaluation evidence. Share weights or data only when license, privacy and user authorization allow it. State where results are exploratory.

Use `ai-system-evaluation` for comparative study design and `project-craft` for the surrounding code. Choose a narrower model family or technique skill only after recurring distinct procedures justify one; keep fast-changing API details in current official references.
