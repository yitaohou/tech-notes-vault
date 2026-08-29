---
title: Data Synchronization Problem When Scaling
aliases: []
tags:
- concept
summary: 多台服务器各自持有本地数据副本时，用户写入某一台服务器的数据不会被其他服务器感知，从而产生数据不同步问题。
created: '2026-08-26'
updated: '2026-08-26'
---

# Data Synchronization Problem When Scaling

%% ytkb:def %%
多台服务器各自持有本地数据副本时，用户写入某一台服务器的数据不会被其他服务器感知，从而产生数据不同步问题。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[backend-service-architecture-patterns]] · [[backend]]
%% ytkb:end %%

## 要点

%% ytkb:video:Qa-7iWxDz1A %%
### 来自 [[2026-06-08-fundamentals-of-backend-architecture---how-to-desi]]
- 用户向服务器A写入数据后，该数据只存在于服务器A本地，服务器B完全不知道这次写入，导致不同实例间数据不一致。（[06:01](https://youtu.be/Qa-7iWxDz1A?t=361)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[data-coupled-server-scaling-problem]]
- [[decoupled-database-architecture]]
%% ytkb:end %%
