---
title: Prompting-to-Fine-tuning Escalation Path
aliases: []
tags:
- concept
summary: 改进模型行为时建议遵循的递进策略：先用 prompting 加示例，再尝试 RAG，仍不行则 fine-tuning，最后可结合 RAG 与 fine-tuning。
created: '2026-08-26'
updated: '2026-08-26'
---

# Prompting-to-Fine-tuning Escalation Path

%% ytkb:def %%
改进模型行为时建议遵循的递进策略：先用 prompting 加示例，再尝试 RAG，仍不行则 fine-tuning，最后可结合 RAG 与 fine-tuning。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-prompt-engineering]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:JV3pL1_mn2M %%
### 来自 [[2025-04-01-ai-engineering-in-76-minutes-complete-coursespeedr]]
- 当模型仅靠 prompting 无法达成目标时，建议按顺序升级：先在提示词中加入更多示例，若仍有信息类失败则尝试更高级的 RAG（如 embedding-based retrieval），若仍有行为类问题则采用 fine-tuning，最后可将 RAG 与 fine-tuning 结合以获得更大性能提升。（[45:04](https://youtu.be/JV3pL1_mn2M?t=2704)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[parameter-efficient-fine-tuning]]
- [[retrieval-augmented-generation]]
%% ytkb:end %%
