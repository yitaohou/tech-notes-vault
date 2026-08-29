---
title: Stateless Server + Database Decoupling
aliases: []
tags:
- concept
summary: 把服务器设计为无状态（stateless），将数据存储职责剥离给独立数据库层，从而实现数据持久化、不因服务器重启或宕机而丢失的架构模式。
created: '2026-08-26'
updated: '2026-08-26'
---

# Stateless Server + Database Decoupling

%% ytkb:def %%
把服务器设计为无状态（stateless），将数据存储职责剥离给独立数据库层，从而实现数据持久化、不因服务器重启或宕机而丢失的架构模式。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[backend-service-architecture-patterns]] · [[backend]]
%% ytkb:end %%

## 要点

%% ytkb:video:Qa-7iWxDz1A %%
### 来自 [[2026-06-08-fundamentals-of-backend-architecture---how-to-desi]]
- 解决服务器宕机丢数据问题的关键不只是简单地添加一个数据库，而是把服务器变成无状态（stateless），让它每次请求都从独立的数据库中读写数据。（[03:00](https://youtu.be/Qa-7iWxDz1A?t=180)）
- 引入数据库并将服务器改为无状态后，即使服务器实例发生故障，用户数据依然被安全持久化在数据库中，不会因服务器状态丢失。（[03:00](https://youtu.be/Qa-7iWxDz1A?t=180)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[single-point-of-failure]]
- [[stateful-server-data-coupling]]
%% ytkb:end %%
