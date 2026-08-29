---
title: Observability 的日志黄金法则
aliases: []
tags:
- concept
summary: observability 的黄金法则是「记录一切」（log everything），当指标提示出现问题时，详细日志能帮助准确定位故障点。
created: '2026-08-26'
updated: '2026-08-26'
---

# Observability 的日志黄金法则

%% ytkb:def %%
observability 的黄金法则是「记录一切」（log everything），当指标提示出现问题时，详细日志能帮助准确定位故障点。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-observability]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:JV3pL1_mn2M %%
### 来自 [[2025-04-01-ai-engineering-in-76-minutes-complete-coursespeedr]]
- pipeline 中每个组件都应有自己的指标，并且要理解这些指标与业务北极星指标（Northstar metric）的关联；同时应遵循「记录一切」的黄金法则，以便出问题时通过详细日志定位原因。（[72:08](https://youtu.be/JV3pL1_mn2M?t=4328)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[ai-system-observability]]
- [[observability-metrics-mttd-mttr-cfr]]
%% ytkb:end %%
