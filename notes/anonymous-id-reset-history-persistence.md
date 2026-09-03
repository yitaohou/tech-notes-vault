---
title: Anonymous ID Reset but History Persistence
aliases: []
tags:
- concept
summary: 用户可以通过删除本机的匿名 ID 文件来在下次启动时获得一个全新的匿名编号，但换新之前积累的历史记录依然挂在旧编号上，不会被清除。
created: '2026-09-03'
updated: '2026-09-03'
---

# Anonymous ID Reset but History Persistence

%% ytkb:def %%
用户可以通过删除本机的匿名 ID 文件来在下次启动时获得一个全新的匿名编号，但换新之前积累的历史记录依然挂在旧编号上，不会被清除。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-safety-security]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:WrwA7FYGPdQ %%
### 来自 [[2026-09-02-deepseek-harness-开源-11-天爆-5-个漏洞ai-读网页电脑被控有人-api-额度]]
- 删除本机保存匿名 ID 的文件后，下次启动 Harness 会生成一串全新的 ID，但换新之前的历史使用记录仍然挂在旧的编号下面，不会随之消失。（[06:02](https://youtu.be/WrwA7FYGPdQ?t=362)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[deepseek-harness-anonymous-id-mechanism]]
%% ytkb:end %%
