---
title: Hidden Injection Payload Location
aliases: []
tags:
- concept
summary: 指攻击者把恶意注入指令藏在PDF元数据、表格单元格、Unicode零宽字符等非正文隐蔽位置，以提高prompt injection攻击成功率的技术手法。
created: '2026-09-03'
updated: '2026-09-03'
---

# Hidden Injection Payload Location

%% ytkb:def %%
指攻击者把恶意注入指令藏在PDF元数据、表格单元格、Unicode零宽字符等非正文隐蔽位置，以提高prompt injection攻击成功率的技术手法。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-safety-security]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:WrwA7FYGPdQ %%
### 来自 [[2026-09-02-deepseek-harness-开源-11-天爆-5-个漏洞ai-读网页电脑被控有人-api-额度]]
- 测试对比发现，恶意指令若直接写在文档正文等普通文本中让AI读取，455次测试成功率为0%，全部被防住。（[21:08](https://youtu.be/WrwA7FYGPdQ?t=1268)）
- 把同样的恶意指令改藏进PDF元数据、表格单元格或Unicode零宽字符（如零宽空格）等隐蔽位置后，455次测试成功率从0%上升到25.5%（成功116次）。（[21:08](https://youtu.be/WrwA7FYGPdQ?t=1268)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[prompt-injection-attack]]
- [[tencent-zhuque-lab-security-assessment]]
%% ytkb:end %%
