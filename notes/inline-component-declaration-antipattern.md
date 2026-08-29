---
title: Inline Component Declaration Antipattern
aliases: []
tags:
- concept
summary: AI 编码模型常见的代码坏味道：把子组件（如某个文本渲染函数）内联声明在父组件内部，而不是提取到外部，导致该子组件在父组件每次渲染时都被重新创建。
created: '2026-08-26'
updated: '2026-08-26'
---

# Inline Component Declaration Antipattern

%% ytkb:def %%
AI 编码模型常见的代码坏味道：把子组件（如某个文本渲染函数）内联声明在父组件内部，而不是提取到外部，导致该子组件在父组件每次渲染时都被重新创建。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[frontend-ai-coding-assistants]] · [[frontend]]
%% ytkb:end %%

## 要点

%% ytkb:video:hA_XnzB1Ef8 %%
### 来自 [[2026-07-07-3-frontend-skills-ai-cant-replace-become-ai-proof]]
- AI 生成的前端代码中常见把一个如 text 渲染这样的子组件直接内联声明在父组件内部，而不是拆分出去，导致其在每次父组件重新渲染时都被重复创建。（[06:02](https://youtu.be/hA_XnzB1Ef8?t=362)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[ai-code-duplication-tendency]]
- [[ai-monolithic-component-antipattern]]
- [[component-logic-extraction]]
%% ytkb:end %%
