# Kit

What you need to set the system up and use it: templates, snippets and
the checklists below. What an Activity or a Project is, and when to create
one, is in [system/](../system/README.md).

> Draft: revisit after the first adoption pass.

## A new AP System setup

What a machine needs before the system can work: the two root directories
with their archives, and an AI tool that knows where sessions start.

- `mkdir -p ~/Activities/_archive ~/Projects/_archive`
- Tell your AI tool where sessions start and how Activities and Projects
  relate. Claude Code: [claude/README.md](claude/README.md).

## A new Activity or Project

- Decide: Activity or Project.
  - Meaning of Activity see in [system/activity.md](../system/activity.md).
  - Meaning of Project see in [system/project.md](../system/project.md).
- Name it by the rules
  - Rules for Activity in [system/activity.md](../system/activity.md).
  - Rules for Project in [system/project.md](../system/project.md).
- Create the directory:
  - `~/Activities/<activity-name>` for Activity.
  - `~/Projects/<verb-project-name>` for Project.
- Copy `AGENTS.md`:
  - from [templates/activity](templates/activity/AGENTS.md) for Activity.
  - from [templates/project](templates/project/AGENTS.md) for Project.
- Create `CLAUDE.md` next to it with one line: `@AGENTS.md`.
- Link what has a life of its own, move what belongs here and nowhere else,
  see [system/filesystem.md](../system/filesystem.md).
- Fill the entry file. Omit sections that do not apply.
- Start the first AI session from the new directory.
