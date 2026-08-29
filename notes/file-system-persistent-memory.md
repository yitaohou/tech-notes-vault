---
title: File System as Persistent Memory (Harness Design Pattern)
aliases: []
tags:
- concept
summary: Harness设计的第二种模式：把文件系统作为持久记忆来管理长周期 agent 运行中产生的丰富状态和产物，而非把所有日志都塞进上下文。
created: '2026-08-26'
updated: '2026-08-26'
---

# File System as Persistent Memory (Harness Design Pattern)

%% ytkb:def %%
Harness设计的第二种模式：把文件系统作为持久记忆来管理长周期 agent 运行中产生的丰富状态和产物，而非把所有日志都塞进上下文。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-agent-architecture]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:z_F0z7wF5XU %%
### 来自 [[2026-07-09-ai自我递归改进先要靠harness工程-lilian-weng最新长文-反馈循环-三个设计模式-核]]
- 长周期 agent 运行会产生实验日志、代码差异、论文摘要、错误栈、历史执行轨迹等产物，这些内容长度很快会超过模型训练时的上下文窗口，因此需要用文件系统而非上下文来存储持久状态。（[03:03](https://youtu.be/z_F0z7wF5XU?t=183)）
- 读写编辑文件系统本来就是大模型的基础能力，通常靠 bash 命令实现，所以用文件管理持久记忆这种方式能天然随着核心模型能力的提升而变强。（[03:03](https://youtu.be/z_F0z7wF5XU?t=183)）
%% ytkb:end %%

%% ytkb:video:KgiwIEBeOHw %%
### 来自 [[2026-06-16-什么是循环工程loop-engineering-coding-agent-子agent-mcp协议]]
- 循环的记忆系统可以是一个普通的Markdown文件，也可以是一个项目看板，任何能存在于单次对话之外、用来记录已完成事项和待办事项的载体都可以。（[13:25](https://youtu.be/KgiwIEBeOHw?t=805)）
- Agent本身会忘记任务进度，但代码仓库和状态文件不会，这正是外部持久化记忆的价值所在。（[13:45](https://youtu.be/KgiwIEBeOHw?t=825)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[agent-memory-system]]
- [[ai-context-amnesia-session]]
- [[context-rot]]
- [[flexible-architecture-for-ai-advances]]
- [[loop-engineering]]
%% ytkb:end %%
