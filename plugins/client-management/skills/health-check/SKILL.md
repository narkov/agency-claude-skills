---
name: health-check
description: Quick health check across all active client projects
disable-model-invocation: true
---

# Client Health Check

Quick scan across all active client projects to identify issues needing attention.

## Steps

1. List all active projects from Notion
2. For each project check:
   - **Last update date** — flag if no update in >14 days
   - **Next step** — is it set? Is the deadline passed?
   - **SEO audit score** — flag if below 70
   - **Keyword rankings** — any significant drops (>5 positions for priority keywords)
   - **Traffic trend** — last 7 days vs previous 7 days
   - **Ad spend** — is budget on track for the month?
3. Score each project: 🟢 healthy / 🟡 needs attention / 🔴 urgent

## Output

```
## Agency Health Check | [date]

🟢 [Client A] — all good, traffic +12%
🟡 [Client B] — no update in 18 days, next step overdue
🔴 [Client C] — rankings dropped for 5 keywords, audit score 52

### Action Required
1. [Client C]: investigate ranking drops, run new audit
2. [Client B]: schedule check-in, update project status
```
