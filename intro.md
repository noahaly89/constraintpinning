---
sidebar_position: 1
slug: /intro
title: Introduction
---

# Constraint Pinning Framework

Constraint Pinning is an open governance framework for making critical requirements **explicit, persistent, verifiable, and auditable** throughout an AI agent's lifecycle.

Modern agents can plan, call tools, delegate work, compress context, and operate over long periods. Instructions that matter at the beginning of a workflow can weaken, disappear, conflict, or become difficult to prove later. Constraint Pinning addresses that governance gap.

## The core idea

A critical requirement should not remain an informal sentence inside a prompt. It should be represented as a governed object with an identity, owner, scope, enforcement mode, version, and validation behavior.

```json
{
  "id": "FIN-001",
  "title": "Transaction approval threshold",
  "description": "Human approval is required above SAR 50,000.",
  "category": "financial",
  "severity": "critical",
  "enforcement": "block",
  "owner": "finance-control",
  "scope": ["procurement-agent"],
  "validation_stage": ["pre_action"],
  "version": "1.0.0",
  "audit_required": true
}
```

## What the framework provides

- A standard **Constraint Object**.
- A governed **Constraint Registry**.
- Versioned **Constraint Contracts** for agents and workflows.
- A lifecycle for creation, activation, validation, exception, and retirement.
- An enforcement pipeline that evaluates proposed actions before execution.
- Evidence that supports audit, incident review, and accountability.

## Project status

Version 1.0 is a foundation release. The specifications are intentionally implementation-neutral and open for review through the RFC process.
