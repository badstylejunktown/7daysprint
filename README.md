# 7 Day Sprint — Claude Code Power User Kit

7 self-contained prompts for a tech professional with 7 days of Claude Code access.

## How to Use

Pick whichever prompt solves the biggest annoyance first. Drop it into Claude Code while sitting in your home directory. Each one takes 30-60 minutes to build and test. You walk away with a real tool installed on your machine that works after the 7 days are over.

The tools are yours — plain files, no cloud dependency, no subscription.

## The Prompts

| # | File | What It Builds | Time |
|---|------|----------------|------|
| 0 | `00_THE_TOUR.md` | Full capability tour, tailored to your work | Start here |
| 1 | `01_PERSONAL_CLI_TOOLKIT.md` | `kit` — your personal multi-command CLI tool | 45 min |
| 2 | `02_GIT_GUARDRAILS.md` | Pre-commit hooks, commit linting, PR checklist | 30 min |
| 3 | `03_PROJECT_BOOTSTRAPPER.md` | `mkproj` — project scaffolder with your conventions | 30 min |
| 4 | `04_OVERNIGHT_WORKER.md` | Cron daemon + morning briefing system | 60 min |
| 5 | `05_WORKLOG.md` | `log` — terminal work journal, plain text forever | 30 min |
| 6 | `06_DEPENDENCY_DOCTOR.md` | `checkup` — audit deps, vulns, disk space | 45 min |

## Recommended Order

**Day 1:** Prompt 0 (the tour — get oriented)
**Day 2-3:** Prompt 1 (CLI toolkit — immediate daily value)
**Day 4:** Prompt 2 + 3 (guardrails + bootstrapper — quality infrastructure)
**Day 5:** Prompt 5 (worklog — start tracking immediately)
**Day 6:** Prompt 4 (overnight worker — automation)
**Day 7:** Prompt 6 (dependency doctor — maintenance)

## Design Principles

Every prompt in this kit follows the same rules:

- **Asks before building** — tailors to your actual stack, not a generic template
- **Local-first** — no SaaS, no cloud, no subscriptions. Files on your machine.
- **Plain formats** — text, TOML, shell scripts. Readable without special tools in 10 years.
- **One source of truth** — configs in `~/.config/`, not copy-pasted into every project
- **Tested before done** — each prompt includes "test it against my actual projects"
- **Growable** — every tool includes an `add` command or template system for extension
