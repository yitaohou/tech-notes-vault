---
title: Overall (Global) Rate Limiting for DDoS Protection
aliases: []
tags:
- concept
summary: 除针对单个用户/IP 的限流外，额外设置一个数值更大的全局请求量阈值，用于防御由大量 bot 发起的分布式流量攻击。
created: '2026-08-26'
updated: '2026-08-26'
---

# Overall (Global) Rate Limiting for DDoS Protection

%% ytkb:def %%
除针对单个用户/IP 的限流外，额外设置一个数值更大的全局请求量阈值，用于防御由大量 bot 发起的分布式流量攻击。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-api-gateway-security]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:oYxTTirKY8M %%
### 来自 [[2026-05-26-system-design-explained-apis-databases-caching-cdn]]
- 当进入服务器的总流量超过预设的全局阈值时，系统会临时封锁所有请求，直到定位到问题根源为止。（[1:57:34](https://youtu.be/oYxTTirKY8M?t=7054)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[ddos-botnet-rate-limit-bypass]]
- [[rate-limiting]]
%% ytkb:end %%
