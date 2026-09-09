---
title: Open-Box Google Routing Case
aliases: []
tags:
- concept
summary: 以访问谷歌为例展示 Open-Box 规则路由与真实路由一致性验证的具体案例。
created: '2026-09-08'
updated: '2026-09-08'
---

# Open-Box Google Routing Case

%% ytkb:def %%
以访问谷歌为例展示 Open-Box 规则路由与真实路由一致性验证的具体案例。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-software-router-tools]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:G_7AmjfSRQ8 %%
### 来自 [[2026-09-07-最新软路由代理-open-box-发布全图形极简配置超越-openclashnikkipasswal]]
- 以谷歌为例：规则路由匹配到谷歌站点集后应通过代理 DNS 访问、出口为美国节点；真实路由验证显示 DNS 请求确实是通过美国节点发出的，与规则路由预期一致。（[06:03](https://youtu.be/G_7AmjfSRQ8?t=363)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[rule-routing-vs-real-routing]]
%% ytkb:end %%
