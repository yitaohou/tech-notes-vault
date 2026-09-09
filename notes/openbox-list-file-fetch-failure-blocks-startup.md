---
title: Open-Box List File Fetch Failure Blocks Startup
aliases: []
tags:
- concept
summary: 如果自定义域名集绑定的 .list 规则文件链接无法拉取，会直接导致 Open-Box 启动报错。
created: '2026-09-08'
updated: '2026-09-08'
---

# Open-Box List File Fetch Failure Blocks Startup

%% ytkb:def %%
如果自定义域名集绑定的 .list 规则文件链接无法拉取，会直接导致 Open-Box 启动报错。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-software-router-tools]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:G_7AmjfSRQ8 %%
### 来自 [[2026-09-07-最新软路由代理-open-box-发布全图形极简配置超越-openclashnikkipasswal]]
- 如果自建域名集配置的 .list 规则文件链接拉取不到，会导致 Open-Box 启动时报错，需要先到目标分流里删掉该规则集的链接，才能让程序继续完成数据库下载并正常启动。（[21:08](https://youtu.be/G_7AmjfSRQ8?t=1268)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[openbox-first-boot-geosite-geoip-download]]
%% ytkb:end %%
