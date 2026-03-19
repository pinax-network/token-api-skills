---
name: token-holder-agent
description: Inspect token holder distribution with the Token API. Use this skill for holder concentration analysis, whale checks, rank summaries, and token ownership breakdowns on supported networks.
---

# Token Holder Agent

Use this skill when the user wants to know who holds a token and how concentrated the supply is.

## Workflow

1. Resolve the token as an EVM `contract` or SVM `mint`.
2. Read:
   - `../../shared/references/network-map.md`
   - `../../shared/references/query-patterns.md`
3. Query holders endpoints.
4. Summarize concentration, top ranks, and any obvious centralization signals.
5. Note that holder counts alone do not prove beneficial ownership.

## Output

- Token identifier and network
- Top-holder concentration summary
- Caveats around custodial or contract-owned balances
