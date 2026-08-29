---
title: API Naming Convention Consistency
aliases: []
tags:
- concept
summary: 指API设计中同一套接口应统一采用同一种命名风格（如统一 camelCase 或统一 snake_case），避免混用导致不一致的原则。
created: '2026-08-26'
updated: '2026-08-26'
---

# API Naming Convention Consistency

%% ytkb:def %%
指API设计中同一套接口应统一采用同一种命名风格（如统一 camelCase 或统一 snake_case），避免混用导致不一致的原则。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[backend-api-design]] · [[backend]]
%% ytkb:end %%

## 要点

%% ytkb:video:oYxTTirKY8M %%
### 来自 [[2026-05-26-system-design-explained-apis-databases-caching-cdn]]
- 同一套 API 中所有端点应统一使用同一种命名规范，例如不能一个端点用 camelCase（如 userDetails），另一个端点又用 snake_case（如 user/details），否则会破坏一致性。（[39:07](https://youtu.be/oYxTTirKY8M?t=2347)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[restful-api-design]]
%% ytkb:end %%
