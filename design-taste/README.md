# design-taste

「设计品味 / 反模板化」前端设计 Skill 集合。核心目标是让 AI 生成的前端界面不再千篇一律（AI slop），而是具备真正有辨识度的设计语言：更强的版式、字体、动效、留白与克制感。

> 适用场景：落地页、作品集、营销页、产品 UI 重构等。不适用于纯后端 / 非 UI 任务。

## Skills

| 目录 | 安装名 | 来源 | 用途 |
| --- | --- | --- | --- |
| [design-taste-frontend](./design-taste-frontend/) | `design-taste-frontend` | [Leonxlnx/taste-skill](https://github.com/Leonxlnx/taste-skill)（v2 experimental） | 反模板化前端设计：读取 brief、推断设计方向，用「方差 / 动效 / 密度」三个旋钮控制版面与动效，附 GSAP 骨架、重构审计协议与发布前自检。适合落地页、作品集、改版。 |
| [impeccable](./impeccable/) | `impeccable` | [pbakaus/impeccable](https://github.com/pbakaus/impeccable)（v4.0.4） | 设计总监视角的完整设计工作流：22 个子命令（shape / critique / audit / polish / bolder / quieter / animate / colorize / typeset / layout / harden / optimize / adapt / live …），配套 60 条 UI 反模式检测规则。适合从设计、审查、打磨到上线前加固的全程。 |

## 如何选择设计类 Skill

本仓库里有多套「设计」Skill，来源不同、职责不同，建议按阶段选，而不是同时全上：

| 想做的事 | 首选 | 说明 |
| --- | --- | --- |
| 从 0 做一个「不能像模板」的前端（落地页 / 作品集 / 改版） | **design-taste-frontend** | 反 slop 最直接，先读 brief 定方向，再按三旋钮产出。 |
| 想要一套完整设计工作流（规划 → 审查 → 打磨 → 加固 → 浏览器里实时调） | **impeccable** | 命令最全，适合把它当作「设计总监」。 |
| 想要偏「设计决策 / 视觉人格」的通用指导（不绑定具体框架） | `frontend-client/frontend-design` | 强调「为每个客户做出不可复制的视觉身份」。 |
| 只想做一次 UI 规范 / 可访问性审查 | `frontend-client/web-design-guidelines` | 偏「检查清单」，不是生成式设计。 |

**重叠说明**：`design-taste-frontend`、`impeccable`、`frontend-design` 三者都围绕「让 AI 不做平庸 UI」，但侧重点不同——前者是「反 slop 落地页实现」，中间是「全流程设计总监 + 反模式检测」，后者是「通用视觉设计决策」。日常只选一个主用，避免多套指令互相打架。

## 安装与使用

- 安装到 Claude Code（项目级）：`npx skills add https://github.com/Leonxlnx/taste-skill --skill "design-taste-frontend"`
- 安装 impeccable：`npx impeccable install`（项目级安装到 `.claude/skills/impeccable/`）
- impeccable 的 `SKILL.md` 内部脚本路径写死为 `.claude/skills/impeccable/scripts/*`，作为独立 skill 安装时请放在该路径下；本目录是「源库」形态，直接整目录拷贝即可。

## 许可

- `design-taste-frontend`：MIT（见 `design-taste-frontend/LICENSE.txt`）
- `impeccable`：Apache 2.0（见 `impeccable/LICENSE`）
