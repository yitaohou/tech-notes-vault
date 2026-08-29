---
video_id: QBHTbtWSECg
title: 'System Design Mock Interview: Design Leetcode ft. Ex Google Engineer'
source: '[[2026-03-15-system-design-mock-interview-design-leetcode-ft-ex]]'
tags:
- summary
_gen:
  prompt_hash: 209b52739480c30c61b7dcc0392dfa4aa0deb99654ee921af5e045409c961f85
  task_hash: 7ca79ab507b3ad0a8ec82c08d90fa72e384d320a3741ebd32a4e0f611cee5904
  schema_version: 1
  model: sonnet
  generated_at: '2026-08-26T19:45:46+00:00'
---

## 一句话总结

这是一场以"设计 LeetCode"为题的系统设计模拟面试（ft. 前 Google 工程师），完整走完从 [[system-design-functional-requirements-first|需求梳理]]、核心实体建模、API 设计、数据库选型，到用户代码安全执行（VM vs container vs serverless）、实时排行榜实现，再到缓存与水平扩展的全流程，是一份可直接对照复盘的系统设计面试范本。

## 核心内容

### 需求梳理：先功能后非功能，明确划定范围

面试按标准套路展开：先写标题，再逐条列出 [[leetcode-core-functional-requirements|核心功能需求]]——浏览题目列表、查看题目并用任意语言编码、提交后即时获得测试结果反馈（00:01），并额外加入 [[leetcode-live-leaderboard|实时排行榜]]需求，因为 LeetCode 的周赛/双周赛是热门场景。同时用 [[system-design-requirement-scoping|范围界定技巧]]把 authorization、profile creation、payment gateway 等显式列为 out of scope（00:01），[[out-of-scope-requirements-technique|这一手法]]贯穿全场，包括后续的备份保留策略（09:03）。

非功能性需求上，选择 [[availability-over-consistency-tradeoff|可用性优先于一致性]]（03:01, 36:11）：不同用户看到的题目数量可以有约10道的偏差（[[eventual-consistency-problem-count-example|示例]]），代码提交反馈也可以延迟，但系统不能宕机（[[eventual-consistency-submission-feedback]]）。同时设定 [[low-latency-response-time-requirement|低延迟目标]]：理想1-2秒返回结果，上限5秒（03:01）。可扩展性方面，先做 [[concurrent-user-estimation|并发估算]]：整体用户数亿级，但 contest 场景并发约5万-10万（06:02），并明确 [[dau-mau-scale-requirement|DAU/MAU 规模]]为百万级 DAU、数亿级 MAU（09:03）。此外还提出 [[fault-tolerance-requirement|容错要求]]，避免 [[single-point-of-failure|单点故障]]，采用 [[distributed-architecture-avoid-spof|分布式多节点架构]]配合 [[consistent-hashing-failover|一致性哈希做故障转移]]（09:03）。[[submission-isolation-requirement|提交隔离]]、[[time-limit-exceeded-handling|超时处理]]也被列为独立关注点（06:02）。

### 核心实体与 API 设计

[[core-entities-identification-step|识别核心实体]]得出：problem、user、solution、leaderboard（09:03, 12:05），并做出 [[system-design-scale-assumption|规模假设]]：约4000-5000道题、约百万用户（12:05）。

API 层面采用 [[restful-api-design|RESTful 设计]]：[[rest-api-get-all-problems|GET /problems]] 支持 [[pagination-api-design|分页]]（默认 page=1、limit=100，13:40）和 [[api-endpoint-filtering|过滤]]（按难度、提交次数、[[problem-type-tabs-filter|题目类型 tab]]，15:06），并遵循 [[pagination-decision-heuristic|分页判断经验]]：几百条可不分页，数千条则必须分页（14:20）；过滤优先 [[filter-via-existing-endpoint|复用已有接口]]而非新建（15:06）。[[rest-api-get-problem-by-id|按 ID 获取题目详情]]接口需要 [[language-filter-problem-submission|语言过滤参数]]，因为 [[problem-supports-multiple-languages|题目支持多语言]]，且 [[language-based-routing-architecture|语言决定了请求要路由到哪个执行节点]]，并需返回 [[code-template-by-language|对应语言的代码模板]]（15:06, 18:07）。

