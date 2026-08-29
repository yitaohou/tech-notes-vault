---
title: Master-Slave Database Replication
aliases: []
tags:
- concept
summary: 数据库采用主从（master-slave）架构，主库处理写入，从库（副本）同步数据，用于提升可用性与扩展性。
created: '2026-08-26'
updated: '2026-08-26'
---

# Master-Slave Database Replication

%% ytkb:def %%
数据库采用主从（master-slave）架构，主库处理写入，从库（副本）同步数据，用于提升可用性与扩展性。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-caching-edge]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:QBHTbtWSECg %%
### 来自 [[2026-03-15-system-design-mock-interview-design-leetcode-ft-ex]]
- 采用 master-slave 架构的数据库中，若主库（primary）宕机，可以将某个从库（replica）提升为新的主库，从而避免单点故障（single point of failure）。（[45:13](https://youtu.be/QBHTbtWSECg?t=2713)）
- master-slave 数据库架构除了提升容错能力外，也是数据库水平扩展（scaling）的常见解决方案之一。（[45:13](https://youtu.be/QBHTbtWSECg?t=2713)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[database-scaling-selective-replication]]
%% ytkb:end %%
