---
name: site-audit
description: Run a comprehensive SEO audit for a client website
disable-model-invocation: true
---

# Site Audit

Run a comprehensive SEO audit for the given domain. Use SE Ranking audit tools if available via MCP.

## Steps

1. Ask for the domain if not provided
2. Check if a project exists in SE Ranking for this domain
3. Run or fetch the latest audit report
4. Analyze critical issues grouped by category:
   - **Technical**: crawl errors, broken links, redirect chains, missing robots.txt/sitemap
   - **On-page**: missing/duplicate titles, meta descriptions, H1 tags, thin content
   - **Performance**: page speed issues, large images, render-blocking resources
   - **Mobile**: mobile usability issues
5. Prioritize issues by impact (critical → warnings → notices)
6. Format a summary with top 10 actionable fixes

## Output format

```
## SEO Audit: [domain]
Date: [date]

### Critical Issues ([count])
- Issue: [description] — [affected pages count] pages
  Fix: [actionable recommendation]

### Warnings ([count])
...

### Quick Wins
1. [highest impact / lowest effort fixes]
```
