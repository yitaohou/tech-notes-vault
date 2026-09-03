---
title: DeepSeek Harness Workspace-Write Default Mode
aliases: []
tags:
- concept
summary: DeepSeek Harness 默认采用的权限模式，AI 只能在指定的工作区（项目文件夹）内修改文件、执行命令，工作区之外的内容只能读取不能修改。
created: '2026-09-03'
updated: '2026-09-03'
---

# DeepSeek Harness Workspace-Write Default Mode

%% ytkb:def %%
DeepSeek Harness 默认采用的权限模式，AI 只能在指定的工作区（项目文件夹）内修改文件、执行命令，工作区之外的内容只能读取不能修改。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-safety-security]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:WrwA7FYGPdQ %%
### 来自 [[2026-09-02-deepseek-harness-开源-11-天爆-5-个漏洞ai-读网页电脑被控有人-api-额度]]
- DeepSeek Harness 默认是 workspace-write 模式，AI 要改文件、跑命令只能在指定的项目文件夹里进行，其他地方只能看不能改。（[27:11](https://youtu.be/WrwA7FYGPdQ?t=1631)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[deepseek-harness-read-only-mode]]
%% ytkb:end %%
