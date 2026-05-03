# MiMo-Project-Guardian: Autonomous Architecture Evolution Agent

## 🚀 项目简介
本项目是专为大规模工程设计的智能化治理工具，底层深度集成 **Xiaomi MiMo-V2.5-Pro** 模型。它利用 MiMo 的 1M+ 超长上下文能力，实现对整个代码库的深度理解、架构风险识别及自动化单元测试重构。

## 核心特性
- **Global Context Mapping**: 自动扫描整个 Source 目录，通过 MiMo-Pro 构建全局依赖图谱（Dependency Graph）。
- **Multi-Agent Orchestration**: 
  - **Planner Agent**: 负责复杂任务拆解，利用 MiMo 的逻辑能力制定演进路线。
  - **Executor Agent**: 基于 Tool-Calling 模式，自动修改代码并修复潜在 Bug。
  - **Audit Agent**: 对重构后的代码进行静态合规性与安全性审查。
- **High-Token Consumption Workflow**: 针对 100k-500k 行代码的项目，单次扫描涉及数千万级别的 Token 处理，充分发挥 MiMo-Pro 的长文本优势。

## 🛠 技术栈
- **Model**: MiMo-V2.5-Pro (Primary)
- **Framework**: LangGraph / PydanticAI
- **Integrations**: Cursor, Aider, Git

## 📈 为什么我们需要 Max 计划？
由于本项目涉及对大规模遗留系统（Legacy Systems）的“全量预读”与“反复回归验证”，单个任务链的上下文注入量常态化维持在 500k 以上。为了完成对多个开源库的适配，我们急需 Max 档位（16 亿 Credits）的算力支持以覆盖全量测试。
