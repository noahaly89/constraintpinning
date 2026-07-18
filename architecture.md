---
title: Architecture
---
# Reference Architecture

```mermaid
flowchart LR
  A[Policy & Risk Owners] --> B[Constraint Authoring]
  B --> C[Review & Approval]
  C --> D[(Constraint Registry)]
  D --> E[Constraint Contract]
  E --> F[Agent Runtime]
  F --> G[Action Proposal]
  G --> H{Validation Engine}
  H -->|allow| I[Tool Execution]
  H -->|approval| J[Human Gate]
  H -->|block| K[Safe Stop]
  I --> L[(Evidence Store)]
  J --> L
  K --> L
```

## Architectural layers

1. **Governance layer** — ownership, policy interpretation, approval, exception, and review.
2. **Control layer** — registry, contracts, validators, compatibility analysis, and decision logic.
3. **Execution layer** — agents, orchestration, tools, data stores, and external services.
4. **Evidence layer** — logs, decisions, versions, exceptions, and audit records.
