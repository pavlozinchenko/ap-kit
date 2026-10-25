# Claude Code

Everything specific to Claude Code. Two steps, nothing else.

## Once: global instructions

Append the contents of [CLAUDE.md](_CLAUDE.md) to `~/.claude/CLAUDE.md`. It
tells Claude Code where sessions start and that the Activity wins over the
Project.

## For each Activity or Project: CLAUDE.md imports AGENTS.md

Claude Code reads `CLAUDE.md`, not `AGENTS.md`. In the root of every
Activity and Project, next to `AGENTS.md`, create `CLAUDE.md` with one line:

```markdown
@AGENTS.md
```

A file, not a symlink: one rule for every machine and every sync tool.
