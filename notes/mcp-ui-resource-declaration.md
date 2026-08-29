---
title: MCP UI Resource Declaration
aliases: []
tags:
- concept
summary: MCP UI 中声明一个 resource 的模式：告诉 LLM 该资源存在、适用场景以及应返回的内容格式，前端应用负责解析并渲染成对应 UI。
created: '2026-08-26'
updated: '2026-08-26'
---

# MCP UI Resource Declaration

%% ytkb:def %%
MCP UI 中声明一个 resource 的模式：告诉 LLM 该资源存在、适用场景以及应返回的内容格式，前端应用负责解析并渲染成对应 UI。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-agent-architecture]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:KuClyhvSzXk %%
### 来自 [[2026-06-18-frontend-system-design-explained-w-senior-engineer]]
- MCP UI 的实现方式是在协议层声明 resource，说明其使用场景和 LLM 应给出的回答格式，再由前端解析该声明并渲染出对应界面。（[27:07](https://youtu.be/KuClyhvSzXk?t=1627)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[design-to-code-mcp]]
%% ytkb:end %%
