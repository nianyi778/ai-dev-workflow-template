# AI Dev Workflow Template

这是一套用于 **AI + 人类协作软件开发** 的工程级模板。

## 作为 GitHub Template Repo 使用
1. 把本仓库推到 GitHub
2. 在 GitHub 仓库页面进入 `Settings` → `General` → 勾选 `Template repository`
3. 之后新项目直接点 `Use this template` 创建

> 仓库已内置 Issue/PR 模板：用 Issue 提交阶段 1 的 Change Request，用 PR 承载实现与自检。

## 核心原则
- 文档优先
- 人工审批
- 分阶段交付
- 未授权禁止写代码
- 每次变更可追溯、可验收、可回滚

## 适用技术栈
本模板流程是**通用的**，适用于任何语言和框架（Java, Rust, Node.js, iOS, Android, Python 等）。

唯一需要针对性修改的是 `CONSTRAINTS.md` 中的 **C2. 技术约束**：
- **Java/Android**: 规定是否用 Room/JPA，是否允许 RxJava 等。
- **Rust**: 规定是否允许 `unsafe`，错误处理规范等。
- **Node.js**: 规定 CommonJS vs ESM，ORM 选择等。
- **iOS**: 规定 UIKit vs SwiftUI，数据层方案等。

## 使用方式（推荐）
1. 新项目 → 复制整个仓库
2. 每次新需求：
   - 把 `AI_INSTRUCTIONS.md` 粘给 AI
   - 使用 `templates/CHANGE_REQUEST.md` 写需求
3. 严格按 WORKFLOW.md 的阶段推进

> ⚠️ AI 不允许跳阶段，不允许未经批准写代码
