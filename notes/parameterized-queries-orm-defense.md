---
title: Parameterized Queries / ORM Safeguards
aliases: []
tags:
- concept
summary: 通过使用参数化查询或 ORM 框架自带的防护机制，避免用户输入被直接拼接进 SQL 语句，从而防御注入攻击。
created: '2026-08-26'
updated: '2026-08-26'
---

# Parameterized Queries / ORM Safeguards

%% ytkb:def %%
通过使用参数化查询或 ORM 框架自带的防护机制，避免用户输入被直接拼接进 SQL 语句，从而防御注入攻击。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[backend-security]] · [[backend]]
%% ytkb:end %%

## 要点

%% ytkb:video:oYxTTirKY8M %%
### 来自 [[2026-05-26-system-design-explained-apis-databases-caching-cdn]]
- 防御 SQL/NoSQL injection 的标准做法是始终使用参数化查询（parameterized queries）或依赖 ORM 提供的安全防护，而不是直接把用户输入拼接进查询字符串。（[1:57:34](https://youtu.be/oYxTTirKY8M?t=7054)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[sql-injection-attack]]
%% ytkb:end %%
