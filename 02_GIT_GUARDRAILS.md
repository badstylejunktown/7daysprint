# Prompt 2 — The Git Guardrails

**Purpose:** Make it structurally hard to ship bad work. Pre-commit hooks, commit linting, PR self-review — installed once, works everywhere.

---

> **Set up my development environment so it's hard to ship bad work.**
>
> Ask me:
> - What languages/frameworks are in my main projects?
> - Do I work solo or on a team? (affects what goes in pre-commit vs CI)
> - What's the last bug that made it to production that a machine could have caught?
>
> Then build me a reusable dev quality setup:
> - **Pre-commit hook suite** — linting, formatting, type checking, secret scanning. Configured for my stack, not a generic template.
> - **Commit message validator** — enforces conventional commits or whatever pattern my team uses. Ask me.
> - **A `dev-setup.sh` bootstrap script** I can run in any new repo to install these hooks in 30 seconds
> - **A PR self-review checklist generator** — reads my staged diff, generates a checklist of things to verify before I open the PR, specific to what I actually changed
>
> Requirements:
> - Everything lives in `~/.config/dev-guardrails/` with symlinks into repos. One source of truth, not copy-pasted into every project.
> - Works offline. No SaaS dependencies.
> - The hooks should be fast — if any hook takes more than 5 seconds, warn me and let me split it into a CI-only check.
>
> Test it against my actual current project before we call it done.
