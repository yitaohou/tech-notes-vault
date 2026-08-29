---
title: NoSQL Schema Flexibility Advantage
aliases: []
tags:
- concept
summary: 指 NoSQL 数据库能够把关联数据（如用户、订单、产品）嵌套存储在单个文档中，从而处理高度动态和大规模的数据集，并针对低延迟和可扩展性做了优化。
created: '2026-08-26'
updated: '2026-08-26'
---

# NoSQL Schema Flexibility Advantage

%% ytkb:def %%
指 NoSQL 数据库能够把关联数据（如用户、订单、产品）嵌套存储在单个文档中，从而处理高度动态和大规模的数据集，并针对低延迟和可扩展性做了优化。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-data-architecture]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:oYxTTirKY8M %%
### 来自 [[2026-05-26-system-design-explained-apis-databases-caching-cdn]]
- 以 customer、order、product 场景为例，MongoDB 可以把用户数据、订单和产品信息全部存储在单个文档中，无需像关系型数据库那样通过 join 组合多张表。（[10:42](https://youtu.be/oYxTTirKY8M?t=642)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[document-store-database]]
%% ytkb:end %%
