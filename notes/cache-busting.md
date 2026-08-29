---
title: Cache Busting
aliases: []
tags:
- concept
summary: module bundler使用的一种缓存失效机制，确保部署新版本后用户获取的是最新资源，而不是仍残留在CDN中的旧版本。
created: '2026-08-26'
updated: '2026-08-26'
---

# Cache Busting

%% ytkb:def %%
module bundler使用的一种缓存失效机制，确保部署新版本后用户获取的是最新资源，而不是仍残留在CDN中的旧版本。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-caching-edge]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:KuClyhvSzXk %%
### 来自 [[2026-06-18-frontend-system-design-explained-w-senior-engineer]]
- cache busting是module bundler采用的机制，用来在部署新版本时强制让用户拿到最新资源，避免误用CDN中还未失效的旧版本静态资源。（[19:20](https://youtu.be/KuClyhvSzXk?t=1160)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[cache-hit-cache-invalidation-terminology]]
- [[cdn-point-of-presence]]
%% ytkb:end %%
