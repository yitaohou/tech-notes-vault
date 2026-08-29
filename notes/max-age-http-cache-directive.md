---
title: max-age HTTP Cache Directive
aliases: []
tags:
- concept
summary: max-age 指定客户端在多久之后需要重新校验或刷新某个缓存资源，是决定资源刷新频率的核心缓存参数。
created: '2026-08-26'
updated: '2026-08-26'
---

# max-age HTTP Cache Directive

%% ytkb:def %%
max-age 指定客户端在多久之后需要重新校验或刷新某个缓存资源，是决定资源刷新频率的核心缓存参数。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-caching-edge]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:AMerB8XjfZ0 %%
### 来自 [[2026-06-30-top-15-frontend-interview-questions-for-2026-wa-se]]
- max-age 本质上是决定客户端多久应该重新检查并刷新某个资源的参数，可以针对不同类型的资源设置不同数值。（[42:09](https://youtu.be/AMerB8XjfZ0?t=2529)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[selective-caching-policy-frontend]]
%% ytkb:end %%
