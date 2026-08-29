---
title: CDN Point of Presence
aliases: []
tags:
- concept
summary: CDN 由分布在全球各地的大量小型服务器节点（point of presence, PoP）组成，用于就近响应用户请求。
created: '2026-08-26'
updated: '2026-08-26'
---

# CDN Point of Presence

%% ytkb:def %%
CDN 由分布在全球各地的大量小型服务器节点（point of presence, PoP）组成，用于就近响应用户请求。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-caching-edge]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:Qa-7iWxDz1A %%
### 来自 [[2026-06-08-fundamentals-of-backend-architecture---how-to-desi]]
- CDN 提供商的优势在于其在全球拥有众多 PoP 节点，用户发起请求时可以直接命中离自己最近的 CDN 节点，而不必先访问源服务器。（[42:09](https://youtu.be/Qa-7iWxDz1A?t=2529)）
%% ytkb:end %%

%% ytkb:video:KuClyhvSzXk %%
### 来自 [[2026-06-18-frontend-system-design-explained-w-senior-engineer]]
- CDN通过在全球部署大量edge location（PoP）服务器，把静态资源提前推送到这些节点；用户发起请求时会被重定向到离自己最近的edge location，从而缩短物理距离、降低延迟。（[18:20](https://youtu.be/KuClyhvSzXk?t=1100)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[cdn-edge-asset-caching]]
- [[cdn-origin-bypass]]
- [[geographic-latency-example]]
%% ytkb:end %%
