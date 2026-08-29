---
title: Role-Based Access Control (RBAC)
aliases: []
tags:
- concept
summary: 根据用户被分配的角色（如 admin、editor、viewer）来决定其在系统中可执行操作范围的权限管理模型。
created: '2026-08-26'
updated: '2026-08-26'
---

# Role-Based Access Control (RBAC)

%% ytkb:def %%
根据用户被分配的角色（如 admin、editor、viewer）来决定其在系统中可执行操作范围的权限管理模型。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[backend-authentication-authorization]] · [[backend]]
%% ytkb:end %%

## 要点

%% ytkb:video:oYxTTirKY8M %%
### 来自 [[2026-05-26-system-design-explained-apis-databases-caching-cdn]]
- 在 RBAC 中，editor 角色权限通常略低于 admin：可以创建、读取和更新内容，但不能删除资源，也不能管理其他用户。（[1:48:30](https://youtu.be/oYxTTirKY8M?t=6510)）
- viewer 角色是 RBAC 中权限最低的角色，只能读取资源和内容，不能更新或创建任何数据。（[1:48:45](https://youtu.be/oYxTTirKY8M?t=6525)）
- RBAC 是最常见的授权模型，被 GitHub、Stripe dashboard、CMS 工具、团队管理工具等日常应用广泛采用。（[1:49:00](https://youtu.be/oYxTTirKY8M?t=6540)）
- RBAC 是三种主流 authorization 模型中使用最广泛的一种，通过将用户分配到诸如 admin、editor、read-only 这样的角色来统一管理权限。（[1:45:30](https://youtu.be/oYxTTirKY8M?t=6330)）
- RBAC 中的 admin 角色通常拥有对所有资源的完全访问权限，包括创建、读取、更新、删除资源，以及管理其他用户的角色分配。（[1:45:30](https://youtu.be/oYxTTirKY8M?t=6330)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[access-control-list]]
- [[attribute-based-access-control]]
- [[github-repo-access-permission-tiers]]
%% ytkb:end %%
