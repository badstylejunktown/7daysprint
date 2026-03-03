# Prompt 3 — The Project Bootstrapper

**Purpose:** Encode how he starts projects into a single command. Never manually create boilerplate again.

---

> **Build me a project generator that encodes how I like to start projects.**
>
> Ask me:
> - What kinds of projects do I start most often? (API service, CLI tool, web app, script, library — pick top 2-3)
> - For each: what's my preferred stack, directory structure, and what files do I always create manually?
> - What do I always forget to set up until I need it? (logging, error handling, CI, .gitignore, Dockerfile, etc.)
>
> Build me a scaffolder that:
> - `mkproj <type> <name>` creates a full project skeleton for that type
> - Includes everything I always set up manually: README template, .gitignore, CI config, Makefile/justfile, Dockerfile, dev container config — ask me what I want
> - Initializes git, creates a CLAUDE.md with my conventions so Claude knows how this project works from the first session
> - Includes a `Makefile` or `justfile` with: `make dev`, `make test`, `make lint`, `make build`, `make deploy` — all wired up for the stack
> - Templates are stored in `~/.config/mkproj/templates/` so I can edit them later
>
> This replaces the 30-minute "set up a new project and remember all the boilerplate" ritual with a 10-second command. Test it by generating a project of each type and verifying everything works.
