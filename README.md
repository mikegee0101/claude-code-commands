# Claude Code Commands

A collection of useful slash commands for Claude Code to streamline common development workflows.

## Available Commands

### git-commit.md
Automates git commits with intelligent staging and message generation. Checks current status, stages changes, and creates descriptive commit messages.

**Tools:** `git`, `cat`

## Usage

To use these commands in Claude Code, simply reference them by filename:

```
/git-commit
```

## Adding New Commands

Create new `.md` files with the following format:

```markdown
---
allowed-tools: Tool1(*), Tool2(specific command)
description: Brief description of what the command does
---

Your command implementation here...
```

## Contributing

Feel free to add new useful commands that automate common development tasks.