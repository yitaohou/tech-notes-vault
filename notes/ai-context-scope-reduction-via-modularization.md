---
title: AI Context Scope Reduction via Modularization
aliases: []
tags:
- concept
summary: 通过将代码库拆分为独立模块（如 micro-frontend），使 AI 编码时只需读取相关模块而非整个代码库，从而降低输入 token 消耗。
created: '2026-08-26'
updated: '2026-08-26'
---

# AI Context Scope Reduction via Modularization

%% ytkb:def %%
通过将代码库拆分为独立模块（如 micro-frontend），使 AI 编码时只需读取相关模块而非整个代码库，从而降低输入 token 消耗。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[frontend-architecture]] · [[frontend]]
%% ytkb:end %%

## 要点

%% ytkb:video:AMerB8XjfZ0 %%
### 来自 [[2026-06-30-top-15-frontend-interview-questions-for-2026-wa-se]]
- 把前端 monolith 拆分为 micro-frontend 后，AI 理想情况下只需读取该特定 micro-frontend 的代码，而非整个代码库，从而减少输入 token 数量。（[15:02](https://youtu.be/AMerB8XjfZ0?t=902)）
%% ytkb:end %%

%% ytkb:video:KuClyhvSzXk %%
### 来自 [[2026-06-18-frontend-system-design-explained-w-senior-engineer]]
- 当开发者只在更小的模块内工作时，AI coding 工具需要处理的 context 更少，因此效率更高、风险更低。（[06:02](https://youtu.be/KuClyhvSzXk?t=362)）
%% ytkb:end %%

%% ytkb:video:hA_XnzB1Ef8 %%
### 来自 [[2026-07-07-3-frontend-skills-ai-cant-replace-become-ai-proof]]
- 拥有清晰模块边界的前端架构，能让 AI agent 在扩展代码时用更少的 token 实现同等价值的功能增量，这是从 context engineering 角度出发选择模块化架构的重要理由。（[00:00](https://youtu.be/hA_XnzB1Ef8?t=0)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[deep-module]]
- [[design-tokens]]
- [[front-end-system-design]]
- [[micro-frontends]]
- [[microservices]]
%% ytkb:end %%
