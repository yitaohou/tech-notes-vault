---
title: AI Code Duplication Tendency
aliases: []
tags:
- concept
summary: AI 编程助手倾向于局部优化，导致同一功能的函数或组件被在多处重复实现的现象。
created: '2026-08-26'
updated: '2026-08-26'
---

# AI Code Duplication Tendency

%% ytkb:def %%
AI 编程助手倾向于局部优化，导致同一功能的函数或组件被在多处重复实现的现象。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[frontend-ai-coding-assistants]] · [[frontend]]
%% ytkb:end %%

## 要点

%% ytkb:video:AMerB8XjfZ0 %%
### 来自 [[2026-06-30-top-15-frontend-interview-questions-for-2026-wa-se]]
- AI 倾向于做局部优化，经常会在代码库的不同位置重复写出功能相同的函数或组件。（[09:01](https://youtu.be/AMerB8XjfZ0?t=541)）
%% ytkb:end %%

%% ytkb:video:hA_XnzB1Ef8 %%
### 来自 [[2026-07-07-3-frontend-skills-ai-cant-replace-become-ai-proof]]
- 内联声明的组件因作用域被局限在父组件内部而无法被复用，导致 AI 每次遇到相似的小问题时都要重新写一遍类似代码，造成大量代码重复。（[06:02](https://youtu.be/hA_XnzB1Ef8?t=362)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[ai-monolithic-component-antipattern]]
- [[inline-component-declaration-antipattern]]
- [[static-code-analysis-beyond-linting]]
%% ytkb:end %%
