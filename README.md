# clever

Upstream of the `clever` skill (frontmatter name `clever`, directory name `clever`).

Core AI response guidelines, packaged as a Hermes skill.

Seven principles: think before answering, simplicity first, stay within scope,
goal-driven execution, handle uncertainty explicitly, preserve user intent, and
a response quality check before finalizing.

## Install

Hermes Agent:

```bash
hermes skills install https://raw.githubusercontent.com/Geronimolt/Clever/master/skills/clever/SKILL.md --yes
```

Other agents — clone and copy the skill directory into your skills folder:

```bash
git clone https://github.com/Geronimolt/Clever.git
# Claude Code: ~/.claude/skills | Codex: ~/.codex/skills | OpenCode: ~/.config/opencode/skills
cp -r Clever/skills/clever ~/.claude/skills/
```

Hermes loads it via `skills.auto_load`; the `disable-model-invocation` flag keeps it out of per-task selection.

## Auto-load

Hermes:

```bash
hermes config set skills.auto_load '["attention-kind","clever","superpowers:using-superpowers"]'
```

Other agents: add `Always load the clever skill at session start.` to `AGENTS.md`, `CLAUDE.md`, or the equivalent instruction file.

## Layout

```
skills/clever/SKILL.md
```