[[submit-problem-api-design|提交 API]]设计为 POST，携带 problem ID、code（字符串）、language（18:07），采用 [[code-as-string-payload|代码即字符串]]的语言无关设计，可选 [[code-encoding-encryption-submission|编码加密]]作为扩展点。[[leaderboard-api-design|排行榜 API]]是 GET 请求，按 competition ID 查询并支持 [[leaderboard-pagination|分页]]（默认100条，18:07）。

### 数据库选型与 schema

架构上，[[leetcode-system-design-basic-architecture|基础架构]]是 client ↔ API server ↔ database 的双向交互（21:07）。数据库选择 [[dynamodb-choice-for-schema-flexibility|DynamoDB]]而非关系型数据库，依据 [[relational-vs-nosql-selection-heuristic|选型经验法则]]：无 join 需求、实体关系简单时用 NoSQL（21:07），并指出如今 [[sql-nosql-feature-convergence|SQL/NoSQL 功能正在相互靠拢]]。[[problem-entity-schema-design|Problem 实体]]遵循 [[minimal-schema-first-design-principle|最小 schema 优先原则]]，只含 ID、description、stats、test cases（21:07），且用 [[nosql-nested-document-storage|嵌套文档]]直接存储测试用例（24:07）。

### 代码执行安全：从 API server 直跑到容器方案

这是全场重点讨论。直接在 [[unsafe-api-server-code-execution|API server 上跑用户代码]]极其危险：可能被植入 malware 删数据、造成资源占用型 DDoS、且缺乏隔离和容错会导致长时间宕机（24:07）。改用 [[vm-based-code-execution|VM 方案]]隔离性更好但存在 [[vm-resource-waste-per-instance|资源浪费]]、[[vm-cost-overhead|维护成本高]]等问题（24:07, 27:08）。

最终方案转向 [[container-lightweight-architecture|容器方案]]：更轻量、[[container-elastic-scaling|弹性伸缩]]更好，代价是 [[vm-container-isolation-tradeoff|隔离性弱于 VM]]（因 [[container-shared-kernel-isolation|共享内核]]），可用 [[container-orchestration-services|ECS/EKS/Kubernetes]]编排，并借助 [[docker-environment-consistency|Docker 保证环境一致性]]（27:08）。具体落地为 [[container-per-language-isolation|按语言分容器]]，容器内部支持多提交并发，并用 [[nested-runtime-scoping|进程级作用域]]做二次隔离（30:08），[[language-based-request-routing|按语言路由请求]]。面试官也指出 [[containerization-operational-overhead|容器化运维成本高]]，可考虑 [[serverless-architecture-alternative|Serverless（Lambda/Cloud Functions）]]作为替代（30:08）。安全兜底还包括 [[execution-timeout-limit|执行超时限制]]防死循环（39:13）和 [[code-sandbox-temp-directory-cleanup|临时目录定期清理]]（36:11）。

### 实时排行榜的设计演进

排行榜没有单独建表，而是 [[leaderboard-as-derived-query|作为 submissions 表上的派生查询]]（33:10）。[[leetcode-submissions-schema|submissions 表]]字段含 ID、competition ID、timestamp、test case result、runtime、error status（33:10），[[leaderboard-ranking-by-completion-time|按完成时间排名]]，[[partition-key-selection-by-query-pattern|以 competition ID 作为 partition key]]而非 submission ID，因为查询模式是按比赛聚合（33:10），这本质上是 [[partition-key-indexing-lookup-speedup|建索引加速查找]]。过程中发现 schema 缺 [[submission-table-user-id|user ID]]需补上，并需 [[competition-submission-filtering|过滤掉非参赛的练习提交]]（36:11）。[[leaderboard-query-flow|端到端流程]]可以用 [[single-api-consolidation|单个 API]]完成查询+聚合+排名（36:11），[[query-optimization-deferred|效率优化留到后面再谈]]。

