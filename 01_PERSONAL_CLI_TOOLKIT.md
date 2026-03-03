# Prompt 1 — The Personal CLI Toolkit

**Purpose:** Build a single multi-command CLI tool that grows with him. Lives at `~/.local/bin/kit` forever.

---

> **Build me a personal CLI multi-tool.** A single command I install once that grows with me.
>
> Start by asking me:
> - What language do I think in? (Python, Node, Go, Rust, shell — pick one, we're not debating)
> - What 3 things do I type into a terminal every day that are more than one command?
> - What information do I alt-tab to look up repeatedly?
>
> Then build me a CLI tool with these properties:
> - **Single entry point**: `kit <subcommand>` (or whatever name I pick)
> - **Subcommands** for each of those daily workflows, collapsing multi-step processes into one call
> - **A `kit add` scaffolder** so I can add new subcommands later without touching plumbing
> - **Local config file** (`~/.config/kit/config.toml` or equivalent) for any values I'd otherwise hardcode
> - **Tab completion** for my shell (bash/zsh/fish — ask which I use)
> - **No external dependencies** beyond the language's standard library where possible
>
> Walk me through:
> 1. Building the core with the first 3 subcommands
> 2. Writing tests for each
> 3. Installing it so `kit` works from any directory
> 4. Adding shell completion
> 5. How to add a new subcommand in under 2 minutes going forward
>
> This tool should still be on my machine and useful in a year. Build it like infrastructure, not a demo.
