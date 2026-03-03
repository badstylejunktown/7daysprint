# Prompt 4 — The Overnight Worker

**Purpose:** A cron-based personal automation daemon. Does recurring work while he sleeps, delivers a morning briefing.

---

> **Build me a personal automation daemon — a cron-based system that does recurring work while I sleep.**
>
> Ask me:
> - What repetitive tasks do I do weekly that a script could do? (examples: clean up downloads folder, back up dotfiles, check if dependencies have security updates, pull and summarize RSS/news, rotate logs, check disk usage)
> - What do I wish I got a morning briefing on? (git activity on my repos, CI status, server health, calendar, weather — whatever)
> - Where do I want notifications? (terminal on login, desktop notification, email, a local web page, a file I check)
>
> Build me:
> - A `~/.config/overnight/` directory with individual task scripts, each independently runnable and testable
> - A coordinator script that runs them in order, captures output, and handles failures gracefully (one failing task doesn't kill the rest)
> - A **morning briefing** that compiles results into a single readable summary delivered however I want it
> - Cron entries (or systemd timers — ask my preference) with sane scheduling
> - A `overnight status` command that shows what ran last night, what passed, what failed
> - A `overnight add` scaffolder for new tasks
>
> Each task must: log to a standard location, have a timeout, exit cleanly on failure, and be individually disableable via config. No task should require network access unless I explicitly approve it. Test every task before scheduling.
