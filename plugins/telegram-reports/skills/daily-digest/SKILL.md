---
name: daily-digest
description: Send a daily digest of all clients' key metrics to Telegram
disable-model-invocation: true
---

# Daily Digest

Compile a daily summary across all active client projects and send to Telegram.

## Steps

1. List all active client projects (from Notion or a configured list)
2. For each client, pull today's GA4 data:
   - Sessions (paid + organic)
   - Conversions
   - Any anomalies (>30% drop vs 7-day average)
3. Compile into a single digest message
4. Send to the agency's internal Telegram chat

## Template

```
📋 Daily Digest | [date]

[Client 1]
  Sessions: [n] | Conv: [n] | Paid clicks: [n]

[Client 2]
  Sessions: [n] | Conv: [n] | Paid clicks: [n]

⚠️ Alerts:
- [Client X]: conversions dropped 40% vs avg
- [Client Y]: no paid traffic detected

✅ All other clients normal
```