获取排行榜数据从最朴素的 [[leaderboard-polling|轮询数据库]]（39:13）演进到引入 [[leaderboard-caching|缓存]]（周期计算+缓存读取，牺牲实时性换取更低数据库负载），缓存框架可选 Redis（[[cache-framework-choice]]），并权衡 [[in-memory-vs-distributed-cache|单机内存缓存 vs 分布式缓存]]（39:13）。客户端侧配合 [[client-polling-leaderboard|周期性拉取]]实现近似实时更新（36:11）。

### 扩展性收尾：从单机到分布式

面对10万甚至百万级并发，先讨论 [[vertical-scaling|垂直扩展]]的局限，转向 [[horizontal-scaling|水平扩展]]（42:13）。执行层采用 [[per-language-runtime-containers|按语言独立水平扩展的 runtime 容器]]，估算约需 [[runtime-service-capacity-estimation|三四台 runtime server]]（42:13）。引入 [[message-queue-load-smoothing|消息队列]]削峰填谷，[[worker-pull-pattern|worker 主动拉取任务]]模式配合 [[exponential-backoff-retry|指数退避重试]]处理失败（42:13）。为支持跨语言判题，测试用例采用 [[language-agnostic-test-case-definition|语言无关的定义]]和 [[language-agnostic-test-case-serialization|JSON 序列化]]，各语言只需实现自己的反序列化（42:13, 45:13）。数据库层面用 [[master-slave-database-replication|master-slave 复制]]做容错和扩展，但 [[database-scaling-selective-replication|按需选择性应用]]：Problems 表数据量小暂不需要，Submissions 表因写入频繁则确实需要（45:13）。

## 值得记住的细节

- 03:01 — 低延迟目标：理想1-2秒返回提交结果，上限5秒
- 06:02 / 09:03 — 规模估算：contest 期间并发5万-10万；整体百万级 DAU、数亿级 MAU
- 12:05 — 规模假设：约4000-5000道题目，约百万用户
- 13:40 — GET /problems 默认分页参数：page=1、limit=100
- 14:20 — 分页经验法则：几百条（如200）可不分页，数千条必须分页
- 18:07 — 排行榜分页默认限制100条选手
- 18:07 — 提交 API：POST，字段为 problem ID + submission{code: string, language: string}
- 33:10 — submissions 表字段：ID、competition ID、timestamp、test case result、runtime（秒）、error status
- 33:10 — partition key 选 competition ID 而非 submission ID（按查询模式决定）
- 39:13 — 排行榜轮询周期示例：每5秒或10秒查询一次数据库
- 39:13 — 执行超时上限示例：2秒或5秒，超时即判 TLE
- 42:13 — runtime server 数量估算：约三四台可支撑百万级用户
- 45:13 — Problems 表当前约4000条数据，暂不需要 master-slave 复制；若扩大到数十万条才需要考虑
- 45:13 — 推荐资源：[[hello-interview-resource|Hello Interview]] 博客/视频、[[shrians-jen-youtube-channel|Shrians Jen YouTube 频道]]

## 这个视频适合谁 / 可以跳过什么

适合正在准备系统设计面试、想看一个完整实战案例（尤其是想学习"如何在面试中逐步权衡取舍并把讨论收敛"）的人，对于纠结 VM vs container vs serverless 代码执行方案、以及排行榜这类"派生查询 vs 独立表"设计取舍特别有参考价值。如果已经很熟悉基础的 functional/non-functional requirements 梳理套路（00:01-09:03 部分）或 RESTful 分页/过滤这类通用 API 设计套路（13:10-18:07），可以适当快进，重点看 24:07 之后的代码执行安全方案演进和 33:10 之后的排行榜与扩展性设计。
