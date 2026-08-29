---
title: Enum Parameter Design
aliases: []
tags:
- concept
summary: 把工具参数定义为枚举类型（如状态只能是 pending、inprogress、completed），模型看到取值范围即可自行理解如何使用，无需额外说明。
created: '2026-08-26'
updated: '2026-08-26'
---

# Enum Parameter Design

%% ytkb:def %%
把工具参数定义为枚举类型（如状态只能是 pending、inprogress、completed），模型看到取值范围即可自行理解如何使用，无需额外说明。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-agent-architecture]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:Lle_EJljIoo %%
### 来自 [[2026-07-26-删掉80提示词后claude-5反而变强了anthropic官方的做减法哲学]]
- Todo 工具把状态参数定义为 pending、inprogress、completed 三个枚举值，模型看到后就能自己理解如何调用，无需长篇文字说明。（[03:01](https://youtu.be/Lle_EJljIoo?t=181)）
- 在枚举参数基础上再加一句「保持只有一个任务处于 in_progress 状态」这样的简短说明，就足以定义期望的行为。（[03:01](https://youtu.be/Lle_EJljIoo?t=181)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[interface-design-over-prompting]]
%% ytkb:end %%
