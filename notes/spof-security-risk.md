---
title: SPOF Security Risk
aliases: []
tags:
- concept
summary: 单点故障组件（如 load balancer）容易成为攻击目标，攻击者通过发送海量流量使其失效即可拖垮整个系统。
created: '2026-08-26'
updated: '2026-08-26'
---

# SPOF Security Risk

%% ytkb:def %%
单点故障组件（如 load balancer）容易成为攻击目标，攻击者通过发送海量流量使其失效即可拖垮整个系统。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-api-gateway-security]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:oYxTTirKY8M %%
### 来自 [[2026-05-26-system-design-explained-apis-databases-caching-cdn]]
- 单点故障也是安全隐患：攻击者可以针对该单点（如 load balancer）发送大量流量，一旦其失效，整个系统随之瘫痪。（[27:03](https://youtu.be/oYxTTirKY8M?t=1623)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[rate-limiting]]
- [[single-point-of-failure]]
%% ytkb:end %%
