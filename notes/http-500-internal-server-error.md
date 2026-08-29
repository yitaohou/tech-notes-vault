---
title: HTTP 500 Internal Server Error
aliases: []
tags:
- concept
summary: 表示服务器内部发生非客户端导致的未知错误的 HTTP 状态码。
created: '2026-08-26'
updated: '2026-08-26'
---

# HTTP 500 Internal Server Error

%% ytkb:def %%
表示服务器内部发生非客户端导致的未知错误的 HTTP 状态码。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[backend-api-design]] · [[backend]]
%% ytkb:end %%

## 要点

%% ytkb:video:oYxTTirKY8M %%
### 来自 [[2026-05-26-system-design-explained-apis-databases-caching-cdn]]
- HTTP 500 属于 5xx 服务端错误系列，用于客户端请求本身没有问题、但服务器内部出现未知异常的情况，通常会连带返回一条 server error 消息。（[72:17](https://youtu.be/oYxTTirKY8M?t=4337)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[http-status-code-categories]]
%% ytkb:end %%
