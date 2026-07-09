# FDE工程师skill合集

面向 FDE（Field Deployment Engineer / 落地交付工程师）与产品研发全流程的可复用 Agent Skills 仓库。

覆盖从想法验证、需求分析、方案设计到开发交付、评审复盘的完整链路，可在 **Codex** / **Cursor** 中直接调用。

## 安装

复制单个 skill 到本地：

```bash
# Codex
mkdir -p ~/.codex/skills
cp -R skills/<skill-name> ~/.codex/skills/

# Cursor
mkdir -p ~/.cursor/skills
cp -R skills/<skill-name> ~/.cursor/skills/
```

在 Codex 中也可输入 `/skills` 查看已加载的 skill，或通过 `/skill名`、`$skill名` 调用。

---

## Skills 总览（按产品诞生阶段）

### 1. 分析阶段（为什么做）

| Skill | 作用 | 使用方法 |
|------|------|----------|
| `bmad-brainstorming` | 创意头脑风暴，用多种技法发散想法 | 说「帮我头脑风暴」或 `$bmad-brainstorming` |
| `bmad-forge-idea` | 人格化拷问，压力测试想法是否站得住 | 说「压力测试这个想法」或「打磨这个 idea」 |
| `bmad-product-brief` | 创建 / 更新 / 校验产品简报 Product Brief | 说「写个产品简报」或「product brief」 |
| `bmad-prfaq` | Working Backwards PRFAQ，从客户反推产品概念 | 说「做 PRFAQ」或「从客户倒推」 |
| `bmad-domain-research` | 行业 / 领域调研 | 说「做领域调研」 |
| `bmad-market-research` | 市场与竞品调研 | 说「做市场调研」 |
| `bmad-technical-research` | 技术与架构可行性调研 | 说「做技术调研报告」 |
| `bmad-document-project` | 为存量项目生成 AI 可用文档上下文 | 说「记录这个项目」或「生成项目文档」 |
| `bmad-spec` | 将意图蒸馏成可下游执行的 SPEC 规范 | 说「做成 spec」或「创建规范」 |
| `bmad-agent-analyst` | 召唤业务分析师人格（Mary） | 说「找分析师」或「找 Mary」 |

### 2. 规划阶段（做什么）

| Skill | 作用 | 使用方法 |
|------|------|----------|
| `bmad-prd` | 创建 / 更新 / 校验 PRD（主入口，推荐使用） | 说「写 PRD」「改 PRD」「校验 PRD」 |
| `prd-to-prototype` | **PRD to Prototype**：从想法零提问直出 PRD，再生成移动端/PC 端高保真 HTML 原型 | 说「我想做一个…」「帮我设计…」，或 `$prd-to-prototype`；PRD 生成后回复「确认移动端」/「确认PC端」 |
| `bmad-ux` | UX 设计模式与交互规格 | 说「做 UX 设计」或「写 UX 规格」 |
| `bmad-agent-pm` | 召唤产品经理人格（John） | 说「找 PM」或「找 John」 |
| `bmad-agent-ux-designer` | 召唤 UX 设计师人格（Sally） | 说「找 UX」或「找 Sally」 |
| `bmad-create-prd` | ~~已弃用~~，功能已并入 `bmad-prd` | 请改用 `$bmad-prd` |
| `bmad-edit-prd` | ~~已弃用~~，功能已并入 `bmad-prd` | 请改用 `$bmad-prd` |
| `bmad-validate-prd` | ~~已弃用~~，功能已并入 `bmad-prd` | 请改用 `$bmad-prd` |

### 3. 方案设计阶段（怎么做）

| Skill | 作用 | 使用方法 |
|------|------|----------|
| `bmad-architecture` | 产出技术架构方案（主入口，推荐使用） | 说「写架构」或「做技术方案」 |
| `bmad-create-epics-and-stories` | 将需求拆分为 Epic 与用户故事 | 说「拆 epic 和 story」 |
| `bmad-create-story` | 为单个故事生成可实施的 story 文件 | 说「创建下一个 story」 |
| `bmad-check-implementation-readiness` | 检查 PRD / UX / 架构 / Epics 是否可开工 | 说「检查是否可以开工」 |
| `bmad-generate-project-context` | 生成 `project-context.md`（AI 编码约束） | 说「生成项目上下文」 |
| `bmad-agent-architect` | 召唤架构师人格（Winston） | 说「找架构师」或「找 Winston」 |
| `bmad-create-architecture` | ~~已弃用~~，功能已并入 `bmad-architecture` | 请改用 `$bmad-architecture` |

### 4. 实施阶段（落地交付）

