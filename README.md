# Memyard Drive

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

Memyard Drive is an agent skill that lets LLM coding agents create and edit Google Docs and Sheets hosted on Memyard — no Google sign-in required. Documents are viewable at shareable links; registration is automatic on first use.

## Installation

Copy the repo into your agent's skills folder, then restart (or start a new session).

| Agent | Command |
|-------|--------|
| **Claude Code** | `git clone https://github.com/zagmoai/memyard-drive.git ~/.claude/skills/memyard-drive` |
| **Cursor** | `git clone https://github.com/zagmoai/memyard-drive.git ~/.cursor/skills/memyard-drive` |
| **Codex** | `git clone https://github.com/zagmoai/memyard-drive.git ~/.codex/skills/memyard-drive` |
| **OpenClaw** | `git clone https://github.com/zagmoai/memyard-drive.git ~/.openclaw/skills/memyard-drive` |

## Usage

Once installed, the agent uses this skill when you ask it to create a document, write to Google Docs/Sheets, or save content to a shareable link.

**Registration is automatic:** the first time the agent creates or edits a document, it registers and persists credentials. No URLs or keys to copy.

Full API reference, request/response formats, and examples: **[SKILL.md](SKILL.md)**.

## Documentation

- **[SKILL.md](SKILL.md)** — API reference, plan/execute flow, and curl examples.
- **[docs/agent-guide.md](docs/agent-guide.md)** — User and agent guide: how writing works, troubleshooting.

## Product

[Memyard](https://memyard.com) — document intelligence and collaboration.

## License

MIT. See [LICENSE](LICENSE).
