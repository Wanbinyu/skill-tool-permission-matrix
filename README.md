# Tool Permission Matrix

**English** | [中文](README.zh-CN.md)

<p align="center">
  <strong>Standalone Agent Skill</strong> · <code>tool-permission-matrix</code>
</p>

<p align="center">
  <a href="LICENSE"><img src="https://img.shields.io/badge/license-MIT-blue.svg" alt="MIT" /></a>
  <a href="https://github.com/agentskills/agentskills"><img src="https://img.shields.io/badge/format-Agent%20Skills-111827" alt="Agent Skills" /></a>
</p>

Build a permission and blast-radius matrix for agent tools. Use when deciding which tools an agent may call, least privilege, or Chinese "工具权限", "爆炸半径", "最小权限", "tool 白名单". Defensive product control - not penetration testing.

---

## Install (Claude Code)

```powershell
git clone https://github.com/Wanbinyu/skill-tool-permission-matrix.git
cd skill-tool-permission-matrix
.\scripts\install.ps1 -Claude
```

```bash
git clone https://github.com/Wanbinyu/skill-tool-permission-matrix.git
cd skill-tool-permission-matrix
chmod +x scripts/install.sh
./scripts/install.sh --claude
```

Claude skill id remains **`tool-permission-matrix`** (no `skill-` prefix):

`~/.claude/skills/tool-permission-matrix/`

Restart Claude Code after install.

### Plugin

```text
/plugin marketplace add Wanbinyu/skill-tool-permission-matrix
/plugin install tool-permission-matrix@tool-permission-matrix
/reload-plugins
```

---

## What this skill does

See [`SKILL.md`](SKILL.md) (same as `skills/tool-permission-matrix/SKILL.md`).

The YAML `description` at the top of `SKILL.md` holds triggers (often EN + ZH).

> **Note:** `SKILL.md` body is English so agents follow instructions reliably.  
> Human docs are bilingual: this file + [`README.zh-CN.md`](README.zh-CN.md).

---

## One skill = one project

This repo ships **only this skill**.  
Bulk install of related skills:

- Collection: [ai-surface-skills](https://github.com/Wanbinyu/ai-surface-skills)
- Catalog: [`CATALOG.md`](../CATALOG.md) / [`CATALOG.zh-CN.md`](../CATALOG.zh-CN.md) (local `G:\\skill\\solo`)

---

## Layout

```text
skill-tool-permission-matrix/   (GitHub)  or  solo/tool-permission-matrix/  (local)
  README.md              # English
  README.zh-CN.md        # Chinese
  SKILL.md
  skills/tool-permission-matrix/SKILL.md
  scripts/install.ps1
  .claude-plugin/
```

## License

MIT · [Wanbinyu](https://github.com/Wanbinyu)
