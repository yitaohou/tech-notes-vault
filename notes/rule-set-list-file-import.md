---
title: .list File Rule Set Import
aliases: []
tags:
- concept
summary: 除内置 Geosite/GeoIP 外，Open-Box 目标分流还支持通过 Raw 链接导入自定义 .list 格式域名文件作为规则集。
created: '2026-09-08'
updated: '2026-09-08'
---

# .list File Rule Set Import

%% ytkb:def %%
除内置 Geosite/GeoIP 外，Open-Box 目标分流还支持通过 Raw 链接导入自定义 .list 格式域名文件作为规则集。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-software-router-tools]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:G_7AmjfSRQ8 %%
### 来自 [[2026-09-07-最新软路由代理-open-box-发布全图形极简配置超越-openclashnikkipasswal]]
- 自定义域名可以整理成 .list 文件，复制该文件的 Raw 链接后粘贴到「规则集链接」字段，即可批量导入为规则集，无需逐条手动添加。（[18:07](https://youtu.be/G_7AmjfSRQ8?t=1087)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[geosite-geoip-builtin-support]]
- [[target-routing-domain-set]]
%% ytkb:end %%
