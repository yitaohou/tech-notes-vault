---
title: SSR Scaling Bottleneck
aliases: []
tags:
- concept
summary: SSR 架构下，所有获取到静态资源的客户端最终都要回源向服务器请求页面渲染，导致渲染请求全部集中到服务器端，形成可扩展性瓶颈。
created: '2026-08-26'
updated: '2026-08-26'
---

# SSR Scaling Bottleneck

%% ytkb:def %%
SSR 架构下，所有获取到静态资源的客户端最终都要回源向服务器请求页面渲染，导致渲染请求全部集中到服务器端，形成可扩展性瓶颈。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[frontend-rendering-strategies]] · [[frontend]]
%% ytkb:end %%

## 要点

%% ytkb:video:AMerB8XjfZ0 %%
### 来自 [[2026-06-30-top-15-frontend-interview-questions-for-2026-wa-se]]
- SSR 的复杂性在于，用户拿到静态资源后仍需回源请求服务器完成渲染，所有用户的渲染请求都集中打到同一服务器，形成 scaling bottleneck。（[45:09](https://youtu.be/AMerB8XjfZ0?t=2709)）
- SSR 除了扩展性瓶颈外还引入额外延迟：用户虽能快速拿到静态资源，但完成页面渲染仍需再发起一次回源请求，等待服务器返回渲染结果。（[45:09](https://youtu.be/AMerB8XjfZ0?t=2709)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[edge-computing-ssr]]
- [[horizontal-scaling]]
- [[single-point-of-failure]]
%% ytkb:end %%
