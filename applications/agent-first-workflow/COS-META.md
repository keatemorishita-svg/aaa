# COS-META

## Identity
- **Name**: Agent-First 开发工作流
- **Author**: AAA 社区
- **Version**: 1.0
- **Date**: 2026-06

## Architecture Mapping

- [ ] Cognition Layer
- [ ] Protocol Layer
- [x] Execution Layer — 定义了"怎么做事"的完整流程
- [x] Evolution Layer — 工作流本身在持续精炼（CLAUDE.md 迭代、模型切换）

## Primitive Check

- **Access** — 提供了一个可复制的工作流模板，降低了 AI-native 开发的进入门槛
- **Mutation** — 工具组合、模型选择、CLAUDE.md 模板全部可替换
- **Recursion** — 工作流的改进（如新的 prompt 模式、新的审核方法）可以回流到模板中

## Dependencies
- **Requires**: VS Code + Claude Code（或其他 Agent 工具）
- **Extends**: AAA Execution Layer 的"行动基础设施"概念
- **Conflicts**: 与传统"手写代码为主"的开发教学有张力——本工作流假设 AI 承担实现工作

## Fork Instructions
- **Best fork point**: 工具组合（换成你的编辑器/Agent/API）
- **What to keep**: Agent-first 的核心逻辑（AI 写，人审）
- **What to change**: 模型选择、CLAUDE.md 模板内容、审核流程细节
