# Project

A Project is something with an end: a quantity to reach, a date to meet, or
a result to deliver. It exists to be achieved and then archived.

Examples: `develop-site`, `buy-car`, `migrate-hosting`.

## Naming

Starts with a verb, kebab-case: `buy-car`, not `car`. The name is unique
forever, including the archive, so a Project can always be found again by
name alone.

## Threshold

Something becomes a Project when it needs several sessions, spans several
days, or has a structure with many subtasks. Anything smaller is a task
inside an Activity, not a Project. The threshold is personal, but it is
written here so it stays the same over time.

## What it holds

- The goal and what "done" means.
- Constraints and rules specific to this Project.
- Links to things with a life of their own (repositories, documents).
- Files that exist only for this Project.
- Tasks.
- A short note to yourself for the next time you return.

See [entry-file.md](entry-file.md).

## Relation to Activities

A Project may be directly related, partially related, or unrelated to any
Activity. The Project names its related Activities in its entry file and
asks the AI to read them first.

When instructions conflict, the Activity wins: it describes the wider scope.
The conflict is reported, and both files are adjusted if needed.

Nothing references a Project by path. Activities mention Projects by name
and meaning only. This is what makes archiving a plain move.

## Closing a Project

> Draft: revisit after the first two closings.

Answer three questions, then move the directory.

1. What did I learn that is useful without this Project? Write it into the
   related Activity's entry file: constraints, decisions, pitfalls.
2. Which files or links have a life after the Project? Move or re-link them
   into the Activity. A repository in `~/Git` stays where it is.
3. What is still open and worth keeping? Put it under "When there's time" in
   the Activity's tasks. Everything else dies with the Project.

Then, in the Activity, update the mention of the Project to one line:
name and outcome. Finally `mv` the Project to `~/Projects/_archive/`.

## Project becoming an Activity

> Draft: revisit after the first real transition.

Trigger: the goal is reached but tasks keep appearing, or you keep returning
to the Project without a new goal.

Two paths:

- **Convert** — the Project has lost its end. Rename to a noun, move to
  `~/Activities`, remove the goal section, keep the rest.
- **Branch** — the Project still has an end. Create an Activity next to it,
  move "what has value and structure" there, leave "what will finish" in the
  Project, and have the Project mention the Activity by name.

Default: if the end is still visible, branch; otherwise convert.
