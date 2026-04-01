---
name: client-load
description: Load a client profile from memory to set context for all subsequent work
---

# Load Client Context

Load a previously onboarded client's full profile into the current session context.

## Instructions

1. Ask the user which client to load (or use the argument provided)
2. Retrieve all stored data from the client's memory namespace
3. Display a brief summary of the loaded context
4. Confirm the session is now "in context" for that client

## Keys to Retrieve

From namespace `[client-slug]`:
- `profile` — business basics
- `brand-voice` — tone and style guide
- `target-audience` — personas and demographics
- `competitors` — competitive landscape
- `goals-kpis` — targets and metrics
- `channels` — active marketing channels
- `tech-stack` — platforms and tools
- `notes` — additional context

## After Loading

Confirm to the user:
> Client context loaded: **[Client Name]**
> - Brand voice: [tone summary]
> - Primary goal: [goal]
> - Active channels: [channels]
> - Budget: [range]
>
> All content, campaigns, and reports will use this client's context.

## Usage

```
/client-load acme-corp
```
