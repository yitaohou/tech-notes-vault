---
title: Single Server Setup
aliases: []
tags:
- concept
summary: 把 web 应用、数据库、缓存等所有组件全部部署在同一台服务器上的最简系统架构，适用于小规模用户场景。
created: '2026-08-26'
updated: '2026-08-26'
---

# Single Server Setup

%% ytkb:def %%
把 web 应用、数据库、缓存等所有组件全部部署在同一台服务器上的最简系统架构，适用于小规模用户场景。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-scalability]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:oYxTTirKY8M %%
### 来自 [[2026-05-26-system-design-explained-apis-databases-caching-cdn]]
- 在单服务器架构中，web 应用、数据库、缓存等组件全部运行在同一台服务器上，这是系统设计从零开始最基本的起点，之后再随用户规模增长逐步演化。（[00:00](https://youtu.be/oYxTTirKY8M?t=0)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[horizontal-scaling]]
- [[incremental-system-design-approach]]
- [[vertical-scaling]]
%% ytkb:end %%
