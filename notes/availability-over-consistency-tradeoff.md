---
title: Availability Over Consistency Tradeoff
aliases: []
tags:
- concept
summary: 系统设计非功能需求中，在可用性与一致性之间做权衡时优先选择高可用、采用 eventual consistency 模型而非强一致性的设计决策。
created: '2026-08-26'
updated: '2026-08-26'
---

# Availability Over Consistency Tradeoff

%% ytkb:def %%
系统设计非功能需求中，在可用性与一致性之间做权衡时优先选择高可用、采用 eventual consistency 模型而非强一致性的设计决策。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-scalability]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:QBHTbtWSECg %%
### 来自 [[2026-03-15-system-design-mock-interview-design-leetcode-ft-ex]]
- 针对 LeetCode 系统的非功能需求，明确选择让系统始终保持高可用（highly available），可以接受 eventual consistency，而不是追求强一致性。（[03:01](https://youtu.be/QBHTbtWSECg?t=181)）
- 该系统的非功能性需求中明确选择优先保障 availability，而非 consistency，这是 CAP 权衡下针对该场景做出的具体设计取舍。（[36:11](https://youtu.be/QBHTbtWSECg?t=2171)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[code-sandbox-temp-directory-cleanup]]
- [[eventual-consistency-submission-feedback]]
- [[out-of-scope-requirements-technique]]
%% ytkb:end %%
