---
title: VPN for Private API Access
aliases: []
tags:
- concept
summary: 通过 VPN 限制某些私有 API 只能从特定网络内被访问，作为额外的网络层安全控制手段。
created: '2026-08-26'
updated: '2026-08-26'
---

# VPN for Private API Access

%% ytkb:def %%
通过 VPN 限制某些私有 API 只能从特定网络内被访问，作为额外的网络层安全控制手段。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-api-gateway-security]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:oYxTTirKY8M %%
### 来自 [[2026-05-26-system-design-explained-apis-databases-caching-cdn]]
- 对于只应被特定网络访问的私有 API，可以使用 VPN 来限制其可访问范围，而非直接对公网开放。（[1:57:34](https://youtu.be/oYxTTirKY8M?t=7054)）
%% ytkb:end %%
