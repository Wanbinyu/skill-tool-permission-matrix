# Tool Permission Matrix

**English** | [中文](README.zh-CN.md)

<p align="center"><strong>One skill. Install in 30 seconds. Use in Claude / Codex / Cursor.</strong></p>
<p align="center"><code>tool-permission-matrix</code> · MIT · Agent Skills format</p>

---

## Start here

### Install

```powershell
git clone https://github.com/Wanbinyu/skill-tool-permission-matrix.git
cd skill-tool-permission-matrix
.\scripts\install.ps1 -Claude
```

```bash
git clone https://github.com/Wanbinyu/skill-tool-permission-matrix.git
cd skill-tool-permission-matrix
chmod +x scripts/install.sh && ./scripts/install.sh --claude
```

→ `~/.claude/skills/tool-permission-matrix/` · **Restart Claude Code**

### Then say (examples)

- *Use the `tool-permission-matrix` skill on my current change.*
- Or any phrase matching the triggers in `SKILL.md` frontmatter (EN + ZH).

---

## What this skill is for

Build a permission and blast-radius matrix for agent tools. Use when deciding which tools an agent may call, least privilege, or Chinese "工具权限", "爆炸半径", "最小权限", "tool 白名单". Defensive product control - not penetration testing.

Full workflow (steps, exit criteria, report template): **[`SKILL.md`](SKILL.md)**

> Human docs: EN + [中文](README.zh-CN.md).  
> `SKILL.md` body is English so agents execute consistently.

---

## One skill = one project

- This repo: **only** `tool-permission-matrix`
- Bulk packs: [ai-surface-skills](https://github.com/Wanbinyu/ai-surface-skills)
- All solo skills: https://github.com/Wanbinyu?tab=repositories&q=skill-

### Plugin

```text
/plugin marketplace add Wanbinyu/skill-tool-permission-matrix
/plugin install tool-permission-matrix@tool-permission-matrix
```

## License

MIT · [Wanbinyu](https://github.com/Wanbinyu)
