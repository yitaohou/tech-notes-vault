---
title: Netflix RAM Pre-warming Exception
aliases: []
tags:
- concept
summary: 个别业务场景下（如 Netflix 应对热门新剧首波流量），会破例把整份大文件预先放入 RAM 以提供更优服务体验。
created: '2026-08-26'
updated: '2026-08-26'
---

# Netflix RAM Pre-warming Exception

%% ytkb:def %%
个别业务场景下（如 Netflix 应对热门新剧首波流量），会破例把整份大文件预先放入 RAM 以提供更优服务体验。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-caching-edge]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:Qa-7iWxDz1A %%
### 来自 [[2026-06-08-fundamentals-of-backend-architecture---how-to-desi]]
- 也存在例外情况：例如 Netflix 可能会在一部新剧或电影即将爆红时，把它预先放进 RAM，只为应对最初那波用户激增流量，以提供更好的服务体验。（[39:09](https://youtu.be/Qa-7iWxDz1A?t=2349)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[ram-caching-large-files-anti-pattern]]
%% ytkb:end %%
