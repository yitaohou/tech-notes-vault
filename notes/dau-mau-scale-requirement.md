---
title: DAU/MAU-based Scale Requirement
aliases: []
tags:
- concept
summary: 用每日活跃用户数（DAU）和每月活跃用户数（MAU）等指标来量化系统需要支持的可扩展性需求。
created: '2026-08-26'
updated: '2026-08-26'
---

# DAU/MAU-based Scale Requirement

%% ytkb:def %%
用每日活跃用户数（DAU）和每月活跃用户数（MAU）等指标来量化系统需要支持的可扩展性需求。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-interview-methodology]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:QBHTbtWSECg %%
### 来自 [[2026-03-15-system-design-mock-interview-design-leetcode-ft-ex]]
- 系统设计中提出的可扩展性需求是要支持百万级 daily active users 和数亿级 monthly active users。（[09:03](https://youtu.be/QBHTbtWSECg?t=543)）
%% ytkb:end %%

%% ytkb:video:Qa-7iWxDz1A %%
### 来自 [[2026-06-08-fundamentals-of-backend-architecture---how-to-desi]]
- 举例说明业务规模增长（如达到10,000月活用户）会带来新的资源消耗与性能问题，促使系统需要考虑 caching 等优化手段。（[36:09](https://youtu.be/Qa-7iWxDz1A?t=2169)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[caching-motivation-repeated-access]]
- [[contest-traffic-spike-pattern]]
%% ytkb:end %%
