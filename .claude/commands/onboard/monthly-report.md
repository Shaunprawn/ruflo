---
name: monthly-report
description: Generate a monthly performance report using client context and KPIs
---

# Monthly Report Generator

Generate a structured monthly marketing performance report using the client's stored KPIs, channels, and historical context.

## Instructions

1. Load client context from memory
2. Ask the user for this month's data (or guide them to paste it):
   - Channel performance metrics (impressions, clicks, conversions, spend, revenue)
   - Key wins and highlights
   - Issues or underperformance areas
   - Any external factors (seasonality, market changes, client-side changes)

3. Generate the report:

## Report Template

```markdown
# Monthly Marketing Report: [Client Name]
## Period: [Month Year]
## Prepared by: [Agency Name]

---

### Executive Summary
[2-3 sentence overview: what happened, what it means, what's next]

### KPI Dashboard

| KPI | Target | Actual | vs Target | vs Last Month | Trend |
|-----|--------|--------|-----------|---------------|-------|
| [metric] | [target] | [actual] | [+/-] | [+/-] | [arrow] |

### Channel Performance

#### [Channel 1]
- **Spend**: $X (budget: $Y)
- **Key Metrics**: [impressions, clicks, CTR, conversions, CPA, ROAS]
- **What Worked**: [highlights]
- **What Didn't**: [issues]
- **Next Month**: [action items]

[Repeat for each active channel]

### Wins This Month
1. [Win with data]
2. [Win with data]
3. [Win with data]

### Challenges & Learnings
1. [Challenge + what we learned + action taken]

### Competitive Updates
[Any notable competitor activity observed]

### Recommendations for Next Month
1. **[Action]** — [Expected impact] — Priority: [High/Med/Low]
2. **[Action]** — [Expected impact] — Priority: [High/Med/Low]
3. **[Action]** — [Expected impact] — Priority: [High/Med/Low]

### Budget Summary

| Channel | Allocated | Spent | Remaining | Recommendation |
|---------|-----------|-------|-----------|----------------|
| [channel] | [$] | [$] | [$] | [reallocate/maintain/increase] |
| **Total** | **[$]** | **[$]** | **[$]** | |

### 30-Day Action Plan
- [ ] [Specific action with owner and deadline]
- [ ] [Specific action with owner and deadline]
- [ ] [Specific action with owner and deadline]

---
*Next report: [Date]*
```

4. Store the report in client namespace under `report-[YYYY-MM]`
5. Store key metrics under `metrics-[YYYY-MM]` for trend analysis

## Usage

```
/monthly-report acme-corp
```
