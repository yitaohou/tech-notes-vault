---
title: MCP UI
aliases: []
tags:
- concept
summary: MCP UI 是连接传统网页应用与 LLM 驱动应用之间的桥梁机制，使聊天场景下 LLM 的回答不再局限于纯文本，还能渲染出实际的 UI 组件（如产品卡片、地图）。
created: '2026-08-26'
updated: '2026-08-26'
---

# MCP UI

%% ytkb:def %%
MCP UI 是连接传统网页应用与 LLM 驱动应用之间的桥梁机制，使聊天场景下 LLM 的回答不再局限于纯文本，还能渲染出实际的 UI 组件（如产品卡片、地图）。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-agent-architecture]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:KuClyhvSzXk %%
### 来自 [[2026-06-18-frontend-system-design-explained-w-senior-engineer]]
- MCP UI 使聊天应用中 LLM 的回答不再局限于纯文本，还能渲染出实际的 UI 组件，例如产品卡片或地图。（[24:07](https://youtu.be/KuClyhvSzXk?t=1447)）
- 要让 LLM 的回答中包含可渲染的 UI 组件，前端需要与后端进行通信才能完成组件渲染，这正是 MCP UI 所要解决的问题。（[24:07](https://youtu.be/KuClyhvSzXk?t=1447)）
- MCP UI 的工作机制是：model harness 在上下文中提供 tool registry 与已接入的 MCP servers 信息（连同用户 prompt）一起传给 LLM，LLM 返回的内容中除文字回答外，还包含渲染特定 UI 组件的指令。（[24:07](https://youtu.be/KuClyhvSzXk?t=1447)）
- 前端会解析 LLM 返回内容中携带的渲染指令，并据此把对应的 UI 组件实际渲染到页面上。（[24:07](https://youtu.be/KuClyhvSzXk?t=1447)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[mcp-connectors]]
%% ytkb:end %%
