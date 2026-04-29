# 🚀 Software Product Development Framework

> **Interested in this idea? Let's build it together!** Contact me: wmw88800@163.com

[English](#-software-product-development-framework) | [中文](#-软件产品研发流程框架)

---

![No Coding](https://img.shields.io/badge/Goal-No_Coding-ff6b6b)
![Vibe Coding](https://img.shields.io/badge/Vibe_Coding-Enabled-blueviolet)
![Harness Engineering](https://img.shields.io/badge/Harness_Engineering-Powered-orange)
![AI Driven](https://img.shields.io/badge/AI-Driven-4ea8de)
![Document Driven](https://img.shields.io/badge/Document-Driven-2ecc71)
![License](https://img.shields.io/badge/License-MIT-lightgrey)

---

> ### Marching Toward No-Coding
> **A structured Boss × AI Agent collaboration framework covering the complete process from "idea" to "deployment & beyond".**

## 🌐 Design Philosophy

The ultimate destination of AI Coding evolution is freeing humans entirely from thinking in code at the application layer — this is not a distant future, but a trend already unfolding.

**This framework is the first step on the path to No-Coding.** It replaces "code-driven" with "document-driven", pushing projects with well-defined requirements infinitely closer to the goal of "fully AI-generated, zero human intervention."

The core design principle is **assigning Agents by phase** — different phases can plug in different models and Agents based on capability and cost:

| Phase | Agent Strategy |
|-------|---------------|
| 📐 Planning & Architecture | High-capability Agent + strongest model, ensuring decision quality |
| 🔨 Development Execution | Cost-efficient Agent cluster, executing task cards in parallel |
| 🧪 Testing & Validation | Orchestrated workflows + AI combination for automated testing and regression |
| 🚀 Deployment & Operations | DevOps Agent for infrastructure assessment, deployment execution, and monitoring |

This design thinking is not limited to the current version's scope — as AI capabilities evolve, each phase of the framework can progressively adopt more autonomous Agent implementations.

## 📖 What is this?

This is a **document-based** software product development framework that defines a complete collaboration process from product idea to deployment and iteration.

In this framework:
- 🧑 **Boss** is the only human role, responsible for proposing ideas, making decisions, approving deliverables, procurement, and leading retrospectives
- 🤖 **AI Agents** play professional roles such as Product Analyst, Requirements Engineer, Quality Reviewer, Technical Architect, QA Engineer, DevOps Manager, etc.
- 🔄 **Agents are swappable** — you can replace any Agent with alternatives, such as those from [gstack](https://github.com/garrytan/gstack), [agency-agents](https://github.com/msitarzewski/agency-agents), or [agency-agents-zh](https://github.com/jnMetaCode/agency-agents-zh)
- 📄 **All progress is captured in documents** — you can pause, modify, or roll back at any time based on the document trail

The framework provides complete **process definitions + document templates + example content**, ready to use out of the box.

## 🎯 What problems does it solve?

- ❌ Many personal project ideas but lack systematic organization process
- ❌ Directly asking AI to write code, skipping requirements analysis and architecture design
- ❌ AI-generated documents lack structure and have unstable quality
- ❌ No structured testing, deployment, or feedback loop after coding
- ✅ **This framework enables you to collaborate with AI Agents following a professional 10-phase, 21-step development process**, ensuring each step has input, output, and validation

## 🔄 Core Workflow

The framework covers 10 phases and 21 steps, from initial idea to deployment and retrospective:

```
Idea → Requirements → Validation → Technical Design → Task Decomposition → Coding → Testing & Acceptance → Deployment → Retrospective
```

| Step | Role | Deliverable |
|------|------|-------------|
| 1 | 👔 Boss | Initial Idea |
| 2 | 🔍 Product Analyst | Complete Idea (Draft) |
| 3 | 👔 + 🔍 Collaboration | Complete Idea (Final) |
| 4 | 📋 Requirements Engineer | PRD (Draft) |
| 5 | 👔 + 📋 Collaboration | PRD (Final) |
| 6 | 🛡️ Quality Reviewer + 👔 | PRD Consistency Validation + Decision |
| 7 | 🏗️🖥️⚙️🎨 All Architects + UI | Technical Kickoff Consensus |
| 8 | Four roles in parallel | Architecture / Frontend / Backend / UI Design |
| 9 | 🛡️ Quality Reviewer | Design Coupling Validation Report |
| 9b | 👔 + All Roles | Diagnosis Meeting (triggered when step 9 fails) |
| 10 | 👔 Boss | Final Approval |
| 11 | 🏗️🖥️⚙️🎨 All roles in parallel | Task Cards (decomposed into executable units) |
| 12 | 👔 + All Architects | Task Cross-review |
| — | All tech roles | Coding Execution (parallel, per task board) |
| 13 | 🧪 QA Engineer | Test Cases (parallel with coding) |
| 14 | 🧪 QA Engineer | Module Testing + Integration Testing + PRD Traceability |
| 15 | 🧪 QA Engineer | Test Report |
| 16 | 👔 Boss | Acceptance Approval |
| 16b | All Roles | Acceptance Diagnosis Meeting (triggered after 10+ failures) |
| 17 | 🚀 DevOps Manager | Deployment Requirements & Deliverables Checklist |
| 18 | 👔 Boss | Procurement & Handover |
| 19 | 🚀 DevOps Manager | Deployment Execution & Verification |
| 20 | 🚀 + 🔍 | Collect Runtime Data & User Feedback |
| 21 | 👔 Boss + All Roles | Retrospective Meeting → Next Iteration |

> 📄 For complete flowchart and step details, see [`00-流程与规范/研发流程总览.md`](00-流程与规范/研发流程总览.md)

## 👥 Agent Roles

| Role | Type | Responsibilities | Key Steps |
|------|------|------------------|-----------|
| 👔 Boss | 🧑 Human | Vision, decisions, approval, procurement, retrospective | 1,3,5,6,9b,10,12,16,16b,18,21 |
| 🔍 Product Analyst | 🤖 Agent | Expand ideas, clarify questions, collect feedback | 2,3,16b,20,21 |
| 📋 Requirements Engineer | 🤖 Agent | Transform ideas into structured PRD | 4,5,21 |
| 🛡️ Quality Reviewer | 🤖 Agent | Document consistency & design coupling validation | 6,9,21 |
| 🏗️ Technical Architect | 🤖 Agent | System architecture, tech selection, task decomposition, coding | 7,8a,9b,11a,12,coding,16b,21 |
| 🖥️ Frontend Architect | 🤖 Agent | Frontend architecture, routing, state management, coding | 7,8b,9b,11b,12,coding,16b,21 |
| ⚙️ Backend Architect | 🤖 Agent | API design, data models, service architecture, coding | 7,8c,9b,11c,12,coding,16b,21 |
| 🎨 UI/UX Designer | 🤖 Agent | Design system, wireframes, interaction prototypes, coding | 7,8d,9b,11d,12,coding,16b,21 |
| 🧪 QA Engineer | 🤖 Agent | Test cases, execution, defect tracking, reports | 13,14,15,16,16b,21 |
| 🚀 DevOps Manager | 🤖 Agent | Deployment assessment, resource verification, deployment | 17,19,20,21 |

## 📁 Directory Structure

```
Project Root/
├── 00-流程与规范/           ← Process definitions, Agent roles, version management
├── 01-初步想法/             ← Boss's initial idea (template + example)
├── 02-完整想法/             ← Product Analyst's complete idea (template + example)
├── 03-产品需求文档/         ← Requirements Engineer's PRD (template + example)
├── 04-校验记录/             ← Quality Reviewer's validation (template + example)
├── 05-技术与设计方案/       ← Technical & Design Solutions
│   ├── 技术初步共识/        ← Step 7: Kickoff consensus
│   ├── 整体架构/            ← Technical Architect (template + example)
│   ├── 前端方案/            ← Frontend Architect (template + example)
│   ├── 后端方案/            ← Backend Architect (template + example), with API docs
│   └── UI设计/              ← UI/UX Designer (template)
├── 06-全局任务管理/         ← Global task board and task cards
├── 07-测试验收/             ← QA Engineer: test cases, defect reports, test reports, acceptance
├── 08-部署上线/             ← DevOps Manager: deployment requirements, verification reports
├── 09-迭代复盘/             ← Retrospective reports
└── 归档/                    ← Historical version archive
```

**Each directory contains:**
- **`_模板-xxx.md`**: Blank templates for creating new documents
- **`示例-xxx.md`**: Complete examples based on "Smart Todo App"

## 🚀 Quick Start

### 1. Clone the Repository

```bash
git clone https://github.com/Challiwei/common-project-development-framework.git
```

### 2. Open with Obsidian

Open the cloned directory as an Obsidian Vault to see the complete document structure and internal links.

### 3. Start Your Project

1. Read [`00-流程与规范/研发流程总览.md`](00-流程与规范/研发流程总览.md) to understand the complete process
2. Copy `01-初步想法/_模板-初步想法.md` and write down your product idea
3. Follow the 21-step process to collaborate with AI Agents, completing the journey from idea to deployment

## 💡 Use Cases

- **Individual Developers**: Use AI to help with product analysis, architecture, testing, and deployment
- **Small Teams**: Establish unified collaboration processes and documentation standards
- **Learning Reference**: Understand the complete development lifecycle from idea to production
- **Obsidian Users**: A ready-to-use project management template

## 📋 Example Content

The project includes a complete **"Smart Todo App"** example, covering process steps from initial idea to API documentation, helping you understand what each deliverable should look like.

## 🤝 Contributing

Welcome to submit Issues and Pull Requests! Common contribution directions:

- Optimize existing template content
- Improve process specifications
- Provide translations in other languages
- Share your experience using this framework

## 📄 License

This project is open-sourced under the [MIT License](LICENSE).

## 📝 Changelog

### v4.0 - 2026-04-29

**New Phases & Steps**

1. **Coding Execution Phase** — All tech roles execute coding tasks per the global task board in independent sessions
2. **Testing & Acceptance Phase (Steps 13–16b)** — QA Engineer writes test cases (parallel with coding), executes module & integration tests with PRD traceability, produces test reports, and assists Boss with acceptance
3. **Deployment Phase (Steps 17–19)** — DevOps Manager assesses infrastructure needs, Boss procures resources, DevOps Manager verifies deliverables and executes deployment
4. **Retrospective Phase (Steps 20–21)** — Collect runtime data & user feedback, all-hands retrospective meeting, output action items for next iteration

**New Agent Roles**

- 🧪 **QA Engineer**: Test case authoring, module/integration testing, PRD requirement traceability, defect tracking, test reports
- 🚀 **DevOps Manager**: Deployment requirements assessment, resource verification, deployment execution, runtime data collection

**New Templates**

- `07-测试验收/`: Test case, defect report, test report, acceptance report templates
- `08-部署上线/`: Deployment requirements checklist, deployment verification report templates
- `09-迭代复盘/`: Version retrospective report template

**Other Changes**

- Added cross-boundary dependency collaboration section to global task board
- Updated all existing roles with coding execution, testing, and retrospective participation steps
- Added `项目记录.md` for project progress tracking

---

### v3.0 - 2026-04-27

**New Features**

1. **Design Coupling Validation (Step 9)** — Quality Reviewer validates consistency across four design documents and PRD coverage
2. **All-hands Diagnosis Meeting (Step 9b)** — Triggered when coupling validation fails; root cause determines fix scope
3. **Boss Final Approval (Step 10)** — Separated from collective review into objective validation + subjective approval
4. **Task Decomposition (Steps 11 & 12)** — Parallel task card decomposition with 65% context capacity rule + cross-review

---

### v2.0 - 2026-04-24

**New Features**

1. **UI/UX Designer Role** — Design specification and interaction prototype templates
2. **Technical Kickoff Meeting (Step 7)** — Boundary and constraint alignment before parallel work
3. **Global Task Management** — Task card template, global task board, 65% context capacity rule
4. **CLAUDE.md** — Project guidance for Claude Code

**Structure Changes**

- Directory renamed: `05-技术架构/` → `05-技术与设计方案/`
- Workflow optimized: Original steps 7-10 adjusted to steps 7-9

---

# 🚀 软件产品研发流程框架

> **对这个想法有兴趣？一起来把它做出来！** 联系我：wmw88800@163.com

[English](#-software-product-development-framework) | [中文](#-软件产品研发流程框架)

---

![No Coding](https://img.shields.io/badge/Goal-No_Coding-ff6b6b)
![Vibe Coding](https://img.shields.io/badge/Vibe_Coding-Enabled-blueviolet)
![Harness Engineering](https://img.shields.io/badge/Harness_Engineering-Powered-orange)
![AI Driven](https://img.shields.io/badge/AI-Driven-4ea8de)
![Document Driven](https://img.shields.io/badge/Document-Driven-2ecc71)
![License](https://img.shields.io/badge/License-MIT-lightgrey)

---

> ### 为了无代码（No Coding）而努力向前
> **一套结构化的 Boss × AI Agent 协作研发框架，覆盖从「灵感」到「部署上线及迭代复盘」的完整流程。**

## 🌐 设计理念

AI Coding 的演进终点，是人类在应用层彻底从代码思维中解放出来——这不是遥远的未来，而是正在发生的趋势。

**本框架是迈向 No-Coding 路径上的第一步。** 它用「文档驱动」替代「代码驱动」，让需求足够明确的项目无限接近于「全 AI 自动生成、无需人工干预」的目标。

框架的核心设计思路是**按阶段分配 Agent**，不同阶段可替换不同能力和成本的模型与 Agent：

| 阶段 | Agent 策略 |
|------|------------|
| 📐 规划 & 架构 | 高消耗 Agent + 最强模型，保证决策质量 |
| 🔨 研发执行 | 高性价比 Agent 集群，批量并行执行任务卡片 |
| 🧪 测试验证 | 编排工作流 + AI 组合，覆盖自动化测试与回归 |
| 🚀 部署运维 | 运维 Agent 评估基础设施、执行部署、监控运行 |

这个设计思路不限于当前版本的覆盖范围——随着 AI 能力的演进，框架的每个阶段都可以逐步接入更自动化的 Agent 实现。

## 📖 这是什么？

这是一个**基于文档**的软件产品研发流程框架，定义了从产品想法到部署上线及迭代复盘的完整协作流程。

在这个框架中：
- 🧑 **老板（Boss）** 是唯一的人类角色，负责提出想法、做出决策、审批产出物、完成采购交付、主持复盘
- 🤖 **AI Agent** 扮演产品分析师、需求工程师、质量审核员、技术架构师、测试工程师、运维经理等专业角色
- 🔄 **Agent 可随时替换** — 你可以替换为任何其他 Agent 实现，例如 [gstack](https://github.com/garrytan/gstack)、[agency-agents](https://github.com/msitarzewski/agency-agents)、[agency-agents-zh](https://github.com/jnMetaCode/agency-agents-zh) 中的 Agent
- 📄 **所有进度都落到文档中** — 基于文档可以随时暂停、修改、回退

框架提供了完整的 **流程定义 + 文档模板 + 示例内容**，开箱即用。

## 🎯 解决什么问题？

- ❌ 个人项目想法多，但缺乏系统性梳理流程
- ❌ 直接让 AI 写代码，跳过了需求分析和架构设计
- ❌ AI 产出的文档缺乏结构，质量不稳定
- ❌ 编码完成后缺乏结构化的测试、部署和反馈闭环
- ✅ **本框架让你和 AI Agent 按照专业的 10 阶段 21 步研发流程协作**，确保每一步都有输入、有产出、有校验

## 🔄 核心流程

框架覆盖 10 个阶段、21 个步骤，从初步想法到部署上线及迭代复盘：

```
想法 → 需求 → 校验 → 技术设计 → 任务拆解 → 编码执行 → 测试验收 → 部署上线 → 迭代复盘
```

| 步骤 | 角色 | 产出物 |
|------|------|--------|
| 1 | 👔 老板 | 初步想法 |
| 2 | 🔍 产品分析师 | 完整想法（草稿）|
| 3 | 👔 + 🔍 协作 | 完整想法（定稿）|
| 4 | 📋 需求工程师 | 产品需求文档 PRD（草稿）|
| 5 | 👔 + 📋 协作 | PRD（定稿）|
| 6 | 🛡️ 质量审核员 + 👔 | PRD 一致性校验记录 + 决策 |
| 7 | 🏗️🖥️⚙️🎨 全架构师 + UI | 技术初步共识 |
| 8 | 四角色并行 | 整体架构 / 前端方案 / 后端方案 / UI 设计 |
| 9 | 🛡️ 质量审核员 | 设计耦合校验报告 |
| 9b | 👔 + 全员 | 全员诊断会议（耦合校验未通过时触发）|
| 10 | 👔 老板 | 最终审批 |
| 11 | 🏗️🖥️⚙️🎨 各角色并行 | 任务卡片（拆解为可执行单元）|
| 12 | 👔 + 全架构师 | 任务交叉评审 |
| — | 各技术角色 | 编码执行（按任务看板并行）|
| 13 | 🧪 测试工程师 | 测试用例（与编码并行编写）|
| 14 | 🧪 测试工程师 | 分模块测试 + 联调测试 + PRD 需求回溯 |
| 15 | 🧪 测试工程师 | 测试报告 |
| 16 | 👔 老板 | 验收审批 |
| 16b | 全员 | 验收诊断会议（累计不通过超 10 次时触发）|
| 17 | 🚀 运维经理 | 部署需求清单 + 交付物清单 |
| 18 | 👔 老板 | 完成采购并交付 |
| 19 | 🚀 运维经理 | 验收交付物并执行部署 |
| 20 | 🚀 + 🔍 | 收集线上数据与用户反馈 |
| 21 | 👔 老板 + 全员 | 全员复盘会议 → 开启新迭代 |

> 📄 完整流程图和步骤详解请查看 [`00-流程与规范/研发流程总览.md`](00-流程与规范/研发流程总览.md)

## 👥 Agent 角色

| 角色 | 类型 | 职责 | 参与步骤 |
|------|------|------|----------|
| 👔 老板 | 🧑 人类 | 提出想法、决策审批、验收、采购交付、主持复盘 | 1,3,5,6,9b,10,12,16,16b,18,21 |
| 🔍 产品分析师 | 🤖 Agent | 扩写想法、提出澄清问题、收集用户反馈 | 2,3,16b,20,21 |
| 📋 需求工程师 | 🤖 Agent | 将想法转化为结构化 PRD | 4,5,21 |
| 🛡️ 质量审核员 | 🤖 Agent | 文档一致性校验、设计耦合校验 | 6,9,21 |
| 🏗️ 技术架构师 | 🤖 Agent | 系统架构设计、技术选型、任务拆解、编码执行 | 7,8a,9b,11a,12,编码,16b,21 |
| 🖥️ 前端架构师 | 🤖 Agent | 前端架构、页面路由、状态管理、编码执行 | 7,8b,9b,11b,12,编码,16b,21 |
| ⚙️ 后端架构师 | 🤖 Agent | API 设计、数据模型、服务架构、编码执行 | 7,8c,9b,11c,12,编码,16b,21 |
| 🎨 UI/UX 设计师 | 🤖 Agent | 设计系统、线框图、交互原型、设计交付 | 7,8d,9b,11d,12,编码,16b,21 |
| 🧪 测试工程师 | 🤖 Agent | 测试用例、执行测试、缺陷跟踪、出具报告 | 13,14,15,16,16b,21 |
| 🚀 运维经理 | 🤖 Agent | 评估部署需求、验收交付物、执行部署、收集工程数据 | 17,19,20,21 |

## 📁 目录结构

```
项目根目录/
├── 00-流程与规范/           ← 流程定义、Agent 角色说明、版本管理规范
├── 01-初步想法/             ← 老板的初步想法（模板 + 示例）
├── 02-完整想法/             ← 产品分析师扩写的完整想法（模板 + 示例）
├── 03-产品需求文档/         ← 需求工程师输出的 PRD（模板 + 示例）
├── 04-校验记录/             ← 质量审核员的校验结果（模板 + 示例）
├── 05-技术与设计方案/       ← 技术与设计方案
│   ├── 技术初步共识/        ← 步骤7 Kickoff 产出
│   ├── 整体架构/            ← 技术架构师输出（模板 + 示例）
│   ├── 前端方案/            ← 前端架构师输出（模板 + 示例）
│   ├── 后端方案/            ← 后端架构师输出（模板 + 示例），含 API 文档
│   └── UI设计/              ← UI/UX 设计师输出（模板）
├── 06-全局任务管理/         ← 全局任务看板与任务卡片
├── 07-测试验收/             ← 测试工程师：测试用例、缺陷报告、测试报告、验收报告
├── 08-部署上线/             ← 运维经理：部署需求清单、部署验收报告
├── 09-迭代复盘/             ← 版本复盘报告
└── 归档/                    ← 历史版本归档
```

**每个目录下都有：**
- **`_模板-xxx.md`**：空白模板，创建新文档时复制使用
- **`示例-xxx.md`**：基于"智能待办应用"的完整示例

## 🚀 快速开始

### 1. 克隆本仓库

```bash
git clone https://github.com/Challiwei/common-project-development-framework.git
```

### 2. 用 Obsidian 打开

将克隆的目录作为 Obsidian Vault 打开，即可看到完整的文档结构和内部链接。

### 3. 开始你的项目

1. 阅读 [`00-流程与规范/研发流程总览.md`](00-流程与规范/研发流程总览.md) 了解完整流程
2. 复制 `01-初步想法/_模板-初步想法.md`，写下你的产品想法
3. 按 21 步流程依次与 AI Agent 协作，完成从想法到部署上线的全过程

## 💡 使用场景

- **个人独立开发者**：用 AI 帮你做产品分析、技术架构、测试和部署
- **小团队**：建立统一的协作流程和文档规范
- **学习参考**：了解从想法到上线的完整研发生命周期
- **Obsidian 用户**：一套开箱即用的项目管理模板

## 📋 示例内容

项目中包含了一个完整的 **「智能待办应用」** 示例，覆盖了从初步想法到 API 文档的流程步骤，方便你理解每个环节的产出物应该长什么样。

## 🤝 贡献

欢迎提出 Issue 和 Pull Request！常见的贡献方向：

- 优化现有模板内容
- 改进流程规范
- 提供其他语言的翻译
- 分享你使用本框架的经验

## 📄 开源协议

本项目采用 [MIT License](LICENSE) 开源。

## 📝 更新日志

### v4.0 - 2026-04-29

**新增阶段与步骤**

1. **编码执行阶段** — 各技术角色按全局任务看板在独立对话中执行编码开发
2. **测试验收阶段（步骤 13–16b）** — 测试工程师编写测试用例（与编码并行）、执行分模块测试和联调测试并逐项回溯 PRD、出具测试报告、协助老板验收
3. **部署上线阶段（步骤 17–19）** — 运维经理评估基础设施需求、老板完成采购交付、运维经理验收并执行部署
4. **迭代复盘阶段（步骤 20–21）** — 收集线上数据与用户反馈、全员复盘会议、输出行动项开启新迭代

**新增 Agent 角色**

- 🧪 **测试工程师**：测试用例编写、分模块/联调测试、PRD 需求回溯、缺陷跟踪、测试报告
- 🚀 **运维经理**：部署需求评估、交付物验收、部署执行、线上工程数据收集

**新增模板**

- `07-测试验收/`：测试用例、缺陷报告、测试报告、验收报告模板
- `08-部署上线/`：部署需求清单、部署验收报告模板
- `09-迭代复盘/`：版本复盘报告模板

**其他变更**

- 全局任务看板新增跨界协同任务区域
- 所有已有角色新增编码执行、测试验收、迭代复盘参与步骤
- 新增 `项目记录.md` 用于项目进度追踪

---

### v3.0 - 2026-04-27

**新增内容**

1. **设计耦合校验（步骤 9）** — 质量审核员验证四份设计文档之间的一致性及对 PRD 的覆盖度
2. **全员诊断会议（步骤 9b）** — 耦合校验不通过时触发，根据根因决定修正范围
3. **老板最终审批（步骤 10）** — 从集体评审中拆分为客观校验 + 主观审批
4. **任务拆解（步骤 11、12）** — 各角色并行拆解任务卡片（65% 容量规则）+ 交叉评审

---

### v2.0 - 2026-04-24

**新增内容**

1. **UI/UX 设计师角色** — 设计规范与交互原型模板
2. **技术初步共识环节（步骤 7）** — 并行工作前的边界与约束对齐
3. **全局任务管理机制** — 任务卡片模板、全局任务看板、65% 上下文容量规则
4. **CLAUDE.md** — 为 Claude Code 提供项目指引

**结构调整**

- 目录重命名：`05-技术架构/` → `05-技术与设计方案/`
- 流程优化：原步骤 7-10 调整为步骤 7-9
