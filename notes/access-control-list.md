---
title: Access Control List (ACL)
aliases: []
tags:
- concept
summary: 针对具体资源（如某个文档）维护一份用户权限清单、逐一指定各用户可执行操作的授权模型。
created: '2026-08-26'
updated: '2026-08-26'
---

# Access Control List (ACL)

%% ytkb:def %%
针对具体资源（如某个文档）维护一份用户权限清单、逐一指定各用户可执行操作的授权模型。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-authentication-authorization]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:oYxTTirKY8M %%
### 来自 [[2026-05-26-system-design-explained-apis-databases-caching-cdn]]
- ACL 为特定资源（如一份文档）单独维护权限列表，明确记录哪些用户拥有访问权、以及各自具体拥有读或写等哪些权限。（[1:50:20](https://youtu.be/oYxTTirKY8M?t=6620)）
- ACL 需要同时管理两件事：哪些用户被允许访问该资源，以及每个用户具体拥有什么权限（如只读、读写或无权限）。（[1:50:35](https://youtu.be/oYxTTirKY8M?t=6635)）
- ACL 高度具体且以用户为中心（user-centric），因此在拥有数百万用户的系统中很难良好扩展。（[1:50:50](https://youtu.be/oYxTTirKY8M?t=6650)）
- ACL 让每个资源都拥有自己独立的权限列表，用于决定谁能访问该资源及能做什么，Google Docs 的权限管理就是典型例子。（[1:45:30](https://youtu.be/oYxTTirKY8M?t=6330)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[attribute-based-access-control]]
- [[role-based-access-control]]
%% ytkb:end %%
