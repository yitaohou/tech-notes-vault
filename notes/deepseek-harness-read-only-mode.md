---
title: DeepSeek Harness Read-Only Mode
aliases: []
tags:
- concept
summary: DeepSeek Harness 中用于处理不可信内容的权限模式，切换后 AI 无法对文件进行任何修改。
created: '2026-09-03'
updated: '2026-09-03'
---

# DeepSeek Harness Read-Only Mode

%% ytkb:def %%
DeepSeek Harness 中用于处理不可信内容的权限模式，切换后 AI 无法对文件进行任何修改。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-safety-security]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:WrwA7FYGPdQ %%
### 来自 [[2026-09-02-deepseek-harness-开源-11-天爆-5-个漏洞ai-读网页电脑被控有人-api-额度]]
- 处理不可信内容（如从网上下载的陌生仓库、外部文档）时应先切到 read-only 模式，最新版 DeepSeek Harness 中输入 permission read only 即可切换，切换后沙箱和审批策略会一并切换。（[27:11](https://youtu.be/WrwA7FYGPdQ?t=1631)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[deepseek-harness-workspace-write-default]]
%% ytkb:end %%
