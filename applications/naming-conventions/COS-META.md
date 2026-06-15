# COS-META

## Identity
- **Name**: AXA v3 文件命名规范
- **Author**: AAA 社区
- **Version**: 1.0
- **Date**: 2026-06

## Architecture Mapping

- [ ] Cognition Layer
- [x] Protocol Layer — 定义了文件命名这一最小交互协议
- [ ] Execution Layer
- [x] Evolution Layer — 协议本身可以版本迭代（v1 → v2 → v3）

## Primitive Check

- **Access** — 文件名即文档元数据，降低信息检索的认知成本
- **Mutation** — 标记位可以扩展（增加新的自动/手动标记）
- **Recursion** — 命名规范本身可以通过 PR 修改（v3 → v4）

## Dependencies
- **Requires**: Obsidian 或任何字符串排序的文件管理器
- **Extends**: AAA Protocol Layer 的"最小协议"概念——协议不必是 API，文件名也是一种协议
- **Conflicts**: 与"全文搜索替代一切分类"的范式有张力

## Fork Instructions
- **Best fork point**: 标记位定义（换成你领域的元数据维度）
- **What to keep**: 倒序分排序逻辑、渐进标注原则
- **What to change**: 标记位含义（G/A → 你的标记）
