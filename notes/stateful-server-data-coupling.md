---
title: Stateful Server Data Coupling
aliases: []
tags:
- concept
summary: 数据直接存储在服务器实例内部（而非独立存储层）的设计方式，服务器宕机会导致数据永久丢失。
created: '2026-08-26'
updated: '2026-08-26'
---

# Stateful Server Data Coupling

%% ytkb:def %%
数据直接存储在服务器实例内部（而非独立存储层）的设计方式，服务器宕机会导致数据永久丢失。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[backend-service-architecture-patterns]] · [[backend]]
%% ytkb:end %%

## 要点

%% ytkb:video:Qa-7iWxDz1A %%
### 来自 [[2026-06-08-fundamentals-of-backend-architecture---how-to-desi]]
- 最初版的简单架构中，数据（如文件 ID 到位置的映射）直接以内存结构耦合存放在服务器实例内部，一旦服务器崩溃数据就会丢失。（[03:00](https://youtu.be/Qa-7iWxDz1A?t=180)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[single-point-of-failure]]
- [[stateless-server-database-decoupling]]
%% ytkb:end %%
