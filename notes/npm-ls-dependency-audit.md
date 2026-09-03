---
title: npm ls 依赖审计
aliases: []
tags:
- concept
summary: 使用「npm ls --all」命令列出插件背后完整依赖树，用于检查依赖包是否存在供应链风险的做法。
created: '2026-09-03'
updated: '2026-09-03'
---

# npm ls 依赖审计

%% ytkb:def %%
使用「npm ls --all」命令列出插件背后完整依赖树，用于检查依赖包是否存在供应链风险的做法。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-safety-security]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:WrwA7FYGPdQ %%
### 来自 [[2026-09-02-deepseek-harness-开源-11-天爆-5-个漏洞ai-读网页电脑被控有人-api-额度]]
- 插件自身代码干净不代表依赖也干净，攻击者常把恶意代码埋在依赖包里实施供应链攻击，因此还需用「npm ls --all」列出插件的完整依赖清单逐一检查。（[30:12](https://youtu.be/WrwA7FYGPdQ?t=1812)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[dependency-count-anomaly-signal]]
- [[typosquatting-dependency-risk]]
%% ytkb:end %%
