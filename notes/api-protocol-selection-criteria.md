---
title: API Protocol Selection Criteria
aliases: []
tags:
- concept
summary: 在为系统选择合适的 API 协议时需要综合考虑的一组因素，包括交互模式、性能需求、客户端兼容性、负载大小与编码、安全需求及开发者体验。
created: '2026-08-26'
updated: '2026-08-26'
---

# API Protocol Selection Criteria

%% ytkb:def %%
在为系统选择合适的 API 协议时需要综合考虑的一组因素，包括交互模式、性能需求、客户端兼容性、负载大小与编码、安全需求及开发者体验。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-api-design]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:oYxTTirKY8M %%
### 来自 [[2026-05-26-system-design-explained-apis-databases-caching-cdn]]
- 选择 API 协议时首先要考虑交互模式：默认请求-响应场景用 HTTP，而实时通信（如实时聊天）场景则需要用 WebSocket。（[54:11](https://youtu.be/oYxTTirKY8M?t=3251)）
- 当系统中存在多个服务器或微服务相互通信、且有机会使用 gRPC 时，可以选用 gRPC 来提升通信性能和速度，这是性能需求维度的考量。（[54:11](https://youtu.be/oYxTTirKY8M?t=3251)）
- 客户端兼容性也是协议选择的重要考量，例如大多数浏览器不支持最新版本的 HTTP，导致 gRPC 在浏览器与服务器通信中并不常用。（[54:11](https://youtu.be/oYxTTirKY8M?t=3251)）
- 协议选择还需考虑负载大小（数据量）与编码方式、基于认证和加密的安全需求，以及开发者体验（即该协议的工具链和文档是否完善）。（[54:11](https://youtu.be/oYxTTirKY8M?t=3251)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[grpc-protocol]]
- [[grpc-server-to-server-usage]]
%% ytkb:end %%
