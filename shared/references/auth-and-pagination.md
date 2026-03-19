# Auth And Pagination

Authentication:

- Use `Authorization: Bearer <token>` when possible.
- Support `X-Api-Key` when bearer auth is not available.

Common list parameters:

- `limit`
- `page`

Skill guidance:

- Default to conservative page sizes unless the user asks for exhaustive output.
- Call out partial results when pagination may hide long tails.
- Prefer exact filters such as `network`, `contract`, `address`, `mint`, or time
  windows before increasing page size.
