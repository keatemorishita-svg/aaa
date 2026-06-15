# Agent-First 开发工作流

> AI 写代码，人定方向、审核产出、持续精炼。

---

## 工具组合

- **编辑器**: VS Code
- **AI Agent**: Claude Code
- **API 后端**: DeepSeek API（通过 ANTHROPIC_BASE_URL 路由）
- **模型**: deepseek-v4-pro（主）、deepseek-v4-flash（轻量）

---

## 工作范式：Agent-first

不是"自己写代码 + AI 补全"，而是"与 AI 共同创造需求、定义目标、审核产出"。

| 传统范式 | Agent-first 范式 |
|---|---|
| 人写代码，AI 补全 | AI 写代码，人审核 |
| 人做实现，AI 做辅助 | AI 做实现，人做架构 |
| 速度 = 打字速度 | 速度 = 审核速度 |
| 工具价值 = 补全准确率 | 工具价值 = 意图理解深度 |

---

## 核心原则

1. **行内补全对 Agent-first 范式几乎没有价值** — Copilot Tab 补全解决的是"人写代码"的问题，不是"人审核 AI 代码"的问题
2. **模型灵活性 > 模型性能** — 能接入最新/最便宜的模型，比当前模型跑分高 5% 更重要
3. **CLAUDE.md 是核心资产** — 工具定义能力，CLAUDE.md 定义方向。好的 CLAUDE.md 能让 91 分的工具逼近 95 分
4. **成本是设计约束** — 选择了 DeepSeek 而非 Anthropic 直连，性价比优先
