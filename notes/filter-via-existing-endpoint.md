---
title: Reusing Existing Endpoint for Filtering
aliases: []
tags:
- concept
summary: 在接口设计中选择复用已有 GET 接口加过滤参数，而非为过滤功能单独新建一个接口的设计取舍。
created: '2026-08-26'
updated: '2026-08-26'
---

# Reusing Existing Endpoint for Filtering

%% ytkb:def %%
在接口设计中选择复用已有 GET 接口加过滤参数，而非为过滤功能单独新建一个接口的设计取舍。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[backend-api-design]] · [[backend]]
%% ytkb:end %%

## 要点

%% ytkb:video:QBHTbtWSECg %%
### 来自 [[2026-03-15-system-design-mock-interview-design-leetcode-ft-ex]]
- 题目列表的过滤功能既可以在原有的 get all 接口上加过滤参数实现，也可以单独建一个接口，但认为目前没必要单独建。（[15:06](https://youtu.be/QBHTbtWSECg?t=906)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[problem-list-filtering]]
- [[rest-api-get-all-problems]]
%% ytkb:end %%
