---
title: Unused File Detection
aliases: []
tags:
- concept
summary: 通过静态分析工具检测代码库中未被任何地方引用、已成为死代码的文件数量，用于发现代码库臃肿和维护负担。
created: '2026-08-26'
updated: '2026-08-26'
---

# Unused File Detection

%% ytkb:def %%
通过静态分析工具检测代码库中未被任何地方引用、已成为死代码的文件数量，用于发现代码库臃肿和维护负担。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[frontend-code-quality-tooling]] · [[frontend]]
%% ytkb:end %%

## 要点

%% ytkb:video:hA_XnzB1Ef8 %%
### 来自 [[2026-07-07-3-frontend-skills-ai-cant-replace-become-ai-proof]]
- 同一份静态分析报告显示该代码库中存在 153 个未使用的文件（unused files），这会显著恶化 AI 的 context management 并降低 AI 给出的结果质量。（[09:03](https://youtu.be/hA_XnzB1Ef8?t=543)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[code-duplication-analysis]]
- [[context-dilution]]
%% ytkb:end %%
