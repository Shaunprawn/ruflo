---
name: site-audit
description: Run a digital presence audit for a client website and marketing channels
---

# Digital Presence Audit

Perform a comprehensive audit of a client's digital marketing presence during onboarding or as a periodic health check.

## Instructions

1. Load client context from memory (website URL, channels, tech stack)
2. If no client loaded, ask for:
   - Website URL
   - Active marketing channels
   - Industry/vertical

3. Conduct the audit:

### Website Audit

**Technical Foundations**
- Site structure and URL patterns
- Mobile responsiveness approach
- Page speed indicators (heavy images, scripts, render-blocking resources)
- SSL/HTTPS status
- Sitemap and robots.txt presence
- Schema markup / structured data
- Core Web Vitals considerations

**On-Page SEO**
- Title tags (unique, keyword-rich, proper length)
- Meta descriptions (compelling, proper length)
- Header hierarchy (H1-H3 structure)
- Image alt text presence
- Internal linking structure
- URL structure (clean, descriptive)
- Content freshness and depth

**Conversion Optimization**
- CTA visibility and clarity
- Form usability (field count, friction points)
- Trust signals (testimonials, logos, certifications)
- Value proposition clarity above the fold
- Navigation and user flow
- Contact information accessibility

**Content Assessment**
- Blog/resource center existence and quality
- Content frequency and recency
- Topic coverage and depth
- Content types (text, video, infographics, tools)
- Lead magnets and gated content

### Channel Audit

**For each active channel, assess:**

#### Paid Search (Google Ads)
- Account structure recommendations
- Keyword strategy observations
- Ad copy quality indicators
- Landing page alignment
- Budget efficiency considerations

#### Paid Social (Meta/LinkedIn/TikTok)
- Audience targeting approach
- Creative quality and variety
- Funnel alignment (awareness → consideration → conversion)
- Retargeting setup indicators
- Platform-specific best practices

#### SEO / Organic
- Domain authority indicators
- Content gap analysis
- Local SEO setup (Google Business Profile)
- Backlink profile observations
- Keyword ranking opportunities

#### Email Marketing
- List health indicators
- Automation/flow setup
- Template design quality
- Segmentation approach
- Deliverability best practices

#### Social Media (Organic)
- Posting frequency and consistency
- Content mix and engagement patterns
- Community management approach
- Platform presence vs. activity
- Bio/profile optimization

### Output Format

```markdown
# Digital Presence Audit: [Client Name]
## Date: [Date]

### Audit Score Summary

| Area | Score (1-10) | Priority |
|------|-------------|----------|
| Website Technical | [score] | [High/Med/Low] |
| On-Page SEO | [score] | [High/Med/Low] |
| Conversion Optimization | [score] | [High/Med/Low] |
| Content Strategy | [score] | [High/Med/Low] |
| Paid Channels | [score] | [High/Med/Low] |
| Organic/SEO | [score] | [High/Med/Low] |
| Email Marketing | [score] | [High/Med/Low] |
| Social Media | [score] | [High/Med/Low] |
| **Overall** | **[avg]** | |

### Critical Issues (Fix Immediately)
1. [Issue + impact + recommended fix]

### High-Impact Opportunities
1. [Opportunity + estimated impact + effort level]

### Detailed Findings

[Per-section detailed analysis with screenshots/examples where possible]

### Recommended Roadmap

| Priority | Action | Channel | Est. Impact | Est. Effort |
|----------|--------|---------|-------------|-------------|
| 1 | [action] | [channel] | [High/Med/Low] | [hours/days] |
| 2 | [action] | [channel] | [High/Med/Low] | [hours/days] |
| ... | | | | |

### Quick Wins (This Week)
- [ ] [Specific, actionable item]
- [ ] [Specific, actionable item]
- [ ] [Specific, actionable item]
```

4. Store audit results in client namespace under `audit-[YYYY-MM]`

## Usage

```
/site-audit acme-corp
/site-audit https://example.com
```
