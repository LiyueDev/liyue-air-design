# liyue-air-design

一套给 AI Agent 用的设计风格 Skill。**只给风格方向，不规定版式** —— 官网、后台、小组件都能共用同一套观感，不会被固定的首屏结构或栅格约束。

A visual style skill for AI agents. It describes how things should *look*, not how pages should be *structured*.

## 包含什么

只有两个文件：

| 文件 | 作用 |
| --- | --- |
| `SKILL.md` | 风格描述：气质、配色、字体、质感、动效的取向 |
| `references/tokens.md` | 数值查表：色值、字号区间、圆角、阴影、图标规格 |

页面怎么组织由项目自己决定，这份 Skill 不参与。

## 风格速览

- **气质**：白净、通透、克制、安静，产品优先
- **主色**：`#2F6BEE`，深一档 `#2359D6`，浅底 `#DCE9FF`
- **中性色**：`#161C28` / `#5F6570` / `#8A919F`，页底 `#F8FAFE`
- **面板渐变**：`#FFFFFF → #E8F0FE`
- **字体**：Noto Sans SC 优先，英文 Segoe UI 一族
- **质感**：细描边、收敛圆角、轻而偏蓝的阴影、线性图标

## 安装

克隆仓库：

```bash
git clone https://github.com/QinHaoR/liyue-air-design.git
```

把 `liyue-air-design/` 目录复制到你的 Agent skills 目录：

| Agent | Skills 目录 |
| --- | --- |
| WorkBuddy | `~/.workbuddy/skills/` |
| Claude Code | `~/.claude/skills/` |
| Codex | `~/.codex/skills/` |

Windows PowerShell 示例：

```powershell
git clone https://github.com/QinHaoR/liyue-air-design.git
Copy-Item -Recurse .\liyue-air-design "$HOME\.workbuddy\skills\"
```

macOS / Linux 示例：

```bash
git clone https://github.com/QinHaoR/liyue-air-design.git
cp -R ./liyue-air-design ~/.claude/skills/
```

复制完成后重启 Agent 或刷新 Skill 列表。

## 使用

安装后用自然语言唤起即可，不需要记命令：

- 「用我的风格做个落地页」
- 「按 liyue-air 的风格美化这个界面」
- 「用黎月风格设计一个小组件」

Skill 靠描述里的触发词自动匹配，也可以直接写 `/liyue-air-design`（视 Agent 是否支持斜杠调用）。

## 许可

MIT
