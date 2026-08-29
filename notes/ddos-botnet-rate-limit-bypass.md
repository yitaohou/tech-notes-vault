---
title: DDoS Botnet Rate Limit Bypass
aliases: []
tags:
- concept
summary: 攻击者通过控制大量分散的 bot，使每个 bot 的请求量保持在单个 IP 的 rate limit 阈值以下，从而绕过针对单一用户/IP 的限流规则、实现事实上的
  DDoS 攻击。
created: '2026-08-26'
updated: '2026-08-26'
---

# DDoS Botnet Rate Limit Bypass

%% ytkb:def %%
攻击者通过控制大量分散的 bot，使每个 bot 的请求量保持在单个 IP 的 rate limit 阈值以下，从而绕过针对单一用户/IP 的限流规则、实现事实上的 DDoS 攻击。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[backend-security]] · [[backend]]
%% ytkb:end %%

## 要点

%% ytkb:video:oYxTTirKY8M %%
### 来自 [[2026-05-26-system-design-explained-apis-databases-caching-cdn]]
- 即使对每个用户或 IP 设置了 rate limit（例如每 IP 100 次请求），攻击者仍可通过启动大量 bot、让每个 bot 各自把请求量控制在限额之内，从而使总请求量远超系统承载能力。（[1:57:34](https://youtu.be/oYxTTirKY8M?t=7054)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[overall-rate-limiting-ddos-protection]]
- [[rate-limiting]]
%% ytkb:end %%
