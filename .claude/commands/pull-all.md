---
description: Pull all git repositories in ~/Documents/Code
---

Pull all git repositories. Checks both ~/Documents/Code and ~/finn:

```bash
for dir in ~/Documents/Code ~/finn; do
  if [ -d "$dir" ]; then
    find "$dir" -maxdepth 2 -name ".git" -type d -exec dirname {} \; | while read repo; do echo "=== Pulling $repo ===" && git -C "$repo" pull; done
  fi
done
```

This will:
- Find all git repositories (up to 2 levels deep) in known code directories
- Pull latest changes from remote for each repo
- Show status for each repository
- Skip directories that don't exist
