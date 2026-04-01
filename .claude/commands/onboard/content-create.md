---
name: content-create
description: Generate marketing content using stored client brand voice and audience data
---

# Content Creator

Generate on-brand marketing content using the client's stored profile, brand voice, and audience data.

## Instructions

1. Load client context from memory
2. Ask what content is needed (or use the argument):
   - Blog post
   - Social media posts (specify platform)
   - Email (welcome, nurture, promotional, re-engagement)
   - Ad copy (Google, Meta, LinkedIn)
   - Landing page copy
   - Newsletter
   - Case study outline
   - Video script outline

3. For each content type, automatically apply:
   - **Brand voice** from stored profile
   - **Target audience** language and pain points
   - **USPs** woven into messaging
   - **CTAs** aligned with campaign goals
   - **SEO keywords** where relevant

## Content Guidelines

### Blog Posts
- Write in the client's brand voice
- Include H2/H3 structure for SEO
- Open with the audience's pain point
- Close with clear CTA
- Suggest meta title and description
- Recommend internal/external links

### Social Media
- Platform-specific formatting (character limits, hashtag conventions)
- Multiple variations for A/B testing
- Mix of content types: educational, promotional, engagement, social proof
- Include suggested posting times based on platform best practices

### Email Copy
- Subject line variations (3-5 options)
- Preview text
- Body copy with personalization tokens
- Clear single CTA
- Mobile-first formatting

### Ad Copy
- Headline variations (5-10)
- Description variations (5-10)
- Platform-specific specs (character limits, formats)
- Audience targeting recommendations
- Negative keyword suggestions (for search)

### Landing Pages
- Hero section with headline + subheadline
- Problem/solution framework
- Social proof section
- Feature/benefit blocks
- FAQ section
- CTA placement strategy
- Form field recommendations

## Output

Store all generated content in client namespace under `content-[type]-[date]`

## Usage

```
/content-create acme-corp blog "5 Ways to Reduce Cloud Costs"
/content-create acme-corp social-meta "Product launch campaign"
/content-create acme-corp email-nurture "Welcome sequence"
/content-create acme-corp ads-google "Lead gen campaign"
```
