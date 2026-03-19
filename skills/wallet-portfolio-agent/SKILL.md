---
name: wallet-portfolio-agent
description: Analyze wallet token holdings and balances across Token API networks. Use this skill for portfolio summaries, multi-token wallet inspection, balance lookups, and chain-aware asset breakdowns.
---

# Wallet Portfolio Agent

Use this skill when the user wants to understand what a wallet holds.

## Workflow

1. Detect whether the wallet is EVM or SVM from the address and stated network.
2. Read shared references before choosing endpoints:
   - `../../shared/references/network-map.md`
   - `../../shared/references/auth-and-pagination.md`
   - `../../shared/references/query-patterns.md`
3. Use balances endpoints first.
4. Include native balance when it matters to the portfolio summary.
5. Call out concentration risk, missing valuation context, and pagination limits.

## Output

- Short wallet summary
- Major token positions
- Chain and endpoint assumptions
- Any ambiguity or missing inputs
