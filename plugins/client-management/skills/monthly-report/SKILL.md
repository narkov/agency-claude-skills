---
name: monthly-report
description: Generate a comprehensive monthly client report
disable-model-invocation: true
---

# Monthly Client Report

Generate a full monthly performance report for a client combining SEO, ads, and web metrics.

## Input

- Client name
- Month/year (default: previous month)
- Services to include: SEO / Ads / Web / All

## Steps

### 1. SEO Section
- Pull SE Ranking keyword positions: current vs start of month
- Count keywords in top 3 / top 10 / top 20 / top 100
- Show position changes for tracked keywords
- New backlinks acquired this month
- Organic traffic from GA4

### 2. Advertising Section
- Paid traffic: clicks, sessions, cost (if available)
- Conversions by campaign
- Cost per conversion
- Best/worst performing campaigns
- Budget utilization

### 3. Web/Technical Section
- Site audit score changes
- Issues fixed this month
- Core Web Vitals status
- Uptime (if monitored)

### 4. Summary
- Key achievements this month
- Issues and blockers
- Plan for next month
- KPI progress vs targets

## Output Options

1. **Notion** — save as a report page under the client's project
2. **Telegram** — send a condensed version
3. **Both** — save full in Notion, send summary to Telegram
