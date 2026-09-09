---
title: Open-Box Baidu Routing Case
aliases: []
tags:
- concept
summary: 以访问百度为例展示 Open-Box 规则路由与真实路由完全一致、验证无黑洞的具体案例。
created: '2026-09-08'
updated: '2026-09-08'
---

# Open-Box Baidu Routing Case

%% ytkb:def %%
以访问百度为例展示 Open-Box 规则路由与真实路由完全一致、验证无黑洞的具体案例。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-software-router-tools]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:G_7AmjfSRQ8 %%
### 来自 [[2026-09-07-最新软路由代理-open-box-发布全图形极简配置超越-openclashnikkipasswal]]
- 以百度为例：规则路由按域名后缀 baidu.com 匹配到「国内」规则集，对应直连 DNS 和国内直连出口；真实路由验证显示确实用直连 DNS 解析出百度真实 IP，并通过国内直连节点访问，返回 HTTP 200，规则路由与真实路由完全一致，没有黑洞。（[06:03](https://youtu.be/G_7AmjfSRQ8?t=363)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[rule-routing-vs-real-routing]]
%% ytkb:end %%
