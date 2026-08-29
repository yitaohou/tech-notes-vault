---
title: gRPC over HTTP/2
aliases: []
tags:
- concept
summary: gRPC 使用 HTTP/2（第二版 HTTP）作为其底层传输协议。
created: '2026-08-26'
updated: '2026-08-26'
---

# gRPC over HTTP/2

%% ytkb:def %%
gRPC 使用 HTTP/2（第二版 HTTP）作为其底层传输协议。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[backend-grpc]] · [[backend]]
%% ytkb:end %%

## 要点

%% ytkb:video:oYxTTirKY8M %%
### 来自 [[2026-05-26-system-design-explained-apis-databases-caching-cdn]]
- gRPC 使用 HTTP/2 作为传输层，这意味着客户端必须支持 HTTP/2 才能使用 gRPC 进行通信。（[54:11](https://youtu.be/oYxTTirKY8M?t=3251)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[grpc-protocol]]
- [[grpc-server-to-server-usage]]
%% ytkb:end %%
