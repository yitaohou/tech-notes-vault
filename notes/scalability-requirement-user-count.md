---
title: Scalability Requirement Based on User Count
aliases: []
tags:
- concept
summary: 在系统设计中，需要先明确要支持的用户规模，才能决定是否需要构建更具可扩展性的解决方案。
created: '2026-08-26'
updated: '2026-08-26'
---

# Scalability Requirement Based on User Count

%% ytkb:def %%
在系统设计中，需要先明确要支持的用户规模，才能决定是否需要构建更具可扩展性的解决方案。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-scalability]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:QBHTbtWSECg %%
### 来自 [[2026-03-15-system-design-mock-interview-design-leetcode-ft-ex]]
- 在设计判题系统前应先弄清楚需要支持多少用户，用户量越大就越需要考虑更具可扩展性的方案。（[06:02](https://youtu.be/QBHTbtWSECg?t=362)）
%% ytkb:end %%

%% ytkb:video:CyLYY_xb5bQ %%
### 来自 [[2025-08-25-you-can-learn-ai-agent-system-design-in-19-min-rag]]
- 设计 agentic 系统时，scalability、每秒请求数（requests per second）、seasonality 等服务端相关的非功能性需求容易被非技术视角忽略，但产品经理最终仍需与工程负责人共同讨论确定这些指标才能让产品具备上生产环境的条件。（[18:05](https://youtu.be/CyLYY_xb5bQ?t=1085)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[architecture-holistic-scope]]
- [[concurrent-user-estimation]]
- [[contest-traffic-surge]]
%% ytkb:end %%
