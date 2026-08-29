---
title: Polling (Real-Time Communication)
aliases: []
tags:
- concept
summary: 客户端通过定时器（如 setInterval）按固定时间间隔主动调用后端接口获取最新数据，是实现'实时'通信最简单的技术方式。
created: '2026-08-26'
updated: '2026-08-26'
---

# Polling (Real-Time Communication)

%% ytkb:def %%
客户端通过定时器（如 setInterval）按固定时间间隔主动调用后端接口获取最新数据，是实现'实时'通信最简单的技术方式。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-communication-patterns]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:AMerB8XjfZ0 %%
### 来自 [[2026-06-30-top-15-frontend-interview-questions-for-2026-wa-se]]
- 实现类似实时通信最简单的方式是 polling：使用 setInterval 等定时器函数每隔几秒调用一次后端接口，检查是否有新数据并更新界面。（[45:09](https://youtu.be/AMerB8XjfZ0?t=2709)）
%% ytkb:end %%

%% ytkb:video:KuClyhvSzXk %%
### 来自 [[2026-06-18-frontend-system-design-explained-w-senior-engineer]]
- polling 通过反复调用某个接口（如用 setTimeout 不断请求交易状态接口，直到状态变为 completed）来实现类实时效果，用纯 JavaScript 即可轻松实现，但会对服务器造成过多请求、扩展性差，还可能引发 race condition。（[33:07](https://youtu.be/KuClyhvSzXk?t=1987)）
%% ytkb:end %%

%% ytkb:video:oYxTTirKY8M %%
### 来自 [[2026-05-26-system-design-explained-apis-databases-caching-cdn]]
- 轮询方式在没有新数据时仍会产生完整的请求-响应往返，导致延迟增加、带宽浪费在空响应上，并且无谓消耗服务器资源。（[51:09](https://youtu.be/oYxTTirKY8M?t=3069)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[client-polling-leaderboard]]
- [[real-time-communication-alternatives]]
- [[websocket-communication]]
%% ytkb:end %%
