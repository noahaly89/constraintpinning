---
title: Constraint Object
---
# Constraint Object Specification

## Required fields

| Field | Type | Description |
|---|---|---|
| `id` | string | Stable, unique identifier. |
| `title` | string | Human-readable name. |
| `description` | string | Normative requirement. |
| `category` | string | Governance domain. |
| `severity` | enum | `low`, `medium`, `high`, or `critical`. |
| `enforcement` | enum | `observe`, `warn`, `approve`, `transform`, or `block`. |
| `owner` | string | Accountable role or entity. |
| `scope` | array | Systems, agents, tools, actions, or environments covered. |
| `validation_stage` | array | Checkpoints at which evaluation occurs. |
| `version` | string | Semantic version. |
| `status` | enum | `draft`, `active`, `suspended`, `deprecated`, or `retired`. |

## Example

```json
{
  "id": "PRI-004",
  "title": "Personal data export restriction",
  "description": "Personal data must not be exported outside approved regions.",
  "category": "privacy",
  "severity": "critical",
  "enforcement": "block",
  "owner": "data-protection-office",
  "scope": ["customer-service-agent", "export-tool"],
  "validation_stage": ["pre_tool_call", "post_tool_response"],
  "version": "1.0.0",
  "status": "active",
  "audit_required": true,
  "effective_from": "2026-07-18T00:00:00Z"
}
```
