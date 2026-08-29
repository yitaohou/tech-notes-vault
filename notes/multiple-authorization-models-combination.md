---
title: Combining Multiple Authorization Models
aliases: []
tags:
- concept
summary: 生产系统常常同时组合RBAC、ABAC、ACL等多种authorization模型，以获得更复杂、更安全的访问控制体系，而非仅依赖单一模型。
created: '2026-08-26'
updated: '2026-08-26'
---

# Combining Multiple Authorization Models

%% ytkb:def %%
生产系统常常同时组合RBAC、ABAC、ACL等多种authorization模型，以获得更复杂、更安全的访问控制体系，而非仅依赖单一模型。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-authentication-authorization]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:oYxTTirKY8M %%
### 来自 [[2026-05-26-system-design-explained-apis-databases-caching-cdn]]
- 各authorization模型各有取舍，实际系统往往会把 RBAC、ABAC、ACL 等多种模型组合使用，以满足具体安全需求，而非只采用单一模型。（[1:45:30](https://youtu.be/oYxTTirKY8M?t=6330)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[access-control-list]]
- [[attribute-based-access-control]]
- [[role-based-access-control]]
%% ytkb:end %%
