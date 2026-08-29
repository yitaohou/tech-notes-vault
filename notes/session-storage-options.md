---
title: Session Storage Options
aliases: []
tags:
- concept
summary: 存储 session 数据可选用的几种方案，包括内存变量、Redis、SQL 数据库和文件系统，各自在持久性和可扩展性上存在权衡。
created: '2026-08-26'
updated: '2026-08-26'
---

# Session Storage Options

%% ytkb:def %%
存储 session 数据可选用的几种方案，包括内存变量、Redis、SQL 数据库和文件系统，各自在持久性和可扩展性上存在权衡。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[backend-authentication-authorization]] · [[backend]]
%% ytkb:end %%

## 要点

%% ytkb:video:oYxTTirKY8M %%
### 来自 [[2026-05-26-system-design-explained-apis-databases-caching-cdn]]
- session storage 可以简单地用内存变量实现，但服务器重启或崩溃后数据会丢失；也可以用 Redis 或 SQL 数据库持久化存储；用服务器本地文件系统存储的方式非常少见，且不具备可扩展性。（[90:23](https://youtu.be/oYxTTirKY8M?t=5423)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[redis-in-ram-key-value-cache]]
- [[session-based-authentication]]
%% ytkb:end %%
