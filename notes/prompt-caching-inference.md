---
title: Prompt Caching
aliases: []
tags:
- concept
summary: prompt caching 是在推理服务中缓存重复出现的文本片段（如系统提示词或参考文档），避免每次请求都重新处理这些内容的技术。
created: '2026-08-26'
updated: '2026-08-26'
---

# Prompt Caching

%% ytkb:def %%
prompt caching 是在推理服务中缓存重复出现的文本片段（如系统提示词或参考文档），避免每次请求都重新处理这些内容的技术。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-inference-optimization]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:JV3pL1_mn2M %%
### 来自 [[2025-04-01-ai-engineering-in-76-minutes-complete-coursespeedr]]
- prompt caching 会缓存诸如 system prompt 或参考文档等在多次请求间重复出现的文本片段，避免每次查询都重新处理，对长对话或针对同一文档的多次查询尤为有价值。（[66:06](https://youtu.be/JV3pL1_mn2M?t=3966)）
%% ytkb:end %%
