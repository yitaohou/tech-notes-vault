---
title: CDN Origin Bypass
aliases: []
tags:
- concept
summary: 当请求命中 CDN 缓存时，用户请求完全绕过源服务器及其后端数据库/缓存查询链路，直接由 CDN 边缘节点返回结果。
created: '2026-08-26'
updated: '2026-08-26'
---

# CDN Origin Bypass

%% ytkb:def %%
当请求命中 CDN 缓存时，用户请求完全绕过源服务器及其后端数据库/缓存查询链路，直接由 CDN 边缘节点返回结果。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-caching-edge]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:Qa-7iWxDz1A %%
### 来自 [[2026-06-08-fundamentals-of-backend-architecture---how-to-desi]]
- CDN 的强大之处在于一旦内容被缓存，后续用户请求可以完全跳过源服务器上原本用于获取文件的整套计算流程（DB 查询、cache 查询等），直接由 CDN 节点响应。（[42:09](https://youtu.be/Qa-7iWxDz1A?t=2529)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[cache-aside-pattern]]
- [[cdn-point-of-presence]]
%% ytkb:end %%
