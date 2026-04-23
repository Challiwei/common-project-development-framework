---
项目名称: 智能待办应用
版本: v1
创建时间: 2026-04-20
创建者: ⚙️ 后端架构师
基于文档:
  - PRD: "[[03-产品需求文档/示例-智能待办应用-PRD]]"
  - 后端技术方案: "[[05-技术架构/后端方案/示例-智能待办应用-后端技术方案]]"
状态: 定稿
---

# API 文档：智能待办应用（SmartTodo）

## 文档信息

| 项目 | 内容 |
|------|------|
| Base URL | `https://api.smarttodo.app/v1` |
| 认证方式 | Bearer Token (JWT) |
| 数据格式 | JSON |
| 字符编码 | UTF-8 |

---

## API 列表总览

| 模块 | 方法 | 路径 | 说明 | 对应PRD |
|------|------|------|------|---------|
| 认证 | POST | /auth/register | 用户注册 | 基础能力 |
| 认证 | POST | /auth/login | 用户登录 | 基础能力 |
| 认证 | POST | /auth/refresh | 刷新 Token | 基础能力 |
| 任务 | POST | /tasks | 创建任务（自然语言） | FR-001 |
| 任务 | GET | /tasks | 获取任务列表 | FR-002 |
| 任务 | GET | /tasks/today | 获取今日推荐 | FR-003 |
| 任务 | GET | /tasks/:id | 获取任务详情 | 基础能力 |
| 任务 | PUT | /tasks/:id | 更新任务 | 基础能力 |
| 任务 | DELETE | /tasks/:id | 删除任务 | 基础能力 |
| 任务 | PUT | /tasks/:id/priority | 手动覆盖优先级 | FR-002 |
| 用户 | GET | /users/me | 获取当前用户信息 | 基础能力 |
| 用户 | PUT | /users/me/preferences | 更新用户偏好 | 基础能力 |

---

## API 详细定义

### 模块一：认证

#### `POST /auth/register`

**说明**：新用户注册

**请求参数**：

| 参数 | 类型 | 是否必须 | 说明 |
|------|------|----------|------|
| email | string | 是 | 邮箱地址 |
| password | string | 是 | 密码（6-32位） |
| name | string | 是 | 用户昵称 |

**请求示例**：
```json
{
  "email": "boss@example.com",
  "password": "secure123",
  "name": "老板"
}
```

**成功响应**（201）：
```json
{
  "code": "SUCCESS",
  "data": {
    "user": {
      "id": "uuid-xxx",
      "email": "boss@example.com",
      "name": "老板"
    },
    "accessToken": "eyJhbG...",
    "refreshToken": "eyJhbG..."
  }
}
```

**错误响应**：

| 错误码 | 说明 |
|--------|------|
| AUTH_003 | 邮箱已注册 |

---

#### `POST /auth/login`

**说明**：用户登录

**请求参数**：

| 参数 | 类型 | 是否必须 | 说明 |
|------|------|----------|------|
| email | string | 是 | 邮箱地址 |
| password | string | 是 | 密码 |

**成功响应**（200）：
```json
{
  "code": "SUCCESS",
  "data": {
    "user": { "id": "uuid-xxx", "email": "boss@example.com", "name": "老板" },
    "accessToken": "eyJhbG...",
    "refreshToken": "eyJhbG..."
  }
}
```

---

### 模块二：任务

#### `POST /tasks`

**说明**：通过自然语言创建任务，AI 自动解析内容和截止日期

**请求参数**：

| 参数 | 类型 | 是否必须 | 说明 |
|------|------|----------|------|
| input | string | 是 | 自然语言输入（如"下周五之前跟供应商确认报价"） |

**请求示例**：
```json
{
  "input": "下周五之前跟供应商确认报价"
}
```

**成功响应**（201）：
```json
{
  "code": "SUCCESS",
  "data": {
    "task": {
      "id": "uuid-task-001",
      "title": "跟供应商确认报价",
      "description": null,
      "dueDate": "2026-04-25T23:59:59Z",
      "priority": "HIGH",
      "status": "TODO",
      "isAiPriority": true
    },
    "aiParsing": {
      "parsedTitle": "跟供应商确认报价",
      "parsedDueDate": "2026-04-25",
      "confidence": 0.95
    }
  }
}
```

**错误响应**：

| 错误码 | 说明 |
|--------|------|
| AI_002 | 无法解析输入内容 |
| AI_001 | AI 服务暂不可用（降级：创建无AI标签的任务） |

---

#### `GET /tasks/today`

**说明**：获取 AI 推荐的今日任务清单（3-7个）

**成功响应**（200）：
```json
{
  "code": "SUCCESS",
  "data": {
    "tasks": [
      {
        "id": "uuid-task-001",
        "title": "跟供应商确认报价",
        "dueDate": "2026-04-25T23:59:59Z",
        "priority": "HIGH",
        "aiReason": "截止日期临近（还剩5天），且涉及外部合作方"
      },
      {
        "id": "uuid-task-002",
        "title": "审核产品设计稿",
        "dueDate": "2026-04-22T23:59:59Z",
        "priority": "HIGH",
        "aiReason": "截止日期为明天，阻塞开发流程"
      }
    ],
    "generatedAt": "2026-04-20T08:00:00Z"
  }
}
```

---

#### `GET /tasks`

**说明**：获取任务列表，支持筛选和分页

**查询参数**：

| 参数 | 类型 | 是否必须 | 说明 |
|------|------|----------|------|
| status | string | 否 | 筛选状态：TODO, IN_PROGRESS, DONE |
| priority | string | 否 | 筛选优先级：HIGH, MEDIUM, LOW |
| sort | string | 否 | 排序：due_date, priority, created_at（默认 priority） |
| page | int | 否 | 页码（默认1） |
| page_size | int | 否 | 每页数量（默认20） |

**成功响应**（200）：
```json
{
  "code": "SUCCESS",
  "data": {
    "items": [
      {
        "id": "uuid-task-001",
        "title": "跟供应商确认报价",
        "dueDate": "2026-04-25T23:59:59Z",
        "priority": "HIGH",
        "status": "TODO",
        "isAiPriority": true,
        "createdAt": "2026-04-20T01:30:00Z"
      }
    ],
    "total": 42,
    "page": 1,
    "pageSize": 20
  }
}
```

---

#### `PUT /tasks/:id/priority`

**说明**：手动覆盖 AI 设置的优先级（AI 会学习此反馈）

**请求参数**：

| 参数 | 类型 | 是否必须 | 说明 |
|------|------|----------|------|
| priority | string | 是 | HIGH / MEDIUM / LOW |

**成功响应**（200）：
```json
{
  "code": "SUCCESS",
  "data": {
    "task": {
      "id": "uuid-task-001",
      "priority": "MEDIUM",
      "isAiPriority": false
    }
  },
  "message": "优先级已更新，AI 将学习您的偏好"
}
```

---

> [!note] 下一步
> ✅ API 文档已完成。需在步骤10中与 **👔 老板** 和其他架构师一起评审。
