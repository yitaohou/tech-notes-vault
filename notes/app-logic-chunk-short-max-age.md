---
title: App Logic Chunk with Short max-age
aliases: []
tags:
- concept
summary: 把频繁变化的应用逻辑和组件代码打包成单独的 chunk，并设置较短的 max-age（如5分钟），确保用户能及时拿到最新版本。
created: '2026-08-26'
updated: '2026-08-26'
---

# App Logic Chunk with Short max-age

%% ytkb:def %%
把频繁变化的应用逻辑和组件代码打包成单独的 chunk，并设置较短的 max-age（如5分钟），确保用户能及时拿到最新版本。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[frontend-performance-optimization]] · [[frontend]]
%% ytkb:end %%

## 要点

%% ytkb:video:AMerB8XjfZ0 %%
### 来自 [[2026-06-30-top-15-frontend-interview-questions-for-2026-wa-se]]
- 由于应用的业务逻辑和组件代码会频繁部署，这部分应该单独打包，并设置很短的 max-age（例如5分钟），以保证用户总能拿到最新的 JavaScript。（[42:09](https://youtu.be/AMerB8XjfZ0?t=2529)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[selective-caching-policy-frontend]]
- [[stable-vendor-chunk-long-max-age]]
%% ytkb:end %%
