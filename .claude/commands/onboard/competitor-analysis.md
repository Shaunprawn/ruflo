---
name: competitor-analysis
description: Run a competitor analysis using parallel agents for a client
---

# Competitor Analysis

Run a structured competitive analysis using the client's stored competitor list and industry data.

## Instructions

1. Load client context — specifically `competitors` and `target-audience` from their namespace
2. If no competitors stored, ask the user to provide 3-5 competitor names/URLs
3. For each competitor, analyze:

### Analysis Framework

**For each competitor, evaluate:**

#### Positioning & Messaging
- What is their core value proposition?
- What language/tone do they use?
- Who are they targeting?
- What pain points do they address?

#### Digital Presence
- Website quality and UX observations
- Content strategy (blog frequency, topics, depth)
- Social media presence and engagement style
- Email marketing (sign up and note welcome flow if possible)
- Paid advertising presence (note any visible ads)

#### Strengths & Weaknesses
- What do they do well that we should learn from?
- Where are they weak that our client can exploit?
- What are they missing entirely?

#### SEO Indicators
- Content themes and keyword focus areas
- Site structure and navigation patterns
- Blog/resource center depth and quality

### Output Format

```markdown
# Competitive Analysis: [Client Name]
## Date: [Date]

### Market Landscape Summary
[Overview of competitive environment, market positioning map]

### Competitor Profiles

#### [Competitor 1]
- **URL**: [url]
- **Positioning**: [their core message]
- **Target Audience**: [who they speak to]
- **Strengths**: [what they do well]
- **Weaknesses**: [where they fall short]
- **Content Strategy**: [what they publish, how often, what topics]
- **Key Takeaway**: [one actionable insight]

[Repeat for each competitor]

### Opportunity Matrix

| Opportunity | Competitors Missing It | Difficulty | Impact | Priority |
|------------|----------------------|------------|--------|----------|
| [gap] | [which ones] | [Low/Med/High] | [Low/Med/High] | [1-5] |

### Differentiation Strategy
[How the client should position against these competitors]

### Content Gaps
[Topics/formats competitors aren't covering that the client should own]

### Quick Wins
1. [Actionable item the client can do this week]
2. [Actionable item]
3. [Actionable item]
```

4. Store results in client namespace under `competitor-analysis-[YYYY-MM]`

## Usage

```
/competitor-analysis acme-corp
```
