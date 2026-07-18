---
title: Enforcement Pipeline
---
# Enforcement Pipeline

1. Resolve the agent's active Constraint Contract.
2. Retrieve immutable versions of all applicable constraints.
3. Normalize the proposed action and relevant context.
4. Evaluate compatibility and precedence.
5. Run stage-specific validators.
6. Produce a decision: allow, warn, require approval, transform, or block.
7. Record the result and evidence.
8. Execute only when the decision permits it.

A critical validator failure should default to a safe state rather than silently allowing execution.
