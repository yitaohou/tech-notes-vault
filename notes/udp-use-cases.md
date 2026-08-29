---
title: UDP Use Cases
aliases: []
tags:
- concept
summary: UDP 协议适用的典型场景，即那些能容忍少量数据丢失、更看重实时性的应用。
created: '2026-08-26'
updated: '2026-08-26'
---

# UDP Use Cases

%% ytkb:def %%
UDP 协议适用的典型场景，即那些能容忍少量数据丢失、更看重实时性的应用。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[backend-networking-protocols]] · [[backend]]
%% ytkb:end %%

## 要点

%% ytkb:video:oYxTTirKY8M %%
### 来自 [[2026-05-26-system-design-explained-apis-databases-caching-cdn]]
- 视频通话、在线游戏和直播是 UDP 的典型应用场景：即使某个数据包丢失（如通话中对方网络卡顿导致片段丢失），也无需重新获取这部分旧数据，可以直接跳过继续处理后续数据包。（[60:11](https://youtu.be/oYxTTirKY8M?t=3611)）
- 视频流、直播和游戏等场景通常使用 UDP，因为这些场景更看重传输速度而非每个数据包都完整送达。（[60:11](https://youtu.be/oYxTTirKY8M?t=3611)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[udp-protocol]]
%% ytkb:end %%
