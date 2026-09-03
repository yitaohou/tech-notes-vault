---
title: Trajectory Log Append-Only Property
aliases: []
tags:
- concept
summary: 轨迹日志只能追加写入、不能修改或删除已写入记录的防篡改特性。
created: '2026-09-03'
updated: '2026-09-03'
---

# Trajectory Log Append-Only Property

%% ytkb:def %%
轨迹日志只能追加写入、不能修改或删除已写入记录的防篡改特性。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-safety-security]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:WrwA7FYGPdQ %%
### 来自 [[2026-09-02-deepseek-harness-开源-11-天爆-5-个漏洞ai-读网页电脑被控有人-api-额度]]
- 轨迹日志只能追加新记录，已写入的记录无法被修改或删除，即使攻击者拿到了命令执行权限、想删除记录消灭证据也做不到，因为日志本身具有防篡改性。（[33:14](https://youtu.be/WrwA7FYGPdQ?t=1994)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[deepseek-harness-trajectory-log]]
%% ytkb:end %%
