# API Overview

Token API exposes blockchain token and activity data across multiple runtimes.

Current reference groupings:

- Monitoring: health, version, networks
- EVM: tokens, balances, transfers, holders, swaps, pools, NFTs
- SVM: tokens, balances, transfers, holders, swaps
- TVM: expected to follow the same pattern as coverage expands

Design guidance for skills:

- Start from the user's task, not the raw endpoint family.
- Prefer network-aware workflows that can branch into EVM, SVM, or TVM.
- Use shared references for auth, pagination, and common response patterns.
