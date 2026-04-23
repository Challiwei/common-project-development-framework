# 更新日志 | Update Log

## v2.0 - 2024-04-24

### 新增内容 | New Features

1. **新增 UI/UX 设计师角色** | Added UI/UX Designer Role
   - 新增 `05-技术与设计方案/UI设计/` 目录
   - 包含 UI 设计规范模板和交互原型模板
   - Added `05-技术与设计方案/UI设计/` directory
   - Includes UI design specification and interaction prototype templates

2. **新增技术初步共识环节** | Added Technical Kickoff Meeting
   - 新增 `05-技术与设计方案/技术初步共识/` 目录
   - 步骤 7：所有技术角色在并行工作前先进行边界和约束的对齐
   - Added `05-技术与设计方案/技术初步共识/` directory
   - Step 7: All technical roles align on boundaries and constraints before parallel work

3. **新增全局任务管理机制** | Added Global Task Management
   - 新增 `06-全局任务管理/` 目录
   - 包含任务卡片模板和全局任务看板
   - 引入 65% 上下文容量规则，防止大模型记忆丢失
   - Added `06-全局任务管理/` directory
   - Includes task card template and global task board
   - Introduced 65% context capacity rule to prevent LLM memory loss

4. **新增 CLAUDE.md** | Added CLAUDE.md
   - 为 Claude Code 提供项目指引文档
   - Provides project guidance for Claude Code

### 结构调整 | Structure Changes

1. **目录重命名** | Directory Renamed
   - `05-技术架构/` → `05-技术与设计方案/`
   - 更准确地反映该阶段包含技术和设计两个维度
   - Better reflects that this phase includes both technical and design dimensions

2. **流程优化** | Workflow Optimization
   - 原步骤 7-10 调整为步骤 7-9
   - 步骤 7：技术初步共识会议（新增）
   - 步骤 8：四个角色并行工作（8a/8b/8c/8d）
   - 步骤 9：集体评审
   - Original steps 7-10 adjusted to steps 7-9
   - Step 7: Technical kickoff meeting (new)
   - Step 8: Four roles work in parallel (8a/8b/8c/8d)
   - Step 9: Collective review

### 文档更新 | Documentation Updates

1. 更新 `00-流程与规范/研发流程总览.md`
   - 新增全局任务管理机制说明
   - 更新流程图为泳道式布局
   - Updated with global task management mechanism
   - Updated flowchart to swimlane layout

2. 更新 `00-流程与规范/Agent角色说明.md`
   - 新增 UI/UX 设计师角色说明
   - 新增通用工作准则章节
   - Added UI/UX Designer role description
   - Added general work guidelines section

3. 更新 README.md
   - 新增中英双语支持
   - 更新目录结构说明
   - Added bilingual (Chinese/English) support
   - Updated directory structure description

---

# 它当前什么状态 | Current Status

当前版本，它还没达到可用状态，未来会继续完成这个项目。
随着自用版本的完善，当前这个项目也会同步完善。

The current version is not yet production-ready. This project will continue to evolve.
As the private version improves, this public version will be updated accordingly.

---

# 🚀 软件产品研发流程框架 | Software Product Development Framework

> **一套结构化的 Boss × AI Agent 协作研发框架，覆盖从「灵感」到「技术方案」的完整流程。**
>
> **A structured Boss × AI Agent collaboration framework covering the complete process from "idea" to "technical design".**

---

## 📖 这是什么？ | What is this?

这是一个**基于文档**的软件产品研发流程框架，定义了从产品想法到技术设计的完整协作流程。

在这个框架中：
- 🧑 **老板（Boss）** 是唯一的人类角色，负责提出想法、做出决策、审批产出物
- 🤖 **AI Agent** 扮演产品分析师、需求工程师、质量审核员、技术架构师等专业角色

框架提供了完整的 **流程定义 + 文档模板 + 示例内容**，开箱即用。

---

This is a **document-based** software product development framework that defines a complete collaboration process from product idea to technical design.

