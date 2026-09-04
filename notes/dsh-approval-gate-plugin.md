---
title: DSH Approval Gate Plugin
aliases: []
tags:
- concept
summary: 一款为 DeepSeek Harness 提供智能审批能力的插件，让智能体执行命令前先自我判断风险，简单命令自动放行、疑似危险命令转交人工确认，用于兼顾安全性与使用自由度。
created: '2026-09-04'
updated: '2026-09-04'
---

# DSH Approval Gate Plugin

%% ytkb:def %%
一款为 DeepSeek Harness 提供智能审批能力的插件，让智能体执行命令前先自我判断风险，简单命令自动放行、疑似危险命令转交人工确认，用于兼顾安全性与使用自由度。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-safety-security]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:buYQ-_V2Wv0 %%
### 来自 [[2026-09-04-一个视频搞懂deepseek-harness]]
- 安装 DSH-Approval-Gate 插件后，智能体在执行命令前会先自查风险：简单无害的命令直接放行，疑似危险的命令则转为人工审批，从而在只读/完全访问两个极端之间取得平衡。（[03:01](https://youtu.be/buYQ-_V2Wv0?t=181)）
- DSH-Approval-Gate 插件用久后会根据用户自身的使用习惯自动改进其放行规则，并且智能体历史申请过的所有权限都可以在新增的审批标签页中查看。（[03:01](https://youtu.be/buYQ-_V2Wv0?t=181)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[deepseek-harness-approval-fail-close]]
- [[deepseek-harness-permission-tiers]]
%% ytkb:end %%
