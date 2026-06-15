# COS-SOP

## How this was made

1. **范式识别**: 从实际工作行为中识别出"用户不是在写代码，而是在审核 AI 写的代码"
2. **工具匹配**: 基于 Agent-first 需求重新评估所有工具——不是找"最好的工具"，而是找"对 Agent-first 范式最优的工具组合"
3. **成本优化**: 在模型灵活性的前提下，选择性价比最高的 API 后端
4. **持续迭代**: CLAUDE.md 和 memory 系统在工作过程中持续精炼

## Key Decisions

1. **模型选择优先于工具选择** — 先选模型（deepseek-v4-pro，性价比最优），再选支持该模型的工具（Claude Code，模型灵活性满分）
2. **CLAUDE.md 作为一等资产** — 不只是配置，而是工作流的"认知外骨骼"
3. **放弃行内补全** — Agent-first 范式下，Tab 补全是解决错误问题的正确工具

## What you tried and abandoned

- 尝试在 Cursor 中实现 Agent-first 工作流，但模型锁定的限制导致成本不可控
- 尝试全 Anthropic 直连（更高性能），但成本差异不值得性能差异
