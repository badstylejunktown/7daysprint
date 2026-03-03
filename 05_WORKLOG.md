# Prompt 5 — The Worklog & Time Machine

**Purpose:** Answer "what did I do last week?" instantly, forever. Plain text, no SaaS, no database.

---

> **Build me a dead-simple work log system that runs in my terminal.**
>
> I want to answer "what did I do last week?" instantly, forever. No app, no SaaS, no browser.
>
> Ask me:
> - Do I track time for billing, or just for personal awareness?
> - Do I work on multiple projects or one main project?
> - Do I want this integrated with git (auto-log commits) or purely manual?
>
> Build me:
> - `log "what I did"` — appends a timestamped entry. That's the core interaction. Must be zero-friction.
> - `log show` — today's entries
> - `log week` — this week's entries, grouped by day
> - `log search <term>` — full text search across all history
> - `log summary` — uses a local LLM or simple text processing to generate a weekly summary I can paste into a standup or status report
> - If I want git integration: a post-commit hook that auto-logs commit messages with project context
>
> Data format: **plain text, one file per month, in `~/.local/share/worklog/`**. I should be able to `cat` or `grep` the files directly. No database. No binary format. This data should be readable in 10 years without any special tools.
>
> If I bill time: add `log start` / `log stop` with elapsed time tracking, and `log invoice <project> <date-range>` to generate a time report.
