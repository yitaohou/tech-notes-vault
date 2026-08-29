---
title: Rate Limiting Per User/IP
aliases: []
tags:
- concept
summary: 根据具体用户账号或 IP 地址分别统计并限制请求次数的 rate limiting 设置方式。
created: '2026-08-26'
updated: '2026-08-26'
---

# Rate Limiting Per User/IP

%% ytkb:def %%
根据具体用户账号或 IP 地址分别统计并限制请求次数的 rate limiting 设置方式。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-api-gateway-security]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:oYxTTirKY8M %%
### 来自 [[2026-05-26-system-design-explained-apis-databases-caching-cdn]]
- rate limiting 也可以按用户或 IP 地址粒度设置，一旦某个 IP 的请求次数超过限额（如第101次请求），该 IP 就会被封锁。（[1:54:33](https://youtu.be/oYxTTirKY8M?t=6873)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[rate-limiting]]
- [[rate-limiting-per-endpoint]]
%% ytkb:end %%
