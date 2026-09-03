---
video_id: ky7_1K3wfAY
url: https://www.youtube.com/watch?v=ky7_1K3wfAY
title: Agent搜索和记忆的基础设施：腾讯云 Elastichsearch Service 企业版详细攻略
channel: 技术爬爬虾  TechShrimp
published: '2026-08-26'
duration: '10:06'
transcript_origin: whisper
tags:
- video
---

# Agent搜索和记忆的基础设施：腾讯云 Elastichsearch Service 企业版详细攻略

摘要: [[2026-08-26-agent搜索和记忆的基础设施腾讯云-elastichsearch-service-企业版详细攻略-summary|完整摘要]]

## 知识点

- [[agentic-search]] — 搜索的第三次范式转变是 agentic search：以前搜索引擎服务人，现在搜索引擎开始服务 agent，agent 会执行规划、检索、判断、再检索的循环，搜索能力越强背后工程复杂度也越高。（[00:00](https://youtu.be/ky7_1K3wfAY?t=0)）
- [[cos-cold-data-tiering]] — 大量历史日志和冷数据不需要一直放在昂贵的高性能磁盘里，可以放到成本更低的 COS 对象存储里，需要时依然能够搜索。（[03:00](https://youtu.be/ky7_1K3wfAY?t=180)）
- [[cross-cluster-unified-platform]] — 大型企业往往有多个 ES 集群，企业版支持跨集群查询，同时把搜索、日志分析、可观测性和安全能力整合在同一平台里。（[03:00](https://youtu.be/ky7_1K3wfAY?t=180)）
- [[disk-bbq-vector-compression]] — 腾讯云 Elasticsearch Service 企业版通过 Disk BBQ 技术降低向量检索的成本。（[09:02](https://youtu.be/ky7_1K3wfAY?t=542)）
- [[disk-bbq-vector-retrieval]] — 传统向量搜索比较吃内存，数据规模一大成本就很高；企业版提供 Disk BBQ 这类磁盘型向量检索能力，让大规模向量搜索不再高度依赖内存。（[03:00](https://youtu.be/ky7_1K3wfAY?t=180)）
- [[diskbbq-vector-index]] — 创建索引时，文本字段使用传统倒排索引做关键词搜索，向量字段则使用DiskBBQ做语意检索，DiskBBQ可以把向量数据存储在磁盘上，避免把海量向量全部塞进内存，从而大幅降低大规模向量搜索的内存成本。（[06:01](https://youtu.be/ky7_1K3wfAY?t=361)）
- [[elasticsearch]] — 视频认为要构建能在毫秒级从百万本书中找到答案、同时支持精确关键词检索与模糊语义匹配、并能服务上亿用户扛住高并发的问答系统，Elasticsearch 基本是唯一成熟的技术栈，本地知识库方案在这种企业级场景下只能算小打小闹。（[00:00](https://youtu.be/ky7_1K3wfAY?t=0)）
- [[elasticsearch-scale-reliability-usecase]] — 对于个人知识库，很多轻量方案已经足够；但当数据规模达到十亿、十一亿级别，同时要求高并发、高可用和长期稳定运行时，Elasticsearch 是最成熟的选择。（[09:02](https://youtu.be/ky7_1K3wfAY?t=542)）
- [[embedding-based-retrieval]] — Elasticsearch 的语义搜索阶段会先用嵌入模型对文本块做向量化，检索时把用户问题同样向量化并计算向量相似度，从而在问题与原文没有相同关键词时依然能找到语义最相近的内容。（[00:00](https://youtu.be/ky7_1K3wfAY?t=0)）
- [[embedding-model-integration-methods-es]] — 将向量模型接入ES集群有两种方案，一种是直接在ES集群的机器学习节点上部署向量模型，另一种是使用腾讯云提供的原子化推理服务，作者选择了后者。（[06:01](https://youtu.be/ky7_1K3wfAY?t=361)）
- [[es-agent-builder-inference-mcp-integration]] — 腾讯云 Elasticsearch Service 企业版通过 Agent Builder、Inference API 和 MCP，把模型、数据和智能体（agent）真正串联起来。（[09:02](https://youtu.be/ky7_1K3wfAY?t=542)）
- [[es-agent-mcp-external-integration]] — 通过 API、MCP 等接口，可以把 ES 的数据和 Agent 的能力接入其他 AI 业务系统，甚至调用自定义工具完成更多任务，减少了大量自己拼接基础设施的工作。（[03:00](https://youtu.be/ky7_1K3wfAY?t=180)）
- [[es-enterprise-cluster-deployment-challenge]] — 部署企业级 Elasticsearch 最大的门槛是如何把一个大规模集群长期稳定地运行下去，比起自建服务，使用云上托管服务被认为是更可靠的方案。（[00:00](https://youtu.be/ky7_1K3wfAY?t=0)）
- [[es-enterprise-four-upgrade-pillars]] — 腾讯云 ES 企业版这次升级可归纳为四点：检索更强、Agentic AI 更友好、存储成本更低、平台更统一。（[03:00](https://youtu.be/ky7_1K3wfAY?t=180)）
- [[es-enterprise-platinum-price-parity-upgrade]] — 腾讯云 ES 企业版与白金版同价，只需在控制台一键把集群从 8 版本升级到 9 版本，就能解锁企业版功能。（[03:00](https://youtu.be/ky7_1K3wfAY?t=180)）
- [[es-enterprise-version-9-4-2-full-unlock]] — 在腾讯云 ES 服务新建集群时，ES 版本选择最高版本 9.4.2，即可解锁企业版的全部能力。（[03:00](https://youtu.be/ky7_1K3wfAY?t=180)）
- [[es-hybrid-search-performance-gains]] — 腾讯云ES通过冷热分离架构、文本向量融合索引、查询并行化、排序加速、读写分离、熔断限流、存算分离等一系列优化，在部分场景下性能最高提升5倍，混合搜索延迟下降60%，内存资源占用减少50%以上。（[00:00](https://youtu.be/ky7_1K3wfAY?t=0)）
- [[es-inference-api-model-integration]] — ES 企业版深度集成腾讯云基础设施，Inference API 可以直接对接云上的大模型、向量和重排服务。（[03:00](https://youtu.be/ky7_1K3wfAY?t=180)）
- [[es-inference-endpoint]] — 复制官方提供的创建推理端点DSL，在Kibana控制台粘贴并将其中的URL与API key替换为推理服务的实际值后执行，即可在ES集群中创建一个对接外部推理服务的推理端点。（[06:01](https://youtu.be/ky7_1K3wfAY?t=361)）
- [[es-inference-service-api-key]] — 在ES控制台左侧菜单的推理服务-向量化页面点击获取密钥按钮，即可创建并保存用于调用推理服务的API密钥。（[06:01](https://youtu.be/ky7_1K3wfAY?t=361)）
- [[es-ingest-pipeline-auto-embedding]] — 创建ingest pipeline后，数据写入ES索引时会自动调用之前创建的推理端点对文本进行向量化，无需手动预先做embedding再写入。（[06:01](https://youtu.be/ky7_1K3wfAY?t=361)）
- [[es-outbound-access-for-inference]] — 要让ES集群使用腾讯云的原子化推理服务，需要先在集群管理的更多设置中打开节点出站访问的开关，允许集群机器访问外部推理服务。（[06:01](https://youtu.be/ky7_1K3wfAY?t=361)）
- [[es-public-network-ip-whitelist-config]] — 在集群管理的可视化访问控制中，修改公网访问策略、把 IP 白名单改成允许所有 IP 地址访问，即可从公网打开 Kibana 管理界面。（[03:00](https://youtu.be/ky7_1K3wfAY?t=180)）
- [[es-rag-app-builder-platform]] — 在ES控制台的应用开发中新建应用并选择目标ES集群后，平台会自动创建索引、对接模型，无需任何提前配置即可把ES集群变成一个开箱即用的RAG应用。（[06:01](https://youtu.be/ky7_1K3wfAY?t=361)）
- [[es-rag-document-library-upload]] — 创建RAG应用的文档库时可以直接上传PDF、Word、PPT等多种格式的文档，系统会自动完成文档切分（chunking）并存入ES集群构建知识库。（[06:01](https://youtu.be/ky7_1K3wfAY?t=361)）
- [[es-rag-one-click-deploy]] — RAG应用测试完毕后，只需在发布管理中发布新版本，即可把该RAG服务一键部署到腾讯云并上线。（[06:01](https://youtu.be/ky7_1K3wfAY?t=361)）
- [[es-rag-online-testing-params]] — 在RAG应用的在线测试界面中可以手动调整检索方式、召回权重、召回数量以及所使用的LLM类型等参数，并通过在线测试直接对比不同配置下的回答效果。（[06:01](https://youtu.be/ky7_1K3wfAY?t=361)）
- [[es-self-deployment-option]] — 如果不想使用托管服务，也可以下载腾讯云 Elasticsearch Service 平台自动生成的代码，在此基础上修改后自行部署。（[09:02](https://youtu.be/ky7_1K3wfAY?t=542)）
- [[es-storage-ops-cost-reduction]] — 腾讯云 Elasticsearch Service 企业版借助对象存储、日志压缩和跨集群能力，进一步压低存储、运维和管理的成本。（[09:02](https://youtu.be/ky7_1K3wfAY?t=542)）
- [[filtered-disk-bbq-architecture]] — 腾讯云自研了文本向量融合索引的 Filtered Disk BBQ 架构，用于提升关键词与向量混合检索的效率。（[00:00](https://youtu.be/ky7_1K3wfAY?t=0)）
- [[gpu-accelerated-vector-index-build]] — 企业版支持用 GPU 节点直接构建向量索引，大幅缩短了海量数据的索引构建时间。（[03:00](https://youtu.be/ky7_1K3wfAY?t=180)）
- [[gpu-accelerated-vector-indexing]] — 腾讯云 Elasticsearch Service 企业版利用 GPU 提升向量索引的构建效率。（[09:02](https://youtu.be/ky7_1K3wfAY?t=542)）
- [[hybrid-retrieval-pipeline]] — 腾讯云 Elasticsearch Service 企业版通过混合检索（hybrid retrieval）与重排序（rerank）来提高 RAG 系统的召回质量。（[09:02](https://youtu.be/ky7_1K3wfAY?t=542)）
- [[hybrid-search-rerank-fusion]] — 企业版可以把关键词搜索和语义搜索两种结果自动融合，再通过内置的重排序模型进一步优化召回结果。（[03:00](https://youtu.be/ky7_1K3wfAY?t=180)）
- [[inverted-index]] — 倒排索引通过对文本分词并记录词项出现位置，使关键词搜索时能直接定位到包含该词的原文段落，是 Elasticsearch 第一阶段关键词搜索的核心技术。（[00:00](https://youtu.be/ky7_1K3wfAY?t=0)）
- [[kibana-agent-rag-validation]] — 可以直接在控制面板 Kibana 中创建智能体，用真实数据当场验证 RAG 知识库的效果，并自由配置大模型、Embedding 和重排序模型。（[03:00](https://youtu.be/ky7_1K3wfAY?t=180)）
- [[managed-es-reduces-infra-burden]] — 使用托管的 Elasticsearch Service 企业版后，不需要自己维护一套庞大的底层基础设施，也可以快速搭建出企业级的 AI 检索系统。（[09:02](https://youtu.be/ky7_1K3wfAY?t=542)）
- [[rrf-hybrid-search]] — RRF混合检索会同时执行两路查询——第一路做传统关键词匹配，第二路根据向量索引做语意检索，最终ES通过RRF算法把两路结果综合排序，返回最相关的几个文本块。（[06:01](https://youtu.be/ky7_1K3wfAY?t=361)）
- [[slice-disk-bbq-architecture]] — 腾讯云针对大规模云上场景自研了冷热分离的 Slice Disk BBQ 架构，是其一系列性能优化技术之一。（[00:00](https://youtu.be/ky7_1K3wfAY?t=0)）
- [[snapshot-archive-recovery-optimization]] — 再配合快照归档和集群恢复优化，可以显著降低海量日志和历史数据的长期存储成本。（[03:00](https://youtu.be/ky7_1K3wfAY?t=180)）
- [[synthetic-source-logsdb-compression]] — 借助 Synthetic Source、压缩和 LogsDB 等能力，可以减少原始数据和重复日志的存储占用。（[03:00](https://youtu.be/ky7_1K3wfAY?t=180)）
- [[tencent-cloud-elasticsearch-service]] — 微信读书最近上线的AI问书功能底层基于腾讯云 Elasticsearch Service；相比传统向量数据库方案需要超过400台64GB机器、成本达百万级，采用腾讯云ES方案后机器数量降至30台，大幅降低了硬件成本。（[00:00](https://youtu.be/ky7_1K3wfAY?t=0)）
- [[tencent-cloud-es-community-contribution]] — 腾讯云是 Elasticsearch 开源社区贡献最多的第三方公司，累计提交了260多个PR，两次获得 Elasticsearch 创始人的点赞。（[00:00](https://youtu.be/ky7_1K3wfAY?t=0)）
- [[tencent-cloud-es-enterprise-edition]] — 腾讯云在AI搜索技术大会上正式推出ES企业版，在全托管服务之上开放了 Elastic Enterprise 订阅的完整能力，除支持传统的日志搜索和安全分析外，还专门针对 agentic search 场景做了深度适配。（[00:00](https://youtu.be/ky7_1K3wfAY?t=0)）