| Skill | 作用 | 使用方法 |
|------|------|----------|
| `bmad-sprint-planning` | 从 Epics 生成冲刺计划与状态跟踪 | 说「做 sprint planning」 |
| `bmad-sprint-status` | 查看冲刺进度与风险 | 说「看 sprint 状态」 |
| `bmad-dev-story` | 按 story 文件落地实现代码 | 说「开发这个 story」 |
| `bmad-quick-dev` | 快速实现功能、修 bug、小改动 | 直接描述要改的内容即可 |
| `bmad-dev-auto` | 无人值守开发循环（单轮迭代） | `$bmad-dev-auto` |
| `bmad-code-review` | 对抗式多层代码审查 | 说「做 code review」 |
| `bmad-checkpoint-preview` | 人工检查点：带你走读变更重点 | 说「checkpoint」或「带我看下这次改动」 |
| `bmad-correct-course` | Sprint 中途重大变更纠偏 | 说「纠偏」或「correct course」 |
| `bmad-qa-generate-e2e-tests` | 为已有功能生成 E2E 自动化测试 | 说「给某某功能写 E2E 测试」 |
| `bmad-retrospective` | Epic 复盘，沉淀经验 | 说「做 retrospective」或「复盘这个 epic」 |
| `bmad-agent-dev` | 召唤开发者人格（Amelia） | 说「找开发」或「找 Amelia」 |
| `bmad-agent-tech-writer` | 召唤技术文档写手人格（Paige） | 说「找文档写手」或「找 Paige」 |

### 5. 跨阶段通用

| Skill | 作用 | 使用方法 |
|------|------|----------|
| `bmad-help` | 根据当前状态推荐下一步该用哪个 skill | 说「bmad help」或「下一步做什么」 |
| `bmad-party-mode` | 多 Agent 圆桌讨论，或自定义讨论团 | 说「开党会 / party mode / 圆桌」 |
| `bmad-advanced-elicitation` | 用苏格拉底、红队、事前验尸等方法深挖输出 | 说「再深挖一下」「红队挑战」 |
| `bmad-customize` | 自定义 / 覆盖 BMAD skill 行为 | 说「自定义 bmad」或「override skill」 |
| `bmad-editorial-review-prose` | 文风与表达审阅 | 说「润色文风」或「prose review」 |
| `bmad-editorial-review-structure` | 文档结构重组与精简建议 | 说「看下结构」或「structural review」 |
| `bmad-review-adversarial-general` | 批判性审查，产出问题清单 | 说「批判性审查一下」 |
| `bmad-review-edge-case-hunter` | 穷尽边界条件与分支路径 | 说「找边界情况」 |
| `bmad-index-docs` | 为目录生成 / 更新 `index.md` | 说「给这个目录做索引」 |
| `bmad-shard-doc` | 按二级标题拆分大文档 | 说「拆分文档」或「shard document」 |

### 其他实用 Skills（原合集）

| Skill | 作用 |
|------|------|
| `mobile-ui-prototype` | 按截图还原可交互移动端 HTML |
| `prd-generator` | 专业级 PRD 生成（用例、数据字典、交互与 UI 规范） |
| `image-to-editable-ppt` | 图片 / 截图转可编辑 PPT |
| `codex-ppt` | 文章 / 报告生成统一风格 PPT |
| `business-writing` | 商业写作与研报 |
| `competitive-analysis` | 竞争分析 |
| `prompt-architect` | 提示词设计 |
| 其他 | 见 `skills/` 目录 |

---

## 推荐主链路

```text
bmad-help
  → bmad-brainstorming / bmad-forge-idea
  → bmad-product-brief / bmad-prfaq
  → bmad-prd
  → bmad-ux
  → bmad-architecture
  → bmad-create-epics-and-stories
  → bmad-sprint-planning
  → bmad-create-story
  → bmad-dev-story
  → bmad-code-review
```

不确定从哪开始时，先调用：`$bmad-help`

**快速出原型链路（适合 FDE 早期验证）：**

```text
prd-to-prototype
  → 直出 PRD（docs/prd.md）
  → 确认移动端 / PC 端
  → 生成可交互 HTML 原型（prototype/）
```

来源：[ClawHub — PRD to Prototype](https://clawhub.ai/zengxming45/prd-to-prototype)（v1.0.0）

---

## 说明

- 每个 skill 均为独立目录，并包含 `SKILL.md`
- 目录名即 skill 名（如 `bmad-prd`），便于按需复制安装
- 建议按版本打 tag：`v1.0.0`
- 使用时优先遵守各 skill 内的触发条件与约束
