---
name: quant-projects
description: Route and conduct personal quantitative-finance research and engineering projects involving market data, signals, strategies, backtests, or execution. Use after project inception; select asset and platform specifics only when they affect the method. Excludes generic company valuation or personal financial advice.
---

# Quant projects

Begin with the project's hypothesis or system objective, investable universe, asset class, venue, frequency, data entitlement, and intended output. Choose the research path before a trading platform.

## Method

- For a signal or factor, use `factor-mining` for source discovery, point-in-time design, trial records, replication, and validation. Keep platform and asset choices explicit here; do not repeat the factor protocol in this entrypoint.
- For a strategy or portfolio, state the decision rule, constraints, position sizing, risk exposure, and realistic order path. Separate a research backtest from paper or live trading. Verify data timestamps, survivorship, corporate actions, liquidity and asset-specific market mechanics.
- For a strategy or portfolio, compare against a simple baseline on the same dates, universe and costs. Keep development and later evaluation separate; report uncertainty and failure cases, not just the best equity curve.
- Use `project-craft` for implementation and `debug-ledger` for reproduced SDK, data or backtest failures.

## Subdomain routing

- **Platform:** Use `juejinquant` when the user has selected GM/MyQuant/GoldMiner or its SDK. Check changing endpoints against current official docs. Other platforms need their own reference or skill only after a recurring, distinctive workflow is observed.
- **Asset:** Record stock, ETF, bond, convertible bond, futures, options, crypto, or other asset mechanics in the project design. Split an asset into its own skill when repeated projects need different data provenance, execution rules and validation. Do not assume A-share rules apply to other venues.
- **Research type:** Factor discovery, strategy evaluation, portfolio construction and execution can share this entrypoint while using focused methods where available.

For a public deliverable, check data and report licenses before sharing raw material or derived files.
