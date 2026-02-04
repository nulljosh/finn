---
description: Generate daily standup summary of tasks and progress
---

Generate a daily standup report.

No emojis. No AI-speak. No m-dashes. Be direct and concise.

1. Yesterday's Progress: Check git commits across all repos, list what was accomplished (features, fixes, updates)
2. Today's Focus: Check TODO comments, in-progress branches, identify next tasks
3. Blockers: Check for error logs, failed tests, broken builds, dependencies
4. Portfolio Check: Summary of performance vs yesterday, any earnings or major events
   - If no stock positions, skip portfolio performance section.

Format as:
```
Daily Standup - [Date]

Yesterday:
- Shipped X
- Fixed Y
- Updated Z

Today:
- Work on A
- Review B
- Deploy C

Blockers: None / [List issues]

Portfolio: +X% ($Y) [Brief note]
```

Keep it factual and straightforward.
