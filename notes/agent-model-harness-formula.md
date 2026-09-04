---
title: Agent = Model + Harness Formula
aliases: []
tags:
- concept
summary: DeepSeek 官方提出的公式，用于说明 agent 由负责决策的 model 与负责执行的 harness 两部分组成。
created: '2026-09-03'
updated: '2026-09-04'
---

# Agent = Model + Harness Formula

%% ytkb:def %%
DeepSeek 官方提出的公式，用于说明 agent 由负责决策的 model 与负责执行的 harness 两部分组成。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-agent-architecture]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:WrwA7FYGPdQ %%
### 来自 [[2026-09-02-deepseek-harness-开源-11-天爆-5-个漏洞ai-读网页电脑被控有人-api-额度]]
- DeepSeek 官方提出 agent 等于 model 加 harness 的公式：model 负责理解语言、做决策、生成回复；harness 负责把 model 的决策转化为文件读写、代码修改、命令执行等实际操作。（[00:00](https://youtu.be/WrwA7FYGPdQ?t=0)）
%% ytkb:end %%

%% ytkb:video:buYQ-_V2Wv0 %%
### 来自 [[2026-09-04-一个视频搞懂deepseek-harness]]
- 该公式可以类比为「模型是发动机，Harness是车架」；同一个模型接不同的 Harness 表现会有明显差异，例如 Claude 模型接 Claude Code 效果拔群，接 Codex 能力就掉下来了。（[00:00](https://youtu.be/buYQ-_V2Wv0?t=0)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[agent-definition]]
- [[agent-harness]]
- [[deepseek-harness]]
%% ytkb:end %%
