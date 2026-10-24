# Activity

An Activity is something that has meaning and structure but no end goal and
no deadline. It is maintained, not finished.

Examples: `site-support`, `yard-management`, `bookkeeping`, `3d-printing`,
`fpv-flying`.

## Naming

A noun phrase, kebab-case, no verb: `site-support`, not `support-site`.
The name answers "what is this about", not "what am I doing". It is unique
forever, including the archive, so an Activity can always be found again by
name alone.

## What it holds

- Purpose: why this is maintained at all. The counterpart of a Project's goal.
- Constraints and rules for working in this area, for you and for the AI.
- Links to things with a life of their own (repositories, photo libraries).
- Files that belong to the Activity and nowhere else.
- Tasks: what can or should be done here.
- A short note to yourself for the next time you return.

All of this is organised by the entry file, see [entry-file.md](entry-file.md).

## Relation to Projects

An Activity may mention Projects by name and by meaning: "`develop-site`
delivered the new module in 2026". It never references a Project by path,
so a Project moving to the archive changes nothing in the Activity.

Knowledge, files and tasks move from a Project into an Activity when they
are useful without the Project. See the closing checklist in
[project.md](project.md).

## Archiving

An Activity does not end, but it can stop being relevant: the drone is sold,
the site is handed over. Move it to `~/Activities/_archive/`. The meaning is
"no longer maintaining", not "achieved". Nothing else changes.
