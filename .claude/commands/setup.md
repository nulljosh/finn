---
description: Check Mac mini dev environment setup and flag anything missing
---

Check the dev environment and report what's installed vs missing.

No emojis. No AI-speak. No m-dashes. Be direct and concise.

Run these checks and report status for each:

```bash
# Package manager
brew --version 2>/dev/null || echo "MISSING: brew"

# Dev tools
git --version 2>/dev/null || echo "MISSING: git"
gh --version 2>/dev/null || echo "MISSING: gh (GitHub CLI)"
claude --version 2>/dev/null || echo "MISSING: claude (Claude Code)"

# Git config
echo "Git user: $(git config --global user.name) <$(git config --global user.email)>"
echo "Git SSH: $(ssh -T git@github.com 2>&1 | head -1)"

# Shell
echo "Shell: $SHELL"
```

Expected setup:
- brew (Homebrew)
- git with user "Joshua Trommel <trommatic@icloud.com>"
- gh (GitHub CLI), authenticated
- Claude Code CLI
- SSH key configured for GitHub

Report as a checklist. Flag anything missing or misconfigured.
