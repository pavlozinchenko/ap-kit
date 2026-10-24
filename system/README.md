# AP System

AP stands for Activity and Project. The system is a set of practices for
managing things in life that need files, conversations with an AI assistant,
and some definiteness in the form of tasks. It is built for one person, not
a team.

## Two kinds of things

- **Activity** — something with meaning and structure that has no end goal
  and no deadline. Maintaining a website, yard upkeep, bookkeeping, a hobby.
  See [activity.md](activity.md).
- **Project** — something with an end: in quantity, in time, or in
  completion. It exists to be achieved and archived. See
  [project.md](project.md).

An Activity and a Project may be directly related, partially related, or
not related at all. The relation is expressed by name, never by path.

## Where things live

Two directories, `~/Activities` and `~/Projects`, each entry self-describing
through a single `AGENTS.md`. Everything else on the machine stays
unstructured. See [filesystem.md](filesystem.md) and
[entry-file.md](entry-file.md).

## Principles

- One entry file per Activity or Project. It is state, not history.
- A session with an AI starts only inside an Activity or a Project.
- Nothing references a Project by path. Archiving is a move.
- Repositories and other things with a life of their own live outside and
  are linked, not moved.
- What the system does not do is delegated, not bolted on: push reminders
  and a cross-cutting "what today" view belong to other tools.
- Structure appears when a need appears, not before.
