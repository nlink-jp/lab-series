# lab-series

Experimental projects under active development by [nlink-jp](https://github.com/nlink-jp).

> These tools are works in progress. APIs, features, and interfaces may change without notice.

## Projects

| Project | Description | Language |
|---|---|---|
| [agent-skeleton](https://github.com/nlink-jp/agent-skeleton) | Autonomous agent skeleton — plan-approve-execute loop, per-tool approval, 2-tier memory compression, MCP support | Python |
| [agentic-web-search](https://github.com/nlink-jp/agentic-web-search) | ~~Agentic web search~~ **FROZEN** (search API ToS concerns) | Go |
| [llm-othello](https://github.com/nlink-jp/llm-othello) | Browser-based Othello against a local LLM — server-side move generation via OpenAI-compatible API | Go |
| [log-analyzer](https://github.com/nlink-jp/log-analyzer) | Log analysis tool | Go |
| [m5-clock](https://github.com/nlink-jp/m5-clock) | NTP-synchronized digital clock for M5Stack Core2 — night mode, RTC backup, SD card config | C++ |
| [m5-data-receiver](https://github.com/nlink-jp/m5-data-receiver) | Serverless AWS backend for m5-vehicle-logger — API Gateway + Lambda + S3 with deploy/destroy scripts | Bash/CFn |
| [m5-vehicle-logger](https://github.com/nlink-jp/m5-vehicle-logger) | Vehicle data logger for M5Stack — GNSS + 9-axis IMU + barometer, 3-page display, gravity compensation | C++ |
| [magi-system](https://github.com/nlink-jp/magi-system) | Multi-agent discussion system with 3 AI personas (MELCHIOR / BALTHASAR / CASPER) | Python |
| [magi-system2](https://github.com/nlink-jp/magi-system2) | Multi-persona AI discussion with dynamic persona generation, dual memory, and adaptive facilitation via Gemini | Python |
| [mail-watcher](https://github.com/nlink-jp/mail-watcher) | Mail monitoring workflow — watches for incoming eml/msg files, analyzes with LLM, and posts Slack notifications | Bash |
| [mcp-skeleton](https://github.com/nlink-jp/mcp-skeleton) | MCP server skeleton — raw JSON-RPC 2.0 over stdio/SSE with API key auth, for learning MCP internals | Python |
| [meeting-note](https://github.com/nlink-jp/meeting-note) | Meeting minutes structuring tool — audio/transcript to structured JSON via Gemini, then compile to Markdown/HTML | Python |
| [sai](https://github.com/nlink-jp/sai) | Context-aware Slack bot with RAG memory and natural language command execution | Python |
| [slack-monitor](https://github.com/nlink-jp/slack-monitor) | Real-time Slack channel summarizer with local/cloud LLM and Textual TUI | Python |
| [virtual-reviewer](https://github.com/nlink-jp/virtual-reviewer) | AI-powered security review system with LLM expert models — no RAG, UNIX philosophy | Python |
| [workflow-builder](https://github.com/nlink-jp/workflow-builder) | LLM-powered workflow builder — generates shell scripts from natural language using CLI tool registry | Design phase |

## Related Series

- [cli-series](https://github.com/nlink-jp/cli-series) — Slack / Confluence / Splunk CLI tools
- [chatops-series](https://github.com/nlink-jp/chatops-series) — Slack ChatOps automation tools
- [cybersecurity-series](https://github.com/nlink-jp/cybersecurity-series) — AI-powered security tools
- [lite-series](https://github.com/nlink-jp/lite-series) — Local-first LLM and pipeline CLI tools
- [util-series](https://github.com/nlink-jp/util-series) — General-purpose data conversion tools
