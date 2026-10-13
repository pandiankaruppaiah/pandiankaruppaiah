# Pandian Karuppaiah

**AI Tech Lead · agentic AI engineer.** I build with Claude Code and its plugin system, and the instrumentation that shows what AI-assisted work costs.

---

### What I work on

- **Agentic workflows.** Subagents, skills and MCP servers in Claude Code, with the agent kept on a short leash: it reads only what the task needs.
- **Developer tooling.** Claude Code plugins, skills, lifecycle hooks and status lines.
- **Cost and quota engineering.** Token attribution by model, project and tool; forecasting against rate limits; prompt caching.
- **Testing and review.** Generated test fixtures instead of real logs, CI on three operating systems, and a second model reviewing every design and code change.

### Featured

**[quotameter](https://github.com/pandiankaruppaiah/quotameter)**: see where your Claude Pro or Max quota goes across Claude Code, Claude Desktop and claude.ai.

- A Claude Code plugin and command-line tool. Node only, no dependencies, Windows, macOS and Linux.
- Rebuilds usage from local logs and Claude Code's free `/usage` command, then learns from your own history how much of the limit a dollar of usage costs, so it can estimate the chat share that leaves no local trace.
- Forecasts when you will hit the 5-hour and weekly limits, counts how many more sessions fit, and re-prices Opus work on Sonnet and Haiku.
- Never stores message text, makes no network calls of its own, and summarises data older than 90 days instead of keeping it raw.
- Built with Claude Code. Every design and code change was reviewed by a second model, and the review log is in the repository.

### Engineering focus

- **Fail loudly:** a hard stop with a clear message instead of a guess when a step fails.
- **Guardrails in code, not prompts:** checks the program enforces, such as refusing to record a `/usage` reading if it cost a model call.
- **Local telemetry:** usage data that stays on the user's machine, keeping only the fields that are needed.

### Toolbox

Claude Code (plugins, skills, hooks, subagents) · Model Context Protocol · prompt caching · Node.js · GitHub Actions · multi-model review

---

Open to conversations about agentic AI, AI developer tooling and LLM cost engineering. Start a discussion on [quotameter](https://github.com/pandiankaruppaiah/quotameter/discussions).
