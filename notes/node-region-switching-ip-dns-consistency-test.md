---
title: Node Region Switching IP/DNS Consistency Test
aliases: []
tags:
- concept
summary: 切换代理站点集到不同地区节点后，通过 DNS 泄露检测工具验证出口 IP 与 DNS 解析地区是否与所选节点地区一致的测试方法。
created: '2026-09-08'
updated: '2026-09-08'
---

# Node Region Switching IP/DNS Consistency Test

%% ytkb:def %%
切换代理站点集到不同地区节点后，通过 DNS 泄露检测工具验证出口 IP 与 DNS 解析地区是否与所选节点地区一致的测试方法。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-network-quality-testing]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:G_7AmjfSRQ8 %%
### 来自 [[2026-09-07-最新软路由代理-open-box-发布全图形极简配置超越-openclashnikkipasswal]]
- 把代理站点集分别切换为香港、日本、美国的自动节点后，用 DNS 泄露检测工具刷新验证，IP 和 DNS 显示的地区均与所切换的节点地区完全一致，说明没有出现 DNS 泄露。（[03:00](https://youtu.be/G_7AmjfSRQ8?t=180)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[app-specific-traffic-routing-policy]]
%% ytkb:end %%
