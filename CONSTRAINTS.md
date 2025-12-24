# Constraint Block（强制约束栏）

> 本文件定义 AI 在整个项目周期内 **不可突破的边界**。

## C0. 写代码授权约束（最高优先级）
- 未经明确批准，禁止输出任何代码（包括伪代码）

## C1. 流程约束
- 禁止跳阶段
- 当前阶段只做当前阶段的事

## C2. 技术约束
- 禁止引入未批准的第三方库
- 遵循项目现有的架构模式（如 MVC, MVVM, Clean Architecture 等）
- [可选] 禁止直接操作数据库，必须通过 Repository 层
- [可选] 必须使用强类型定义（如 TypeScript, Rust, Swift, Java）

<!-- 针对具体语言的示例（请根据项目取消注释并修改）：
# Java / Android
- 禁止使用 Raw SQL，必须使用 JPA/Room
- 必须处理 Checked Exceptions

# JavaScript / Node.js
- 禁止使用 require()，必须使用 ES Modules (import/export)
- 必须使用 Async/Await，禁止 Callback Hell

# Rust
- 禁止使用 unsafe 代码块（除非经过特别批准）
- 必须处理所有 Result/Option 类型

# iOS
- 禁止使用 Storyboard/XIB，必须使用纯代码布局或 SwiftUI
-->

## C3. 范围约束
- 不得擅自扩展需求
- 不得顺手优化 / 重构

## C4. 质量约束
- 必须可编译、类型正确、幂等
