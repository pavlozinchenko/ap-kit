# Global snippet for Claude Code

Add once to `~/.claude/CLAUDE.md`. Two things: where sessions start, and
how `CLAUDE.md` reaches `AGENTS.md`.

## Session start

```markdown
## AP System
- Activities live in `~/Activities`, Projects in `~/Projects`. Each has an
  `AGENTS.md`; read it first.
- If the working directory is not under `~/Activities` or `~/Projects`
  (for example a repository in `~/Git`), ask which Activity or Project this
  session belongs to before doing anything else.
- A Project's `AGENTS.md` names related Activities. Read their `AGENTS.md`
  too. If instructions conflict, the Activity wins; say so.
```

## CLAUDE.md to AGENTS.md

Claude Code reads `CLAUDE.md`. In each Activity or Project directory, either:

```bash
ln -s AGENTS.md CLAUDE.md
```

or create `CLAUDE.md` with one line:

```markdown
@AGENTS.md
```

The symlink is simpler. The import is safer if a sync tool does not keep
symlinks.
