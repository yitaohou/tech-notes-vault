---
title: Chat Template Mismatch
aliases: []
tags:
- concept
summary: system prompt 与 user prompt 组合成模型输入时若使用了错误的模板格式，可能导致模型表现异常且不易察觉的问题。
created: '2026-08-26'
updated: '2026-08-26'
---

# Chat Template Mismatch

%% ytkb:def %%
system prompt 与 user prompt 组合成模型输入时若使用了错误的模板格式，可能导致模型表现异常且不易察觉的问题。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-prompt-engineering]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:JV3pL1_mn2M %%
### 来自 [[2025-04-01-ai-engineering-in-76-minutes-complete-coursespeedr]]
- system prompt 与 user prompt 的组合模板因模型和版本而异，若使用错误模板（哪怕只是多了一个换行符）都可能引发难以察觉的性能异常（silent failure），使用第三方工具构建 prompt 时尤其要严格遵循模型的 chat template。（[24:02](https://youtu.be/JV3pL1_mn2M?t=1442)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[system-prompt-vs-user-prompt]]
%% ytkb:end %%
