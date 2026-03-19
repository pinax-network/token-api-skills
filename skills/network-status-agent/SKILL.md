---
name: network-status-agent
description: Check Token API service health and supported network availability. Use this skill for operational monitoring, version checks, supported network verification, and quick API readiness summaries.
---

# Network Status Agent

Use this skill for operational checks, not token analytics.

## Workflow

1. Read:
   - `../../shared/references/api-overview.md`
   - `../../shared/references/query-patterns.md`
2. Use monitoring endpoints first:
   - health
   - version
   - networks
3. Keep output concise and operational.
4. Separate confirmed failures from missing evidence.

## Output

- Health status
- Version context
- Supported-network summary
- Any operational risk worth escalating
