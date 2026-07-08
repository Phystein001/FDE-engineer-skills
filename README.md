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
| `bmad-advanced-elicitation` | Push the LLM to reconsider, refine, and improve its recent output. ... |
| `bmad-agent-analyst` | Strategic business analyst and requirements expert. Use when the us... |
| `bmad-agent-architect` | System architect and technical design leader. Use when the user ask... |
| `bmad-agent-dev` | Senior software engineer for story execution and code implementatio... |
| `bmad-agent-pm` | Product manager for PRD creation and requirements discovery. Use wh... |
| `bmad-agent-tech-writer` | Technical documentation specialist and knowledge curator. Use when ... |
| `bmad-agent-ux-designer` | UX designer and UI specialist. Use when the user asks to talk to Sa... |
| `bmad-architecture` | Produce the architecture: a lean spine of invariants that keeps eve... |
| `bmad-brainstorming` | Facilitate a brainstorming session using diverse creative technique... |
| `bmad-check-implementation-readiness` | Validate PRD, UX, Architecture and Epics specs are complete. Use wh... |
| `bmad-checkpoint-preview` | LLM-assisted human-in-the-loop review. Make sense of a change, focu... |
| `bmad-code-review` | Review code changes adversarially using parallel review layers (Bli... |
| `bmad-correct-course` | Manage significant changes during sprint execution. Use when the us... |
| `bmad-create-architecture` | DEPRECATED — consolidated into bmad-architecture create intent - th... |
| `bmad-create-epics-and-stories` | Break requirements into epics and user stories. Use when the user s... |
| `bmad-create-prd` | DEPRECATED — consolidated into bmad-prd create intent - this skill ... |
| `bmad-create-story` | Creates a dedicated story file with all the context the agent will ... |
| `bmad-customize` | Authors and updates customization overrides for installed BMad skil... |
| `bmad-dev-auto` | One iteration of an unattended development loop. Use when invoked b... |
| `bmad-dev-story` | Execute story implementation following a context filled story spec ... |
| `bmad-document-project` | Document brownfield projects for AI context. Use when the user says... |
| `bmad-domain-research` | Conduct domain and industry research. Use when the user says wants ... |
| `bmad-edit-prd` | DEPRECATED — consolidated into bmad-prd update intent - this skill ... |
| `bmad-editorial-review-prose` | Clinical copy-editor that reviews text for communication issues. Us... |
| `bmad-editorial-review-structure` | Structural editor that proposes cuts, reorganization, and simplific... |
| `bmad-forge-idea` | Pressure-test an idea through persona-driven interrogation until it... |
| `bmad-generate-project-context` | Create project-context.md with AI rules. Use when the user says "ge... |
| `bmad-help` | Analyzes current state and user query to answer BMad questions or r... |
| `bmad-index-docs` | Generates or updates an index.md to reference all docs in the folde... |
| `bmad-market-research` | Conduct market research on competition and customers. Use when the ... |
| `bmad-party-mode` | Orchestrates lively group discussions between installed BMAD agents... |
| `bmad-prd` | Create, update, or validate a PRD. Use when the user wants help pro... |
| `bmad-prfaq` | Working Backwards PRFAQ challenge that stress-tests a product conce... |
| `bmad-product-brief` | Create, update, or validate a product brief. Use when the user want... |
| `bmad-qa-generate-e2e-tests` | Generate end to end automated tests for existing features. Use when... |
| `bmad-quick-dev` | Implements any user intent, requirement, story, bug fix or change r... |
| `bmad-retrospective` | Post-epic review to extract lessons and assess success. Use when th... |
| `bmad-review-adversarial-general` | Perform a Cynical Review and produce a findings report. Use when th... |
| `bmad-review-edge-case-hunter` | Walk every branching path and boundary condition in content, report... |
| `bmad-shard-doc` | Splits large markdown documents into smaller, organized files based... |
| `bmad-spec` | Distill any intent input into the SPEC kernel + companions — the ca... |
| `bmad-sprint-planning` | Generate sprint status tracking from epics. Use when the user says ... |
| `bmad-sprint-status` | Summarize sprint status and surface risks. Use when the user says "... |
| `bmad-technical-research` | Conduct technical research on technologies and architecture. Use wh... |
| `bmad-ux` | Plan UX patterns and design specifications. Use when the user says ... |
| `bmad-validate-prd` | DEPRECATED — consolidated into bmad-prd validate intent - this skil... |
| 其他 skill | 见 `skills/` 目录 |

## Publish notes

- 每个 skill 都有独立目录，并包含 `SKILL.md`
- 建议按版本打 tag：`v1.0.0`
- 复用时优先遵守各 skill 内的 Use when / Do not use when
