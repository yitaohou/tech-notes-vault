---
title: Automated Daily Triage Skill Workflow
aliases: []
tags:
- concept
summary: 循环工程中的一种典型工作流：自动化任务每天调用分类Skill，读取CI失败记录、未解决issue和最近代码提交，整理问题并写入Markdown文件或项目看板。
created: '2026-08-26'
updated: '2026-08-26'
---

# Automated Daily Triage Skill Workflow

%% ytkb:def %%
循环工程中的一种典型工作流：自动化任务每天调用分类Skill，读取CI失败记录、未解决issue和最近代码提交，整理问题并写入Markdown文件或项目看板。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-coding-agents]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:KgiwIEBeOHw %%
### 来自 [[2026-06-16-什么是循环工程loop-engineering-coding-agent-子agent-mcp协议]]
- 一个典型场景是：每天早上一个自动化任务在代码仓库上运行，调用分类Skill读取前一天的持续集成失败记录、未解决issue、最近的代码提交，把发现的问题整理好写入Markdown文件或项目看板。（[14:00](https://youtu.be/KgiwIEBeOHw?t=840)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[file-system-persistent-memory]]
- [[loop-engineering]]
%% ytkb:end %%
