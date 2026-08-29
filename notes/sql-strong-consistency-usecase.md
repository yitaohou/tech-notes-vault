---
title: SQL Database Strong Consistency Use Case
aliases: []
tags:
- concept
summary: 指当应用需要强一致性（strong consistency）与事务完整性时，应优先选择关系型（SQL）数据库的选型准则，例如金融或银行系统。
created: '2026-08-26'
updated: '2026-08-26'
---

# SQL Database Strong Consistency Use Case

%% ytkb:def %%
指当应用需要强一致性（strong consistency）与事务完整性时，应优先选择关系型（SQL）数据库的选型准则，例如金融或银行系统。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-data-architecture]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:oYxTTirKY8M %%
### 来自 [[2026-05-26-system-design-explained-apis-databases-caching-cdn]]
- 金融应用或银行系统这类需要strong consistency和事务完整性（transactional integrity）的场景，应该使用SQL数据库。（[12:00](https://youtu.be/oYxTTirKY8M?t=720)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[cap-theorem]]
- [[relational-vs-nosql-selection-heuristic]]
%% ytkb:end %%
