---
title: REST Statelessness
aliases: []
tags:
- concept
summary: REST API 的无状态特性，指每个请求都自带处理所需的全部信息，服务端处理当前请求时不依赖之前的请求。
created: '2026-08-26'
updated: '2026-08-26'
---

# REST Statelessness

%% ytkb:def %%
REST API 的无状态特性，指每个请求都自带处理所需的全部信息，服务端处理当前请求时不依赖之前的请求。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[backend-api-design]] · [[backend]]
%% ytkb:end %%

## 要点

%% ytkb:video:oYxTTirKY8M %%
### 来自 [[2026-05-26-system-design-explained-apis-databases-caching-cdn]]
- REST API 的一大优势是无状态（stateless）：每个请求都包含处理该请求所需的全部信息，不需要依赖任何先前的请求即可被独立处理。（[30:03](https://youtu.be/oYxTTirKY8M?t=1803)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[restful-api-design]]
%% ytkb:end %%
