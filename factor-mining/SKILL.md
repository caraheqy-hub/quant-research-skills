---
name: factor-mining
description: Research, reproduce, and evaluate public-market quantitative factors from brokerage reports, papers, and factor libraries; use for factor discovery, factor catalogs, and A-share signal validation.
---

# Factor mining

Turn a source into a testable hypothesis, then into a reproducible result. Keep **source claims**, **implementation choices**, and **measured results** separate.

## Choose evidence before code

- Search current original brokerage reports, academic papers, official platform documentation, and maintained source code. Record author, publication date, original URL, page or code location, and access limits. Community posts can suggest ideas but do not verify a report's formula.
- Classify each candidate: `exact formula`, `partial description`, or `idea only`. Do not implement a purported report replication from a title, abstract, or inaccessible formula. Label adaptations explicitly.
- Maintain a trial ledger that includes rejected ideas and every parameter tried. A broad search is a catalog; it is not evidence that all catalog entries work.
- Before sharing a project publicly, check report copyright and market-data license terms. Link sources and publish your own method and derived findings; keep restricted raw reports and bars out of the repository.

## Define the experiment

For each candidate, write a compact factor card: economic intuition, mathematical expression and sign, fields and units, lookback, universe, frequency, neutralization, missing-value rule, source time range, **earliest usable timestamp**, signal timestamp, execution timestamp, and future-return label. For financial statements, analyst forecasts, constituents, and classifications, use the actual publication or effective date and record revisions. When point-in-time history is unavailable, mark the backtest as exploratory.

Compare candidates on the same dates and investable universe. Use only past information at each signal date. Separate discovery, parameter selection, and later evaluation; once a holdout influences a decision, mark it as seen. Assess coverage, cross-sectional Rank IC, distribution by period/industry, quantile monotonicity, turnover, transaction costs, liquidity/capacity, and exposure to size/industry/known factors. Test whether a new factor adds information beyond a simpler existing one. Avoid presenting an in-sample winner or raw IC as deployable alpha; many trials raise false-discovery risk.

For A-share execution, account for next-session entry, suspensions, price limits, ST status, corporate actions, and the chosen long-only or hedge constraints. State what the data cannot model. A few securities or retrospectively adjusted bars can demonstrate code flow but cannot establish a live edge.

## Reuse the right capability

- Use `project-craft` for a substantial code project and `jupyter-notebooks` when a rerunnable notebook improves review.
- Use the available Public Equity Investing skills for company fundamentals, filings, financial statement normalization, valuation, and portfolio risk when those tasks actually arise. Quant signal generation stays in this workflow.
- Use `juejinquant` for local GoldMiner/GM API details, and cross-check changing endpoints against official SDK documentation. Never place tokens in code or outputs.
- Use `debug-ledger` when an SDK call, factor calculation, or backtest fails; consult matching cases without assuming the same root cause.

Read [methodology](references/methodology.md) when designing a new experiment or reviewing a factor claim. Read [source and factor card](references/source-card.md) when importing a report, paper, or community idea.
