# Entry file: AGENTS.md

Every Activity and Project has exactly one entry file, `AGENTS.md`, at its
root. It is the same thing as the `notes.txt` you would write for yourself,
now written so that both you and the AI read it first.

## State, not history

The entry file describes how things are, not how they got there. Anything
you want to append chronologically at the bottom is either deleted or lives
in a separate file. Otherwise, in six months, it is a journal again.

## Sections

```
# <name>
Two or three lines: what this is.
Related: <activities or projects, by name>.

## Purpose              (Activity)
## Goal / Done when     (Project)

## Links
<path> — why it is linked rather than moved

## Constraints and rules
What holds here: standards, formats, things not to do, decisions made.

## Structure
What exists here and what each part is for.

## Tasks
### Important
### When there's time

## On return
A few lines for the next time you open this. Overwritten, never appended.
```

Sections that do not apply are omitted. Templates:
[kit/templates/activity/AGENTS.md](../kit/templates/activity/AGENTS.md),
[kit/templates/project/AGENTS.md](../kit/templates/project/AGENTS.md).

## Purpose and Goal

An Activity has a Purpose: why it is maintained. A Project has a Goal: what
it achieves, and a "done when" list that makes the end observable. One or
the other, never both.

## Constraints and rules

Present in both. What must hold when working here: standards, formats,
things not to do, non-trivial choices already made. One line per rule. When
a Project and an Activity are related and their rules conflict, the
Activity wins; the conflict is reported.

## Structure

What exists in this Activity or Project and what each part is for: a
directory of invoices, a linked repository, a spreadsheet, an external
service. It explains the parts, not the folder tree. If a part has no
purpose you can name, it probably should not be here.

## Tasks

Two lists, nothing else: no priorities, no dates, no statuses.

- **Important** — what should be done.
- **When there's time** — what could be done.

If the Important list does not fit on one screen, that is a re-triage, not
a list. Done tasks are deleted.

## On return

The note to your future self: what you were in the middle of, what not to
forget, what to check first. A few lines. Rewrite it when you leave; do not
add to it.

## For the AI

The AI reads this file first. For a Project, the file names related
Activities and asks the AI to read their entry files before anything else.
Claude Code reads `CLAUDE.md`, not `AGENTS.md`: add a one-line import or a
symlink, see [kit/claude/global-snippet.md](../kit/claude/global-snippet.md).
