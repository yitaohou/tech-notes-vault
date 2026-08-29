---
title: Authentication vs Authorization
aliases: []
tags:
- concept
summary: authentication 指是否拥有访问应用的资格，authorization 指是否拥有执行特定操作（如上传文件）的权限，二者含义不同但相关。
created: '2026-08-26'
updated: '2026-08-26'
---

# Authentication vs Authorization

%% ytkb:def %%
authentication 指是否拥有访问应用的资格，authorization 指是否拥有执行特定操作（如上传文件）的权限，二者含义不同但相关。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-authentication-authorization]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:Qa-7iWxDz1A %%
### 来自 [[2026-06-08-fundamentals-of-backend-architecture---how-to-desi]]
- authentication 回答「你是否有权访问这个应用」，authorization 回答「你是否有权限执行某个具体操作（如上传文件）」，两者可以放在同一服务实现，但概念上是不同的。（[24:05](https://youtu.be/Qa-7iWxDz1A?t=1445)）
%% ytkb:end %%

%% ytkb:video:oYxTTirKY8M %%
### 来自 [[2026-05-26-system-design-explained-apis-databases-caching-cdn]]
- Authentication 的作用是在系统能够做出任何授权或限制决策之前，先验证发起请求的用户（通过浏览器或移动端）或第三方服务的身份是否与其所声称的一致。（[81:20](https://youtu.be/oYxTTirKY8M?t=4880)）
- 身份认证（authentication）解决的是用户是谁、是否能登录系统的问题，是访问系统的第一步；授权（authorization）解决的是用户登录后能访问哪些资源、执行哪些操作的问题，发生在认证通过之后。（[1:42:29](https://youtu.be/oYxTTirKY8M?t=6149)）
- 系统处理请求时 authentication 发生在先，确认用户身份及是否有权访问系统；authorization 在下一步，决定该用户在系统内具体能执行哪些操作。（[1:45:30](https://youtu.be/oYxTTirKY8M?t=6330)）
- authorization 不仅像 authentication 一样负责放行用户进入系统，还进一步控制用户进入后能够访问哪些资源和操作。（[1:54:33](https://youtu.be/oYxTTirKY8M?t=6873)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[authorization-header-token-transport]]
- [[jwt-token-authentication]]
- [[role-based-access-control]]
- [[single-sign-on]]
%% ytkb:end %%
