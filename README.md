# ap-kit

AP System is a personal management method for activities and projects that
need files, work with an AI assistant, and a short list of tasks.
This repository describes the system and holds the few templates it needs.

- `system/` — the method itself, tool-agnostic. Start with
  [system/README.md](system/README.md).
- `kit/` — templates and tool-specific snippets. Minimal by design.

The system lives in the filesystem as `~/Activities` and `~/Projects`,
each entry having one `AGENTS.md` that serves both you and the AI.
