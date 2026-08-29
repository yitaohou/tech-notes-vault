---
title: Observing SSE in ChatGPT/Claude Network Requests
aliases: []
tags:
- concept
summary: 指在浏览器开发者工具的Network面板中查看ChatGPT或Claude的对话请求，可以在event stream标签下看到token被逐个通过SSE推送的过程。
created: '2026-08-26'
updated: '2026-08-26'
---

# Observing SSE in ChatGPT/Claude Network Requests

%% ytkb:def %%
指在浏览器开发者工具的Network面板中查看ChatGPT或Claude的对话请求，可以在event stream标签下看到token被逐个通过SSE推送的过程。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-communication-patterns]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:AMerB8XjfZ0 %%
### 来自 [[2026-06-30-top-15-frontend-interview-questions-for-2026-wa-se]]
- 打开ChatGPT或Claude的浏览器开发者工具Network面板，在对应请求的event stream标签中可以直接看到token一个个被推送过来，验证了这些主流聊天应用底层确实采用SSE传输模型输出。（[48:09](https://youtu.be/AMerB8XjfZ0?t=2889)）
%% ytkb:end %%

%% ytkb:video:KuClyhvSzXk %%
### 来自 [[2026-06-18-frontend-system-design-explained-w-senior-engineer]]
- 在浏览器开发者工具 Network 面板中找到 ChatGPT 或 Claude 的对话请求，可以看到响应是以 event stream 形式一块块（chunk）返回的，这正是构建 LLM 聊天 UI 的技术基础。（[36:09](https://youtu.be/KuClyhvSzXk?t=2169)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[server-sent-events-llm]]
%% ytkb:end %%
