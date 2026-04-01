---
name: product-context
description: When the user wants to create or update their product/brand context document. Also use when the user mentions "product context," "brand context," "set up context," "positioning," or wants to avoid repeating foundational information across marketing tasks.
---

# Product Marketing Context

You help create a reusable context document that all other marketing skills reference. This is the foundation — set it up once, and every skill automatically uses it.

## What This Creates

A `.claude/product-context.md` file containing:

### 1. Company & Product
- Company name
- What you sell (1 sentence)
- Product/service category
- Website URL

### 2. Target Audience (ICP)
- Primary audience (role, seniority, industry)
- Secondary audiences
- Company size / type (B2B, B2C, enterprise, SMB)
- Geographic focus

### 3. Value Proposition
- Core problem you solve
- How you solve it differently
- Key benefits (top 3)
- Competitive advantage

### 4. Brand Voice & Tone
- Voice characteristics (e.g., "professional but approachable")
- Words/phrases to USE
- Words/phrases to AVOID
- Example sentence in brand voice

### 5. Competitive Landscape
- Top 3 competitors
- How you differentiate from each
- Your unique positioning

### 6. Key Metrics & Social Proof
- Customer count, revenue, growth stats
- Notable customers or logos
- Awards, certifications, press mentions
- Key testimonials or case studies

## Process

Ask the user these questions one section at a time. Keep it conversational — don't overwhelm with all questions at once. After gathering info, generate the `.claude/product-context.md` file.

## Output

Save to `.claude/product-context.md` in clean markdown format. This file will be automatically read by all other marketing skills (copywriting, cold-email, ad-creative, etc.) to ensure consistent messaging.

## Related Skills

All marketing skills check for this file. Create it first for the best results.
