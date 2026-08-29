---
title: API Versioning
aliases: []
tags:
- concept
summary: 在 REST API URL 中加入版本前缀（如 /api/v1、/api/v2）以便迭代新功能时不破坏仍在使用旧版本的客户端。
created: '2026-08-26'
updated: '2026-08-26'
---

# API Versioning

%% ytkb:def %%
在 REST API URL 中加入版本前缀（如 /api/v1、/api/v2）以便迭代新功能时不破坏仍在使用旧版本的客户端。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-api-design]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:oYxTTirKY8M %%
### 来自 [[2026-05-26-system-design-explained-apis-databases-caching-cdn]]
- REST API 请求通常带有 /api/v1、/api/v2 这样的版本前缀；当未来迁移 API 并在新版本中引入可能破坏旧功能的改动时，仍在使用旧版本号的前端不会受到影响，可以继续使用旧版本的功能。（[76:25](https://youtu.be/oYxTTirKY8M?t=4585)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[restful-api-design]]
%% ytkb:end %%
