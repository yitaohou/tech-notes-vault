---
title: Real-Time Communication Alternatives
aliases: []
tags:
- concept
summary: 当业务场景需要突破传统请求-响应（request-response）循环时，可选用 polling、WebSocket 或 Server-Sent
  Events 三种技术手段来实现类实时通信。
created: '2026-08-26'
updated: '2026-08-26'
---

# Real-Time Communication Alternatives

%% ytkb:def %%
当业务场景需要突破传统请求-响应（request-response）循环时，可选用 polling、WebSocket 或 Server-Sent Events 三种技术手段来实现类实时通信。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-communication-patterns]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:KuClyhvSzXk %%
### 来自 [[2026-06-18-frontend-system-design-explained-w-senior-engineer]]
- 实现不遵循传统请求-响应循环的实时通信，通常有三种可选技术方案：polling、WebSocket 和 Server-Sent Events。（[33:07](https://youtu.be/KuClyhvSzXk?t=1987)）
%% ytkb:end %%

%% ytkb:video:oYxTTirKY8M %%
### 来自 [[2026-05-26-system-design-explained-apis-databases-caching-cdn]]
- HTTP 协议擅长处理请求-响应模式，但在需要频繁轮询数据的场景（如聊天应用）中存在局限性，这类需求通常需要借助 WebSocket 等协议来解决。（[51:00](https://youtu.be/oYxTTirKY8M?t=3060)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[polling-technique]]
- [[server-sent-events-llm]]
- [[websocket-communication]]
%% ytkb:end %%
