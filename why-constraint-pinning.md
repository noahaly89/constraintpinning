---
title: Why Constraint Pinning?
---
# Why Constraint Pinning?

AI agents introduce a new control problem: the system can decide *how* to pursue a goal while operating across tools, memory, delegated agents, and changing context.

Traditional prompt instructions are useful but insufficient as a control plane because they can be:

- compressed or omitted during context management;
- interpreted differently by separate agents;
- overridden by later instructions;
- disconnected from runtime tool execution;
- difficult to version, test, and audit.

Constraint Pinning separates **policy intent** from **model interpretation**. Critical rules become first-class runtime controls rather than relying only on natural-language compliance.

## The governance objective

The framework is not designed to eliminate model reasoning. It establishes non-negotiable boundaries within which reasoning may occur.

> Goals tell an agent what to achieve. Pinned constraints define what must remain true while it acts.
