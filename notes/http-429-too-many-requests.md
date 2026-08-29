---
title: HTTP 429 Too Many Requests
aliases: []
tags:
- concept
summary: HTTP 429 状态码表示客户端因请求过于频繁而被限流拒绝。
created: '2026-08-26'
updated: '2026-08-26'
---

# HTTP 429 Too Many Requests

%% ytkb:def %%
HTTP 429 状态码表示客户端因请求过于频繁而被限流拒绝。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[backend-api-design]] · [[backend]]
%% ytkb:end %%

## 要点

%% ytkb:video:Qa-7iWxDz1A %%
### 来自 [[2026-06-08-fundamentals-of-backend-architecture---how-to-desi]]
- 当用户请求次数超过设定阈值（例如达到10次）时，服务器会返回 HTTP 429 状态码，告知客户端已被 rate limited。（[45:11](https://youtu.be/Qa-7iWxDz1A?t=2711)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[rate-limiting]]
%% ytkb:end %%
