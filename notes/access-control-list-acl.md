---
title: Access Control List (ACL)
aliases: []
tags:
- concept
summary: 一种细粒度授权模型，可以针对单个资源为每个用户或对象单独设置访问权限，而非按角色统一授权。
created: '2026-08-26'
updated: '2026-08-26'
---

# Access Control List (ACL)

%% ytkb:def %%
一种细粒度授权模型，可以针对单个资源为每个用户或对象单独设置访问权限，而非按角色统一授权。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-authentication-authorization]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:oYxTTirKY8M %%
### 来自 [[2026-05-26-system-design-explained-apis-databases-caching-cdn]]
- ACL（access control list）允许为具体资源（如某一份文档）单独设置每个用户的访问权限，而不是像 RBAC 那样按角色统一授权。（[1:51:32](https://youtu.be/oYxTTirKY8M?t=6692)）
- Google Drive/Google Docs 是 ACL 的典型应用：可以把一份文档分享给某人并只给只读权限，再分享给另一人并允许其编辑和添加评论。（[1:51:32](https://youtu.be/oYxTTirKY8M?t=6692)）
- ACL 能对资源提供更精细的权限控制，但当用户或对象数量达到百万级时管理和扩展难度较大；不过 Google Drive 在文档、表格等产品上的实践证明这种规模下依然可行。（[1:51:32](https://youtu.be/oYxTTirKY8M?t=6692)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[authentication-vs-authorization]]
%% ytkb:end %%
