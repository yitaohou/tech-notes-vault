---
title: Synchronous Downstream Call Risk
aliases: []
tags:
- concept
summary: 上游服务在事件发生后直接同步调用下游服务，若下游服务宕机、变慢或超时，主流程仍会成功返回，但下游副作用永远不会发生且不会被察觉的风险。
created: '2026-08-26'
updated: '2026-08-26'
---

# Synchronous Downstream Call Risk

%% ytkb:def %%
上游服务在事件发生后直接同步调用下游服务，若下游服务宕机、变慢或超时，主流程仍会成功返回，但下游副作用永远不会发生且不会被察觉的风险。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[backend-service-architecture-patterns]] · [[backend]]
%% ytkb:end %%

## 要点

%% ytkb:video:Qa-7iWxDz1A %%
### 来自 [[2026-06-08-fundamentals-of-backend-architecture---how-to-desi]]
- 若上传成功后直接同步调用缩略图服务，一旦该服务返回 404、503 或请求超时，视频会永久缺失缩略图，而系统完全不会意识到这一失败，因为上传本身已经成功返回。（[33:08](https://youtu.be/Qa-7iWxDz1A?t=1988)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[message-broker-necessity]]
- [[presigned-url-direct-upload]]
%% ytkb:end %%
