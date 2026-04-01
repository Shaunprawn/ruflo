---
name: onboard-help
description: Show all available client onboarding commands and workflows
---

# Client Onboarding System — Command Reference

A complete client management toolkit for digital marketing agencies.

## Onboarding Workflow

Run these in order for new clients:

```
Step 1:  /onboard                        — Full intake wizard (profile, brand, goals, audit)
Step 2:  /competitor-analysis [client]    — Deep competitive analysis
Step 3:  /site-audit [client]             — Digital presence audit
Step 4:  /strategy-plan [client] Q2 2026  — Quarterly strategy
Step 5:  /campaign-brief [client]         — First campaign brief
```

## Day-to-Day Commands

| Command | What It Does |
|---------|-------------|
| `/client-list` | Show all onboarded clients |
| `/client-load [client]` | Load a client's context into session |
| `/content-create [client] [type]` | Generate on-brand content |
| `/campaign-brief [client]` | Create a new campaign brief |
| `/monthly-report [client]` | Generate monthly performance report |
| `/competitor-analysis [client]` | Run/refresh competitor analysis |
| `/site-audit [client]` | Run/refresh digital presence audit |
| `/strategy-plan [client] [quarter]` | Build quarterly strategy |

## Content Types (for /content-create)

- `blog` — Blog posts with SEO structure
- `social-meta` — Facebook/Instagram posts
- `social-linkedin` — LinkedIn posts
- `social-tiktok` — TikTok scripts
- `email-welcome` — Welcome sequence
- `email-nurture` — Nurture sequence
- `email-promo` — Promotional email
- `ads-google` — Google Ads copy
- `ads-meta` — Meta Ads copy
- `ads-linkedin` — LinkedIn Ads copy
- `landing-page` — Landing page copy
- `newsletter` — Newsletter content
- `case-study` — Case study outline
- `video-script` — Video script outline

## How Client Memory Works

Each client gets a memory namespace (e.g., `acme-corp`) with these keys:

| Key | Content |
|-----|---------|
| `profile` | Business basics, contact, budget |
| `brand-voice` | Tone, style, dos/don'ts |
| `target-audience` | Personas, demographics, pain points |
| `competitors` | Competitor names and URLs |
| `goals-kpis` | Measurable targets |
| `channels` | Active marketing channels |
| `tech-stack` | CMS, CRM, analytics tools |
| `notes` | Additional context |
| `audit-YYYY-MM` | Site audit results |
| `competitor-analysis-YYYY-MM` | Competitive analysis |
| `report-YYYY-MM` | Monthly reports |
| `metrics-YYYY-MM` | Raw metrics for trends |
| `strategy-Q#-YYYY` | Quarterly strategies |
| `campaign-[slug]` | Campaign briefs |
| `content-[type]-[date]` | Generated content |

Context persists across sessions. Load any client with `/client-load [slug]`.
