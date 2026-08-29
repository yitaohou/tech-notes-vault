---
title: CDN Edge Asset Caching
aliases: []
tags:
- concept
summary: CDN（内容分发网络）部署在系统集群之外的边缘位置，本质上也是一种缓存，专门用于高效缓存图片、视频等大体积静态资产。
created: '2026-08-26'
updated: '2026-08-26'
---

# CDN Edge Asset Caching

%% ytkb:def %%
CDN（内容分发网络）部署在系统集群之外的边缘位置，本质上也是一种缓存，专门用于高效缓存图片、视频等大体积静态资产。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-caching-edge]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:Qa-7iWxDz1A %%
### 来自 [[2026-06-08-fundamentals-of-backend-architecture---how-to-desi]]
- CDN 部署在集群外部的网络边缘（edge），本质上也是一种缓存，但特别适合用来缓存图片、视频这类体积较大的资产，弥补 Redis 无法胜任大文件缓存的短板。（[39:09](https://youtu.be/Qa-7iWxDz1A?t=2349)）
%% ytkb:end %%

%% ytkb:video:KuClyhvSzXk %%
### 来自 [[2026-06-18-frontend-system-design-explained-w-senior-engineer]]
- CDN（内容分发网络）用于在客户端-服务器模型中，把静态的 JavaScript、CSS、HTML 等资源缓存到离用户更近的边缘节点，从而减少跨地域访问带来的延迟。（[15:04](https://youtu.be/KuClyhvSzXk?t=904)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[geographic-latency-example]]
- [[redis-large-blob-limitation]]
%% ytkb:end %%
