# Prompt 6 — The Dependency Doctor

**Purpose:** Single command that audits every project on his machine for vulnerabilities, outdated deps, and wasted disk space.

---

> **Build me a tool that audits my development environment and keeps it healthy.**
>
> Ask me:
> - What languages/runtimes do I use? (Python, Node, Go, Rust, Java, etc.)
> - How many active projects do I have? Where do they live on disk?
> - Do I use containers, or do dependencies live on my host?
>
> Build me:
> - `checkup` — a single command that scans my projects and reports:
>   - Security vulnerabilities in dependencies (using each ecosystem's native audit tool)
>   - Outdated dependencies with available updates (major/minor/patch breakdown)
>   - Unused dependencies I'm carrying
>   - Disk space used by dependency caches (`node_modules`, `.venv`, `target/`, etc.) with a `checkup clean` option
>   - Runtime version mismatches (project expects Node 20, I have Node 18)
> - `checkup <project-path>` for a single project deep-dive
> - `checkup all` scans every project in my workspace
> - Output: clean terminal table by default, `--json` flag for scripting
>
> This runs locally, offline, using each ecosystem's built-in tools (npm audit, pip-audit, cargo audit, etc.). No third-party security SaaS. Install the native audit tools if I'm missing them. Test it against my actual projects.
