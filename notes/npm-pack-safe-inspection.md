---
title: npm pack 安全下载检查
aliases: []
tags:
- concept
summary: 使用「npm pack 插件名」命令把 npm 包下载为压缩文件而不执行其中任何安装脚本，用于在不安装的前提下先行检查包内容的做法。
created: '2026-09-03'
updated: '2026-09-03'
---

# npm pack 安全下载检查

%% ytkb:def %%
使用「npm pack 插件名」命令把 npm 包下载为压缩文件而不执行其中任何安装脚本，用于在不安装的前提下先行检查包内容的做法。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-safety-security]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:WrwA7FYGPdQ %%
### 来自 [[2026-09-02-deepseek-harness-开源-11-天爆-5-个漏洞ai-读网页电脑被控有人-api-额度]]
- 审查代码阶段应先用「npm pack 插件名」把包下载成压缩文件，该命令不会触发包内任何安装脚本，之后再解压检查内容，而不是直接执行安装。（[30:12](https://youtu.be/WrwA7FYGPdQ?t=1812)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[grep-dangerous-keywords-plugin-review]]
%% ytkb:end %%
