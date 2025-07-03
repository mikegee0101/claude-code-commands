---
allowed-tools: Bash(git *), Bash(cat *)
description: Create a git commit with automated staging and message generation
---

I'll create a git commit by checking the current status, staging changes, and generating an appropriate commit message.

First, let me check what changes need to be committed:

```bash
git status
git diff
git log --oneline -5
```

Now I'll add the changes and create a commit with a descriptive message:

```bash
git add .
git commit -m "$(cat <<'EOF'
[Generated commit message based on changes]
EOF
)"
```

Finally, I'll verify the commit was successful:

```bash
git status
```