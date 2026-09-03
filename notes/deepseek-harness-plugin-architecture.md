---
title: DeepSeek Harness Plugin Architecture
aliases: []
tags:
- concept
summary: DeepSeek Harness 奉行的'一切皆插件'设计理念，模型、工具、沙箱、界面乃至 agent 主循环核心逻辑都可作为插件替换或卸载。
created: '2026-09-03'
updated: '2026-09-03'
---

# DeepSeek Harness Plugin Architecture

%% ytkb:def %%
DeepSeek Harness 奉行的'一切皆插件'设计理念，模型、工具、沙箱、界面乃至 agent 主循环核心逻辑都可作为插件替换或卸载。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-agent-architecture]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:WrwA7FYGPdQ %%
### 来自 [[2026-09-02-deepseek-harness-开源-11-天爆-5-个漏洞ai-读网页电脑被控有人-api-额度]]
- DeepSeek Harness 中模型、工具、沙箱（sandbox）、网页界面，甚至决定 agent 下一步行为的主循环核心逻辑本身都是可插拔的插件，理论上可以整体替换重启。（[00:00](https://youtu.be/WrwA7FYGPdQ?t=0)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[deepseek-harness]]
%% ytkb:end %%
