---
title: Software Router Blackhole Problem
aliases: []
tags:
- concept
summary: 传统软路由系统（如 OpenClash、Nikki）中站点访问规则不透明的问题：用户难以得知某个站点具体如何被 DNS 解析、走的是哪个出口，排查起来极其复杂。
created: '2026-09-08'
updated: '2026-09-08'
---

# Software Router Blackhole Problem

%% ytkb:def %%
传统软路由系统（如 OpenClash、Nikki）中站点访问规则不透明的问题：用户难以得知某个站点具体如何被 DNS 解析、走的是哪个出口，排查起来极其复杂。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-software-router-tools]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:G_7AmjfSRQ8 %%
### 来自 [[2026-09-07-最新软路由代理-open-box-发布全图形极简配置超越-openclashnikkipasswal]]
- 传统软路由（如 OpenClash、Nikki）存在多种「黑洞」，其中之一是站点访问规则黑洞：站点的 DNS 解析方式与实际出口难以追溯，排查非常复杂。（[06:03](https://youtu.be/G_7AmjfSRQ8?t=363)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[rule-routing-vs-real-routing]]
%% ytkb:end %%
