---
title: Blast Radius of Dependency/Config Changes
aliases: []
tags:
- concept
summary: 指依赖或全局配置层面的改动一旦出错，其影响范围（blast radius）远大于单个组件写得不够优的情况。
created: '2026-08-26'
updated: '2026-08-26'
---

# Blast Radius of Dependency/Config Changes

%% ytkb:def %%
指依赖或全局配置层面的改动一旦出错，其影响范围（blast radius）远大于单个组件写得不够优的情况。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-architecture-fundamentals]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:AMerB8XjfZ0 %%
### 来自 [[2026-06-30-top-15-frontend-interview-questions-for-2026-wa-se]]
- 代码审查时应优先检查依赖或全局配置的改动，因为这类改动一旦出错的影响范围（blast radius）远大于某个组件写得不够优（sub-optimal）的情况，后者通常够用且问题不大。（[06:00](https://youtu.be/AMerB8XjfZ0?t=360)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[manual-review-trigger-config-changes]]
%% ytkb:end %%
