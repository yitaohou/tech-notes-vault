---
title: gRPC Server-to-Server Usage
aliases: []
tags:
- concept
summary: 由于对 HTTP/2 客户端支持的要求，gRPC 通常被用于服务器与服务器（如微服务）之间的通信，而非客户端浏览器与服务器之间。
created: '2026-08-26'
updated: '2026-08-26'
---

# gRPC Server-to-Server Usage

%% ytkb:def %%
由于对 HTTP/2 客户端支持的要求，gRPC 通常被用于服务器与服务器（如微服务）之间的通信，而非客户端浏览器与服务器之间。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[backend-grpc]] · [[backend]]
%% ytkb:end %%

## 要点

%% ytkb:video:oYxTTirKY8M %%
### 来自 [[2026-05-26-system-design-explained-apis-databases-caching-cdn]]
- 因为多数浏览器不支持最新版本的 HTTP，gRPC 在浏览器-服务器通信中并不常见，而更常用于多个微服务之间彼此通信的场景。（[54:11](https://youtu.be/oYxTTirKY8M?t=3251)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[grpc-http2-transport]]
- [[grpc-protocol]]
%% ytkb:end %%
