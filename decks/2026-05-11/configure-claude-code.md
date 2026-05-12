---
marp: true
theme: default
paginate: true
---

# Configuring the Claude Code CLI

Five slides. Concrete examples. No fluff.

1. Install & auth
2. `settings.json` layers
3. Permissions / allowlist
4. Hooks
5. `CLAUDE.md` memory

---

## 1. Install & auth

```bash
# Install (Node 18+)
npm install -g @anthropic-ai/claude-code

# First run prompts for OAuth in the browser
claude

# Or use an API key directly
export ANTHROPIC_API_KEY=sk-ant-...
claude
```

Verify:

```bash
claude --version
claude config list
```

Config lives at `~/.claude/` (user) and `./.claude/` (project).

---

## 2. `settings.json` — three layers

Merged in this order; later wins:

| Layer    | Path                            | Checked in?     |
|----------|---------------------------------|-----------------|
| User     | `~/.claude/settings.json`       | no              |
| Project  | `./.claude/settings.json`       | yes             |
| Local    | `./.claude/settings.local.json` | no (gitignored) |

Example user `~/.claude/settings.json`:

```json
{
  "model": "claude-opus-4-7",
  "env": { "EDITOR": "nvim" },
  "theme": "dark"
}
```

Project overrides are scoped to the repo — shared with the team.

---

## 3. Permissions / allowlist

Skip prompts for safe, read-only commands. Project `.claude/settings.json`:

```json
{
  "permissions": {
    "allow": [
      "Bash(git status)",
      "Bash(git diff:*)",
      "Bash(npm test:*)",
      "Read(./src/**)",
      "WebFetch(domain:docs.anthropic.com)"
    ],
    "deny": [
      "Bash(rm -rf:*)",
      "Bash(git push --force:*)"
    ]
  }
}
```

`:*` = wildcard suffix. Deny always wins over allow.

---

## 4. Hooks

Run shell commands on lifecycle events. `.claude/settings.json`:

```json
{
  "hooks": {
    "PostToolUse": [{
      "matcher": "Edit|Write",
      "hooks": [{
        "type": "command",
        "command": "prettier --write \"$CLAUDE_FILE_PATHS\""
      }]
    }],
    "Stop": [{
      "hooks": [{
        "type": "command",
        "command": "osascript -e 'display notification \"done\"'"
      }]
    }]
  }
}
```

Events: `PreToolUse`, `PostToolUse`, `UserPromptSubmit`, `Stop`, `Notification`.

---

## 5. `CLAUDE.md` memory

Auto-loaded into context every session. Project root `./CLAUDE.md`:

```markdown
# Project: payments-api

## Stack
- Node 20, TypeScript, Fastify, Postgres 15

## Conventions
- Tests: `npm test -- <file>` (vitest)
- Lint before commit: `npm run lint:fix`
- Never edit `db/migrations/*` manually — use `npm run migrate:create`

## Don't touch
- `src/legacy/**` — frozen, scheduled for deletion 2026-Q3
```

Global user memory: `~/.claude/CLAUDE.md`. Import others with `@./path/to/file.md`.
