# Filesystem

The system is expressed directly in the filesystem. No database, no index.

## Layout

```
~/Activities/
  site-support/
    AGENTS.md
    ...
  yard-management/
  _archive/
~/Projects/
  develop-site/
    AGENTS.md
    ...
  buy-car/
  _archive/
```

Each Activity or Project is a directory named by the rules in
[activity.md](activity.md) and [project.md](project.md), with one
`AGENTS.md` at its root, see [entry-file.md](entry-file.md).

## Everything else is unstructured

`~/Documents`, `~/Downloads`, `~/Photos`, `~/Videos` and similar directories
are outside the system. They simply exist. When it becomes clear that some
files belong to an Activity or a Project, they move there. Not before.

## Move or link

- **Move** files that belong to this Activity or Project and nowhere else.
- **Link** things that have a life of their own outside it: a git repository
  in `~/Git`, a photo library, a shared folder. They stay where they are and
  are symlinked into the Activity or Project directory.

The same repository may be linked from an Activity (`site-support`) and a
Project (`develop-site`) at the same time. Each link exists for its own
context. The decision to move or link is yours; the criterion above is what
keeps it consistent.

Links are a convenience for you in a file manager. For the AI, the entry
file also names the linked path in text, so the context does not depend on
how a tool resolves symlinks.

## Sessions start in an Activity or a Project

An AI session starts only from an Activity or a Project directory. Never
from inside a linked repository: the tool would resolve the real path under
`~/Git` and the entry file would not exist for it.

This is enforced by one rule in the global AI instructions, see
[kit/claude/README.md](../kit/claude/README.md). Not by
memory, which is per-directory and would not fire where it is needed.

## Three layers of instructions

| Layer | File | About |
|---|---|---|
| Repository | `AGENTS.md` / `CLAUDE.md` inside the repo | the code; valid for anyone who clones it |
| Project | `~/Projects/<name>/AGENTS.md` | focus: what we are doing now, goal, done-when |
| Activity | `~/Activities/<name>/AGENTS.md` | wider scope: context, constraints, standards |

Each layer is about a different thing. When a Project and an Activity are
related and their instructions conflict, the Activity wins. The conflict is
reported and the files are adjusted.

## Archive

`~/Activities/_archive/` and `~/Projects/_archive/`. Archiving is `mv`.
Nothing breaks because nothing references an entry by path.
