---
title: Data Coupled to Server Instance Scaling Problem
aliases: []
tags:
- concept
summary: 若数据与服务器实例本地耦合，横向扩展出多个服务器实例时会导致同一份数据在各实例间重复存储的问题。
created: '2026-08-26'
updated: '2026-08-26'
---

# Data Coupled to Server Instance Scaling Problem

%% ytkb:def %%
若数据与服务器实例本地耦合，横向扩展出多个服务器实例时会导致同一份数据在各实例间重复存储的问题。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[backend-service-architecture-patterns]] · [[backend]]
%% ytkb:end %%

## 要点

%% ytkb:video:Qa-7iWxDz1A %%
### 来自 [[2026-06-08-fundamentals-of-backend-architecture---how-to-desi]]
- 如果数据和服务器实例绑定在一起，扩展成两台服务器后，数据会在两边各自保留一份，形成数据重复。（[06:01](https://youtu.be/Qa-7iWxDz1A?t=361)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[data-synchronization-problem-scaling]]
- [[decoupled-database-architecture]]
%% ytkb:end %%
