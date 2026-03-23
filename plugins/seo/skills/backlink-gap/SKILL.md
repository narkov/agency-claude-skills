---
name: backlink-gap
description: Find backlink opportunities by comparing with competitors
disable-model-invocation: true
---

# Backlink Gap Analysis

Find backlink opportunities that competitors have but the client doesn't.

## Steps

1. Take the client domain and 2-4 competitor domains
2. If competitors not provided, use SE Ranking competitor discovery or SERP-based discovery
3. Pull referring domains for each domain via backlinks API
4. Find domains linking to competitors but NOT to the client
5. **Filter out spam/junk domains**:
   - SEO tool/directory spam (seo-tip.com, backlink.wiki, etc.)
   - URL shorteners
   - Forum spam networks (forumotion, creartuforo, forum.cool)
   - Foreign hacked sites
   - Domains with DA < 10
6. Score remaining opportunities by:
   - Domain Authority
   - Relevance to client's niche
   - Number of competitors linking from this domain
7. Categorize opportunities: guest posts, directories, news/PR, resource pages, forums

## Output format

```
## Backlink Gap: [client] vs [competitors]

### Top Opportunities ([count])

| Domain | DA | Type | Competitors linking | Action |
|--------|-----|------|-------------------|--------|

### Summary
- Total unique opportunities: [count]
- By type: [breakdown]
- Recommended outreach priority: [top 10]
```
