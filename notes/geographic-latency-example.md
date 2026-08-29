---
title: Geographic Latency Example
aliases: []
tags:
- concept
summary: 用具体跨地域网络延迟数字说明物理距离对延迟的影响。
created: '2026-08-26'
updated: '2026-08-26'
---

# Geographic Latency Example

%% ytkb:def %%
用具体跨地域网络延迟数字说明物理距离对延迟的影响。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-networking]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:Qa-7iWxDz1A %%
### 来自 [[2026-06-08-fundamentals-of-backend-architecture---how-to-desi]]
- 举例说明地理距离对延迟的影响：美国到里斯本之间的网络延迟大约是 300 毫秒，这正是需要把内容缓存在靠近用户地理位置的原因。（[42:09](https://youtu.be/Qa-7iWxDz1A?t=2529)）
%% ytkb:end %%

%% ytkb:video:KuClyhvSzXk %%
### 来自 [[2026-06-18-frontend-system-design-explained-w-senior-engineer]]
- 以美国用户访问部署在欧洲的应用为例：若没有 CDN，获取 JavaScript、CSS、HTML 等静态资源需要跨越大西洋一个往返，这段物理距离直接带来额外的网络延迟。（[15:04](https://youtu.be/KuClyhvSzXk?t=904)）
- 光速是网络延迟无法绕开的物理极限：无论应用多么高效，长距离传输数据仍会因光速限制给每次请求增加大约200到250毫秒的延迟。（[18:05](https://youtu.be/KuClyhvSzXk?t=1085)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[cdn-edge-asset-caching]]
- [[cdn-point-of-presence]]
%% ytkb:end %%
