# ai-collab-rules · AI 协作规则正本（万能版）

这是「**AI 协作规则 · 0基础全托管万能版**」的**正本（master）**。适用于任何用 Cursor/AI 开发的项目，不绑技术栈、不绑路径。

> 给 0 基础项目拥有者：你只管 3 件事（说需求 / 答选择题 / 验收），全部工程严谨由 AI 内部承担。

## 怎么用（推荐：零手动）

在 Cursor「设置 → Rules → User（用户级）」放一句**瘦指针**（全局设一次，所有项目通用）：

> 我的 AI 协作规则正本仓库：`https://github.com/gthubtom1/ai-collab-rules`（文件 `ai-collab-zero-base.mdc`）。每次进入一个项目的第一次对话，先检查本地有没有 `.cursor/rules/ai-collab-zero-base.mdc`：有就读它、按它执行、冲突时以它为准；没有就**自动**从上面仓库下载该文件写入 `.cursor/rules/` 再执行。全程不用我手动操作。

之后每开一个新项目，AI 第一次对话会**自动**把规则拉到 `.cursor/rules/`，你什么都不用做。

## 手动方式（可选）

也可以手动把本仓库的 [`ai-collab-zero-base.mdc`](./ai-collab-zero-base.mdc) 复制到新项目的 `.cursor/rules/ai-collab-zero-base.mdc`。

## 三层同步（单一源，防漂移）

- **正本（master）** = 本仓库 `ai-collab-zero-base.mdc`
- **工作副本** = 各项目 `.cursor/rules/ai-collab-zero-base.mdc`（Cursor 真正加载的那份）
- **系统设置** = 瘦指针（全局一次，几乎永不用改）

## 自进化（越用越强）

每次踩坑/事故后，AI 主动复盘「这暴露了规则哪条缺口」→ 改工作副本（落盘，本会话立刻重读生效）→ `git commit`（message 写「事故 → 补了哪条」）→ push 回本仓库。**git 提交历史 = 进化履历**。

## 规则全文

见 [`ai-collab-zero-base.mdc`](./ai-collab-zero-base.mdc)（含第一部分给用户看、第二部分给 AI 看：总则 + 8 阶段生命周期 + 横切铁律）。
