---
title: Rule Routing vs Real Routing
aliases: []
tags:
- concept
summary: Open-Box 提供的诊断功能：对输入的域名同时展示理论上应匹配的规则路由，以及路由器真实执行一遍后得到的真实路由，用于对比验证是否存在黑洞。
created: '2026-09-08'
updated: '2026-09-08'
---

# Rule Routing vs Real Routing

%% ytkb:def %%
Open-Box 提供的诊断功能：对输入的域名同时展示理论上应匹配的规则路由，以及路由器真实执行一遍后得到的真实路由，用于对比验证是否存在黑洞。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-software-router-tools]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:G_7AmjfSRQ8 %%
### 来自 [[2026-09-07-最新软路由代理-open-box-发布全图形极简配置超越-openclashnikkipasswal]]
- 在 Open-Box 的规则页面输入域名（如 www.baidu.com）后，系统会同时展示「规则路由」（理论上应匹配的规则集、DNS 和出口）与「真实路由」（路由器真实执行一遍得到的结果），两者对比即可验证是否存在黑洞。（[06:03](https://youtu.be/G_7AmjfSRQ8?t=363)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[open-box-baidu-routing-case]]
- [[open-box-google-routing-case]]
- [[software-router-blackhole-problem]]
%% ytkb:end %%
