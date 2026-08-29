---
title: SQL/NoSQL Injection Attack
aliases: []
tags:
- concept
summary: 一类注入攻击，指当用户输入被直接拼接进数据库查询语句时，攻击者可以构造恶意输入绕过校验逻辑，进而读取、篡改或删除数据库中的数据。
created: '2026-08-26'
updated: '2026-08-26'
---

# SQL/NoSQL Injection Attack

%% ytkb:def %%
一类注入攻击，指当用户输入被直接拼接进数据库查询语句时，攻击者可以构造恶意输入绕过校验逻辑，进而读取、篡改或删除数据库中的数据。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[backend-security]] · [[backend]]
%% ytkb:end %%

## 要点

%% ytkb:video:oYxTTirKY8M %%
### 来自 [[2026-05-26-system-design-explained-apis-databases-caching-cdn]]
- SQL/NoSQL injection 的风险在于攻击者构造的输入能完全绕过应用原本的校验逻辑，直接对数据库执行任意读取、修改或删除操作，甚至删除全部用户数据和其他数据表。（[1:57:34](https://youtu.be/oYxTTirKY8M?t=7054)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[parameterized-queries-orm-defense]]
%% ytkb:end %%
