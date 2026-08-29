---
title: State Duplication as a Performance Risk
aliases:
- AI-Induced Redundant State and Duplicate Fetching
tags:
- concept
summary: AI 生成代码时容易重复创建同一份数据的 state，这种冗余状态往往会在后期演变成性能问题。
created: '2026-08-26'
updated: '2026-08-26'
---

# State Duplication as a Performance Risk

%% ytkb:def %%
AI 生成代码时容易重复创建同一份数据的 state，这种冗余状态往往会在后期演变成性能问题。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[frontend-ai-coding-assistants]] · [[frontend]]
%% ytkb:end %%

## 要点

%% ytkb:video:AMerB8XjfZ0 %%
### 来自 [[2026-06-30-top-15-frontend-interview-questions-for-2026-wa-se]]
- AI 生成前端代码时容易把同一份数据在 state 中重复表示，这类 state 重复常常会在后期变成性能瓶颈。（[03:00](https://youtu.be/AMerB8XjfZ0?t=180)）
%% ytkb:end %%

%% ytkb:video:hA_XnzB1Ef8 %%
### 来自 [[2026-07-07-3-frontend-skills-ai-cant-replace-become-ai-proof]]
- 如果用 AI 独立地在各处生成组件而不做架构层面的沟通协调，很容易出现 local state 遍地开花且相互冗余，同一份数据被在两个不同地方分别从后端 fetch，造成重复请求。（[12:03](https://youtu.be/hA_XnzB1Ef8?t=723)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[ai-prompt-to-ui-overoptimization]]
- [[essential-state]]
- [[single-record-principle]]
%% ytkb:end %%
