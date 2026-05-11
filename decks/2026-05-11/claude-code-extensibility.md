---
marp: true
theme: default
paginate: true
---

# Extending Claude Code

> Four primitives. Small, composable, project-local.

- **Skills** — packaged, on-demand capabilities
- **Subagents** — delegated worker contexts
- **Hooks** — deterministic shell triggers
- **Rules / Memory** — `CLAUDE.md` and friends

Pick what you need; ignore the rest.

---

## Capability primitives — Skills & Subagents

**Skills**

- Live under `.claude/skills/<name>/` as a `SKILL.md` plus optional scripts and references
- The `SKILL.md` frontmatter declares triggers; loaded only when the model decides it's relevant
- Keeps your base context lean — capability stays cold until needed

**Subagents**

- Spawned via the `Agent` tool; each gets its own Claude context
- Have a separate system prompt, tool allowlist, and scratch space
- Use for: investigation, parallel work, context isolation

> Skills give the agent *what to do*; subagents give it *who does it*.

---

## Control primitives — Hooks & Rules

**Hooks** (`~/.claude/settings.json` or project `.claude/settings.json`)

- Shell commands wired to lifecycle events: `PreToolUse`, `PostToolUse`, `Stop`, `SessionStart`, …
- Run by the harness, not the model — automation is guaranteed
- Typical uses: auto-format on write, block dangerous commands, append session logs

**Rules / Memory**

- `CLAUDE.md` — project memory loaded every session (conventions, architecture, do / don't)
- `~/.claude/CLAUDE.md` — user-global memory
- Slash commands under `.claude/commands/` for reusable prompts

> Skills + subagents extend *ability*. Hooks + rules extend *policy*.

Next step: peek at `~/.claude/settings.json` and `.claude/skills/`.