In this framework:
- 🧑 **Boss** is the only human role, responsible for proposing ideas, making decisions, and approving deliverables
- 🤖 **AI Agents** play professional roles such as Product Analyst, Requirements Engineer, Quality Reviewer, Technical Architect, etc.

The framework provides complete **process definitions + document templates + example content**, ready to use out of the box.

---

## 🎯 解决什么问题？ | What problems does it solve?

- ❌ 个人项目想法多，但缺乏系统性梳理流程
- ❌ 直接让 AI 写代码，跳过了需求分析和架构设计
- ❌ AI 产出的文档缺乏结构，质量不稳定
- ✅ **本框架让你和 AI Agent 按照专业研发流程协作**，确保每一步都有输入、有产出、有校验

---

- ❌ Many personal project ideas but lack systematic organization process
- ❌ Directly asking AI to write code, skipping requirements analysis and architecture design
- ❌ AI-generated documents lack structure and have unstable quality
- ✅ **This framework enables you to collaborate with AI Agents following professional development processes**, ensuring each step has input, output, and validation

---

## 🔄 核心流程 | Core Workflow

```
阶段一：想法孵化 → 阶段二：想法对齐 → 阶段三：需求产出 → 阶段四：一致性校验 → 阶段五：技术与设计
Stage 1: Idea Incubation → Stage 2: Idea Alignment → Stage 3: Requirements → Stage 4: Consistency Check → Stage 5: Technical & Design
```

| 步骤 Step | 角色 Role | 产出物 Deliverable |
|------|------|--------|
| 1 | 👔 老板 Boss | 初步想法 Initial Idea |
| 2 | 🔍 产品分析师 Product Analyst | 完整想法（草稿）Complete Idea (Draft) |
| 3 | 👔 + 🔍 协作 Collaboration | 完整想法（定稿）Complete Idea (Final) |
| 4 | 📋 需求工程师 Requirements Engineer | 产品需求文档 PRD（草稿）PRD (Draft) |
| 5 | 👔 + 📋 协作 Collaboration | PRD（定稿）PRD (Final) |
| 6 | 🛡️ 质量审核员 + 👔 Quality Reviewer + Boss | 校验记录 + 决策 Validation Record + Decision |
| 7 | 🏗️🖥️⚙️🎨 全架构师 + UI All Architects + UI | 技术初步共识 Technical Kickoff Consensus |
| 8a | 🏗️ 技术架构师 Technical Architect | 整体技术架构 Overall Architecture |
| 8b | 🖥️ 前端架构师 Frontend Architect | 前端技术方案 Frontend Solution |
| 8c | ⚙️ 后端架构师 Backend Architect | 后端方案 + API Backend Solution + API |
| 8d | 🎨 UI/UX 设计师 UI/UX Designer | 设计规范 + 原型 Design Specs + Prototype |
| 9 | 👔 + 架构师们 Boss + Architects | 技术方案评审 Technical Review |

> 📄 完整流程图和步骤详解请查看 [`00-流程与规范/研发流程总览.md`](00-流程与规范/研发流程总览.md)
>
> 📄 For complete flowchart and step details, see [`00-流程与规范/研发流程总览.md`](00-流程与规范/研发流程总览.md)

---

## 📁 目录结构 | Directory Structure

