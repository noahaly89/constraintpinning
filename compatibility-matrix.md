---
title: Compatibility Matrix
---
# Constraint Compatibility Matrix

Constraints can conflict even when each is valid in isolation. A compatibility matrix documents known relationships and precedence.

| Constraint A | Constraint B | Relationship | Resolution |
|---|---|---|---|
| Budget limit | Emergency response | Conditional conflict | Emergency exception with time limit and approval. |
| Privacy minimization | Audit logging | Tension | Log decision metadata without prohibited content. |
| Human approval | Automatic execution | Direct conflict | Human approval takes precedence. |

Conflicts should be resolved before deployment. Runtime discovery of an unresolved critical conflict should trigger a safe stop.
