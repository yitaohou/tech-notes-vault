---
title: 关系型数据库与 NoSQL 的选择经验法则
aliases: []
tags:
- concept
summary: 根据数据实体间是否存在明显关系及是否需要 join 多表，来决定使用关系型数据库还是 NoSQL 的判断准则。
created: '2026-08-26'
updated: '2026-08-26'
---

# 关系型数据库与 NoSQL 的选择经验法则

%% ytkb:def %%
根据数据实体间是否存在明显关系及是否需要 join 多表，来决定使用关系型数据库还是 NoSQL 的判断准则。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-data-architecture]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:QBHTbtWSECg %%
### 来自 [[2026-03-15-system-design-mock-interview-design-leetcode-ft-ex]]
- 选择关系型数据库（RDBMS）而非 NoSQL 的经验法则是：当数据实体间存在明显的 relations、或确定需要 join 多张表查询时才使用关系型数据库，否则 NoSQL 更合适。（[21:07](https://youtu.be/QBHTbtWSECg?t=1267)）
%% ytkb:end %%

%% ytkb:video:oYxTTirKY8M %%
### 来自 [[2026-05-26-system-design-explained-apis-databases-caching-cdn]]
- 如果应用数据结构清晰、实体间存在明确关系（例如电商应用中追踪 customer 和 order），适合使用 SQL 数据库。（[11:05](https://youtu.be/oYxTTirKY8M?t=665)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[dynamodb]]
- [[dynamodb-choice-for-schema-flexibility]]
- [[nosql-database-types]]
- [[sql-nosql-feature-convergence]]
%% ytkb:end %%
