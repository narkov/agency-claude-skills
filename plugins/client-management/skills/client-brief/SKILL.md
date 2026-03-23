---
name: client-brief
description: Generate a client brief document from discovery call notes
disable-model-invocation: true
---

# Client Brief

Transform discovery call notes or raw info into a structured client brief.

## Input

Provide raw notes from a sales/discovery call. Include whatever is available:
- Client business description
- Goals and pain points
- Current marketing efforts
- Budget range
- Timeline expectations
- Competitors they mentioned

## Template

```
## Client Brief: [Company Name]
Website: [URL]
Contact: [Name, role, email/phone]
Date: [date]

### Business Overview
[What they do, market, size, location]

### Current State
- Website: [platform, age, traffic estimate]
- SEO: [any current efforts]
- Advertising: [channels, budget]
- Pain points: [what's not working]

### Goals
1. [Primary goal + KPI]
2. [Secondary goal + KPI]
3. [Timeline expectations]

### Competitors
| Competitor | URL | Notes |
|-----------|-----|-------|

### Proposed Services
- [ ] SEO: [scope]
- [ ] Ads: [channels, budget]
- [ ] Web dev: [scope]

### Budget & Timeline
- Monthly budget: [range]
- Contract length: [months]
- Start date: [date]

### Next Steps
1. [action] — [owner] — [deadline]
```

## Output

Save to Notion under a new or existing project, or output as text.
