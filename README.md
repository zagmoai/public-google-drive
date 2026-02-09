# Memyard Drive

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

Memyard Drive is an agent skill that lets LLM coding agents create and edit Google Docs and Sheets hosted on Memyard — no Google sign-in required. Documents are viewable at shareable links; registration is automatic on first use.

## Installation

### Claude Code

Clone the repo into Claude Code's personal or project skills directory:

```bash
# Personal (available across all your projects)
git clone https://github.com/zagmoai/memyard-drive.git ~/.claude/skills/memyard-drive

# Or project-scoped (shared via version control)
git clone https://github.com/zagmoai/memyard-drive.git .claude/skills/memyard-drive
```

Claude Code auto-discovers `SKILL.md` files in these directories. The skill will appear as `/memyard-drive` and Claude will also invoke it automatically when you ask to create documents or write to Google Docs/Sheets.

### Cursor

Clone the repo into one of Cursor's skill directories:

```bash
# Personal (available across all your projects)
git clone https://github.com/zagmoai/memyard-drive.git ~/.cursor/skills/memyard-drive

# Or project-scoped (shared via version control)
git clone https://github.com/zagmoai/memyard-drive.git .cursor/skills/memyard-drive
```

Cursor auto-discovers any `SKILL.md` in these directories.

### Codex / OpenClaw

Ask Codex to install the skill:

```
install the memyard-drive skill from zagmoai/memyard-drive
```

This uses the built-in skill installer to place it in `~/.codex/skills/memyard-drive/`.

### upskill

[upskill](https://github.com/trieloff/gh-upskill) can install skills from any GitHub repo into any agent runtime:

```bash
# Install to .claude/skills/ (for Claude Code)
upskill zagmoai/memyard-drive --all --dest-path .claude/skills

# Install globally to ~/.skills/
upskill -g zagmoai/memyard-drive --all
```

### Other runtimes

Clone the repo and point your agent runtime at the `SKILL.md` file.

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
