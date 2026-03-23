---
name: conversion-check
description: Quick check of today's conversions and ad clicks
disable-model-invocation: true
---

# Quick Conversion Check

Fast daily check of ad clicks and conversions for a client.

## Steps

1. Identify the client's GA4 property
2. Pull today's data:
   - Total sessions from paid sources (google/cpc, etc.)
   - Each conversion event: name, count, breakdown by source
3. Compare with same day last week
4. Flag if conversions are significantly lower than expected

## Output format

```
[Client] | [today's date]

Clicks: [count] (last week: [count])
Conversions:
  - [event_name]: [count]
  - [event_name]: [count]
Total: [count] ([+/-] vs last week)

[⚠ Alert if significant drop]
```
