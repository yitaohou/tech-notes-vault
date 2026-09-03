---
video_id: ky7_1K3wfAY
title: Agent搜索和记忆的基础设施：腾讯云 Elastichsearch Service 企业版详细攻略
source: '[[2026-08-26-agent搜索和记忆的基础设施腾讯云-elastichsearch-service-企业版详细攻略]]'
tags:
- summary
_gen:
  prompt_hash: 209b52739480c30c61b7dcc0392dfa4aa0deb99654ee921af5e045409c961f85
  task_hash: 28e9b627309d772100bf029648594e0dc471028d8c4a328dd45879727199746f
  schema_version: 1
  model: sonnet
  generated_at: '2026-09-03T06:47:36+00:00'
---

## 一句话总结

这期视频介绍了[[elasticsearch]]从关键词搜索到语义搜索、再到面向 [[agentic-search|agent]] 的三次范式演进，并详细演示了[[tencent-cloud-es-enterprise-edition|腾讯云 ES 企业版]]如何通过混合检索、GPU 向量索引、磁盘型向量存储和 RAG 应用一键搭建，用更低成本支撑企业级 AI 检索系统。

## 核心内容

### 搜索的三次范式转变

[00:00] [[elasticsearch]] 近年经历三次范式转变：第一阶段是基于[[inverted-index|倒排索引]]的关键词搜索,通过对文本分词、记录词项位置来精确定位包含关键词的段落;第二阶段是基于[[embedding-based-retrieval|向量索引]]的语义搜索,先用嵌入模型把文本块向量化,检索时把问题也向量化并计算相似度,即使问题与原文没有相同关键词也能找到语义最相关的内容;第三阶段是面向 [[agentic-search|agent]] 的搜索——以前搜索引擎服务人,现在开始服务 agent,agent 会执行"规划-检索-判断-再检索"的循环,搜索能力越强背后的工程复杂度也越高。视频认为要构建毫秒级、百万级文档、支持精确关键词与模糊语义混合匹配、能扛住上亿用户高并发的问答系统,[[elasticsearch]] 几乎是唯一成熟的技术栈,本地知识库方案在这种企业级场景下只能算小打小闹。

### 腾讯云 ES 的落地案例与社区地位

[00:00] 微信读书新上线的 AI 问书功能底层就基于[[tencent-cloud-elasticsearch-service|腾讯云 Elasticsearch Service]]:相比传统向量数据库方案需要400多台64GB机器、成本达百万级,改用腾讯云 ES 后机器数量降到30台,硬件成本大幅下降。同时,[[tencent-cloud-es-community-contribution|腾讯云是 Elasticsearch 开源社区贡献最多的第三方公司]],累计提交260多个 PR,两次获得 Elastic 创始人点赞。[[es-enterprise-cluster-deployment-challenge|企业级 ES 集群长期稳定运行]]是自建服务的最大门槛,相比之下[[managed-es-reduces-infra-burden|使用托管服务能省去自建底层基础设施的负担]]。

### ES 企业版的四大升级方向

[03:00] 腾讯云在 AI 搜索技术大会上正式推出 [[tencent-cloud-es-enterprise-edition|ES 企业版]],在全托管服务之上开放了 Elastic Enterprise 订阅的完整能力,除支持传统日志搜索和安全分析外,专门针对 agentic search 场景做了深度适配。[[es-enterprise-four-upgrade-pillars|升级可归纳为四点]]:检索更强、Agentic AI 更友好、存储成本更低、平台更统一。

**检索更强**方面:自研的[[filtered-disk-bbq-architecture|Filtered Disk BBQ 架构]]提升关键词与向量混合检索效率,[[slice-disk-bbq-architecture|Slice Disk BBQ 架构]]实现冷热分离以适配大规模云上场景;[[disk-bbq-vector-retrieval|Disk BBQ 磁盘型向量检索]]让大规模向量搜索不再高度依赖内存;[[gpu-accelerated-vector-index-build|GPU 节点]]可直接构建向量索引,大幅缩短海量数据索引构建时间;[[hybrid-search-rerank-fusion|关键词与语义搜索结果可自动融合并通过重排序模型优化]]。这些优化叠加带来的[[es-hybrid-search-performance-gains|性能收益]]显著:部分场景性能最高提升5倍,混合搜索延迟下降60%,内存资源占用减少50%以上。

**Agentic AI 更友好**方面:可直接在 [[kibana-agent-rag-validation|Kibana 中创建智能体]],用真实数据当场验证 RAG 效果,自由配置大模型、Embedding 和重排序模型;通过 API、[[es-agent-mcp-external-integration|MCP 等接口]]可把 ES 数据和 Agent 能力接入其他 AI 系统,减少大量自行拼接基础设施的工作;[[es-inference-api-model-integration|Inference API]] 可直接对接云上大模型、向量和重排服务。

**存储成本更低**方面:冷数据可放入更便宜的 [[cos-cold-data-tiering|COS 对象存储]];借助 [[synthetic-source-logsdb-compression|Synthetic Source、压缩和 LogsDB]] 减少原始数据和重复日志占用;配合[[snapshot-archive-recovery-optimization|快照归档和集群恢复优化]]进一步降低长期存储成本。

**平台更统一**方面:支持[[cross-cluster-unified-platform|跨集群查询]],把搜索、日志分析、可观测性和安全能力整合在同一平台。

升级方式很简单:[[es-enterprise-platinum-price-parity-upgrade|企业版与白金版同价]],只需在控制台把集群从8版本一键升级到9版本即可解锁;新建集群时选择[[es-enterprise-version-9-4-2-full-unlock|最高版本9.4.2]]也能解锁全部企业版能力。此外若不想用托管服务,还可以[[es-self-deployment-option|下载平台自动生成的代码自行部署]]。

