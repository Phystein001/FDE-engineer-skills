# Skills Collection

Phystein001 的可复用 Agent Skills 仓库。

## Install

把某个 skill 复制到本地：

```bash
mkdir -p ~/.codex/skills
cp -R skills/<skill-name> ~/.codex/skills/
```

Cursor 个人技能目录也可以：

```bash
mkdir -p ~/.cursor/skills
cp -R skills/<skill-name> ~/.cursor/skills/
```

## Skills

| Skill | 用途 |
|------|------|
| `mobile-ui-prototype` | 按截图还原可交互移动端 HTML |
| `prd-generator` | PRD 生成 |
| `prd-to-prototype` | 需求到高保真原型 |
| `image-to-editable-ppt` | 图片/截图转可编辑 PPT |
| `codex-ppt` | 文章/报告生成统一风格 PPT |
| `business-writing` | 商业写作与研报 |
| `competitive-analysis` | 竞争分析 |
| `prompt-architect` | 提示词设计 |
| 其他 skill | 见 `skills/` 目录 |

## Publish notes

- 每个 skill 都有独立目录，并包含 `SKILL.md`
- 建议按版本打 tag：`v1.0.0`
- 复用时优先遵守各 skill 内的 Use when / Do not use when
