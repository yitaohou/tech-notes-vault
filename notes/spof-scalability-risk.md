---
title: SPOF Scalability Risk
aliases: []
tags:
- concept
summary: 存在单点故障的系统通常难以扩展，因为每新增一个组件都会带来该组件失效导致整体故障的额外风险。
created: '2026-08-26'
updated: '2026-08-26'
---

# SPOF Scalability Risk

%% ytkb:def %%
存在单点故障的系统通常难以扩展，因为每新增一个组件都会带来该组件失效导致整体故障的额外风险。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-scalability]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:oYxTTirKY8M %%
### 来自 [[2026-05-26-system-design-explained-apis-databases-caching-cdn]]
- 系统中存在单点故障会拖累可扩展性，因为每添加一个新组件都会引入新的失效风险点。（[27:03](https://youtu.be/oYxTTirKY8M?t=1623)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[horizontal-scaling]]
- [[single-point-of-failure]]
%% ytkb:end %%
