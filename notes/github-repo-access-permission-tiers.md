---
title: GitHub Repository Permission Tiers Example
aliases: []
tags:
- concept
summary: 以 GitHub 仓库访问权限为例，说明同一系统中不同用户可被授予不同层级的访问权限，是 RBAC 思路的实际应用场景。
created: '2026-08-26'
updated: '2026-08-26'
---

# GitHub Repository Permission Tiers Example

%% ytkb:def %%
以 GitHub 仓库访问权限为例，说明同一系统中不同用户可被授予不同层级的访问权限，是 RBAC 思路的实际应用场景。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[backend-authentication-authorization]] · [[backend]]
%% ytkb:end %%

## 要点

%% ytkb:video:oYxTTirKY8M %%
### 来自 [[2026-05-26-system-design-explained-apis-databases-caching-cdn]]
- 在 GitHub 仓库权限设计中，write access 用户只能 push 代码，read access 用户只能查看仓库但不能 push 或创建 pull request，admin 用户则拥有包括删除仓库在内的完全控制权。（[1:45:30](https://youtu.be/oYxTTirKY8M?t=6330)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[role-based-access-control]]
%% ytkb:end %%
