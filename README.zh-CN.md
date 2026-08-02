# Tool Permission Matrix

[English](README.md) | **中文**

<p align="center"><strong>一个 skill · 30 秒安装 · 用于 Claude / Codex / Cursor</strong></p>
<p align="center"><code>tool-permission-matrix</code> · MIT · Agent Skills 格式</p>

---

## 先从这里开始

### 安装

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

→ `~/.claude/skills/tool-permission-matrix/` · **请重启 Claude Code**

### 然后可以直接说

- 「用 `tool-permission-matrix` skill 处理我当前的改动」
- 或匹配 `SKILL.md` 顶部 `description` 里的中英文触发词

---

## 这个 skill 解决什么

Build a permission and blast-radius matrix for agent tools. Use when deciding which tools an agent may call, least privilege, or Chinese "工具权限", "爆炸半径", "最小权限", "tool 白名单". Defensive product control - not penetration testing.

完整流程（步骤、完成标准、报告模板）见：**[`SKILL.md`](SKILL.md)**

> 给人看的文档：本页中文 + [English](README.md)。  
> `SKILL.md` 正文以英文为主，方便 agent 稳定执行。

---

## 一个 skill = 一个项目

- 本仓库：**仅** `tool-permission-matrix`
- 整包装：[ai-surface-skills](https://github.com/Wanbinyu/ai-surface-skills)
- 全部独立 skill：https://github.com/Wanbinyu?tab=repositories&q=skill-

### 插件

```text
/plugin marketplace add Wanbinyu/skill-tool-permission-matrix
/plugin install tool-permission-matrix@tool-permission-matrix
```

## 许可证

MIT · [Wanbinyu](https://github.com/Wanbinyu)
