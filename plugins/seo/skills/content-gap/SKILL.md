---
name: content-gap
description: Find content topics competitors rank for but client doesn't
disable-model-invocation: true
---

# Content Gap Analysis

Find keywords/topics that competitors rank for in top 20 but the client doesn't rank for at all.

## Steps

1. Take client domain and competitor domains
2. Pull domain keywords for each competitor (top 100 positions)
3. Pull client's current keywords
4. Find keywords where competitors rank but client doesn't
5. Filter by relevance and search volume (>100/mo)
6. Group by topic/content cluster
7. For each cluster, suggest a content piece (title, format, target keywords)

## Output format

```
## Content Gap: [client]

### Missing Topics

#### [Topic Cluster 1]
Keywords: [list with volumes]
Suggested content: [title] — [format: blog/landing/guide]
Estimated traffic potential: [sum of volumes]

...

### Priority Content Calendar
1. [highest potential topic] — [suggested publish date]
2. ...
```