### 实操演示:搭建 RAG 应用全流程

[03:00] 演示先通过[[es-public-network-ip-whitelist-config|修改公网访问 IP 白名单]]从公网打开 Kibana 管理界面。

[06:01] 向量模型接入 ES 有两种方案——直接在 ES 机器学习节点部署模型,或使用腾讯云的[[embedding-model-integration-methods-es|原子化推理服务]],作者选择了后者。具体步骤:先在[[es-outbound-access-for-inference|集群管理的更多设置中打开节点出站访问开关]],允许集群机器访问外部推理服务;在推理服务-向量化页面获取[[es-inference-service-api-key|API 密钥]];复制官方 DSL,在 Kibana 中替换 URL 和 API key,创建对接外部推理服务的[[es-inference-endpoint|推理端点]];创建 [[es-ingest-pipeline-auto-embedding|ingest pipeline]] 后,数据写入索引时会自动调用推理端点做向量化,无需手动预先 embedding。

索引层面,[[diskbbq-vector-index|文本字段用传统倒排索引做关键词搜索,向量字段用 DiskBBQ 做语意检索]],避免海量向量全部塞进内存。检索时采用 [[rrf-hybrid-search|RRF 混合检索]]:同时执行关键词匹配和向量语意检索两路查询,再通过 RRF 算法综合排序返回最相关文本块。

更进一步,在 ES 控制台的应用开发中可以用 [[es-rag-app-builder-platform|RAG 应用构建平台]]:新建应用并选择目标集群后,平台自动创建索引、对接模型,无需任何提前配置就能把 ES 集群变成开箱即用的 RAG 应用。[[es-rag-document-library-upload|文档库]]支持直接上传 PDF、Word、PPT 等格式,系统自动完成 chunking 并存入 ES 构建知识库。在 [[es-rag-online-testing-params|在线测试界面]]可手动调整检索方式、召回权重、召回数量及 LLM 类型,对比不同配置下的回答效果。测试完毕后,在发布管理中发布新版本,即可通过 [[es-rag-one-click-deploy|一键部署]]把 RAG 服务上线。

### 总结:适用场景边界

[09:02] 视频总结强调 [[elasticsearch-scale-reliability-usecase|规模与可靠性的取舍]]:对个人知识库,很多轻量方案已经足够;但当数据规模达到十亿、十一亿级别,同时要求高并发、高可用和长期稳定运行时,Elasticsearch 是最成熟的选择。腾讯云 ES 企业版通过 [[disk-bbq-vector-compression|Disk BBQ 降低向量检索成本]]、[[gpu-accelerated-vector-indexing|GPU 提升向量索引构建效率]]、[[hybrid-retrieval-pipeline|混合检索与重排序提高 RAG 召回质量]]、[[es-agent-builder-inference-mcp-integration|Agent Builder + Inference API + MCP 串联模型数据与智能体]]、以及[[es-storage-ops-cost-reduction|对象存储/日志压缩/跨集群能力压低存储运维成本]],最终让用户无需自建底层基础设施即可快速搭建企业级 AI 检索系统([[managed-es-reduces-infra-burden]])。

## 值得记住的细节

- [00:00] 微信读书 AI 问书:传统向量数据库方案需 400+ 台 64GB 机器、成本百万级;改用腾讯云 ES 后降至 30 台机器。
- [00:00] 腾讯云累计向 Elasticsearch 开源社区提交 260+ 个 PR,两次获创始人点赞。
- [00:00] 性能优化整体收益:最高提升 5 倍性能,混合搜索延迟降低 60%,内存占用减少 50%以上。
- [03:00] 企业版与白金版同价,集群从 8 版本一键升级到 9 版本即解锁;新建集群选版本 9.4.2 可解锁全部企业版能力。
- [03:00] 公网访问 Kibana:在集群管理的可视化访问控制中,把 IP 白名单改为允许所有 IP。
- [06:01] 使用原子化推理服务前需先在"集群管理-更多设置"打开节点出站访问开关。
- [06:01] API 密钥获取路径:左侧菜单"推理服务-向量化"页面点击"获取密钥"。
- [06:01] 创建推理端点:复制官方 DSL,在 Kibana 中粘贴,替换 URL 与 API key 后执行。
- [06:01] RRF 混合检索 = 关键词匹配 + 向量语意检索两路结果,由 RRF 算法综合排序。
- [06:01] RAG 应用构建平台支持直接上传 PDF/Word/PPT,自动完成 chunking。
- [06:01] 在线测试可调参数:检索方式、召回权重、召回数量、LLM 类型。
- [09:02] 规模判断标准:数据量达十亿、十一亿级别且要求高并发/高可用/长期稳定时才需要 Elasticsearch 级别方案,个人知识库场景轻量方案已够用。
- [09:02] 不想用托管服务时,可下载平台自动生成的代码自行修改部署。

## 这个视频适合谁 / 可以跳过什么

适合人群:需要为企业级场景(数据规模十亿级以上、高并发、需要 agent 检索能力)搭建搜索/RAG 系统的技术决策者或工程师,以及想快速上手 ES 企业版 Kibana 操作(接入推理服务、创建索引、构建 RAG 应用)的开发者。

可以跳过:如果只是做个人或小规模知识库,视频开篇关于 [[elasticsearch]] 范式演进和微信读书案例的部分(00:00-03:00)可以快速略过,直接看 06:01 起的 Kibana 实操演示部分获取具体操作步骤即可;若不关心底层原理只想直接用现成 RAG 平台,09:02 的总结部分也可作为快速回顾。
