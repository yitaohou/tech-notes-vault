---
title: Component Extraction for Reuse and Testability
aliases: []
tags:
- concept
summary: 把内联声明在父组件内部的子组件提取到独立文件（并可配合 memoization）的做法，用于提升可复用性并使其可以被单独添加 unit test。
created: '2026-08-26'
updated: '2026-08-26'
---

# Component Extraction for Reuse and Testability

%% ytkb:def %%
把内联声明在父组件内部的子组件提取到独立文件（并可配合 memoization）的做法，用于提升可复用性并使其可以被单独添加 unit test。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[frontend-react-component-design]] · [[frontend]]
%% ytkb:end %%

## 要点

%% ytkb:video:hA_XnzB1Ef8 %%
### 来自 [[2026-07-07-3-frontend-skills-ai-cant-replace-become-ai-proof]]
- 解决内联组件问题的方法是把该组件提取到单独文件，必要时配合 memoization，这样组件既可复用，也可以在需要时为其单独编写 unit test。（[06:02](https://youtu.be/hA_XnzB1Ef8?t=362)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[component-logic-extraction]]
- [[inline-component-declaration-antipattern]]
%% ytkb:end %%
