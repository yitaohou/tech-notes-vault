---
title: HTTPS Handshake Performance Cost
aliases: []
tags:
- concept
summary: HTTPS 相较 HTTP 需要额外的握手往返（round trip）来建立加密连接，因此性能开销更高。
created: '2026-08-26'
updated: '2026-08-26'
---

# HTTPS Handshake Performance Cost

%% ytkb:def %%
HTTPS 相较 HTTP 需要额外的握手往返（round trip）来建立加密连接，因此性能开销更高。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[backend-networking-protocols]] · [[backend]]
%% ytkb:end %%

## 要点

%% ytkb:video:KuClyhvSzXk %%
### 来自 [[2026-06-18-frontend-system-design-explained-w-senior-engineer]]
- HTTPS 通常比 HTTP 性能差，因为需要更多的 round trip 来完成 handshake，这是内部微服务间通信改用 HTTP 的直接原因。（[09:03](https://youtu.be/KuClyhvSzXk?t=543)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[api-gateway-https-http-boundary]]
%% ytkb:end %%
