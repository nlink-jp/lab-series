# CLAUDE.md — lab-series

**Organization rules (mandatory): https://github.com/nlink-jp/.github/blob/main/CONVENTIONS.md**

## Non-negotiable rules

- **Tests are mandatory** — write them with the implementation. A feature is not complete without tests.
- **Design for testability** — pure functions, injected dependencies, no untestable globals.
- **Never `go build` directly** — always use `make build` (outputs to `dist/`). `go build` without `-o dist/...` drops the binary in the project root, polluting the working tree.
- **Docs in sync** — update `README.md` and `README.ja.md` in the same commit as behaviour changes.
- **Small, typed commits** — `feat:`, `fix:`, `test:`, `chore:`, `docs:`, `refactor:`, `security:`

## This series

Experimental projects under active development. APIs and interfaces may change without notice.

```
lab-series/
├── agent-skeleton/     github.com/nlink-jp/agent-skeleton     (Python — autonomous agent skeleton POC)
├── agentic-web-search/ github.com/nlink-jp/agentic-web-search (Go — agentic web search; frozen, search API ToS concerns)
├── llm-othello/        github.com/nlink-jp/llm-othello        (Go — Othello vs local LLM)
├── log-analyzer/       github.com/nlink-jp/log-analyzer       (Go — log analysis tool; archived)
├── m5-clock/           github.com/nlink-jp/m5-clock           (C++ — M5Stack Core2 NTP clock)
├── m5-data-receiver/   github.com/nlink-jp/m5-data-receiver   (Bash/CFn — serverless backend for m5-vehicle-logger)
├── m5-vehicle-logger/  github.com/nlink-jp/m5-vehicle-logger  (C++ — M5Stack vehicle data logger)
├── magi-system/        github.com/nlink-jp/magi-system        (Python — multi-agent discussion v1; archived)
├── magi-system2/       github.com/nlink-jp/magi-system2       (Python — multi-persona discussion v2, Gemini; archived)
├── mail-watcher/       github.com/nlink-jp/mail-watcher       (Bash — mail monitoring workflow; archived)
├── mcp-skeleton/       github.com/nlink-jp/mcp-skeleton       (Python — MCP learning skeleton)
├── meeting-note/       github.com/nlink-jp/meeting-note       (Python — meeting minutes CLI; archived, superseded by the meeting-notes skill)
├── sai/                github.com/nlink-jp/sai                (Python — context-aware Slack bot; archived)
├── slack-monitor/      github.com/nlink-jp/slack-monitor      (Python — Slack channel summarizer)
├── virtual-reviewer/   github.com/nlink-jp/virtual-reviewer   (Python — AI security review, LLM experts; archived → compliance-review skill)
└── workflow-builder/   github.com/nlink-jp/workflow-builder   (— — LLM workflow builder; archived, design phase only)
```

## Release checklist

1. Update `CHANGELOG.md` → commit `chore: release vX.Y.Z` → tag → push
2. `gh release create` (no assets)
3. Build 5 platforms (Go tools): `linux/amd64`, `linux/arm64`, `darwin/amd64`, `darwin/arm64`, `windows/amd64`
4. Zip each binary + `README.md` → upload one by one
5. Update umbrella submodule pointer in this repo
6. Update org profile: `nlink-jp/.github/profile/README.md`
