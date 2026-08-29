---
title: Caching Motivation from Repeated Access
aliases: []
tags:
- concept
summary: 当大量用户在短时间内反复访问同一资源（如同一文件）时，若无缓存机制，每次访问都要重新执行完整的计算与查询链路，造成计算资源浪费，这正是引入缓存的动机。
created: '2026-08-26'
updated: '2026-08-26'
---

# Caching Motivation from Repeated Access

%% ytkb:def %%
当大量用户在短时间内反复访问同一资源（如同一文件）时，若无缓存机制，每次访问都要重新执行完整的计算与查询链路，造成计算资源浪费，这正是引入缓存的动机。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-caching-edge]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:Qa-7iWxDz1A %%
### 来自 [[2026-06-08-fundamentals-of-backend-architecture---how-to-desi]]
- 以500个用户每天反复打开应用首页同一份文件为例：若无缓存，每次请求都会重新触发从 gateway 到 files service、relational database、object storage 的完整计算链路，造成资源浪费。（[36:09](https://youtu.be/Qa-7iWxDz1A?t=2169)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[dau-mau-scale-requirement]]
- [[uncached-file-request-path]]
%% ytkb:end %%
