---
name: dex-liquidity-agent
description: Analyze DEX pools, swaps, and liquidity activity with the Token API. Use this skill for pool inspection, swap flow analysis, protocol checks, and liquidity-oriented market summaries.
---

# DEX Liquidity Agent

Use this skill when the user wants market structure rather than simple balances.

## Workflow

1. Identify the chain, protocol, and pool if available.
2. Read:
   - `../../shared/references/network-map.md`
   - `../../shared/references/query-patterns.md`
3. Use pools, swaps, and OHLCV-style endpoints where available.
4. Prefer normalized user-oriented fields when the API exposes them.
5. Make clear which conclusions are direct observations versus interpretations.

## Output

- Protocol and pool context
- Recent trading or liquidity patterns
- Key addresses or assets involved
- Data gaps and endpoint limitations
