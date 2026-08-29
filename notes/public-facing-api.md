---
title: Public-Facing API
aliases: []
tags:
- concept
summary: 允许来自互联网任意用户发起请求的 API，与仅限 VPN 内部访问的 API 相对。
created: '2026-08-26'
updated: '2026-08-26'
---

# Public-Facing API

%% ytkb:def %%
允许来自互联网任意用户发起请求的 API，与仅限 VPN 内部访问的 API 相对。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-api-gateway-security]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:oYxTTirKY8M %%
### 来自 [[2026-05-26-system-design-explained-apis-databases-caching-cdn]]
- public facing API 允许来自互联网的任意用户请求，而 VPN 内部 API 只允许同一网络内的调用方通过检查并到达。（[2:00:34](https://youtu.be/oYxTTirKY8M?t=7234)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[vpn-api-access-restriction]]
%% ytkb:end %%
