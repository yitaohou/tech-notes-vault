---
title: Web Application Firewall (WAF)
aliases: []
tags:
- concept
summary: 部署在 API 与外部流量之间、充当守门人角色的防火墙，用于过滤具有已知攻击模式的恶意流量，同时放行正常请求。
created: '2026-08-26'
updated: '2026-08-26'
---

# Web Application Firewall (WAF)

%% ytkb:def %%
部署在 API 与外部流量之间、充当守门人角色的防火墙，用于过滤具有已知攻击模式的恶意流量，同时放行正常请求。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-api-gateway-security]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:oYxTTirKY8M %%
### 来自 [[2026-05-26-system-design-explained-apis-databases-caching-cdn]]
- 以 AWS WAF 为例，firewall 可以基于可疑 SQL 关键字、异常 HTTP 方法等已知攻击模式识别并拦截恶意请求，同时允许正常流量顺利到达 API。（[1:57:34](https://youtu.be/oYxTTirKY8M?t=7054)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[sql-injection-attack]]
%% ytkb:end %%
