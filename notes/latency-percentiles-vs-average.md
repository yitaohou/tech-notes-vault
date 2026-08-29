---
title: Latency Percentiles vs Average
aliases: []
tags:
- concept
summary: 由于 latency 在不同请求间波动较大，用百分位数观察比简单平均值更能反映真实表现的度量原则。
created: '2026-08-26'
updated: '2026-08-26'
---

# Latency Percentiles vs Average

%% ytkb:def %%
由于 latency 在不同请求间波动较大，用百分位数观察比简单平均值更能反映真实表现的度量原则。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-observability]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:JV3pL1_mn2M %%
### 来自 [[2025-04-01-ai-engineering-in-76-minutes-complete-coursespeedr]]
- 由于 latency 在不同请求间波动较大，用百分位数（percentiles）来观察比简单的平均值更能反映推理性能的真实表现。（[60:04](https://youtu.be/JV3pL1_mn2M?t=3604)）
%% ytkb:end %%

%% ytkb:video:CyLYY_xb5bQ %%
### 来自 [[2025-08-25-you-can-learn-ai-agent-system-design-in-19-min-rag]]
- 客服 agent 系统的响应延迟目标通常按百分位数设定，例如50%的请求响应时间低于1秒、95%的请求响应时间低于2.5秒。（[00:00](https://youtu.be/CyLYY_xb5bQ?t=0)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[inference-latency]]
- [[response-latency-satisfaction-impact]]
%% ytkb:end %%
