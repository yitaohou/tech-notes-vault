---
title: .dsh Folder Backup and Version Control Caution
aliases: []
tags:
- concept
summary: 指不应将 DeepSeek Harness 的 .dsh 配置文件夹同步到网盘或提交进代码仓库的安全建议。
created: '2026-09-03'
updated: '2026-09-03'
---

# .dsh Folder Backup and Version Control Caution

%% ytkb:def %%
指不应将 DeepSeek Harness 的 .dsh 配置文件夹同步到网盘或提交进代码仓库的安全建议。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-safety-security]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:WrwA7FYGPdQ %%
### 来自 [[2026-09-02-deepseek-harness-开源-11-天爆-5-个漏洞ai-读网页电脑被控有人-api-额度]]
- .dsh 文件夹不应同步到网盘、云备份，也不应提交到代码仓库，因为里面含有 API 密钥等敏感信息；出问题时可以到该文件夹查轨迹日志排查。（[27:11](https://youtu.be/WrwA7FYGPdQ?t=1631)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[dsh-hidden-config-folder]]
%% ytkb:end %%
