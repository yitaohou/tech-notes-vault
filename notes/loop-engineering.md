---
title: Loop Engineering
aliases: []
tags:
- concept
summary: 循环工程（Loop Engineering）是硅谷AI技术圈提出的新概念，指用程序员设计的自动化循环系统来驱动Coding Agent运转，取代人工逐轮手动写提示词调用Agent的协作模式。
created: '2026-08-26'
updated: '2026-08-26'
---

# Loop Engineering

%% ytkb:def %%
循环工程（Loop Engineering）是硅谷AI技术圈提出的新概念，指用程序员设计的自动化循环系统来驱动Coding Agent运转，取代人工逐轮手动写提示词调用Agent的协作模式。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-coding-agents]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:KgiwIEBeOHw %%
### 来自 [[2026-06-16-什么是循环工程loop-engineering-coding-agent-子agent-mcp协议]]
- 循环工程的核心理念是：程序员未来的核心工作可能不再是直接给Coding Agent写提示词，而是设计一套能自动驱动Agent运转的循环系统。（[00:00](https://youtu.be/KgiwIEBeOHw?t=0)）
- 循环工程处于 Agent Harness Engineering 的上一层，是一个跑在计时器上、能自主生成辅助子 Agent 并自我驱动持续运转的运行环境。（[03:01](https://youtu.be/KgiwIEBeOHw?t=181)）
- 循环工程的核心是只设计一次循环规则，之后不需要对每个步骤手动提示，AI 就能按规则自动运行下去。（[15:04](https://youtu.be/KgiwIEBeOHw?t=904)）
- 同一套循环规则不依赖具体工具，无论放在 Codex 还是 Claude Code 中都能跑通，因为两者底层模块是一样的。（[15:04](https://youtu.be/KgiwIEBeOHw?t=904)）
- 循环工程改变的是工作的形态，并没有把人从工作中剔除出去。（[15:04](https://youtu.be/KgiwIEBeOHw?t=904)）
- 循环工程仍处于非常早期的阶段，如果完全依赖自动化循环修复问题而不做人工审核，产品质量大概率会下滑，甚至陷入越修问题越多的恶性循环。（[15:04](https://youtu.be/KgiwIEBeOHw?t=904)）
- 循环最终能产生什么样的结果完全取决于使用它的人，两个人搭建出完全一样的循环也可能得到截然相反的结果。（[15:04](https://youtu.be/KgiwIEBeOHw?t=904)）
- 循环工程不用否定直接提示 Agent 的价值，找到自动化循环与手动提示两者之间的平衡才是最重要的。（[15:04](https://youtu.be/KgiwIEBeOHw?t=904)）
- 设计循环比写提示词更难，因为循环规则需要预先考虑各种情况，而不是像提示词那样临场调整。（[15:04](https://youtu.be/KgiwIEBeOHw?t=904)）
- Boris Cherny 认为AI时代程序员的工作本身并没有变简单，而是工作的杠杆点发生了转移：以前杠杆来自写好提示词，现在杠杆来自设计好一套能持续运行的系统，即所谓的『循环工程』。（[18:06](https://youtu.be/KgiwIEBeOHw?t=1086)）
- 循环工程的实践建议是：搭建循环时要以工程师的身份去设计系统，而不是做一个只会按下启动键、被动等待结果的人。（[18:06](https://youtu.be/KgiwIEBeOHw?t=1086)）
- 把子Agent分工、独立持久记忆等模块全部拼到一起后，一个完整的循环就从单次的任务执行，变成了一个小型的自主工作系统。（[13:55](https://youtu.be/KgiwIEBeOHw?t=835)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[coding-agent]]
- [[coding-agent-harness-convergence]]
- [[cognitive-surrender]]
- [[explorer-implementer-verifier-agent-pattern]]
- [[factory-model]]
- [[file-system-persistent-memory]]
- [[harness-engineering]]
- [[paradigm-shift-human-designs-context]]
- [[prompt-engineering]]
%% ytkb:end %%
