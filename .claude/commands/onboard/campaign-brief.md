---
name: campaign-brief
description: Generate a campaign brief using stored client context
---

# Campaign Brief Generator

Create a structured campaign brief using the client's stored profile, brand voice, audience data, and goals.

## Instructions

1. Load the client context from memory (ask which client if not specified)
2. Ask the user for campaign-specific details:
   - Campaign name/theme
   - Campaign objective (awareness, leads, sales, retention)
   - Channels to activate (or recommend based on client profile)
   - Duration and timeline
   - Specific offers, promotions, or messaging hooks
   - Budget allocation (or use client's default)

3. Generate the brief using this structure:

## Brief Template

```markdown
# Campaign Brief: [Campaign Name]
## Client: [Client Name] | Date: [Date]

### Objective
[What this campaign aims to achieve, tied to client KPIs]

### Target Audience
[From stored persona data — demographics, pain points, motivations]

### Key Message
[Core message aligned with brand voice]

### Supporting Messages
1. [Message pillar 1]
2. [Message pillar 2]
3. [Message pillar 3]

### Brand Voice Reminders
- Tone: [from stored brand voice]
- Do: [guidelines]
- Don't: [guidelines]

### Channel Plan
| Channel | Format | Budget | Timeline | KPI |
|---------|--------|--------|----------|-----|
| [channel] | [ad/post/email] | [$] | [dates] | [metric] |

### Creative Requirements
- [ ] Ad copy variations (x per channel)
- [ ] Landing page
- [ ] Email sequence
- [ ] Social posts
- [ ] Visual assets needed

### Success Metrics
| KPI | Target | Measurement |
|-----|--------|-------------|
| [metric] | [target] | [how measured] |

### Timeline
| Week | Milestone |
|------|-----------|
| 1 | [setup/creative] |
| 2 | [launch] |
| 3-4 | [optimize] |

### Approvals Required
- [ ] Client approval on messaging
- [ ] Creative approval
- [ ] Budget sign-off
- [ ] Landing page review
```

4. Store the brief in client memory namespace under key `campaign-[slug]`

## Usage

```
/campaign-brief acme-corp
```
