---
name: ad-performance
description: Analyze Google Ads or paid campaign performance from GA4 data
disable-model-invocation: true
---

# Ad Performance Analysis

Analyze paid advertising performance using GA4 data filtered by ad traffic sources.

## Steps

1. Pull GA4 data filtered by source/medium containing "cpc", "ppc", "paid"
2. Break down by:
   - Campaign (if utm_campaign available)
   - Source/medium
   - Landing page
   - Device category
3. Calculate for each:
   - Sessions, users
   - Conversions and conversion rate
   - Cost per conversion (if cost data available)
   - Bounce rate
4. Identify:
   - Best performing campaigns/pages
   - Underperforming campaigns (high spend, low conversions)
   - Device-specific issues (e.g., mobile bounce rate too high)

## Output format

```
## Ad Performance: [client] | [date range]

### Campaign Summary
| Campaign | Sessions | Conversions | Conv Rate | CPA |
|----------|----------|-------------|-----------|-----|

### Landing Page Performance
| Page | Sessions | Conv Rate | Bounce Rate | Issue? |
|------|----------|-----------|-------------|--------|

### Recommendations
1. [actionable optimization suggestions]
```
