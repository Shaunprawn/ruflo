---
name: client-list
description: List all onboarded clients and their status
---

# Client List

Display all onboarded clients with their key details and account health.

## Instructions

1. Search memory for all client namespaces that contain a `profile` key
2. For each client found, display:

```markdown
# Active Clients

| Client | Industry | Monthly Budget | Primary Goal | Channels | Onboarded | Last Report |
|--------|----------|---------------|--------------|----------|-----------|-------------|
| [name] | [industry] | [$range] | [goal] | [channels] | [date] | [date] |

## Quick Access
- `/client-load [slug]` — Load client context
- `/campaign-brief [slug]` — New campaign brief
- `/content-create [slug]` — Create content
- `/monthly-report [slug]` — Generate report
- `/competitor-analysis [slug]` — Competitor analysis
- `/site-audit [slug]` — Digital presence audit
- `/strategy-plan [slug]` — Quarterly strategy
```

## Usage

```
/client-list
```
