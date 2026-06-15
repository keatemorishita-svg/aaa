# 🏪 AAA App Store Protocol v1.0

> The interface that turns a personal repository into a shared civilization.

---

## 核心设计原则

一个文明的应用商店不是一个"市场"——它是一个**进化空间**。

| 传统 App Store | AAA App Store |
|---|---|
| 中心审核 | Fork 即发布 |
| 统一标准 | 协议兼容即可 |
| 官方认证 | 使用量 = 认证 |
| 封闭围墙 | 任何人的 Fork 都可以有自己的 Store |
| 平台抽成 | 零成本，MIT 许可证 |

---

## 🧱 接口规范：如何把任何项目接入 AAA

### 最小接入要求（3 个文件）

任何人想把他们的项目接入 AAA App Store，只需要在项目根目录下增加三个文件：

```
<your-project>/
├── ...（你的原有项目文件）
├── COS-META.md          # ① 映射文件：你的项目在文明架构中的位置
├── COS-SOP.md           # ② 方法文件：你用什么方法造出这个东西的
└── COS-EVOLUTION.md     # ③ 进化文件：你希望这个东西怎么被 Fork / 改进
```

这三个文件是 **AAA 的 USB 接口**——格式统一，内容自由。

---

### ① COS-META.md —— 架构映射

```markdown
# COS-META

## Identity
- **Name**: <项目名称>
- **Author**: <作者 / 团队>
- **Version**: <版本号>
- **Date**: <创建日期>

## Architecture Mapping
这个项目主要工作在 AAA 的哪一层？

- [ ] Cognition Layer — 帮助理解某个领域
- [ ] Protocol Layer — 定义交互规则/标准
- [ ] Execution Layer — 做什么/怎么做
- [ ] Evolution Layer — 如何自我改进

> 可以勾选多个。一个项目可以跨层。

## Primitive Check
这个项目为文明的三个原语贡献了什么？

- **Access** — 它让什么变得更可进入？
- **Mutation** — 它允许什么被修改？
- **Recursion** — 它如何接受自己的改变？

> 每个至少写一句话。如果你写不出来，可能你的项目不适合这里。

## Dependencies
- **Requires**: 需要什么前置知识/工具？
- **Extends**: 基于 AAA 的哪个部分？
- **Conflicts**: 与什么已知观点/工具有张力？

## Fork Instructions
- **Best fork point**: 从哪里开始 Fork 最有用？
- **What to keep**: Fork 时必须保留什么？
- **What to change**: Fork 时最值得改什么？
```

---

### ② COS-SOP.md —— 方法溯源

```markdown
# COS-SOP

## How this was made
描述你用什么方法/流程造出这个项目的。

如果是用 AAA Refinement SOP：
- [ ] 经过了第 1 轮：本体论定位
- [ ] 经过了第 2 轮：命题强度分析
- [ ] 经过了第 3 轮：薄弱点定向攻击
- [ ] 经过了第 4 轮：维度切换攻击
- [ ] 经过了第 5 轮：价值识别
- [ ] 经过了第 6 轮：操作化

如果是自己的方法：
> 描述你的流程。越具体越好。方法本身就是有价值的产出。

## Key Decisions
列出你在过程中做出的 3-5 个关键决策及其理由。

## What you tried and abandoned
列出你尝试过但最终放弃的方向。这对后来者可能比成功路径更有价值。
```

---

### ③ COS-EVOLUTION.md —— 进化邀请

```markdown
# COS-EVOLUTION

## Current State
- **Maturity**: [ ] Draft  [ ] Stable  [ ] Evolving  [ ] Legacy
- **Known weaknesses**: 列出你知道的薄弱点（诚实比完美更有价值）

## Evolution Invitation
- **Best contribution type**: PR / Fork / Discussion / Challenge
- **What needs improvement most**: 你最希望别人帮你改进什么？
- **What should NOT be changed**: 哪些部分是你不希望被改的？（如果你有强烈的理由，说出来）

## Fork Policy
- **Fork friendly?**: [ ] Yes, fork anything  [ ] Yes, but keep core intact  [ ] Please discuss first
- **Merge preference**: 你希望 Fork 最终 Merge 回来吗？
- **Succession**: 如果你消失两年，这个项目应该由谁/如何继续？
```

---

## 🏪 如何提交到 App Store

### 提交路径（Fork 模型）

