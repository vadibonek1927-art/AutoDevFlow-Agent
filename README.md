# AutoDevFlow-Agent
Multi-Agent Workflow System for Autonomous Software Engineering. Provides automated GitHub Issue analysis, task planning, code generation, testing, PR review, and CI retry loops.
# AutoDevFlow-Agent

Multi-Agent Workflow System for Autonomous Software Engineering.  
AutoDevFlow-Agent 是一个多 Agent 协作的自动化研发平台，用于自动完成 GitHub Issue 分析、任务拆解、代码生成、自动测试、PR 修复与代码 Review。

---

## Features

- Multi-Agent Orchestration
- Autonomous Coding Workflow
- GitHub Issue → PR Automation
- DAG-based Workflow Routing
- CI Retry & Auto Fix
- Long Context Memory
- Token Usage Analytics
- GitHub Actions Integration
- Workflow Runtime Engine

---

## Core Agents

- **Planner Agent**：需求分析与任务拆解  
- **Router Agent**：DAG 工作流调度与上下文分发  
- **Coder Agent**：代码生成与重构  
- **Test Agent**：自动执行单元测试与错误分析  
- **Reviewer Agent**：自动进行代码规范检查与 PR Review  
- **Fix Agent**：在 CI 失败后自动修复并重试 Workflow  

---

## Workflow
GitHub Issue
↓
Planner Agent
↓
Router Agent
↓
Coder Agent
↓
Test Agent
↓
Reviewer Agent
↓
Fix Agent
↓
Pull Request

---

## Example Terminal Logs

> 以下为伪终端日志示例，用于展示 Agent 流程执行情况
[Planner Agent] Analyzing GitHub Issue...
[Planner Agent] Generating execution plan...
[Router Agent] Dispatching workflow DAG...
[Coder Agent] Generating code patch...
[Test Agent] Running unit tests...
[Test Agent] Detected CI failure...
[Fix Agent] Applying retry patch...
[Reviewer Agent] Running code review...
[Reviewer Agent] Review completed successfully.
[Workflow Runtime] Creating Pull Request...
[Token Analytics] Total Tokens Used: 582,193

---

## Architecture & Workflow Diagram

- `architecture.png`：系统架构图示意  
- `workflow.png`：多 Agent Workflow DAG 图  

(可以使用 draw.io / Figma 绘制并上传到仓库)

---

## Token Usage Example
Daily Token Usage
5,231,991

说明：复杂任务场景下，单次完整 Workflow Token 消耗约 30万~80万 Tokens，长链路代码修复场景中消耗更高。

---

## References & Base Projects

项目参考并工程化整合了多个开源 Agent Workflow 项目的设计思想，包括：

- [Optio](https://github.com/jonwiggins/optio)  
- [Agent Orchestrator](https://github.com/ComposioHQ/agent-orchestrator)  
- [Claworc](https://github.com/gluk-w/claworc)  

---

## Tech Stack

- Python  
- FastAPI  
- LangGraph  
- Celery  
- Redis  
- PostgreSQL  
- Docker  
- GitHub Actions  
- OpenAI API  

---

## Notes
