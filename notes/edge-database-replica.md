---
title: Edge Database Replica
aliases: []
tags:
- concept
summary: 为配合边缘计算架构，把数据库的只读副本也部署到靠近用户的边缘位置，使数据访问同样具备低延迟特性。
created: '2026-08-26'
updated: '2026-08-26'
---

# Edge Database Replica

%% ytkb:def %%
为配合边缘计算架构，把数据库的只读副本也部署到靠近用户的边缘位置，使数据访问同样具备低延迟特性。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-caching-edge]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:AMerB8XjfZ0 %%
### 来自 [[2026-06-30-top-15-frontend-interview-questions-for-2026-wa-se]]
- 一旦后端被分布式部署到边缘 worker，数据库也必须随之下沉到边缘，通常做法是通过 Prisma 等服务提供的分布式只读数据库副本，把数据放在靠近用户的位置。（[45:09](https://youtu.be/AMerB8XjfZ0?t=2709)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[edge-architecture-write-consistency-tradeoff]]
- [[edge-computing-ssr]]
%% ytkb:end %%
