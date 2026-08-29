---
title: Time to Publish (TTP)
aliases: []
tags:
- concept
summary: 部分团队使用的延迟指标，指首个 token 真正展示给用户的时间，区别于模型内部生成第一个 token 的时间。
created: '2026-08-26'
updated: '2026-08-26'
---

# Time to Publish (TTP)

%% ytkb:def %%
部分团队使用的延迟指标，指首个 token 真正展示给用户的时间，区别于模型内部生成第一个 token 的时间。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-inference-optimization]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:JV3pL1_mn2M %%
### 来自 [[2025-04-01-ai-engineering-in-76-minutes-complete-coursespeedr]]
- TTP（time to publish）指首个 token 真正展示给用户的时间，因为模型有时会先生成 plan 或进行 Chain of Thought 推理，生成的第一个 token 不一定会立即展示给用户。（[60:04](https://youtu.be/JV3pL1_mn2M?t=3604)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[time-to-first-token]]
%% ytkb:end %%
