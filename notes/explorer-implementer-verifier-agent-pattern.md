---
title: Explorer-Implementer-Verifier Agent Pattern
aliases: []
tags:
- concept
summary: 多Agent协作循环中常见的三角色分工模式：一个Agent负责探索需求，一个负责实现代码，另一个负责对照需求规格进行验证。
created: '2026-08-26'
updated: '2026-08-26'
---

# Explorer-Implementer-Verifier Agent Pattern

%% ytkb:def %%
多Agent协作循环中常见的三角色分工模式：一个Agent负责探索需求，一个负责实现代码，另一个负责对照需求规格进行验证。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-agent-architecture]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:KgiwIEBeOHw %%
### 来自 [[2026-06-16-什么是循环工程loop-engineering-coding-agent-子agent-mcp协议]]
- 无论用哪款工具，最常见的分工模式都是一致的：一个Agent负责探索需求，一个负责实现代码，还有一个负责对照需求规格做验证。（[12:40](https://youtu.be/KgiwIEBeOHw?t=760)）
- 循环会再派出第二个子Agent，对照项目的技能规范和已有的测试用例，审查第一个子Agent起草的修复方案。（[14:30](https://youtu.be/KgiwIEBeOHw?t=870)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[agent-specialization]]
- [[claude-code-agent-teams]]
- [[isolated-worktree-per-task]]
%% ytkb:end %%
