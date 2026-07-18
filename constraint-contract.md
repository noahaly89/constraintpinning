---
title: Constraint Contract
---
# Constraint Contract

A Constraint Contract binds a defined set of constraints to an execution scope.

```json
{
  "contract_id": "PROCUREMENT_AGENT_V1",
  "version": "1.0.0",
  "applies_to": ["procurement-agent"],
  "constraints": ["FIN-001@1.0.0", "PRI-004@1.0.0", "APP-002@2.1.0"],
  "effective_from": "2026-08-01T00:00:00Z",
  "fallback": "block"
}
```

Contracts make the applicable control baseline reviewable, testable, and reproducible.
