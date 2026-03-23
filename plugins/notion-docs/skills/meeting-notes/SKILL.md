---
name: meeting-notes
description: Create structured meeting notes in Notion from a summary
disable-model-invocation: true
---

# Meeting Notes

Create formatted meeting notes in Notion under the client's project.

## Input

Provide the raw notes or summary of the meeting. Include:
- Client name
- Who attended
- Key points discussed

## Template

```
## Meeting: [Client] | [Date]

**Attendees**: [list]

### Discussed
- [topic 1]: [decision/outcome]
- [topic 2]: [decision/outcome]

### Action Items
- [ ] [task] — [owner] — [deadline]
- [ ] [task] — [owner] — [deadline]

### Next Meeting
[date/time if set]
```

## Steps

1. Find client project in Notion
2. Navigate to Meeting Notes sub-page
3. Create a new page with the formatted notes
4. Extract action items and optionally create tasks in the Tasks database
