---
title: Sub-agent Code Review Separation
aliases: []
tags:
- concept
summary: 把写代码的角色和检查代码的角色拆分给不同 Agent、以便发现第一个 Agent 忽略或主动回避问题的子 Agent 设计模式。
created: '2026-08-26'
updated: '2026-08-26'
---

# Sub-agent Code Review Separation

%% ytkb:def %%
把写代码的角色和检查代码的角色拆分给不同 Agent、以便发现第一个 Agent 忽略或主动回避问题的子 Agent 设计模式。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-agent-architecture]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:KgiwIEBeOHw %%
### 来自 [[2026-06-16-什么是循环工程loop-engineering-coding-agent-子agent-mcp协议]]
- 让写代码的模型自己评审自己的代码往往会出现判断宽松的问题，很难发现自身的逻辑漏洞，而使用第二个拥有不同指令甚至不同模型的 Agent 来评审，就能发现第一个 Agent 忽略掉或主动回避的问题。（[09:03](https://youtu.be/KgiwIEBeOHw?t=543)）
- 在 Codex 中，只有当用户主动要求时系统才会生成子 Agent，多个子 Agent 可以同时并行运行，最后把结果合并成一个统一的答案。（[09:03](https://youtu.be/KgiwIEBeOHw?t=543)）
- 子 Agent 可以在专门的配置目录里用配置文件定义，每个子 Agent 可以设置名称、描述和指令。（[09:03](https://youtu.be/KgiwIEBeOHw?t=543)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[claude-code-agent-teams]]
- [[code-review-skill]]
%% ytkb:end %%
