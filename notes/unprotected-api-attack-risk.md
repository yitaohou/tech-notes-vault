---
title: Unprotected API Attack Risk
aliases: []
tags:
- concept
summary: API 若未设置 rate limiting 等防护机制，攻击者可以短时间内发送海量请求压垮系统（造成类似 DoS 的效果）或用于暴力破解用户数据。
created: '2026-08-26'
updated: '2026-08-26'
---

# Unprotected API Attack Risk

%% ytkb:def %%
API 若未设置 rate limiting 等防护机制，攻击者可以短时间内发送海量请求压垮系统（造成类似 DoS 的效果）或用于暴力破解用户数据。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-api-gateway-security]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:oYxTTirKY8M %%
### 来自 [[2026-05-26-system-design-explained-apis-databases-caching-cdn]]
- 若不对 API 设置 rate limiting，攻击者可以每分钟发送数千请求压垮系统，或借此对数据进行暴力破解。（[1:54:33](https://youtu.be/oYxTTirKY8M?t=6873)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[rate-limiting]]
%% ytkb:end %%