```
① Fork aaa 仓库
② 把你的项目（含 3 个 COS 文件）放在 applications/<your-project-name>/
③ 在 applications/INDEX.md 中添加一行
④ 开 PR
⑤ 维护者 Review COS-META.md（审查架构映射，不审查内容质量）
⑥ Merge → 你的应用进入 App Store
```

### 审查标准（极简）

PR 只会因为以下原因被拒绝：

| 拒绝原因 | 说明 |
|---|---|
| COS-META.md 缺失或不完整 | 必须完成架构映射和原语检查 |
| COS-SOP.md 缺失 | 必须说明方法——空项目没有进化价值 |
| 与已有应用完全重复 | 如果内容完全重复且没有新视角，建议 Fork 已有应用而非新建 |
| 违反 MIT 许可证 | 你的项目必须也是开放许可证 |

**不会因为以下原因被拒绝：**
- "质量不够好"——质量通过使用量自然选择
- "与我们观点冲突"——冲突是 Fork 的燃料
- "太简单"——最小原语就是简单的
- "不成熟"——Draft 状态的项目可以进入 App Store

---

## 📇 applications/INDEX.md —— 应用目录

App Store 需要一个索引文件，列出所有已接入的应用：

```markdown
# AAA App Store — Index

## Core Applications（官方维护）

| 应用 | 层 | 成熟度 | 描述 |
|---|---|---|---|
| [tool-comparison](./tool-comparison/) | Cognition | Stable | 10-dimension AI tool comparison framework |
| [agent-first-workflow](./agent-first-workflow/) | Execution | Stable | AI-native development paradigm |
| [naming-conventions](./naming-conventions/) | Protocol | Stable | Information-dense file naming protocol |
| [refinement-sop](./refinement-sop/) | Evolution | Evolving | 6-round adversarial refinement methodology |
| [core-questions](./core-questions/) | Cognition | Stable | 10 adversarial probes of the framework |
| [fable-5-analysis](./fable-5-analysis/) | Cognition | Stable | Model vs tool hierarchy distinction |

## Community Applications（社区贡献）

| 应用 | 作者 | 层 | 成熟度 | 描述 |
|---|---|---|---|---|
| *（你的项目可以出现在这里）* ||||
```

---

## 🌐 为什么这个接口设计是成立的

### 1. 最小接入成本 = 3 个 Markdown 文件

不需要学新技术、不需要改代码、不需要签协议。三个文件，纯文本，写完就能提交。这是 **Access 原语**在接口层的实现。

### 2. COS-META 强制架构映射

每个贡献者必须回答"我的项目在四层架构的哪一层"和"我的项目为三个原语贡献了什么"。这保证了接入的项目不是随意的——它们必须与 AAA 有结构性的关联。即使只是回答"我不知道，勾了三个层"，这个回答本身也是有信息量的。

### 3. COS-SOP 暴露方法

这是 AAA 与其他框架的关键区别——**我们不只要产出，我们要产出的方法**。一个没写 SOP 的项目无法被别人改进，因为别人不知道它是怎么造出来的。暴露方法 = 暴露可改进的点。

### 4. COS-EVOLUTION 内置 Fork 逻辑

每个项目自带"怎么 Fork 我"的说明书。这意味着：
- Fork 从逆向工程变成了按图施工
- 作者明确说了"改这里最有价值"
- 进化路径是预设的，不是事后发现的

### 5. 审查只审查接口，不审查内容

这像 TCP/IP——只检查包的格式是否正确，不检查包里的内容是什么。内容的好坏由使用量（Selection）来决定，不由维护者（Central Authority）来决定。

**这就是"协议层"在应用商店中的实例化。**

---

## 🔮 未来的进化路径

### 阶段 1：手动 INDEX（当前）
INDEX.md 手动维护，PR 手动 Review。

### 阶段 2：社区索引
当社区应用超过 20 个时，INDEX.md 按层分类，增加搜索友好的标签系统。

### 阶段 3：Fork 商店
任何人的 Fork 都可以维护自己的 App Store，有自己的 INDEX.md 和自己的审查标准。不同的 Store 之间竞争——用户用注意力投票。

### 阶段 4：自进化商店
商店协议本身（COS-META/COS-SOP/COS-EVOLUTION 格式）可以通过 PR 被修改。商店进化商店自己。

---

## 一句话总结

> The App Store is not a gate. It is a protocol. Any project that speaks the protocol is part of the civilization.
