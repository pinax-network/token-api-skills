---
name: api-integration-helper
description: Help developers integrate with the Token API. Use this skill for choosing endpoints, mapping user needs to request parameters, explaining auth and pagination, and drafting implementation-ready API call plans.
---

# API Integration Helper

Use this skill when the user is building against the API rather than analyzing chain data directly.

## Workflow

1. Read all shared references relevant to the request:
   - `../../shared/references/api-overview.md`
   - `../../shared/references/auth-and-pagination.md`
   - `../../shared/references/network-map.md`
   - `../../shared/references/query-patterns.md`
2. Map the user goal to the smallest useful endpoint set.
3. Prefer explicit request examples over broad endpoint dumps.
4. Note assumptions about network, identifier type, and pagination.

## Output

- Endpoint recommendation
- Required parameters
- Optional filters worth using
- Integration caveats and next request to make
