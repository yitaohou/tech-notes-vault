---
title: ACID Transactions
aliases: []
tags:
- concept
summary: 关系型数据库事务应具备的四个特性：atomicity（原子性）、consistency（一致性）、isolation（隔离性）、durability（持久性）。
created: '2026-08-26'
updated: '2026-08-26'
---

# ACID Transactions

%% ytkb:def %%
关系型数据库事务应具备的四个特性：atomicity（原子性）、consistency（一致性）、isolation（隔离性）、durability（持久性）。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[backend-databases]] · [[backend]]
%% ytkb:end %%

## 要点

%% ytkb:video:oYxTTirKY8M %%
### 来自 [[2026-05-26-system-design-explained-apis-databases-caching-cdn]]
- ACID 事务的 atomicity 指整个事务被当作单一单元处理，要么完全成功，要么完全失败。（[09:00](https://youtu.be/oYxTTirKY8M?t=540)）
- ACID 事务的 consistency 指事务执行后会把数据库从一个有效状态转换为另一个有效状态。（[09:00](https://youtu.be/oYxTTirKY8M?t=540)）
- ACID 事务的 isolation 指并发事务所做的修改彼此隔离，不会互相干扰。（[09:00](https://youtu.be/oYxTTirKY8M?t=540)）
- ACID 事务的 durability 指即使系统或数据库服务器发生故障，已提交的数据依然会被保留。（[09:00](https://youtu.be/oYxTTirKY8M?t=540)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[nosql-database-types]]
%% ytkb:end %%
