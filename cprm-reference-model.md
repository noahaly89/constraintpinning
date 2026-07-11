# Constraint Pinning Reference Model (CPRM)

**Version:** 0.1  
**Status:** Discussion Draft  
**Author:** Noah Alrajab  

## Purpose

The Constraint Pinning Reference Model provides a technology-neutral structure for understanding where governance constraints should exist in an AI-agent workflow.

## The Seven Layers

1. **Intent** — Defines the requested outcome.
2. **Constraint Registry** — Stores authoritative constraints and metadata.
3. **Context Resolver** — Determines which constraints apply.
4. **Pinning Layer** — Maintains applicable critical constraints as persistent execution state.
5. **Decision Validator** — Tests intended actions against active constraints.
6. **Tool and Action Gateway** — Controls external execution.
7. **Evidence and Audit** — Records constraints, decisions, approvals, exceptions, and outcomes.

## Reference Outcomes

- Allow
- Block
- Approval Required
- Clarification Required
- Escalate
- Log Only

## Example Constraint Object

```json
{
  "id": "FIN-001",
  "title": "Procurement Budget Limit",
  "category": "Financial",
  "severity": "Critical",
  "enforcement": "Approval Required",
  "owner": "Finance",
  "scope": "Procurement",
  "rule": "Purchases above SAR 50,000 require human approval.",
  "validation_stage": "Pre-execution",
  "version": "1.0",
  "audit": true
}
```

## Position

The CPRM is a discussion draft, technology-neutral, and implementation-agnostic. It is not a regulatory standard or certification model.
