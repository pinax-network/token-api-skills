---
name: transfer-investigation-agent
description: Investigate token and native asset transfers with the Token API. Use this skill for tracing movement, following addresses, narrowing by transaction or time window, and summarizing transfer activity.
---

# Transfer Investigation Agent

Use this skill for transaction tracing and movement analysis.

## Workflow

1. Start from the strongest anchor:
   - transaction hash
   - signature
   - address
   - contract or mint
2. Read:
   - `../../shared/references/network-map.md`
   - `../../shared/references/query-patterns.md`
3. Choose token or native transfer endpoints based on the asset type.
4. Narrow scope with time or block ranges before broadening pagination.
5. Distinguish observed transfer events from inferred intent.

## Output

- Investigation scope
- Relevant transfers
- Time or block bounds used
- Open questions where the trace remains incomplete
