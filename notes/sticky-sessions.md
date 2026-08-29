---
title: Sticky Sessions (Session Affinity)
aliases: []
tags:
- concept
summary: 负载均衡中尽力将同一用户的后续请求重新路由到其之前访问过的同一台服务器的策略。
created: '2026-08-26'
updated: '2026-08-26'
---

# Sticky Sessions (Session Affinity)

%% ytkb:def %%
负载均衡中尽力将同一用户的后续请求重新路由到其之前访问过的同一台服务器的策略。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-scalability]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:Qa-7iWxDz1A %%
### 来自 [[2026-06-08-fundamentals-of-backend-architecture---how-to-desi]]
- sticky sessions 的核心动机是：如果服务器为该用户保存了某些状态（正在处理的工作），把该用户后续请求继续导向同一服务器会更合理。（[12:03](https://youtu.be/Qa-7iWxDz1A?t=723)）
- sticky sessions 通常通过 session cookie（例如可以是用户的认证 token）来标识用户身份，负载均衡器据此判断应将请求转发到哪台服务器。（[12:03](https://youtu.be/Qa-7iWxDz1A?t=723)）
- sticky sessions 只是「尽力而为」（best effort）的路由策略，并非强保证：清除 cookie 后重新请求可能被路由到不同服务器。（[12:03](https://youtu.be/Qa-7iWxDz1A?t=723)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[nginx-upstream-block]]
- [[round-robin-load-balancing]]
%% ytkb:end %%
