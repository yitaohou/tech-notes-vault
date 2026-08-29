---
title: API Predictable Behavior Principle
aliases: []
tags:
- concept
summary: 好的 API 端点不应在执行预期操作之外产生意料之外的副作用，例如查询接口不应顺带修改数据。
created: '2026-08-26'
updated: '2026-08-26'
---

# API Predictable Behavior Principle

%% ytkb:def %%
好的 API 端点不应在执行预期操作之外产生意料之外的副作用，例如查询接口不应顺带修改数据。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[backend-api-design]] · [[backend]]
%% ytkb:end %%

## 要点

%% ytkb:video:oYxTTirKY8M %%
### 来自 [[2026-05-26-system-design-explained-apis-databases-caching-cdn]]
- 好的 API 端点不应产生超出预期范围的副作用，例如一个用于获取用户详情的 GET 请求不应该顺带更新关注者数据。（[38:10](https://youtu.be/oYxTTirKY8M?t=2290)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[api-design-as-documentation]]
%% ytkb:end %%
