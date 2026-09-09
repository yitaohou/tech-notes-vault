---
title: Open-Box Rule Top-Down Matching
aliases: []
tags:
- concept
summary: Open-Box 中分流规则的命中顺序是从上往下依次匹配，排在前面的规则若已包含某域名或 IP，后面同类规则将不再生效。
created: '2026-09-08'
updated: '2026-09-08'
---

# Open-Box Rule Top-Down Matching

%% ytkb:def %%
Open-Box 中分流规则的命中顺序是从上往下依次匹配，排在前面的规则若已包含某域名或 IP，后面同类规则将不再生效。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-software-router-tools]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:G_7AmjfSRQ8 %%
### 来自 [[2026-09-07-最新软路由代理-open-box-发布全图形极简配置超越-openclashnikkipasswal]]
- 规则命中是从上往下匹配的，如果某个域名集规则排在后面、而前面的规则已经包含了相同的域名或 IP，那么这条规则可能永远不会被命中，因此需要把它拖到最上面确保生效。（[21:08](https://youtu.be/G_7AmjfSRQ8?t=1268)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[openbox-rule-display-order-vs-hit-order]]
%% ytkb:end %%
