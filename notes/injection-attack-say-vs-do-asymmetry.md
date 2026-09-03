---
title: Injection Attack Say-vs-Do Asymmetry
aliases: []
tags:
- concept
summary: 指prompt injection攻击诱导AI「说出秘密」（成功率35.7%）明显比诱导AI「真正调用敏感工具做出行动」（成功率2.5%）容易得多的发现。
created: '2026-09-03'
updated: '2026-09-03'
---

# Injection Attack Say-vs-Do Asymmetry

%% ytkb:def %%
指prompt injection攻击诱导AI「说出秘密」（成功率35.7%）明显比诱导AI「真正调用敏感工具做出行动」（成功率2.5%）容易得多的发现。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-safety-security]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:WrwA7FYGPdQ %%
### 来自 [[2026-09-02-deepseek-harness-开源-11-天爆-5-个漏洞ai-读网页电脑被控有人-api-额度]]
- 对比两组测评数据可以看出，被忽悠着把秘密说出口相对容易，但被诱导真正调用敏感工具动手执行操作则难得多。（[21:08](https://youtu.be/WrwA7FYGPdQ?t=1268)）
- 尽管诱导AI调用敏感工具的成功率只有2.5%，看似很低，但在大规模任务场景下（如数千次调用）仍意味着会出现相当数量的成功攻击，不能被当作绝对安全。（[21:08](https://youtu.be/WrwA7FYGPdQ?t=1268)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[agentic-write-actions]]
- [[information-extraction-attack]]
%% ytkb:end %%
