# Memyard Drive

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

Memyard Drive is an agent skill that lets LLM coding agents create and edit Google Docs and Sheets hosted on Memyard — no Google sign-in required. Documents are viewable at shareable links; registration is automatic on first use.

## Installation

### Claude Code

Personal (all your projects):

```bash
git clone https://github.com/zagmoai/memyard-drive.git ~/.claude/skills/memyard-drive
```

Project-scoped (shared via version control):

```bash
git clone https://github.com/zagmoai/memyard-drive.git .claude/skills/memyard-drive
```

Claude Code auto-discovers `SKILL.md` in these directories. The skill appears as `/memyard-drive` and Claude will also invoke it automatically when relevant.

### Cursor

**Option A — clone:**

```bash
git clone https://github.com/zagmoai/memyard-drive.git ~/.cursor/skills/memyard-drive
```

**Option B — Cursor UI:**
Cursor Settings -> Rules -> Add Rule -> Remote Rule (Github) -> enter `https://github.com/zagmoai/memyard-drive`.

Cursor also discovers skills from `.claude/skills/` and `.codex/skills/` directories for cross-tool compatibility, so a single clone into `~/.claude/skills/` works for both Claude Code and Cursor.

### Codex (OpenAI)

**Option A — inside a Codex session**, use the built-in `$skill-installer`:

```
$skill-installer install https://github.com/zagmoai/memyard-drive
```

It installs to `~/.codex/skills/`. Restart Codex after installing.

**Option B — manual:**

Codex loads user skills from `~/.agents/skills/` per the [official docs](https://developers.openai.com/codex/skills). Some setups use `~/.codex/skills/` instead. Clone into whichever your Codex uses:

```bash
git clone https://github.com/zagmoai/memyard-drive.git ~/.agents/skills/memyard-drive
# or, if your Codex uses that path:
# git clone https://github.com/zagmoai/memyard-drive.git ~/.codex/skills/memyard-drive
```

### OpenClaw

```bash
# Global (shared across all agents)
git clone https://github.com/zagmoai/memyard-drive.git ~/.openclaw/skills/memyard-drive
```

Start a new OpenClaw session to pick up the skill.

### Other runtimes

Clone the repo and point your agent runtime at the `SKILL.md` file at the repository root.

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
