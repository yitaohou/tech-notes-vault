---
title: VPN-Restricted API Access
aliases: []
tags:
- concept
summary: 把某些 API 部署在 VPN（virtual private network）网络内，只有同样处于该网络中的客户端才能访问，网络外的请求会被直接拦截。
created: '2026-08-26'
updated: '2026-08-26'
---

# VPN-Restricted API Access

%% ytkb:def %%
把某些 API 部署在 VPN（virtual private network）网络内，只有同样处于该网络中的客户端才能访问，网络外的请求会被直接拦截。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-api-gateway-security]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:oYxTTirKY8M %%
### 来自 [[2026-05-26-system-design-explained-apis-databases-caching-cdn]]
- VPN 网络内的 API 只能被同处该网络的调用方访问，来自公网、不在该网络内的用户请求会被直接拦截。（[2:00:34](https://youtu.be/oYxTTirKY8M?t=7234)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[public-facing-api]]
- [[vpc-private-network-isolation]]
%% ytkb:end %%
