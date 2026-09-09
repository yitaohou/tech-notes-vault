---
title: Open-Box Same Subnet Requirement
aliases: []
tags:
- concept
summary: 通过 SSH 连接配置 Open-Box 时，要求发起连接的设备与 OpenWrt 路由器处于同一局域网网段。
created: '2026-09-08'
updated: '2026-09-08'
---

# Open-Box Same Subnet Requirement

%% ytkb:def %%
通过 SSH 连接配置 Open-Box 时，要求发起连接的设备与 OpenWrt 路由器处于同一局域网网段。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-software-router-tools]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:G_7AmjfSRQ8 %%
### 来自 [[2026-09-07-最新软路由代理-open-box-发布全图形极简配置超越-openclashnikkipasswal]]
- 用来配置 Open-Box 的设备网络环境必须和刷入 OpenWrt 的路由器处于同一网段，否则无法建立 SSH 连接。（[12:05](https://youtu.be/G_7AmjfSRQ8?t=725)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[hexhub-ssh-tool]]
%% ytkb:end %%
