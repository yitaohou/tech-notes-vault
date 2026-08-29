---
title: MCP-based Connectors
aliases: []
tags:
- concept
summary: 基于 MCP 协议构建、用于把 Agent 接入日常使用的各类工具（如需求跟踪器、数据库、测试环境接口、即时通讯工具）的组件。
created: '2026-08-26'
updated: '2026-08-26'
---

# MCP-based Connectors

%% ytkb:def %%
基于 MCP 协议构建、用于把 Agent 接入日常使用的各类工具（如需求跟踪器、数据库、测试环境接口、即时通讯工具）的组件。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-agent-architecture]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:KgiwIEBeOHw %%
### 来自 [[2026-06-16-什么是循环工程loop-engineering-coding-agent-子agent-mcp协议]]
- 如果一个循环只能操作本地文件系统，能做的事情就非常有限；连接器的作用就是让 Agent 能够读取需求跟踪器、查询数据库、调用测试环境接口，甚至在即时通讯工具里发送消息。（[09:03](https://youtu.be/KgiwIEBeOHw?t=543)）
- 因为 Codex 和 Claude Code 都支持 MCP 协议，所以为其中一款工具编写的连接器，通常在另一款工具里也可以直接复用。（[09:03](https://youtu.be/KgiwIEBeOHw?t=543)）
%% ytkb:end %%

%% ytkb:video:KuClyhvSzXk %%
### 来自 [[2026-06-18-frontend-system-design-explained-w-senior-engineer]]
- 前端工程师应掌握如何使用 MCP server，并针对团队所用的设计工具搭建对应连接器（若尚无现成连接器则需自行开发），再接入 Claude Code（企业中使用最广）或 Codex 等 coding agent。（[21:07](https://youtu.be/KuClyhvSzXk?t=1267)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[figma-mcp-design-to-code]]
- [[model-context-protocol]]
- [[plugins-content-distribution]]
%% ytkb:end %%
