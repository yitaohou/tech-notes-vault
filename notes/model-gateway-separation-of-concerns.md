---
title: Model Gateway Separation of Concerns
aliases: []
tags:
- concept
summary: model gateway带来的架构收益：当模型API发生变化时只需更新gateway，无需逐个修改调用方代码，是软件工程separation of
  concerns原则的体现。
created: '2026-08-26'
updated: '2026-08-26'
---

# Model Gateway Separation of Concerns

%% ytkb:def %%
model gateway带来的架构收益：当模型API发生变化时只需更新gateway，无需逐个修改调用方代码，是软件工程separation of concerns原则的体现。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-model-selection-deployment]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:JV3pL1_mn2M %%
### 来自 [[2025-04-01-ai-engineering-in-76-minutes-complete-coursespeedr]]
- 使用model gateway让代码库更易维护，当某个模型API变化时只需更新gateway一处，而不必修改每个使用该模型的应用代码，是separation of concerns的经典体现。（[69:07](https://youtu.be/JV3pL1_mn2M?t=4147)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[model-gateway]]
%% ytkb:end %%
