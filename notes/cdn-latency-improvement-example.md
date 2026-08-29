---
title: CDN Latency Improvement Example
aliases: []
tags:
- concept
summary: 通过具体数字对比说明 CDN 缓存命中相较于回源查询能带来的响应时间提升。
created: '2026-08-26'
updated: '2026-08-26'
---

# CDN Latency Improvement Example

%% ytkb:def %%
通过具体数字对比说明 CDN 缓存命中相较于回源查询能带来的响应时间提升。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-caching-edge]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:Qa-7iWxDz1A %%
### 来自 [[2026-06-08-fundamentals-of-backend-architecture---how-to-desi]]
- 举例：里斯本某用户首次请求某图片需要走数据库全流程、耗时约 1 秒；该图片被 CDN 缓存后，同一 CDN 节点覆盖范围内后续约 499 个用户的请求可加速到约 20 毫秒。（[42:09](https://youtu.be/Qa-7iWxDz1A?t=2529)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[cdn-point-of-presence]]
- [[geographic-latency-example]]
%% ytkb:end %%
