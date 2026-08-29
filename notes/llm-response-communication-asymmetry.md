---
title: LLM Response Communication Asymmetry
aliases: []
tags:
- concept
summary: LLM交互中客户端通常只发送一次性的查询请求，而模型会以多个连续token/chunk的形式持续返回响应，这种请求小、响应持续分块返回的模式称为通信不对称。
created: '2026-08-26'
updated: '2026-08-26'
---

# LLM Response Communication Asymmetry

%% ytkb:def %%
LLM交互中客户端通常只发送一次性的查询请求，而模型会以多个连续token/chunk的形式持续返回响应，这种请求小、响应持续分块返回的模式称为通信不对称。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-inference-optimization]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:AMerB8XjfZ0 %%
### 来自 [[2026-06-30-top-15-frontend-interview-questions-for-2026-wa-se]]
- 在 LLM 场景下，客户端发送一次查询后，模型会依次返回第一个token、第二个token、第三个token直到最终完整句子，这种高度不对称的通信模式是选择流式传输方案而非轮询或WebSocket的关键原因。（[48:09](https://youtu.be/AMerB8XjfZ0?t=2889)）
%% ytkb:end %%

%% ytkb:video:KuClyhvSzXk %%
### 来自 [[2026-06-18-frontend-system-design-explained-w-senior-engineer]]
- AI 场景中确实需要实时通信，但方向是单向的：客户端只发送一次查询，之后服务端持续推送 token 回来，这种客户端与服务端消息量的不对称正是 SSE 适用的原因。（[36:09](https://youtu.be/KuClyhvSzXk?t=2169)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[server-sent-events-llm]]
- [[websocket-communication]]
%% ytkb:end %%
