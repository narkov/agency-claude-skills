---
name: ga4-report
description: Pull GA4 traffic and conversion report for a client
disable-model-invocation: true
---

# GA4 Performance Report

Generate a GA4 performance report for the specified date range.

## Parameters

- Client/property name (required)
- Date range (default: last 7 days)
- Compare with previous period (default: yes)

## Steps

1. Identify the GA4 property for the client
2. Pull key metrics via GA4 MCP:
   - **Traffic**: sessions, users, new users, pageviews
   - **Engagement**: avg session duration, bounce rate, pages/session
   - **Conversions**: each conversion event with count and value
   - **Sources**: top 10 traffic sources with sessions and conversions
3. Compare with previous period — calculate % change
4. Highlight anomalies: metrics that changed >20%
5. Pull top 10 landing pages by sessions

## Output format

```
## GA4 Report: [client] | [date range]

### Key Metrics (vs previous period)
- Sessions: [value] ([+/-]%)
- Users: [value] ([+/-]%)
- Conversions: [value] ([+/-]%)

### Traffic Sources
| Source/Medium | Sessions | Conversions | Conv Rate |
|--------------|----------|-------------|-----------|

### Top Landing Pages
| Page | Sessions | Bounce Rate | Conversions |
|------|----------|-------------|-------------|

### Alerts
- [any anomalies or significant changes]
```
