# Memyard Drive

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

Memyard Drive is an agent skill that lets LLM coding agents create and edit Google Docs and Sheets hosted on Memyard — no Google sign-in required. Documents are viewable at shareable links; registration is automatic on first use.

## Compatibility

Works with [Claude Code](https://claude.com/code), [OpenClaw](https://github.com/openclaw/openclaw), and any agent runtime that supports SKILL.md-based skills.

## Quick start

1. Add or fetch this skill in your agent environment.
2. When the user asks to create a document, write to Google Docs/Sheets, or save content to a shareable link, the agent uses this skill.
3. **Registration is automatic:** the first time the agent creates or edits a document, it registers and persists credentials (e.g. in `~/.memyard/agent_config.json`). No URLs or keys to copy.

Full API reference, request/response formats, and examples: **[SKILL.md](SKILL.md)**.

## Documentation

- **[SKILL.md](SKILL.md)** — API reference, plan/execute flow, and curl examples.
- **[docs/agent-guide.md](docs/agent-guide.md)** — User and agent guide: how writing works, troubleshooting.

## Product

[Memyard](https://memyard.com) — document intelligence and collaboration.

## License

MIT. See [LICENSE](LICENSE).
