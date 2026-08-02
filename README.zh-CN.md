# Tool Permission Matrix

[English](README.md) | **中文**

<p align="center">
  <strong>独立 Agent Skill 项目</strong> · <code>tool-permission-matrix</code>
</p>

<p align="center">
  <a href="LICENSE"><img src="https://img.shields.io/badge/license-MIT-blue.svg" alt="MIT" /></a>
  <a href="https://github.com/agentskills/agentskills"><img src="https://img.shields.io/badge/format-Agent%20Skills-111827" alt="Agent Skills" /></a>
</p>

Build a permission and blast-radius matrix for agent tools. Use when deciding which tools an agent may call, least privilege, or Chinese "工具权限", "爆炸半径", "最小权限", "tool 白名单". Defensive product control - not penetration testing.

---

## 安装（Claude Code）

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

安装到 Claude 时目录名是 **`tool-permission-matrix`**（不加 `skill-` 前缀）：

`~/.claude/skills/tool-permission-matrix/`

装完后请重启 Claude Code。

### 插件方式

```text
/plugin marketplace add Wanbinyu/skill-tool-permission-matrix
/plugin install tool-permission-matrix@tool-permission-matrix
/reload-plugins
```

---

## 这个 skill 做什么

正文说明见 [`SKILL.md`](SKILL.md)（与 `skills/tool-permission-matrix/SKILL.md` 相同）。

触发词在 `SKILL.md` 顶部 YAML 的 `description` 里（常含中英文）。

> **说明：** `SKILL.md` 正文以**英文**为主，方便 agent 稳定执行。  
> 给人看的文档提供双语：[`README.md`](README.md)（英文）+ 本文件（中文）。

---

## 一个 skill = 一个项目

本仓库**只包含这一个 skill**。  
若要一次安装整包相关技能：

- 合集：[ai-surface-skills](https://github.com/Wanbinyu/ai-surface-skills)
- 目录：[`CATALOG.zh-CN.md`](../CATALOG.zh-CN.md) / [`CATALOG.md`](../CATALOG.md)

---

## 目录结构

```text
skill-tool-permission-matrix/   （GitHub）或  solo/tool-permission-matrix/  （本地）
  README.md              # 英文
  README.zh-CN.md        # 中文
  SKILL.md
  skills/tool-permission-matrix/SKILL.md
  scripts/install.ps1
  .claude-plugin/
```

## 许可证

MIT · [Wanbinyu](https://github.com/Wanbinyu)
