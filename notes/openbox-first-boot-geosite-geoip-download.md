---
title: Open-Box First Boot Geosite/GeoIP Download
aliases: []
tags:
- concept
summary: Open-Box 首次启动时需要联网下载 Geosite 和 GeoIP 数据库，若数据库下载不下来则程序无法正常启动。
created: '2026-09-08'
updated: '2026-09-08'
---

# Open-Box First Boot Geosite/GeoIP Download

%% ytkb:def %%
Open-Box 首次启动时需要联网下载 Geosite 和 GeoIP 数据库，若数据库下载不下来则程序无法正常启动。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-software-router-tools]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:G_7AmjfSRQ8 %%
### 来自 [[2026-09-07-最新软路由代理-open-box-发布全图形极简配置超越-openclashnikkipasswal]]
- Open-Box 第一次启动时会自动去下载 Geosite 和 GeoIP 数据库，如果这两个数据库下载不下来，程序就会启动失败。（[21:08](https://youtu.be/G_7AmjfSRQ8?t=1268)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[openbox-list-file-fetch-failure-blocks-startup]]
%% ytkb:end %%
