---
title: Open-Box Per-Service Routing Policy
aliases: []
tags:
- concept
summary: Open-Box 支持针对具体服务单独指定分流出口节点的策略配置能力。
created: '2026-09-08'
updated: '2026-09-08'
---

# Open-Box Per-Service Routing Policy

%% ytkb:def %%
Open-Box 支持针对具体服务单独指定分流出口节点的策略配置能力。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-software-router-tools]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:G_7AmjfSRQ8 %%
### 来自 [[2026-09-07-最新软路由代理-open-box-发布全图形极简配置超越-openclashnikkipasswal]]
- Open-Box 的分流策略可针对具体服务单独指定出口，例如示例中 Google 走美国自动、Microsoft 走直连、Apple/GitHub/油管走香港自动、TikTok 走台湾节点，且可灵活切换。（[06:03](https://youtu.be/G_7AmjfSRQ8?t=363)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[open-box-node-grouping]]
%% ytkb:end %%
