---
title: SQL Join Operation
aliases: []
tags:
- concept
summary: 把两个或多个表按关联字段合并成一张新表的 SQL 操作，例如将 customers 表和 products 表连接成同时包含双方 ID 信息的 orders
  表。
created: '2026-08-26'
updated: '2026-08-26'
---

# SQL Join Operation

%% ytkb:def %%
把两个或多个表按关联字段合并成一张新表的 SQL 操作，例如将 customers 表和 products 表连接成同时包含双方 ID 信息的 orders 表。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[backend-databases]] · [[backend]]
%% ytkb:end %%

## 要点

%% ytkb:video:oYxTTirKY8M %%
### 来自 [[2026-05-26-system-design-explained-apis-databases-caching-cdn]]
- SQL 支持跨多张表的复杂 join 操作，例如把 customers 表和 products 表连接（join）成一张 orders 表，用于记录哪个客户订购了哪些产品。（[06:00](https://youtu.be/oYxTTirKY8M?t=360)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[relational-database-rdbms]]
- [[relational-vs-nosql-selection-heuristic]]
- [[sql-table-structure]]
%% ytkb:end %%
