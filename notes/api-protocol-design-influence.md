---
title: Protocol Choice Shapes API Design
aliases: []
tags:
- concept
summary: 指API所选用的底层通信协议会从根本上决定该API可采用的设计方式、性能表现与能力边界。
created: '2026-08-26'
updated: '2026-08-26'
---

# Protocol Choice Shapes API Design

%% ytkb:def %%
指API所选用的底层通信协议会从根本上决定该API可采用的设计方式、性能表现与能力边界。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-api-design]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:oYxTTirKY8M %%
### 来自 [[2026-05-26-system-design-explained-apis-databases-caching-cdn]]
- API 底层选用的协议（HTTP、WebSocket、gRPC 等）会从根本上决定其设计方式、性能与能力范围，因此协议选型应基于各协议自身的优劣势来确定。（[41:10](https://youtu.be/oYxTTirKY8M?t=2470)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[restful-api-design]]
- [[websocket-communication]]
%% ytkb:end %%
