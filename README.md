# skills

收录作者个人的 Claude Code / Codex Skill，**主要面向中文开发者**。按分类整理，附带「Skill 组合指南」，告诉你做一个具体项目时该按什么顺序、用哪几套 Skill。

## 分类总览

| 分类 | 说明 | 入口 |
| --- | --- | --- |
| **frontend-client** | 前端 / 客户端开发（React、Vue、Nuxt、Tailwind、Three.js、Remotion、CSS 布局等） | [frontend-client/README.md](./frontend-client/README.md) |
| **mobile-flutter** | Flutter / Dart 客户端开发（架构、布局、路由、数据层、测试、静态分析等） | [mobile-flutter/README.md](./mobile-flutter/README.md) |
| **design-taste** | 设计品味 / 反模板化前端设计（taste-skill + impeccable） | [design-taste/README.md](./design-taste/README.md) |
| **incremental-branch-training** | 增量分支驱动项目训练框架（教练 + Reviewer + 脚手架） | [incremental-branch-training/SKILL.md](./incremental-branch-training/SKILL.md) |
| **reverse-blueprint-pattern** | 逆向施工图模式，按物理依赖顺序逐层交付（Go / Java / Python / 后端 / AI agent / 中间件） | [reverse-blueprint-pattern/SKILL.md](./reverse-blueprint-pattern/SKILL.md) |

## Skill 组合指南

不同 Skill 各司其职，做项目时按阶段取用，而不是全部堆在一起。

### 场景一：从零设计并开发一个 Flutter 前端 App

按下面顺序走，每一阶段用对应的 Skill：

| 阶段 | 做什么 | 用哪个 Skill |
| --- | --- | --- |
| 1. 设计方向 | 先定视觉语言与页面结构，避免「模板脸」 | `design-taste/design-taste-frontend`（或 `impeccable` 走完整设计流程）。注意 taste-skill 偏 Web 落地页，Flutter 侧主要借鉴它的「设计方向 / 反 slop」思路，具体布局交给下面 Flutter Skill |
| 2. 架构分层 | 按 UI / Logic / Data 分层，为后续扩展打底 | `flutter-apply-architecture-best-practices` |
| 3. 页面布局 | 移动端 / 平板 / 桌面自适应；排查 overflow | `flutter-build-responsive-layout`、`flutter-fix-layout-issues` |
| 4. 路由导航 | 页面流、深链、多端导航 | `flutter-setup-declarative-routing` |
| 5. 数据层 | 接服务端接口、JSON 序列化 / model / 代码生成 | `flutter-use-http-package`、`flutter-implement-json-serialization` |
| 6. 测试 | 单测 + Widget 测试 + 集成测试 | `dart-add-unit-test`、`dart-generate-test-mocks`、`flutter-add-widget-test`、`flutter-add-integration-test` |
| 7. 质量收口 | 静态分析、修运行时错误、解依赖冲突 | `dart-run-static-analysis`、`dart-fix-runtime-errors`、`dart-resolve-package-conflicts` |

> 一句话流程：**设计方向 → 架构分层 → 布局 → 路由 → 数据层 → 测试 → 质量收口**。

### 场景二：做一个「不像模板」的 Web 落地页 / 作品集

| 阶段 | 用哪个 Skill |
| --- | --- |
| 设计方向与反 slop | `design-taste/design-taste-frontend`（或 `impeccable`） |
| 框架实现（按技术栈选一个） | `vercel-react-best-practices` / `vue-best-practices` / `nuxt-best-practices` |
| 样式与布局 | `tailwind-css-patterns`、`modern-css-layout` |
| 组件组合模式 | `vercel-composition-patterns` |
| 规范审查（可访问性 / 最佳实践） | `web-design-guidelines` |
| 视频 / 动效（如需要） | `remotion-best-practices` |
| 3D 视觉（如需要） | `threejs-fundamentals` |

### 场景三：后端 / 全栈求职项目训练

- 用 `incremental-branch-training` 训练「能讲清、写出、维护一个项目」的能力。
- 用 `reverse-blueprint-pattern` 按物理依赖顺序逐层交付，同一套流程适配 Go / Java / Python。

## 去重与取舍

- **设计类 Skill 保留多套但明确分工**：`design-taste-frontend`（反 slop 落地页实现）、`impeccable`（全流程设计总监 + 反模式检测）、`frontend-client/frontend-design`（通用视觉设计决策）、`frontend-client/web-design-guidelines`（规范审查）职责不同，日常主用一个即可，见 [design-taste/README.md](./design-taste/README.md) 的选择表。
- **框架类「编码约束」Skill 不合并**：React / Vue / Nuxt 的 best-practices 各自约束各自的框架，互不重叠，按技术栈各取所需。
- **同名不同源的 Skill 以「来源 + 目录」区分**：部分条目来自不同上游仓库，README 里用「来源」列标注，避免误删。
