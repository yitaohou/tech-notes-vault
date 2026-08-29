---
title: API Gateway HTTPS/HTTP Boundary
aliases: []
tags:
- concept
summary: 客户端与 API gateway 之间使用 HTTPS 保证安全，而 API gateway 与内部微服务之间由于处于封闭安全环境中，可改用性能更好的
  HTTP。
created: '2026-08-26'
updated: '2026-08-26'
---

# API Gateway HTTPS/HTTP Boundary

%% ytkb:def %%
客户端与 API gateway 之间使用 HTTPS 保证安全，而 API gateway 与内部微服务之间由于处于封闭安全环境中，可改用性能更好的 HTTP。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-api-gateway-security]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:KuClyhvSzXk %%
### 来自 [[2026-06-18-frontend-system-design-explained-w-senior-engineer]]
- 客户端到 API gateway 用 HTTPS，gateway 到微服务之间用 HTTP，因为内部环境已是封闭网络、不再需要额外的传输安全保障，从而提升整体性能。（[09:03](https://youtu.be/KuClyhvSzXk?t=543)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[api-gateway]]
- [[https-handshake-performance-cost]]
- [[vpc-private-network-isolation]]
%% ytkb:end %%
