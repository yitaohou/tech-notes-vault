---
title: Trajectory Log Replay Diagnosis
aliases: []
tags:
- concept
summary: 通过对比正常与遭受提示注入攻击后的轨迹日志回放，来精确定位攻击生效点和模型异常行为起点的分析方法。
created: '2026-09-03'
updated: '2026-09-03'
---

# Trajectory Log Replay Diagnosis

%% ytkb:def %%
通过对比正常与遭受提示注入攻击后的轨迹日志回放，来精确定位攻击生效点和模型异常行为起点的分析方法。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-safety-security]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:WrwA7FYGPdQ %%
### 来自 [[2026-09-02-deepseek-harness-开源-11-天爆-5-个漏洞ai-读网页电脑被控有人-api-额度]]
- 对比正常绘话与遭受注入后绘话的轨迹日志回放，可以精确看到第几轮读取了恶意文件、读回来了什么内容，以及模型从哪一步开始出现异常行为，注入的生效点一目了然。（[33:14](https://youtu.be/WrwA7FYGPdQ?t=1994)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[deepseek-harness-trajectory-log]]
- [[incident-response-timeline-localization]]
%% ytkb:end %%
