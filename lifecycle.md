---
title: Constraint Lifecycle
---
# Constraint Lifecycle

```mermaid
stateDiagram-v2
  [*] --> Draft
  Draft --> Review
  Review --> Active: approved
  Review --> Draft: changes required
  Active --> Suspended: temporary hold
  Suspended --> Active: reinstated
  Active --> Deprecated: replacement published
  Deprecated --> Retired
  Retired --> [*]
```

Each transition should capture the actor, timestamp, rationale, and associated approval evidence. Runtime systems must not use draft or retired constraints unless an explicit test environment permits it.
