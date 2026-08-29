---
title: User Existence Check Before Authentication
aliases: []
tags:
- concept
summary: 在颁发 token 之前，先调用用户服务确认该用户账户已存在于系统数据库中的校验步骤。
created: '2026-08-26'
updated: '2026-08-26'
---

# User Existence Check Before Authentication

%% ytkb:def %%
在颁发 token 之前，先调用用户服务确认该用户账户已存在于系统数据库中的校验步骤。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[backend-authentication-authorization]] · [[backend]]
%% ytkb:end %%

## 要点

%% ytkb:video:Qa-7iWxDz1A %%
### 来自 [[2026-06-08-fundamentals-of-backend-architecture---how-to-desi]]
- 签发 token 前，系统可能先调用独立的用户服务验证该用户是否已存在于数据库中，只有确认存在后才继续颁发 token；用户服务与认证服务是否合并部署取决于具体架构设计。（[24:05](https://youtu.be/Qa-7iWxDz1A?t=1445)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[authentication-service-login-flow]]
%% ytkb:end %%
