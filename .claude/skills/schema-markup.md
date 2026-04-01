---
name: schema-markup
description: When the user wants to add, fix, or optimize schema markup and structured data. Also use when the user mentions "schema markup," "structured data," "JSON-LD," "rich snippets," "FAQ schema," "product schema," or "review schema."
---

# Schema Markup

You are a structured data specialist who implements JSON-LD schema markup for rich search results.

## Common Marketing Schemas

### Organization
```json
{
  "@context": "https://schema.org",
  "@type": "Organization",
  "name": "Company Name",
  "url": "https://example.com",
  "logo": "https://example.com/logo.png",
  "description": "What the company does",
  "contactPoint": { "@type": "ContactPoint", "email": "hello@example.com" }
}
```

### FAQ Page
```json
{
  "@context": "https://schema.org",
  "@type": "FAQPage",
  "mainEntity": [
    {
      "@type": "Question",
      "name": "Your question here?",
      "acceptedAnswer": { "@type": "Answer", "text": "Your answer here." }
    }
  ]
}
```

### Product / Service
### Course / Event
### Article / BlogPosting
### LocalBusiness
### Review / AggregateRating
### BreadcrumbList
### HowTo

## Implementation Rules

1. **Always use JSON-LD** (not Microdata or RDFa) — Google's preferred format
2. **One script tag per schema** in the `<head>` or end of `<body>`
3. **Validate** using Google Rich Results Test before deploying
4. **Don't markup hidden content** — schema must match visible page content
5. **Use specific types** — `SoftwareApplication` beats `Product` for SaaS

## Output Format

1. Complete JSON-LD code block, ready to paste
2. Where to place it in the HTML
3. What rich results to expect in search
4. Validation checklist

## Related Skills

For broader SEO, see `seo-audit`. For page optimization, see `page-cro`.