```
项目根目录/ Project Root/
├── 00-流程与规范/           ← 流程定义、Agent 角色说明、版本管理规范
│                              Process definitions, Agent roles, version management
├── 01-初步想法/             ← 老板的初步想法（模板 + 示例）
│                              Boss's initial idea (template + example)
├── 02-完整想法/             ← 产品分析师扩写的完整想法（模板 + 示例）
│                              Product Analyst's complete idea (template + example)
├── 03-产品需求文档/         ← 需求工程师输出的 PRD（模板 + 示例）
│                              Requirements Engineer's PRD (template + example)
├── 04-校验记录/             ← 质量审核员的校验结果（模板 + 示例）
│                              Quality Reviewer's validation (template + example)
├── 05-技术与设计方案/       ← 技术与设计方案
│   │                          Technical & Design Solutions
│   ├── 技术初步共识/        ← 步骤7 Kickoff 产出 (Step 7 Kickoff output)
│   ├── 整体架构/            ← 技术架构师输出（模板 + 示例）
│   │                          Technical Architect output (template + example)
│   ├── 前端方案/            ← 前端架构师输出（模板 + 示例）
│   │                          Frontend Architect output (template + example)
│   ├── 后端方案/            ← 后端架构师输出（模板 + 示例），含 API 文档
│   │                          Backend Architect output (template + example), with API docs
│   └── UI设计/              ← UI/UX 设计师输出（模板）
│                              UI/UX Designer output (template)
├── 06-全局任务管理/         ← 全局任务看板与任务卡片
│                              Global task board and task cards
└── 归档/                    ← 历史版本归档
    Archive/                   Historical version archive
```

每个目录下都有：
- **`_模板-xxx.md`**：空白模板，创建新文档时复制使用
- **`示例-xxx.md`**：基于"智能待办应用"的完整示例

Each directory contains:
- **`_模板-xxx.md`**: Blank templates for creating new documents
- **`示例-xxx.md`**: Complete examples based on "Smart Todo App"

---

## 🚀 快速开始 | Quick Start

### 1. 克隆本仓库 | Clone the Repository

```bash
git clone https://github.com/Challiwei/common-project-development-framework.git
```

### 2. 用 Obsidian 打开 | Open with Obsidian

将克隆的目录作为 Obsidian Vault 打开，即可看到完整的文档结构和内部链接。

Open the cloned directory as an Obsidian Vault to see the complete document structure and internal links.

### 3. 开始你的项目 | Start Your Project

1. 阅读 [`00-流程与规范/研发流程总览.md`](00-流程与规范/研发流程总览.md) 了解完整流程
   Read [`00-流程与规范/研发流程总览.md`](00-流程与规范/研发流程总览.md) to understand the complete process

2. 复制 `01-初步想法/_模板-初步想法.md`，写下你的产品想法
   Copy `01-初步想法/_模板-初步想法.md` and write down your product idea

3. 按流程步骤依次与 AI Agent 协作，完成从想法到技术方案的全过程
   Follow the process steps to collaborate with AI Agents, completing the journey from idea to technical solution

---

## 💡 使用场景 | Use Cases

- **个人独立开发者** | Individual Developers：用 AI 帮你做产品分析和技术架构 | Use AI to help with product analysis and technical architecture
- **小团队** | Small Teams：建立统一的协作流程和文档规范 | Establish unified collaboration processes and documentation standards
- **学习参考** | Learning Reference：了解从想法到技术方案的完整研发流程 | Understand the complete development process from idea to technical solution
- **Obsidian 用户** | Obsidian Users：一套开箱即用的项目管理模板 | A ready-to-use project management template

---

## 📋 示例内容 | Example Content

项目中包含了一个完整的 **「智能待办应用」** 示例，覆盖了从初步想法到 API 文档的全部流程步骤，方便你理解每个环节的产出物应该长什么样。

The project includes a complete **"Smart Todo App"** example, covering all process steps from initial idea to API documentation, helping you understand what each deliverable should look like.

---

## 🤝 贡献 | Contributing

欢迎提出 Issue 和 Pull Request！常见的贡献方向：

Welcome to submit Issues and Pull Requests! Common contribution directions:

- 补充新的流程阶段（如测试、部署）| Add new process stages (e.g., testing, deployment)
- 优化现有模板内容 | Optimize existing template content
- 改进流程规范 | Improve process specifications
- 提供其他语言的翻译 | Provide translations in other languages

---

## 📄 License

本项目采用 [MIT License](LICENSE) 开源。

This project is open-sourced under the [MIT License](LICENSE).
