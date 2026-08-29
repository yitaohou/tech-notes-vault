---
title: RAM Caching Large Files Anti-Pattern
aliases: []
tags:
- concept
summary: 把整份大文件（如图片、视频）直接放进 RAM 缓存的做法，通常成本过高、并非推荐实践。
created: '2026-08-26'
updated: '2026-08-26'
---

# RAM Caching Large Files Anti-Pattern

%% ytkb:def %%
把整份大文件（如图片、视频）直接放进 RAM 缓存的做法，通常成本过高、并非推荐实践。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-caching-edge]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:Qa-7iWxDz1A %%
### 来自 [[2026-06-08-fundamentals-of-backend-architecture---how-to-desi]]
- 把整个大文件直接塞进 RAM 缓存是常见的误区，通常成本非常高，不是标准做法。（[39:09](https://youtu.be/Qa-7iWxDz1A?t=2349)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[ram-cost-scarcity]]
%% ytkb:end %%
