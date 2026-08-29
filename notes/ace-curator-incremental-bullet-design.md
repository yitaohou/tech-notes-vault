---
title: ACE Curator Incremental Bullet Update Design
aliases: []
tags:
- concept
summary: ACE中Curator不重写整段提示词、而是输出结构化要点并通过确定性逻辑合并更新，以避免上下文崩塌和简洁性偏差的关键设计。
created: '2026-08-26'
updated: '2026-08-26'
---

# ACE Curator Incremental Bullet Update Design

%% ytkb:def %%
ACE中Curator不重写整段提示词、而是输出结构化要点并通过确定性逻辑合并更新，以避免上下文崩塌和简洁性偏差的关键设计。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-prompt-engineering]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:z_F0z7wF5XU %%
### 来自 [[2026-07-09-ai自我递归改进先要靠harness工程-lilian-weng最新长文-反馈循环-三个设计模式-核]]
- 为避免迭代重写过程中出现上下文崩塌和简洁性偏差，ACE的Curator不重写整段提示词，而是输出带标识的结构化要点，通过确定性逻辑合并进上下文日志并定期精简去重。（[06:04](https://youtu.be/z_F0z7wF5XU?t=364)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[ace-generator-reflector-curator-roles]]
- [[agentic-context-engineering-ace]]
%% ytkb:end %%
