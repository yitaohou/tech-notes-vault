---
title: DeepSeek Harness Prompt Injection Success Rate
aliases: []
tags:
- concept
summary: 针对 DeepSeek Harness 的 prompt injection 攻击在覆盖全部入口、藏法与攻击方法（共约14000多种组合）后测得的整体攻击成功率统计结果。
created: '2026-09-03'
updated: '2026-09-03'
---

# DeepSeek Harness Prompt Injection Success Rate

%% ytkb:def %%
针对 DeepSeek Harness 的 prompt injection 攻击在覆盖全部入口、藏法与攻击方法（共约14000多种组合）后测得的整体攻击成功率统计结果。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-safety-security]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:WrwA7FYGPdQ %%
### 来自 [[2026-09-02-deepseek-harness-开源-11-天爆-5-个漏洞ai-读网页电脑被控有人-api-额度]]
- 研究团队把所有能测的攻击入口、隐藏方式和攻击方法组合全部测了一遍，共约14000多处，测得整体完全成功率为5.6%，即每100次攻击中约有5-6次完全得手。（[24:08](https://youtu.be/WrwA7FYGPdQ?t=1448)）
- 该成功率使用了两种判定器交叉验证：一种是基于规则匹配判断攻击是否成功，测得5.6%；另一种是用其他厂商的AI大模型做语义判断，测得5.3%，两者结果基本一致，说明数据可信。（[24:08](https://youtu.be/WrwA7FYGPdQ?t=1448)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[prompt-injection-attack]]
%% ytkb:end %%
