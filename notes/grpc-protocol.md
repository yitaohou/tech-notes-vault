---
title: gRPC
aliases: []
tags:
- concept
summary: gRPC 是 Google 发明的高性能 RPC 框架，使用 protocol buffers 作为数据序列化格式。
created: '2026-08-26'
updated: '2026-08-26'
---

# gRPC

%% ytkb:def %%
gRPC 是 Google 发明的高性能 RPC 框架，使用 protocol buffers 作为数据序列化格式。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[backend-grpc]] · [[backend]]
%% ytkb:end %%

## 要点

%% ytkb:video:oYxTTirKY8M %%
### 来自 [[2026-05-26-system-design-explained-apis-databases-caching-cdn]]
- gRPC 是由 Google 发明的高性能 RPC 框架，主要使用 protocol buffers 进行数据编码。（[54:11](https://youtu.be/oYxTTirKY8M?t=3251)）
- gRPC 由于基于 HTTP/2，天然自带内置的 streaming 能力。（[54:11](https://youtu.be/oYxTTirKY8M?t=3251)）
- gRPC 使用 HTTP/2 作为传输协议，是一种高性能的 RPC（Remote Procedure Call）框架。（[57:11](https://youtu.be/oYxTTirKY8M?t=3431)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[grpc-http2-transport]]
- [[grpc-server-to-server-usage]]
%% ytkb:end %%
