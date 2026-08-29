---
title: OpenAI SDK Streaming Iterator
aliases: []
tags:
- concept
summary: OpenAI 官方SDK对LLM流式响应提供了迭代器（iterator）封装，开发者可通过迭代方式逐个获取生成的token，底层实际使用SSE实现。
created: '2026-08-26'
updated: '2026-08-26'
---

# OpenAI SDK Streaming Iterator

%% ytkb:def %%
OpenAI 官方SDK对LLM流式响应提供了迭代器（iterator）封装，开发者可通过迭代方式逐个获取生成的token，底层实际使用SSE实现。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-communication-patterns]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:AMerB8XjfZ0 %%
### 来自 [[2026-06-30-top-15-frontend-interview-questions-for-2026-wa-se]]
- OpenAI 的官方包底层使用SSE来传输数据，但对开发者暴露的是一个迭代器接口，使开发者可以直接遍历获取每个生成的token，而无需自己处理原始的SSE事件流。（[48:09](https://youtu.be/AMerB8XjfZ0?t=2889)）
%% ytkb:end %%

%% ytkb:video:KuClyhvSzXk %%
### 来自 [[2026-06-18-frontend-system-design-explained-w-senior-engineer]]
- 在 React 应用中用 OpenAI NPM package 构建聊天应用时，底层实际使用的就是 server-sent events 来接收 token 流。（[36:09](https://youtu.be/KuClyhvSzXk?t=2169)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[server-sent-events-llm]]
%% ytkb:end %%
