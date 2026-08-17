# personal_skills

这是一个面向中文开发者的 Claude Code / Codex Skill 集合。它的主线不是前端页面实现，而是建立一套能长期使用的工程学习能力：读懂真实代码、完成结构化开发、把项目经验沉淀为可复用的工程认知与面试表达。

前端、移动端和设计类 Skill 仍然保留，它们是特定技术方向的生产力工具；仓库最核心的入口是 `engineering-learning/`，其中的 Skill 能跨 Go、Java、Python、TypeScript 等后端项目复用。

## 分类总览

| 分类 | 解决的问题 | 入口 |
| --- | --- | --- |
| **engineering-learning** | 读陌生源码、按工程依赖写代码、通过项目训练建立可讲述的工程能力 | [engineering-learning/README.md](./engineering-learning/README.md) |
| **frontend-client** | React、Vue、Nuxt、Tailwind、Three.js、Remotion、CSS 等前端实现 | [frontend-client/README.md](./frontend-client/README.md) |
| **mobile-flutter** | Flutter / Dart 的架构、布局、路由、数据层、测试与质量收口 | [mobile-flutter/README.md](./mobile-flutter/README.md) |
| **design-taste** | 设计方向、反模板化界面与前端视觉审查 | [design-taste/README.md](./design-taste/README.md) |

## 核心学习路径

这三个通用 Skill 可以单独使用，也可以形成一条连续路径。

| 阶段 | 目标 | Skill |
| --- | --- | --- |
| 读 | 快速建立模块地图、追踪真实调用链、识别工程设计与修改风险 | [code-analysis-coach](./engineering-learning/code-analysis-coach/SKILL.md) |
| 写 | 以可维护的依赖顺序构建服务、基础设施与功能交付 | [reverse-blueprint-pattern](./engineering-learning/reverse-blueprint-pattern/SKILL.md) |
| 练 | 用增量分支训练需求拆解、实现、审查和项目表达 | [incremental-branch-training](./engineering-learning/incremental-branch-training/SKILL.md) |

典型使用方式：先用 `code-analysis-coach` 看懂现有项目的入口和主链路；需要新增或改造能力时，用 `reverse-blueprint-pattern` 保持实现顺序与依赖边界清晰；完成后用 `incremental-branch-training` 进行增量练习、复盘与表达训练。

## 专项能力

### 前端与客户端

- `frontend-client/`：按 Web 技术栈选择 React、Vue、Nuxt、CSS、组件组合或视觉审查 Skill。
- `mobile-flutter/`：覆盖 Flutter/Dart 的布局、路由、数据层、测试与故障排查。
- `design-taste/`：用于建立视觉方向和避免模板化产出，不替代工程学习主线。

### 组合示例

| 场景 | 推荐组合 |
| --- | --- |
| 接手企业后端服务并改一个需求 | `code-analysis-coach` → 按调用链定位修改点 → 项目既有测试/规范 |
| 从零实现可持续扩展的后端项目 | `reverse-blueprint-pattern` → `incremental-branch-training` |
| 把实习项目沉淀成秋招素材 | `code-analysis-coach` 的开发 + 沉淀或面试复盘模式 → `incremental-branch-training` |
| 实现带前端界面的完整项目 | 先选 `engineering-learning/` 的通用 Skill，再按需要叠加 `frontend-client/`、`mobile-flutter/` 或 `design-taste/` |

## 使用原则

- 优先解决当前代码问题，再做长期沉淀；不要为了文档而文档。
- 按任务和技术栈选 Skill，不需要每次全量启用。
- 前端 Skill 服务于界面交付，工程学习 Skill 服务于理解、设计、实现、复盘与表达。
