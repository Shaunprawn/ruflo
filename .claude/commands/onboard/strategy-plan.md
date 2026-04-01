---
name: strategy-plan
description: Generate a quarterly marketing strategy for a client using stored context
---

# Quarterly Strategy Planner

Build a data-informed quarterly marketing strategy using the client's stored profile, past performance, competitive analysis, and goals.

## Instructions

1. Load full client context from memory:
   - `profile` — business basics
   - `goals-kpis` — targets
   - `competitors` — landscape
   - `channels` — active channels
   - Previous `report-*` entries for trend data
   - Previous `audit-*` entries for known issues
   - Previous `competitor-analysis-*` for market context

2. Ask the user:
   - Which quarter? (Q1/Q2/Q3/Q4 + year)
   - Any new priorities or shifts from the client?
   - Budget changes?
   - New product/service launches?
   - Seasonal considerations?

3. Generate the strategy:

## Strategy Template

```markdown
# Quarterly Marketing Strategy: [Client Name]
## [Quarter] [Year]
## Prepared: [Date]

---

### Strategic Context

**Business Situation**
[Summary of where the client is today — performance trends, market position]

**Key Insights from Last Quarter**
- [Insight from reports/audits with data]
- [Insight]
- [Insight]

**Market & Competitive Context**
[Relevant shifts from competitor analysis, industry trends]

---

### Strategic Priorities

#### Priority 1: [Strategic Theme]
**Objective**: [Specific, measurable goal]
**Why Now**: [Business rationale]
**Channels**: [Which channels support this]
**KPI**: [How we measure success]

#### Priority 2: [Strategic Theme]
**Objective**: [Specific, measurable goal]
**Why Now**: [Business rationale]
**Channels**: [Which channels support this]
**KPI**: [How we measure success]

#### Priority 3: [Strategic Theme]
**Objective**: [Specific, measurable goal]
**Why Now**: [Business rationale]
**Channels**: [Which channels support this]
**KPI**: [How we measure success]

---

### Channel Plans

#### [Channel 1]
| Month | Focus | Tactics | Budget | Target KPI |
|-------|-------|---------|--------|------------|
| Month 1 | [focus] | [tactics] | [$] | [target] |
| Month 2 | [focus] | [tactics] | [$] | [target] |
| Month 3 | [focus] | [tactics] | [$] | [target] |

[Repeat for each active channel]

---

### Content Calendar Themes

| Month | Theme | Content Pieces | Channels | Tie-In |
|-------|-------|---------------|----------|--------|
| Month 1 | [theme] | [blog, social, email, etc.] | [channels] | [campaign/seasonal] |
| Month 2 | [theme] | [pieces] | [channels] | [tie-in] |
| Month 3 | [theme] | [pieces] | [channels] | [tie-in] |

---

### Budget Allocation

| Channel | Monthly Budget | Quarterly Total | % of Total | Rationale |
|---------|---------------|-----------------|------------|-----------|
| [channel] | [$] | [$] | [%] | [why this allocation] |
| **Total** | **[$]** | **[$]** | **100%** | |

---

### Testing & Experimentation

| Test | Hypothesis | Channel | Timeline | Success Criteria |
|------|-----------|---------|----------|-----------------|
| [test] | [if we do X, then Y] | [channel] | [when] | [metric] |

---

### Risk Factors & Contingencies

| Risk | Probability | Impact | Mitigation |
|------|------------|--------|------------|
| [risk] | [Low/Med/High] | [Low/Med/High] | [plan B] |

---

### Milestones & Review Cadence

| Date | Milestone | Review Action |
|------|-----------|---------------|
| Month 1, Week 2 | Campaign launches live | Performance check |
| Month 1, End | First month report | Optimize or pivot |
| Month 2, Mid | Mid-quarter review | Budget reallocation if needed |
| Month 3, End | Quarter close | Full performance review + Q+1 planning |

---

### Success Criteria

This quarter is successful if:
1. [KPI 1] reaches [target] (currently [baseline])
2. [KPI 2] reaches [target] (currently [baseline])
3. [KPI 3] reaches [target] (currently [baseline])
```

4. Store in client namespace under `strategy-[quarter]-[year]`

## Usage

```
/strategy-plan acme-corp Q2 2026
```
