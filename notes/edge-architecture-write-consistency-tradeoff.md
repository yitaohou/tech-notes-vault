---
title: Edge Architecture Write/Consistency Tradeoff
aliases: []
tags:
- concept
summary: 在边缘分布式架构中，写操作仍必须指向中心主数据库，写入需要一定时间传播到各边缘只读副本，因此只能获得 eventual consistency 而非强一致性。
created: '2026-08-26'
updated: '2026-08-26'
---

# Edge Architecture Write/Consistency Tradeoff

%% ytkb:def %%
在边缘分布式架构中，写操作仍必须指向中心主数据库，写入需要一定时间传播到各边缘只读副本，因此只能获得 eventual consistency 而非强一致性。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-caching-edge]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:AMerB8XjfZ0 %%
### 来自 [[2026-06-30-top-15-frontend-interview-questions-for-2026-wa-se]]
- 边缘架构中只有一个主版本数据库负责实际写入，所有写操作都要回到这个主 DB；写操作因此成本更高，且写入的数据需要传播到各只读副本，导致只能实现 eventual consistency。（[45:09](https://youtu.be/AMerB8XjfZ0?t=2709)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[cap-theorem]]
- [[edge-database-replica]]
%% ytkb:end %%
