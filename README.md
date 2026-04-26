# 🚀 软件产品研发流程框架

[English](#-software-product-development-framework) | [中文](#-软件产品研发流程框架)

---

> **一套结构化的 Boss × AI Agent 协作研发框架，覆盖从「灵感」到「技术方案」的完整流程。**

## 📖 这是什么？

这是一个**基于文档**的软件产品研发流程框架，定义了从产品想法到技术设计的完整协作流程。

在这个框架中：
- 🧑 **老板（Boss）** 是唯一的人类角色，负责提出想法、做出决策、审批产出物
- 🤖 **AI Agent** 扮演产品分析师、需求工程师、质量审核员、技术架构师等专业角色

框架提供了完整的 **流程定义 + 文档模板 + 示例内容**，开箱即用。

## 🎯 解决什么问题？

- ❌ 个人项目想法多，但缺乏系统性梳理流程
- ❌ 直接让 AI 写代码，跳过了需求分析和架构设计
- ❌ AI 产出的文档缺乏结构，质量不稳定
- ✅ **本框架让你和 AI Agent 按照专业研发流程协作**，确保每一步都有输入、有产出、有校验

## 🔄 核心流程

```
阶段一：想法孵化 → 阶段二：想法对齐 → 阶段三：需求产出 → 阶段四：一致性校验 → 阶段五：技术与设计 → 阶段六：任务拆解
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
| 8a | 🏗️ 技术架构师 | 整体技术架构 |
| 8b | 🖥️ 前端架构师 | 前端技术方案 |
| 8c | ⚙️ 后端架构师 | 后端方案 + API |
| 8d | 🎨 UI/UX 设计师 | 设计规范 + 原型 |
| 9 | 🛡️ 质量审核员 | 设计耦合校验报告 |
| 9b | 👔 + 全架构师 | 全员诊断会议（耦合校验未通过时触发）|
| 10 | 👔 老板 | 最终审批 |
| 11 | 🏗️🖥️⚙️🎨 各角色并行 | 任务卡片（拆解为可执行单元）|
| 12 | 👔 + 全架构师 | 任务交叉评审 |

> 📄 完整流程图和步骤详解请查看 [`00-流程与规范/研发流程总览.md`](00-流程与规范/研发流程总览.md)

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
3. 按流程步骤依次与 AI Agent 协作，完成从想法到技术方案的全过程

## 💡 使用场景

- **个人独立开发者**：用 AI 帮你做产品分析和技术架构
- **小团队**：建立统一的协作流程和文档规范
- **学习参考**：了解从想法到技术方案的完整研发流程
- **Obsidian 用户**：一套开箱即用的项目管理模板

## 📋 示例内容

项目中包含了一个完整的 **「智能待办应用」** 示例，覆盖了从初步想法到 API 文档的全部流程步骤，方便你理解每个环节的产出物应该长什么样。

## 🤝 贡献

欢迎提出 Issue 和 Pull Request！常见的贡献方向：

- 补充新的流程阶段（如测试、部署）
- 优化现有模板内容
- 改进流程规范
- 提供其他语言的翻译

## 📄 开源协议

本项目采用 [MIT License](LICENSE) 开源。

## 📝 更新日志

### v3.0 - 2026-04-27

**新增内容**

1. **新增设计耦合校验（步骤 9）**
   - 新增 `04-校验记录/_模板-设计耦合校验.md` 模板
   - 质量审核员在步骤 9 负责验证四份设计文档之间的一致性，以及对 PRD 的完整覆盖

2. **新增全员诊断会议（步骤 9b）**
   - 耦合校验不通过时触发，由全体角色定位问题根因
   - 按根因决定修正范围：问题在共识则全面重做，问题在某板块则仅修正该板块

3. **老板最终审批独立为步骤 10**
   - 原"集体评审"拆分为质量审核员主导的客观校验（步骤 9）+ 老板的主观审批（步骤 10）

4. **新增阶段六：任务拆解（步骤 11、12）**
   - 步骤 11：各角色并行将设计文档拆解为符合 65% 容量规则的独立任务卡片
   - 步骤 12：全员对任务卡片进行交叉评审，验证依赖关系的完整性

**文档更新**

- 更新 `00-流程与规范/研发流程总览.md`：新增步骤 9/9b/10/11/12 详解，更新流程图
- 更新 `00-流程与规范/Agent角色说明.md`：更新质量审核员和老板的参与步骤和职责
- 更新 `CLAUDE.md`：同步新的阶段划分和角色步骤
- 更新 `README.md`：同步核心流程表格

---

### v2.0 - 2024-04-24

**新增内容**

1. **新增 UI/UX 设计师角色**
   - 新增 `05-技术与设计方案/UI设计/` 目录
   - 包含 UI 设计规范模板和交互原型模板

2. **新增技术初步共识环节**
   - 新增 `05-技术与设计方案/技术初步共识/` 目录
   - 步骤 7：所有技术角色在并行工作前先进行边界和约束的对齐

3. **新增全局任务管理机制**
   - 新增 `06-全局任务管理/` 目录
   - 包含任务卡片模板和全局任务看板
   - 引入 65% 上下文容量规则，防止大模型记忆丢失

4. **新增 CLAUDE.md**
   - 为 Claude Code 提供项目指引文档

**结构调整**

1. **目录重命名**：`05-技术架构/` → `05-技术与设计方案/`
2. **流程优化**：原步骤 7-10 调整为步骤 7-9
   - 步骤 7：技术初步共识会议（新增）
   - 步骤 8：四个角色并行工作（8a/8b/8c/8d）
   - 步骤 9：集体评审

**文档更新**

1. 更新 `00-流程与规范/研发流程总览.md`
   - 新增全局任务管理机制说明
   - 更新流程图为泳道式布局

2. 更新 `00-流程与规范/Agent角色说明.md`
   - 新增 UI/UX 设计师角色说明
   - 新增通用工作准则章节

3. 更新 README.md
   - 新增中英双语支持
   - 更新目录结构说明

---

# 🚀 Software Product Development Framework

[中文](#-软件产品研发流程框架) | [English](#-software-product-development-framework)

---

> **A structured Boss × AI Agent collaboration framework covering the complete process from "idea" to "technical design".**

## 📖 What is this?

This is a **document-based** software product development framework that defines a complete collaboration process from product idea to technical design.

In this framework:
- 🧑 **Boss** is the only human role, responsible for proposing ideas, making decisions, and approving deliverables
- 🤖 **AI Agents** play professional roles such as Product Analyst, Requirements Engineer, Quality Reviewer, Technical Architect, etc.

The framework provides complete **process definitions + document templates + example content**, ready to use out of the box.

## 🎯 What problems does it solve?

- ❌ Many personal project ideas but lack systematic organization process
- ❌ Directly asking AI to write code, skipping requirements analysis and architecture design
- ❌ AI-generated documents lack structure and have unstable quality
- ✅ **This framework enables you to collaborate with AI Agents following professional development processes**, ensuring each step has input, output, and validation

## 🔄 Core Workflow

```
Stage 1: Idea Incubation → Stage 2: Idea Alignment → Stage 3: Requirements → Stage 4: Consistency Check → Stage 5: Technical & Design → Stage 6: Task Decomposition
```

| Step | Role | Deliverable |
|------|------|--------|
| 1 | 👔 Boss | Initial Idea |
| 2 | 🔍 Product Analyst | Complete Idea (Draft) |
| 3 | 👔 + 🔍 Collaboration | Complete Idea (Final) |
| 4 | 📋 Requirements Engineer | PRD (Draft) |
| 5 | 👔 + 📋 Collaboration | PRD (Final) |
| 6 | 🛡️ Quality Reviewer + 👔 | PRD Consistency Validation + Decision |
| 7 | 🏗️🖥️⚙️🎨 All Architects + UI | Technical Kickoff Consensus |
| 8a | 🏗️ Technical Architect | Overall Architecture |
| 8b | 🖥️ Frontend Architect | Frontend Solution |
| 8c | ⚙️ Backend Architect | Backend Solution + API |
| 8d | 🎨 UI/UX Designer | Design Specs + Prototype |
| 9 | 🛡️ Quality Reviewer | Design Coupling Validation Report |
| 9b | 👔 + All Architects | Diagnosis Meeting (triggered when step 9 fails) |
| 10 | 👔 Boss | Final Approval |
| 11 | 🏗️🖥️⚙️🎨 All roles in parallel | Task Cards (decomposed into executable units) |
| 12 | 👔 + All Architects | Task Cross-review |

> 📄 For complete flowchart and step details, see [`00-流程与规范/研发流程总览.md`](00-流程与规范/研发流程总览.md)

## 📁 Directory Structure

```
Project Root/
├── 00-流程与规范/           ← Process definitions, Agent roles, version management
├── 01-初步想法/             ← Boss's initial idea (template + example)
├── 02-完整想法/             ← Product Analyst's complete idea (template + example)
├── 03-产品需求文档/         ← Requirements Engineer's PRD (template + example)
├── 04-校验记录/             ← Quality Reviewer's validation (template + example)
├── 05-技术与设计方案/       ← Technical & Design Solutions
│   ├── 技术初步共识/        ← Step 7 Kickoff output
│   ├── 整体架构/            ← Technical Architect output (template + example)
│   ├── 前端方案/            ← Frontend Architect output (template + example)
│   ├── 后端方案/            ← Backend Architect output (template + example), with API docs
│   └── UI设计/              ← UI/UX Designer output (template)
├── 06-全局任务管理/         ← Global task board and task cards
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
3. Follow the process steps to collaborate with AI Agents, completing the journey from idea to technical solution

## 💡 Use Cases

- **Individual Developers**: Use AI to help with product analysis and technical architecture
- **Small Teams**: Establish unified collaboration processes and documentation standards
- **Learning Reference**: Understand the complete development process from idea to technical solution
- **Obsidian Users**: A ready-to-use project management template

## 📋 Example Content

The project includes a complete **"Smart Todo App"** example, covering all process steps from initial idea to API documentation, helping you understand what each deliverable should look like.

## 🤝 Contributing

Welcome to submit Issues and Pull Requests! Common contribution directions:

- Add new process stages (e.g., testing, deployment)
- Optimize existing template content
- Improve process specifications
- Provide translations in other languages

## 📄 License

This project is open-sourced under the [MIT License](LICENSE).

## 📝 Changelog

### v3.0 - 2026-04-27

**New Features**

1. **Added Design Coupling Validation (Step 9)**
   - Added `04-校验记录/_模板-设计耦合校验.md` template
   - Quality Reviewer validates consistency across four design documents and their coverage of PRD requirements

2. **Added All-hands Diagnosis Meeting (Step 9b)**
   - Triggered when coupling validation fails; all roles collaborate to identify root cause
   - Fix scope determined by root cause: full redesign if issue is in kickoff consensus, targeted fix if issue is in a specific document

3. **Boss Final Approval Separated as Step 10**
   - Previous "collective review" split into objective validation by Quality Reviewer (Step 9) + Boss's subjective approval (Step 10)

4. **Added Stage 6: Task Decomposition (Steps 11 & 12)**
   - Step 11: Each role independently decomposes design documents into task cards following the 65% context capacity rule
   - Step 12: All roles cross-review task cards to verify completeness of dependencies

**Documentation Updates**

- Updated `00-流程与规范/研发流程总览.md`: Added steps 9/9b/10/11/12, updated flowchart
- Updated `00-流程与规范/Agent角色说明.md`: Updated Quality Reviewer and Boss roles
- Updated `CLAUDE.md`: Synced new stage structure and role steps
- Updated `README.md`: Synced core workflow table

---

### v2.0 - 2024-04-24

**New Features**

1. **Added UI/UX Designer Role**
   - Added `05-技术与设计方案/UI设计/` directory
   - Includes UI design specification and interaction prototype templates

2. **Added Technical Kickoff Meeting**
   - Added `05-技术与设计方案/技术初步共识/` directory
   - Step 7: All technical roles align on boundaries and constraints before parallel work

3. **Added Global Task Management**
   - Added `06-全局任务管理/` directory
   - Includes task card template and global task board
   - Introduced 65% context capacity rule to prevent LLM memory loss

4. **Added CLAUDE.md**
   - Provides project guidance for Claude Code

**Structure Changes**

1. **Directory Renamed**: `05-技术架构/` → `05-技术与设计方案/`
2. **Workflow Optimization**: Original steps 7-10 adjusted to steps 7-9
   - Step 7: Technical kickoff meeting (new)
   - Step 8: Four roles work in parallel (8a/8b/8c/8d)
   - Step 9: Collective review

**Documentation Updates**

1. Updated `00-流程与规范/研发流程总览.md`
   - Added global task management mechanism
   - Updated flowchart to swimlane layout

2. Updated `00-流程与规范/Agent角色说明.md`
   - Added UI/UX Designer role description
   - Added general work guidelines section

3. Updated README.md
   - Added bilingual (Chinese/English) support
   - Updated directory structure description
