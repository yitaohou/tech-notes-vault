---
title: Shared Library Module Extraction
aliases: []
tags:
- concept
summary: 将多个模块间会重复用到的功能抽取到共享 library 中，从而避免重复实现，也减少 AI 每次需要搜索或读取的代码范围。
created: '2026-08-26'
updated: '2026-08-26'
---

# Shared Library Module Extraction

%% ytkb:def %%
将多个模块间会重复用到的功能抽取到共享 library 中，从而避免重复实现，也减少 AI 每次需要搜索或读取的代码范围。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-coding-agents]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:hA_XnzB1Ef8 %%
### 来自 [[2026-07-07-3-frontend-skills-ai-cant-replace-become-ai-proof]]
- 为避免 AI 每次都要在整个代码库里重新查找或实现重复功能，可以把可复用功能抽取到 modules 间共享的 library 中，这本身就是前端工程中模块化设计的工作。（[09:03](https://youtu.be/hA_XnzB1Ef8?t=543)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[ai-context-scope-reduction-via-modularization]]
- [[dry-principle]]
- [[micro-frontends]]
%% ytkb:end %%
