---
title: Server-Sent Events (SSE) for LLM Streaming
aliases: []
tags:
- concept
summary: Server-Sent Events（SSE）是一种由服务端向客户端单向持续推送数据的浏览器原生通信机制，适合LLM这类请求少、响应分块持续返回的场景。
created: '2026-08-26'
updated: '2026-08-26'
---

# Server-Sent Events (SSE) for LLM Streaming

%% ytkb:def %%
Server-Sent Events（SSE）是一种由服务端向客户端单向持续推送数据的浏览器原生通信机制，适合LLM这类请求少、响应分块持续返回的场景。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-communication-patterns]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:AMerB8XjfZ0 %%
### 来自 [[2026-06-30-top-15-frontend-interview-questions-for-2026-wa-se]]
- 使用SSE时，客户端发起一个携带完整对话内容的POST请求，然后在该端点上持续监听，随着模型逐步生成内容不断收到对应的token chunk，是目前最健壮的LLM流式传输方式之一。（[48:09](https://youtu.be/AMerB8XjfZ0?t=2889)）
- SSE 是浏览器原生支持的API，无需引入任何第三方库即可用纯JavaScript（vanilla JS）实现流式数据接收。（[48:09](https://youtu.be/AMerB8XjfZ0?t=2889)）
%% ytkb:end %%

%% ytkb:video:KuClyhvSzXk %%
### 来自 [[2026-06-18-frontend-system-design-explained-w-senior-engineer]]
- 使用 SSE 时客户端发送一条消息建立会话，之后在该 endpoint 上持续接收服务端推送的更新（token），大多数 LLM 应用采用这种方式而非 WebSocket 或 polling。（[36:09](https://youtu.be/KuClyhvSzXk?t=2169)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[llm-response-communication-asymmetry]]
- [[long-polling-scalability-limit]]
- [[openai-sdk-streaming-iterator]]
- [[websocket-communication]]
%% ytkb:end %%
