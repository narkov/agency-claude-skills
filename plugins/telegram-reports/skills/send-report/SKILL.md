---
name: send-report
description: Format and send a client report to a Telegram chat
disable-model-invocation: true
---

# Send Report to Telegram

Format data into a readable report and send it to a specified Telegram chat.

## Input

- Report type: daily / weekly / monthly / custom
- Client name
- Data to include (or "pull from GA4/SE Ranking")
- Telegram chat (name or ID)

## Formatting Rules

- Use plain text (Telegram doesn't render full markdown)
- Use emoji sparingly for visual structure:
  - 📊 for metrics sections
  - ✅ for positive changes
  - ⚠️ for alerts/drops
  - 📈📉 for trends
- Keep under 4000 chars (Telegram limit is 4096)
- If data exceeds limit, split into multiple messages with clear headers

## Template

```
📊 [Report Type]: [Client]
📅 [Date/Period]

🔹 Traffic: [sessions] ([+/-]% vs prev)
🔹 Conversions: [count] ([+/-]%)
🔹 Top source: [source] — [sessions]

📈 Top performing:
- [page/keyword/campaign]: [metric]

⚠️ Alerts:
- [any significant drops or issues]

Next: [planned actions]
```

## Steps

1. Gather the data (from GA4, SE Ranking, or user input)
2. Format using the template above
3. Send via Telegram MCP tool
4. Confirm delivery
