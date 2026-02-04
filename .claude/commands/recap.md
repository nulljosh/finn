---
description: Recap recent activity and jog your memory
---

Summarize what's happened recently. No emojis. No AI-speak. Be direct.

1. Check recent git commits: `git log --oneline -15`
2. Check what files changed recently: `git diff --stat HEAD~5`
3. Read ~/finn/NOTES.md if it exists for any persistent reminders/todos
4. Summarize in plain language: what was done, what's pending, any reminders

Format:
```
Recent Activity:
- [what happened]

Pending/Reminders:
- [anything from NOTES.md or in-progress work]
```

Keep it short. This is a memory jog, not a report.
