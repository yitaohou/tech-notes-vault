---
title: On-Demand Tool Loading
aliases: []
tags:
- concept
summary: 渐进式披露理念下工具的加载方式：Agent 一开始只知道某个工具存在，真正需要使用时才加载该工具的具体定义。
created: '2026-08-26'
updated: '2026-08-26'
---

# On-Demand Tool Loading

%% ytkb:def %%
渐进式披露理念下工具的加载方式：Agent 一开始只知道某个工具存在，真正需要使用时才加载该工具的具体定义。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-agent-architecture]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:Lle_EJljIoo %%
### 来自 [[2026-07-26-删掉80提示词后claude-5反而变强了anthropic官方的做减法哲学]]
- 工具的定义也可以像规则一样按需加载：Agent 起初只知道有这么个工具，等真正需要用到时才去加载该工具的具体定义，类似主函数保持干净、业务逻辑封装进模块按需调用。（[06:01](https://youtu.be/Lle_EJljIoo?t=361)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[claude-skills]]
- [[progressive-disclosure]]
%% ytkb:end %%
