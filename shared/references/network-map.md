# Network Map

Use this as the routing layer for agent prompts.

## EVM

- Ethereum mainnet
- Base
- BSC
- Polygon
- Arbitrum

Typical identifiers:

- `network`
- `contract`
- `address`
- `transaction_id`

## SVM

- Solana

Typical identifiers:

- `network`
- `mint`
- `owner`
- `signature`

## TVM

- Reserve this file section for TRON-focused conventions as API coverage lands.

Skill guidance:

- Detect chain family early from the identifier format when possible.
- Ask for network clarification only when ambiguity materially changes the query.
