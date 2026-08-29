---
video_id: QBHTbtWSECg
url: https://www.youtube.com/watch?v=QBHTbtWSECg
title: 'System Design Mock Interview: Design Leetcode ft. Ex Google Engineer'
channel: Anubhav Sethi
published: '2026-03-15'
duration: '48:38'
transcript_origin: subs
tags:
- video
---

# System Design Mock Interview: Design Leetcode ft. Ex Google Engineer

摘要: [[2026-03-15-system-design-mock-interview-design-leetcode-ft-ex-summary|完整摘要]]

## 知识点

- [[api-endpoint-filtering]] — 获取题目列表的接口除了分页参数外，还被设计为支持对题目集合进行过滤（filtering）。（[13:10](https://youtu.be/QBHTbtWSECg?t=790)）
- [[availability-over-consistency-tradeoff]] — 针对 LeetCode 系统的非功能需求，明确选择让系统始终保持高可用（highly available），可以接受 eventual consistency，而不是追求强一致性。（[03:01](https://youtu.be/QBHTbtWSECg?t=181)）
- [[cache-framework-choice]] — 实现排行榜缓存时可以选择 Redis 等缓存框架，但具体使用哪种缓存框架在系统设计面试中通常不是需要深入展开的重点。（[39:13](https://youtu.be/QBHTbtWSECg?t=2353)）
- [[client-polling-leaderboard]] — 客户端可以根据比赛的持续时长，周期性地重新拉取（refetch）排行榜数据，以此实现近似实时的更新效果。（[36:11](https://youtu.be/QBHTbtWSECg?t=2171)）
- [[code-as-string-payload]] — 将完整代码作为字符串传给服务器可以让接口设计更简单，且实现上与具体语言无关（language agnostic）。（[18:07](https://youtu.be/QBHTbtWSECg?t=1087)）
- [[code-encoding-encryption-submission]] — 可以对提交的代码进行编码和加密处理，之后在 compiler 侧再解码，作为初期方案的一个可扩展点。（[18:07](https://youtu.be/QBHTbtWSECg?t=1087)）
- [[code-execution-sandboxing]] — 用户提交的代码可能包含 malware，如果不加隔离运行，可能导致整个 judge 服务被攻击者拖垮。（[06:02](https://youtu.be/QBHTbtWSECg?t=362)）
- [[code-sandbox-temp-directory-cleanup]] — 为了保障用户提交代码执行时的 isolation 和 security，可以让容器把所有输出写入临时目录，并根据设定的时间间隔或提交用户数量定期清理这些临时文件。（[36:11](https://youtu.be/QBHTbtWSECg?t=2171)）
- [[code-template-by-language]] — 当用户选择编程语言（如 Python）后，系统需要提供该语言对应的函数模板，涉及 formatter client、template client 和 compiler client 等组件。（[18:07](https://youtu.be/QBHTbtWSECg?t=1087)）
- [[competition-submission-filtering]] — 如果用户不是在参加比赛、只是单纯练习刷题，即使他解题速度比所有参赛者都快，这条提交记录对该 competition 的排行榜也是冗余信息，因为根本用不到它，应当被过滤掉。（[36:11](https://youtu.be/QBHTbtWSECg?t=2171)）
- [[concurrent-user-estimation]] — 系统整体的月活或日活用户可能达到数亿级别，但针对 LeetCode contest 这一具体场景，并发用户量级可估算为 5 万到 10 万左右。（[06:02](https://youtu.be/QBHTbtWSECg?t=362)）
- [[consistent-hashing-failover]] — 在多节点分布式架构中使用 consistent hashing，当某个节点宕机时，其余存活节点仍能继续承接流量。（[09:03](https://youtu.be/QBHTbtWSECg?t=543)）
- [[container-elastic-scaling]] — 尽管隔离性弱于 VM，container 在资源利用率和弹性伸缩（根据需求快速扩容或缩容）方面通常表现更好。（[27:08](https://youtu.be/QBHTbtWSECg?t=1628)）
- [[container-lightweight-architecture]] — container（如 Docker image）不需要像 VM 那样拥有自己独立的内存和计算资源，因此更加轻量。（[27:08](https://youtu.be/QBHTbtWSECg?t=1628)）
- [[container-orchestration-services]] — AWS 提供 ECS、EKS 等 elastic container service，而 Kubernetes 则是由 Google 主导开发的另一款流行容器编排系统，二者都能用于管理 container 化的部署。（[27:08](https://youtu.be/QBHTbtWSECg?t=1628)）
- [[container-per-language-isolation]] — 针对代码执行系统中支持的每种编程语言，可以为其分配一个独立的 container 来实现隔离运行。（[27:08](https://youtu.be/QBHTbtWSECg?t=1628)）
- [[container-per-language-runtime]] — 为避免每个用户提交都单独占用一个容器造成资源浪费，设计上按语言划分容器（如一个容器跑 Python、一个容器跑 Java），并在同一容器内同时运行多个提交或结果校验任务。（[30:08](https://youtu.be/QBHTbtWSECg?t=1808)）
- [[container-shared-kernel-isolation]] — 容器方案的隔离并非严格意义上的完全隔离，而是因为共享内核（shared kernel），只能为单个进程提供相对较好的隔离性。（[30:08](https://youtu.be/QBHTbtWSECg?t=1808)）
- [[containerization-operational-overhead]] — 面试官指出，用容器化方案实现在线代码执行系统会比较有挑战性，需要大量的优化和配置工作，同时也存在安全方面的隐患。（[30:08](https://youtu.be/QBHTbtWSECg?t=1808)）
- [[contest-traffic-spike-pattern]] — 设计可扩展性需求时要注意，比赛期间的并发用户量（QPS）会远高于非比赛时段，属于突发流量场景。（[09:03](https://youtu.be/QBHTbtWSECg?t=543)）
- [[contest-traffic-surge]] — 由于平台存在 biweekly 和 weekly contest，这些时段会出现活跃用户的激增（surge）。（[06:02](https://youtu.be/QBHTbtWSECg?t=362)）
- [[core-entities-identification-step]] — 在明确完可扩展性和容错性等非功能性需求后，系统设计讨论的下一步是识别核心实体，例如为 LeetCode 类系统识别出「problem」实体。（[09:03](https://youtu.be/QBHTbtWSECg?t=543)）
- [[database-scaling-selective-replication]] — 在 LeetCode 系统设计中，Problems 数据库因数据量小（当前约 4000 条问题）暂不需要 master-slave 复制，但若未来题目规模扩大到数十万，则也需要考虑该架构；而 Submissions 数据库因数据量大、写入频繁，当下就确实需要该架构。（[45:13](https://youtu.be/QBHTbtWSECg?t=2713)）
- [[dau-mau-scale-requirement]] — 系统设计中提出的可扩展性需求是要支持百万级 daily active users 和数亿级 monthly active users。（[09:03](https://youtu.be/QBHTbtWSECg?t=543)）
- [[distributed-architecture-avoid-spof]] — 为避免单点故障，系统应采用分布式架构、部署多个节点，而不是让所有流量都依赖单一服务器。（[09:03](https://youtu.be/QBHTbtWSECg?t=543)）
- [[docker-environment-consistency]] — 使用 Docker 时环境被封装在镜像内部，因此不同环境间部署该服务会变得更容易，避免了「环境不一致导致部署困难」的问题。（[27:08](https://youtu.be/QBHTbtWSECg?t=1628)）
- [[dynamodb]] — DynamoDB 是一种 NoSQL 数据库，适合不需要 join 操作、且实体间关系较少的数据存储场景。（[21:07](https://youtu.be/QBHTbtWSECg?t=1267)）
- [[dynamodb-choice-for-schema-flexibility]] — 面试者为编程题目存储选择 DynamoDB 而非关系型数据库，理由之一是 NoSQL 提供的 schema 灵活性，便于未来扩展新的属性字段。（[21:07](https://youtu.be/QBHTbtWSECg?t=1267)）
- [[eventual-consistency-problem-count-example]] — 在 LeetCode 系统设计中，不同用户在同一时刻看到的题目列表数量可以有小幅偏差（例如相差约10道），这种偏差属于可接受的 eventual consistency 范围，比服务不可用要好得多。（[03:01](https://youtu.be/QBHTbtWSECg?t=181)）
- [[eventual-consistency-submission-feedback]] — 在 LeetCode 系统设计中，代码提交后拿到全部测试用例的即时反馈可以有延迟（eventual consistency），但服务本身不能宕机——保持系统可用比让所有节点对同一提交结果立刻达成一致更重要。（[03:01](https://youtu.be/QBHTbtWSECg?t=181)）
- [[execution-timeout-limit]] — 为防止用户提交的代码出现死循环，可以对代码执行设置超时上限（如2秒或5秒），一旦超过该时限就终止执行（TLE），从而阻止无限循环并进一步保障运行用户代码的安全性。（[39:13](https://youtu.be/QBHTbtWSECg?t=2353)）
- [[exponential-backoff-retry]] — 当代码执行容器处理某次提交失败时，可以引入指数退避重试机制，即每次失败后的重试等待时间随重试次数增加而变长。（[42:13](https://youtu.be/QBHTbtWSECg?t=2533)）
- [[fault-tolerance-requirement]] — 系统设计中提出的非功能性需求之一是尽可能实现 fault tolerance，即没有单一节点是唯一的故障来源。（[09:03](https://youtu.be/QBHTbtWSECg?t=543)）
- [[filter-via-existing-endpoint]] — 题目列表的过滤功能既可以在原有的 get all 接口上加过滤参数实现，也可以单独建一个接口，但认为目前没必要单独建。（[15:06](https://youtu.be/QBHTbtWSECg?t=906)）
- [[hello-interview-resource]] — 受访者推荐 Hello Interview 作为系统设计学习资源，认为其博客和视频内容对纯粹对系统设计感兴趣的人、以及即将面试而临时抱佛脚的人都很有帮助。（[45:13](https://youtu.be/QBHTbtWSECg?t=2713)）
- [[horizontal-scaling]] — 面对用户数持续增长，单纯升级单机的 CPU 和内存并非长期方案，因为算力堆叠终会无法满足需求，更优做法是水平扩展系统，用多台服务器分摊负载。（[42:13](https://youtu.be/QBHTbtWSECg?t=2533)）
- [[in-memory-vs-distributed-cache]] — 排行榜缓存可以选择使用 in-memory cache（单机内存缓存），也可以选择 distributed cache（分布式缓存），两者在架构设计上是可权衡的替代方案。（[39:13](https://youtu.be/QBHTbtWSECg?t=2353)）
- [[language-agnostic-test-case-definition]] — 尽管同一道题在不同编程语言下的数据结构实现不同（如 Java 和 Python 的树结构对象不同），跨语言判题系统仍可为每道题设计统一的测试用例定义，用与语言无关的元数据描述输入输出，从而在不同语言间复用同一套测试逻辑。（[42:13](https://youtu.be/QBHTbtWSECg?t=2533)）
- [[language-agnostic-test-case-serialization]] — 为支持多语言判题（如 online judge 系统），可将测试用例统一序列化（例如用 JSON），每种语言只需实现自己的反序列化逻辑（如 C++ 反序列化成 hashmap，Python 反序列化成 dictionary），核心测试数据本身保持不变。（[45:13](https://youtu.be/QBHTbtWSECg?t=2713)）
- [[language-based-request-routing]] — 用户针对某个 problem 提交代码时，系统会依据所用编程语言把相关请求路由到该语言对应的 runtime 容器进行处理。（[30:08](https://youtu.be/QBHTbtWSECg?t=1808)）
- [[language-based-routing-architecture]] — 语言过滤的核心原因是：系统需要知道该把请求路由到哪个语言专属的编译节点或服务器去执行，因为不同语言通常对应不同的执行节点。（[15:06](https://youtu.be/QBHTbtWSECg?t=906)）
- [[language-filter-problem-submission]] — 获取单个题目详情的接口需要一个语言过滤参数，用来标明用户将用哪种语言提交代码。（[15:06](https://youtu.be/QBHTbtWSECg?t=906)）
- [[leaderboard-api-design]] — 获取比赛排行榜使用 GET 请求，需要传入 competition ID 作为参数来定位具体比赛的排行数据。（[18:07](https://youtu.be/QBHTbtWSECg?t=1087)）
- [[leaderboard-as-derived-query]] — 设计决策：leaderboard 不需要独立的表 schema，只需在 submissions 表上编写查询（拉取 submitted time、test case result、runtime、error 等字段）即可生成排行榜。（[33:10](https://youtu.be/QBHTbtWSECg?t=1990)）
- [[leaderboard-caching]] — 为降低轮询数据库带来的负载，可以引入缓存机制：周期性计算排行榜并将结果存入缓存，读取请求优先从缓存获取，从而减少数据库负载，但代价是排行榜数据不是严格实时的，本质上仍是在定期查询数据库后缓存结果。（[39:13](https://youtu.be/QBHTbtWSECg?t=2353)）
- [[leaderboard-pagination]] — 排行榜接口需要支持分页，以便每页只展示有限数量的选手，例如默认限制为 100 条，且该限制可根据需要调整。（[18:07](https://youtu.be/QBHTbtWSECg?t=1087)）
- [[leaderboard-polling]] — 获取竞赛排行榜最直接的做法是周期性轮询数据库（例如每5秒或10秒查询一次），但这种方式会带来较高的数据库负载和较高的延迟，且无法在大量用户同时参赛时良好扩展。（[39:13](https://youtu.be/QBHTbtWSECg?t=2353)）
- [[leaderboard-query-filter-criteria]] — leaderboard 查询逻辑：先按 competition ID 过滤，再按提交时间排序，只保留 test case result 为通过（passed）的记录，必要时进一步按 runtime 和 error 过滤，并可统计提交（submit）次数。（[33:10](https://youtu.be/QBHTbtWSECg?t=1990)）
- [[leaderboard-query-flow]] — 实时排行榜的端到端流程是：客户端针对某个 competition ID 查询排行榜，后端聚合该比赛下的所有提交并按用户排名，再将排行榜结果返回给客户端。（[36:11](https://youtu.be/QBHTbtWSECg?t=2171)）
- [[leaderboard-ranking-by-completion-time]] — submissions 表中记录时间戳（timestamp）的原因是排行榜排名规则依据完成速度：越快完成得分越高的排名。（[33:10](https://youtu.be/QBHTbtWSECg?t=1990)）
- [[leetcode-core-functional-requirements]] — LeetCode 系统设计的核心功能需求包括：（1）浏览可用编程题目列表；（2）查看具体题目并用任意语言编写代码解答；（3）提交解答后即时获得反馈，判断代码是否通过全部测试用例。（[00:01](https://youtu.be/QBHTbtWSECg?t=1)）
- [[leetcode-live-leaderboard]] — LeetCode 平台的一大热门功能是每周和双周举行的编程竞赛（contest），因此系统设计需要包含一个 live leaderboard，用于实时展示竞赛期间参赛者的排名。（[00:01](https://youtu.be/QBHTbtWSECg?t=1)）
- [[leetcode-submissions-schema]] — submissions 表的字段设计包括：ID、关联特定 contest 的 competition ID、提交时间戳、test case result（通过或失败）、代码运行所需的 runtime（秒），以及 error status。（[33:10](https://youtu.be/QBHTbtWSECg?t=1990)）
- [[leetcode-system-design-basic-architecture]] — 设计编程题目查看系统的基础架构为 client 发送 GET 请求给 API server，API server 再读写 database；这个交互是双向的，因为既要读取题目也要提交解答（submit）。（[21:07](https://youtu.be/QBHTbtWSECg?t=1267)）
- [[live-leaderboard-schema-extension]] — 对于 lead code 周赛和双周赛的实时排行榜（live leaderboard）需求，现有架构基本可以直接复用，只需新增一张存储提交详情及其关联信息的 schema，无需大改架构。（[30:08](https://youtu.be/QBHTbtWSECg?t=1808)）
- [[low-latency-requirement-judge-system]] — 判题系统需要满足低延迟要求，例如把提交结果返回时间限制在类似 2 秒或 5 秒以内，具体阈值留待后续讨论确定。（[06:02](https://youtu.be/QBHTbtWSECg?t=362)）
- [[low-latency-response-time-requirement]] — 该 LeetCode 系统被定位为低延迟平台，理想情况下应在 1-2 秒内返回提交结果，最长可接受的时间上限为 5 秒。（[03:01](https://youtu.be/QBHTbtWSECg?t=181)）
- [[master-slave-database-replication]] — 采用 master-slave 架构的数据库中，若主库（primary）宕机，可以将某个从库（replica）提升为新的主库，从而避免单点故障（single point of failure）。（[45:13](https://youtu.be/QBHTbtWSECg?t=2713)）
- [[message-queue-load-smoothing]] — 在 API server 与代码执行容器之间引入 message queue，可以更好地路由请求并平滑突发流量高峰，避免容器直接承受流量冲击。（[42:13](https://youtu.be/QBHTbtWSECg?t=2533)）
- [[minimal-schema-first-design-principle]] — 系统设计面试中常见做法是数据库 schema 设计初期只保留最基本必要的字段列表，其余 metadata 视需要再补充。（[21:07](https://youtu.be/QBHTbtWSECg?t=1267)）
- [[nested-runtime-scoping]] — 语言级 runtime 容器内部还可以进一步按每个 problem 划出独立的 process 级 runtime 作用域，实现语言层和进程层的两层隔离划分。（[30:08](https://youtu.be/QBHTbtWSECg?t=1808)）
- [[nosql-nested-document-storage]] — 在设计 coding problem 数据模型时，NoSQL 可以把一道题目的所有测试用例作为 nested 数据直接存储在同一个 document 里，这是相对 SQL 数据库的一项优势。（[24:07](https://youtu.be/QBHTbtWSECg?t=1447)）
- [[out-of-scope-deferral-technique]] — 对于备份保留期限这类非核心细节，可以先标记为 out of scope，如果面试结束前还有剩余时间再回来讨论。（[09:03](https://youtu.be/QBHTbtWSECg?t=543)）
- [[out-of-scope-requirements-technique]] — 设计 LeetCode 系统时，将 authentication and authorization、user profiles、payment gateway、per-user analytics 都列为 out of scope requirements，写下来以确保双方对功能范围达成一致。（[03:01](https://youtu.be/QBHTbtWSECg?t=181)）
- [[pagination-api-design]] — 获取题目列表的 GET /problems 接口设计为支持分页，默认 page=1、limit=100，即首次请求返回前 100 道题目。（[13:40](https://youtu.be/QBHTbtWSECg?t=820)）
- [[pagination-decision-heuristic]] — 面试者认为若题目总数在几百的量级（如 200 条）可以不用分页，但当数量达到数千量级时始终应该使用分页以避免所有内容显示在同一页面。（[14:20](https://youtu.be/QBHTbtWSECg?t=860)）
- [[partition-key-indexing-lookup-speedup]] — 把 competition ID 设为 submissions 表的 partition key，本质上是在该字段上建立索引，使得按特定 competition 拉取全部提交记录的查询速度更快。（[33:10](https://youtu.be/QBHTbtWSECg?t=1990)）
- [[partition-key-selection-by-query-pattern]] — submissions 表选择 competition ID 而非 submission ID 作为 partition key，因为查询主要按某个 competition 聚合并排序其下所有提交，而非按单条 submission ID 查找。（[33:10](https://youtu.be/QBHTbtWSECg?t=1990)）
- [[passive-vs-contest-usage-pattern]] — 平时的被动使用没有时间约束，用户可以随时查看题目、之后再提交；而比赛期间用户会集中访问同一组题目。（[09:03](https://youtu.be/QBHTbtWSECg?t=543)）
- [[per-language-runtime-containers]] — 在多语言代码执行系统中，可以为每种编程语言配置专属的 runtime container，并让这些容器各自独立进行水平扩展。（[42:13](https://youtu.be/QBHTbtWSECg?t=2533)）
- [[problem-entity-schema-design]] — 编程题目系统中 Problem 实体的最小属性集合包括：ID、description、提交次数等 stats、以及 test cases。（[21:07](https://youtu.be/QBHTbtWSECg?t=1267)）
- [[problem-list-filtering]] — 题目列表可以按难度（easy、medium、hard）或提交次数等维度进行过滤。（[15:06](https://youtu.be/QBHTbtWSECg?t=906)）
- [[problem-supports-multiple-languages]] — 系统设计上，一道题目应当支持关联多种编程语言，用户可选择其中一种进行提交。（[15:06](https://youtu.be/QBHTbtWSECg?t=906)）
- [[problem-type-tabs-filter]] — 除了难度和语言，题目列表还可以按类型分 tab，例如区分 DSA 题目和 LLD（低级设计）题目。（[15:06](https://youtu.be/QBHTbtWSECg?t=906)）
- [[query-optimization-deferred]] — 在系统设计中可以先提出一个能跑通整体逻辑的查询方案作为好的起点，具体的查询效率问题可以放到后面再讨论和优化，不必一开始就追求最优。（[36:11](https://youtu.be/QBHTbtWSECg?t=2171)）
- [[relational-vs-nosql-selection-heuristic]] — 选择关系型数据库（RDBMS）而非 NoSQL 的经验法则是：当数据实体间存在明显的 relations、或确定需要 join 多张表查询时才使用关系型数据库，否则 NoSQL 更合适。（[21:07](https://youtu.be/QBHTbtWSECg?t=1267)）
- [[rest-api-get-all-problems]] — 系统需要一个简单的 GET 接口用于返回所有题目的列表。（[15:06](https://youtu.be/QBHTbtWSECg?t=906)）
- [[rest-api-get-problem-by-id]] — 用户点击某道题目后，需要通过 problem ID 获取该题的描述、约束条件、样例输入测试用例等全部元数据。（[15:06](https://youtu.be/QBHTbtWSECg?t=906)）
- [[restful-api-design]] — 系统的 API 路由被设计为 RESTful API 端点，用于定义获取题目列表、过滤题目等各类查询操作。（[13:10](https://youtu.be/QBHTbtWSECg?t=790)）
- [[runtime-service-capacity-estimation]] — 对于面向百万级用户的在线代码执行服务，大约三四台 runtime server 即可支撑负载，具体数字应基于实际业务量做更精确的估算。（[42:13](https://youtu.be/QBHTbtWSECg?t=2533)）
- [[scalability-requirement-user-count]] — 在设计判题系统前应先弄清楚需要支持多少用户，用户量越大就越需要考虑更具可扩展性的方案。（[06:02](https://youtu.be/QBHTbtWSECg?t=362)）
- [[serverless-architecture-alternative]] — 面试官建议用 serverless 架构（如 Google Cloud Functions、AWS Lambda）来替代自建容器化方案运行用户提交的代码，以降低运维和安全复杂度。（[30:08](https://youtu.be/QBHTbtWSECg?t=1808)）
- [[shrians-jen-youtube-channel]] — 受访者提到 Shrians Jen 的 YouTube 频道是自己准备系统设计面试时发现的另一个有帮助的资源。（[45:13](https://youtu.be/QBHTbtWSECg?t=2713)）
- [[single-api-consolidation]] — 排行榜功能不必拆成多个 API（一个查询提交、一个聚合排名、一个返回结果），可以用单个 API 执行一条查询：按 competition ID 筛选出所有提交，再按 user ID 分组统计出排名，视情况也可以拆成两个 API。（[36:11](https://youtu.be/QBHTbtWSECg?t=2171)）
- [[single-point-of-failure]] — 如果所有查询都被路由到某一台特定服务器，一旦该服务器宕机，就会导致所有查询都无法返回结果，这就是单点故障。（[09:03](https://youtu.be/QBHTbtWSECg?t=543)）
- [[sql-nosql-feature-convergence]] — 如今 SQL 数据库和 NoSQL 数据库都在相互吸收对方的功能特性，两者的界限不再像早期那样泾渭分明。（[21:07](https://youtu.be/QBHTbtWSECg?t=1267)）
- [[submission-backup-retention-policy]] — 系统设计中可以为用户提交记录保留备份，具体保留时长（如两年或五年）属于可后续讨论的细节。（[09:03](https://youtu.be/QBHTbtWSECg?t=543)）
- [[submission-isolation-requirement]] — 系统需要保证每个用户提交的代码在运行测试用例时彼此隔离，不会互相干扰，也不会影响当前系统的稳定性。（[06:02](https://youtu.be/QBHTbtWSECg?t=362)）
- [[submission-table-user-id]] — submission 表如果缺少 user ID 字段，就无法知道某条提交属于哪个用户，这是设计提交表 schema 时必须补齐的关键信息，需要额外添加。（[36:11](https://youtu.be/QBHTbtWSECg?t=2171)）
- [[submit-problem-api-design]] — 提交问题的 API 设计为 POST 请求，需要 problem ID，submission 中包含 code（字符串类型）和 language（字符串类型）两个字段。（[18:07](https://youtu.be/QBHTbtWSECg?t=1087)）
- [[system-design-core-entity-identification]] — 在设计 LeetCode 系统时，梳理出的核心实体包括 problem（题目）、user（用户）、solution（解答）以及因需支持 live leaderboard 而增加的 leaderboard 实体。（[12:05](https://youtu.be/QBHTbtWSECg?t=725)）
- [[system-design-functional-requirements-first]] — 在系统设计面试中，候选人通常先写下标题，再逐一列出 functional requirements 并与面试官逐条确认是否有误解，之后才转向 non-functional requirements 的讨论。（[00:01](https://youtu.be/QBHTbtWSECg?t=1)）
- [[system-design-requirement-scoping]] — 设计 LeetCode 系统时，可以把 authorization、profile creation、payment gateway（用于 premium 服务）等功能显式列为 out of scope，从而把讨论精力集中在核心功能上。（[00:01](https://youtu.be/QBHTbtWSECg?t=1)）
- [[system-design-scale-assumption]] — 该设计假设当前 LeetCode 架构整体约有 4,000 到 5,000 道题目（不仅限于 DSA 类题目），以及约一百万用户规模。（[12:05](https://youtu.be/QBHTbtWSECg?t=725)）
- [[time-limit-exceeded-handling]] — 系统会遇到大量 time limit exceeded 的提交情况，需要单独深入讨论如何处理这类长时间运行的操作。（[06:02](https://youtu.be/QBHTbtWSECg?t=362)）
- [[unsafe-api-server-code-execution]] — 直接在 API 服务器上运行用户提交的代码是很危险的做法，恶意用户可能在提交的代码中植入 malware，导致系统数据被删除。（[24:07](https://youtu.be/QBHTbtWSECg?t=1447)）
- [[vertical-scaling]] — 为了支持竞赛期间多达10万甚至百万级用户，可考虑的扩展方式之一是 vertical scaling，即通过提升单台服务器的资源来应对增长的负载。（[39:13](https://youtu.be/QBHTbtWSECg?t=2353)）
- [[vm-based-code-execution]] — 相比直接在 API 服务器上执行用户代码，采用基于 VM 的隔离节点执行方案能提供更好的 isolation，系统崩溃的可能性也更低。（[24:07](https://youtu.be/QBHTbtWSECg?t=1447)）
- [[vm-container-isolation-tradeoff]] — VM 通常能提供比 container 更好的隔离性，因为 container 本质上与宿主机共享操作系统和内存等资源空间，没有专属的操作系统。（[27:08](https://youtu.be/QBHTbtWSECg?t=1628)）
- [[vm-cost-overhead]] — 选择 container 而非 VM 的一个原因是 VM 的维护成本更高，因为 VM 自带完整操作系统，比 container 更重。（[27:08](https://youtu.be/QBHTbtWSECg?t=1628)）
- [[vm-resource-waste-per-instance]] — 采用 VM-based 架构为每个执行环境分配独立的内存和计算资源，属于对计算资源的低效使用。（[27:08](https://youtu.be/QBHTbtWSECg?t=1628)）
- [[worker-pull-pattern]] — 在基于队列的架构中，runtime server 作为 worker 主动从队列中拉取（pull）待执行的提交任务，执行完成后更新数据库和缓存。（[42:13](https://youtu.be/QBHTbtWSECg?t=2533)）
