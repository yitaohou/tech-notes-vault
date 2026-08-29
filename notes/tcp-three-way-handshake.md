---
title: TCP Three-Way Handshake
aliases: []
tags:
- concept
summary: TCP 建立连接所使用的三步握手过程：客户端发起请求、服务器确认并同步、客户端再次确认，完成后连接建立。
created: '2026-08-26'
updated: '2026-08-26'
---

# TCP Three-Way Handshake

%% ytkb:def %%
TCP 建立连接所使用的三步握手过程：客户端发起请求、服务器确认并同步、客户端再次确认，完成后连接建立。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[backend-networking-protocols]] · [[backend]]
%% ytkb:end %%

## 要点

%% ytkb:video:oYxTTirKY8M %%
### 来自 [[2026-05-26-system-design-explained-apis-databases-caching-cdn]]
- TCP 三步握手流程为：第一步客户端向服务器发送请求；第二步服务器 SYNC 并 ACK 该请求；第三步客户端向服务器发送 ACK，至此客户端与服务器之间的连接建立完成，双方才能在此连接上开始收发数据。（[60:11](https://youtu.be/oYxTTirKY8M?t=3611)）
- TCP 是面向连接的协议，在发送任何数据之前都需要先通过三次握手（three-way handshake）在客户端和服务端之间建立连接。（[57:11](https://youtu.be/oYxTTirKY8M?t=3431)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[tcp-protocol]]
%% ytkb:end %%
