---
video_id: Qa-7iWxDz1A
url: https://www.youtube.com/watch?v=Qa-7iWxDz1A
title: Fundamentals of Backend Architecture - How to Design Scalable Software
channel: Tiago
published: '2026-06-08'
duration: '48:11'
transcript_origin: subs
tags:
- video
---

# Fundamentals of Backend Architecture - How to Design Scalable Software

摘要: [[2026-06-08-fundamentals-of-backend-architecture---how-to-desi-summary|完整摘要]]

## 知识点

- [[ai-code-generation-outage-correlation]] — 视频作者观察到，虽然用 AI 写代码带来了明显的生产力提升，但同时大型平台上的 outage 和错误消息也变得更加频繁，这促使他重新审视软件架构的重要性。（[00:00](https://youtu.be/Qa-7iWxDz1A?t=0)）
- [[api-gateway]] — API Gateway 接收客户端请求，对其进行分析后转发到正确的后端服务。（[21:05](https://youtu.be/Qa-7iWxDz1A?t=1265)）
- [[architecture-decision-tradeoff-analysis]] — 架构设计的核心不是找到唯一正确答案，而是理解不同方案的优劣，并结合公司所处阶段做出有意识的取舍决策。（[03:00](https://youtu.be/Qa-7iWxDz1A?t=180)）
- [[architecture-design-process]] — 架构设计的核心流程是先理解具体问题和所处的业务领域，然后构建出能以最佳方式解决该问题、并能在未来持续扩展的软件方案。（[45:11](https://youtu.be/Qa-7iWxDz1A?t=2711)）
- [[architecture-holistic-scope]] — 系统架构设计不仅仅是基础设施层面的决策，正如 caching 案例所展示的那样，还涉及算法选择（如 rate limiting 算法）、产品决策以及数据库类型选择等多个维度。（[45:11](https://youtu.be/Qa-7iWxDz1A?t=2711)）
- [[architecture-tutorial-google-drive-clone]] — 视频以设计一个支持上传下载文件的 Google Drive 克隆产品为例，从单机架构开始，逐步演进到 monolith，再讲解 rate limiting、caching、horizontal/vertical scaling 等主题。（[00:00](https://youtu.be/Qa-7iWxDz1A?t=0)）
- [[authentication-service-login-flow]] — 用户在登录页面提交凭证（邮箱密码或 single sign-on token）后，由 gateway 将请求重定向到认证服务，由其验证凭证并签发 token。（[24:05](https://youtu.be/Qa-7iWxDz1A?t=1445)）
- [[authentication-vs-authorization]] — authentication 回答「你是否有权访问这个应用」，authorization 回答「你是否有权限执行某个具体操作（如上传文件）」，两者可以放在同一服务实现，但概念上是不同的。（[24:05](https://youtu.be/Qa-7iWxDz1A?t=1445)）
- [[authorization-header-token-transport]] — 用户发送请求时把 token 放在 authorization header 中，这也是使用 cookie 传递身份凭证的常见做法。（[24:05](https://youtu.be/Qa-7iWxDz1A?t=1445)）
- [[autoscaling]] — autoscaling 允许设定最小实例数（如2个），并在流量增大时自动扩容（如扩到10个），从而在成本与承载能力之间自动平衡。（[16:45](https://youtu.be/Qa-7iWxDz1A?t=1005)）
- [[cache-aside-pattern]] — cache-aside 模式的核心逻辑是先判断 key（如 file123）是否存在于 cache 中，存在则直接返回，避免访问数据库；不存在则查数据库、写入 cache 后再返回给用户，使下一次同样的请求命中缓存变快。（[42:09](https://youtu.be/Qa-7iWxDz1A?t=2529)）
- [[cache-first-lookup-flow]] — 请求先经过 gateway 转发给 file service，file service 优先查询缓存；如果对应文件已经在缓存中处于 warm 且可用状态，就直接从缓存返回文件，无需再访问关系型数据库或对象存储。（[39:09](https://youtu.be/Qa-7iWxDz1A?t=2349)）
- [[cache-precomputed-expensive-results]] — cache 除了用于限流计数外，也很适合预先计算并存储代价高昂的操作结果，例如编译代码这类昂贵计算可以把结果存入 object storage、再通过 cache 读取，而不必每次重新计算。（[45:11](https://youtu.be/Qa-7iWxDz1A?t=2711)）
- [[caching-motivation-repeated-access]] — 以500个用户每天反复打开应用首页同一份文件为例：若无缓存，每次请求都会重新触发从 gateway 到 files service、relational database、object storage 的完整计算链路，造成资源浪费。（[36:09](https://youtu.be/Qa-7iWxDz1A?t=2169)）
- [[cdn-edge-asset-caching]] — CDN 部署在集群外部的网络边缘（edge），本质上也是一种缓存，但特别适合用来缓存图片、视频这类体积较大的资产，弥补 Redis 无法胜任大文件缓存的短板。（[39:09](https://youtu.be/Qa-7iWxDz1A?t=2349)）
- [[cdn-latency-improvement-example]] — 举例：里斯本某用户首次请求某图片需要走数据库全流程、耗时约 1 秒；该图片被 CDN 缓存后，同一 CDN 节点覆盖范围内后续约 499 个用户的请求可加速到约 20 毫秒。（[42:09](https://youtu.be/Qa-7iWxDz1A?t=2529)）
- [[cdn-origin-bypass]] — CDN 的强大之处在于一旦内容被缓存，后续用户请求可以完全跳过源服务器上原本用于获取文件的整套计算流程（DB 查询、cache 查询等），直接由 CDN 节点响应。（[42:09](https://youtu.be/Qa-7iWxDz1A?t=2529)）
- [[cdn-point-of-presence]] — CDN 提供商的优势在于其在全球拥有众多 PoP 节点，用户发起请求时可以直接命中离自己最近的 CDN 节点，而不必先访问源服务器。（[42:09](https://youtu.be/Qa-7iWxDz1A?t=2529)）
- [[combined-scaling-strategy]] — 工程实践中通常会同时结合 vertical scaling（用更强的机器）和 horizontal scaling（用更多机器），而非只选择其中一种方式。（[15:45](https://youtu.be/Qa-7iWxDz1A?t=945)）
- [[data-coupled-server-scaling-problem]] — 如果数据和服务器实例绑定在一起，扩展成两台服务器后，数据会在两边各自保留一份，形成数据重复。（[06:01](https://youtu.be/Qa-7iWxDz1A?t=361)）
- [[data-coupling-scalability-resilience-principle]] — 这一段的关键结论可概括为一句话：数据耦合到机器上等于无法扩展、没有韧性（no scale and no resilience）。（[06:01](https://youtu.be/Qa-7iWxDz1A?t=361)）
- [[data-synchronization-problem-scaling]] — 用户向服务器A写入数据后，该数据只存在于服务器A本地，服务器B完全不知道这次写入，导致不同实例间数据不一致。（[06:01](https://youtu.be/Qa-7iWxDz1A?t=361)）
- [[database-unsuitable-for-large-files]] — 不应把文件直接上传到关系型数据库中，因为文件可能有200MB的图片甚至20GB的视频那么大，而关系型数据库并不是为存储这类大体积二进制数据设计的。（[27:06](https://youtu.be/Qa-7iWxDz1A?t=1626)）
- [[dau-mau-scale-requirement]] — 举例说明业务规模增长（如达到10,000月活用户）会带来新的资源消耗与性能问题，促使系统需要考虑 caching 等优化手段。（[36:09](https://youtu.be/Qa-7iWxDz1A?t=2169)）
- [[dead-letter-queue]] — 如果消息始终无法被投递成功，会被放入一个专门的队列，通常称为 dead letter queue（消息的墓地）。（[36:09](https://youtu.be/Qa-7iWxDz1A?t=2169)）
- [[dead-letter-queue-alerting]] — 需要为 dead letter queue 配置告警机制，将未送达的消息信息发送到 Slack 或 Discord 等渠道，从而及时知晓具体是哪条消息投递失败。（[36:09](https://youtu.be/Qa-7iWxDz1A?t=2169)）
- [[decoupled-database-architecture]] — 解决数据耦合问题的方法是把数据库独立出来，作为一个统一的关系型数据库集中存放用户表、文件表等所有数据，用户请求落到哪台服务器实例都能访问到同一份数据。（[06:01](https://youtu.be/Qa-7iWxDz1A?t=361)）
- [[direct-server-upload-risks]] — 不应该把文件直接流式上传到自己的服务器：一是服务器可能无法承受大体积数据流并因此触发 timeout，二是直接接收上传数据会增加遭受恶意攻击的风险，绕开这种方式有助于提前预防这类攻击。（[27:06](https://youtu.be/Qa-7iWxDz1A?t=1626)）
- [[docker-compose]] — 该演示使用 docker compose up 一次性启动三个完全相同代码的 Golang 服务和一个作为负载均衡器的 Nginx，用于直观展示不同负载均衡算法的效果。（[12:03](https://youtu.be/Qa-7iWxDz1A?t=723)）
- [[domain-driven-service-decomposition]] — 一个 Google Drive clone 可按业务领域拆分为四个独立微服务：file service（处理文件上传下载）、notification service（处理 push、web、desktop 通知）、auth service（处理认证）、real-time service（处理多台个人设备之间的实时同步，如本地上传后同步到云端再同步到其他设备）。（[18:05](https://youtu.be/Qa-7iWxDz1A?t=1085)）
- [[event-fan-out-multiple-subscribers]] — 一个视频上传事件可能需要同时触发缩略图生成服务和跨设备实时同步服务两个完全不同的下游处理逻辑，这种一对多投递需求称为 fan-out。（[33:08](https://youtu.be/Qa-7iWxDz1A?t=1988)）
- [[file-metadata-blob-separation]] — 文件上传架构会把文件本体（blob）与文件元数据分开存储：file service 收到上传请求后，先在关系型数据库中为该文件生成并保存元数据记录，而不是把文件本体本身存进数据库。（[27:06](https://youtu.be/Qa-7iWxDz1A?t=1626)）
- [[file-metadata-caching-rationale]] — 文件元数据（文件名、属性等）几乎不会变化或很少变化，因此是最适合被缓存的内容，应从缓存元数据开始设计优化。（[39:09](https://youtu.be/Qa-7iWxDz1A?t=2349)）
- [[file-metadata-object-storage-split]] — 获取一个文件时通常分两步：先查关系型数据库拿到文件 ID 对应的 URL（元数据），再去 object storage 用该 URL 取出文件本体。（[42:09](https://youtu.be/Qa-7iWxDz1A?t=2529)）
- [[file-upload-request-flow]] — 文件上传的典型流程是：客户端向 API gateway 发送请求，其中包含元数据（如文件名、文件大小）以及文件本体（blob，例如图片数据）；gateway 再把这个请求转发给 file service 处理。（[27:06](https://youtu.be/Qa-7iWxDz1A?t=1626)）
- [[files-table-schema]] — files 表的基本 schema 设计包括：自动生成的文件 ID（generated ID）、文件名（file name）、文件大小（size），以及可选的文件类型字段（type，如 PNG），但不存储文件本身。（[27:06](https://youtu.be/Qa-7iWxDz1A?t=1626)）
- [[gateway-central-decision-point]] — gateway 在整个架构中扮演居中决策者的角色，例如决定请求是否需要转发到认证服务、是否需要在边缘直接拒绝请求等。（[24:05](https://youtu.be/Qa-7iWxDz1A?t=1445)）
- [[gateway-edge-token-verification]] — gateway 可以直接在边缘验证请求中携带的 token 是否合法，若合法则信任其未过期，不必对认证服务发起额外的网络调用。（[24:05](https://youtu.be/Qa-7iWxDz1A?t=1445)）
- [[gateway-single-entry-point]] — 客户端与业务系统通信的唯一方式是经过 Gateway，Gateway 统一负责处理认证（authentication）和路由（routing）。（[21:05](https://youtu.be/Qa-7iWxDz1A?t=1265)）
- [[geographic-latency-example]] — 举例说明地理距离对延迟的影响：美国到里斯本之间的网络延迟大约是 300 毫秒，这正是需要把内容缓存在靠近用户地理位置的原因。（[42:09](https://youtu.be/Qa-7iWxDz1A?t=2529)）
- [[health-check-load-balancing]] — 更智能的 load balancer 会用 health check 持续了解各服务器的真实负载情况，如果某台服务器正在处理耗资源的上传任务而明显更忙，就会把新请求优先发送到状态更好的服务器，而不是机械地轮询。（[09:02](https://youtu.be/Qa-7iWxDz1A?t=542)）
- [[horizontal-scaling]] — 对无状态服务器做横向扩展（增加实例数量）看似简单，但若数据与实例本地耦合，多实例间会出现数据重复且互不感知的问题。（[06:01](https://youtu.be/Qa-7iWxDz1A?t=361)）
- [[http-429-too-many-requests]] — 当用户请求次数超过设定阈值（例如达到10次）时，服务器会返回 HTTP 429 状态码，告知客户端已被 rate limited。（[45:11](https://youtu.be/Qa-7iWxDz1A?t=2711)）
- [[jwt-token-authentication]] — JWT token 本质上是一个签名，携带过期时间（expiry date），用来证明请求方已通过身份验证。（[24:05](https://youtu.be/Qa-7iWxDz1A?t=1445)）
- [[kubernetes-container-orchestration]] — Kubernetes 和 Google Cloud 等平台都提供了 autoscaling 能力，可用服务器模式或 serverless 模式实现。（[16:55](https://youtu.be/Qa-7iWxDz1A?t=1015)）
- [[least-connections-load-balancing]] — least connections 算法的逻辑是：如果某台服务器当前连接数更少，说明它更空闲、可用性更高，因此优先把新请求路由给它。（[12:03](https://youtu.be/Qa-7iWxDz1A?t=723)）
- [[load-balancer]] — load balancer 是架构中位于服务器前方的中间层组件，作用是把用户请求转发给一台健康的服务器，而不是让用户直接访问某台固定服务器。（[09:02](https://youtu.be/Qa-7iWxDz1A?t=542)）
- [[load-balancer-need-multi-server]] — 把服务器扩展成两个实例后，虽然多个服务器之间不需要相互通信，但仍需要一个中间层来决定某个请求具体交给哪台服务器处理，这是进入分布式架构后新出现的问题。（[06:01](https://youtu.be/Qa-7iWxDz1A?t=361)）
- [[load-balancer-path-based-routing]] — 当系统拆分为多个微服务后，负载均衡器需要能识别请求路径（如 POST /api/login）并将其路由到正确的微服务（如 auth service），但并非所有负载均衡器都具备这种基于路径的路由能力。（[18:05](https://youtu.be/Qa-7iWxDz1A?t=1085)）
- [[load-balancer-routing-limitation-implies-gateway]] — 如果负载均衡器不支持按路径路由到不同微服务，说明负载均衡器可能并不是承担这一路由职责的合适组件，暗示需要额外的路由层（如 API gateway）来解决这个问题。（[18:05](https://youtu.be/Qa-7iWxDz1A?t=1085)）
- [[load-balancer-traffic-asymmetry]] — round robin 只保证各服务器收到的请求数量相同，但如果一个用户在上传文件（消耗更多存储和 CPU），另一个用户只是读取文件，两台服务器实际承受的负载其实并不对等。（[09:02](https://youtu.be/Qa-7iWxDz1A?t=542)）
- [[martin-fowler]] — 作者在讨论软件架构时始终以 Martin Fowler 的相关文章作为参考依据。（[00:00](https://youtu.be/Qa-7iWxDz1A?t=0)）
- [[message-broker-high-availability]] — message broker 需要被设计为 highly available，核心目标是保持稳定运行且不丢失（crush）消息。（[36:09](https://youtu.be/Qa-7iWxDz1A?t=2169)）
- [[message-broker-necessity]] — 像 YouTube、Google Drive 这类平台通过在服务间加入具备高持久性（durability）和可靠投递能力的 broker 来解决直接同步调用可能导致事件丢失的问题，这也是不采用服务间直接同步通信的核心原因。（[33:08](https://youtu.be/Qa-7iWxDz1A?t=1988)）
- [[message-broker-pub-sub]] — 为实现服务间解耦，需要引入一个 broker（如 Kafka 或 RabbitMQ）作为 pub/sub 系统，上游只需把消息发给 broker，由 broker 负责分发给各个下游服务。（[30:07](https://youtu.be/Qa-7iWxDz1A?t=1807)）
- [[message-durability-broker-crash]] — 即便 broker 崩溃，消息也要保证 durable（持久化），常见做法是把消息存储在一个单独的数据库中。（[36:09](https://youtu.be/Qa-7iWxDz1A?t=2169)）
- [[message-redelivery-mechanism]] — broker 具备 redelivery（重投）功能：消费服务（如 file service）需要 acknowledge 收到消息，若未确认，broker 会在一定时间后重新投递该消息。（[36:09](https://youtu.be/Qa-7iWxDz1A?t=2169)）
- [[microservice-single-responsibility]] — 在微服务架构中，thumbnail service 只负责实时生成缩略图，notification service 只负责实时文件通知，authentication service 只负责认证，各服务职责单一，这本质上是更大规模下的 separation of concerns。（[36:09](https://youtu.be/Qa-7iWxDz1A?t=2169)）
- [[microservices]] — 当应用盈利、团队规模扩大、且部分接口开始出现响应变慢等问题时，团队往往会考虑转向 microservices 架构，但这被形容为「打开了一扇危险的新世界的大门」。（[17:40](https://youtu.be/Qa-7iWxDz1A?t=1060)）
- [[microservices-architecture]] — 当所有请求都由同一批服务器处理时，某一功能（如文件上传）的负载激增会拖慢整个系统，这正是促使系统从单体架构转向 microservices 的常见诱因。（[18:05](https://youtu.be/Qa-7iWxDz1A?t=1085)）
- [[microservices-suited-for-large-organizations]] — microservices 是一个复杂话题，通常在业务规模较大、可以让不同团队分别专注维护一个服务（如一个团队专做文件服务、另一个团队专做通知服务）时才更值得采用，而非任何规模的项目都适合。（[18:05](https://youtu.be/Qa-7iWxDz1A?t=1085)）
- [[minimum-instance-cost-principle]] — 更多机器或更强机器都等于更多花费，因此工程目标是用尽可能少的实例数量满足流量需求，即维持一个最小可用实例数。（[16:35](https://youtu.be/Qa-7iWxDz1A?t=995)）
- [[netflix-ram-prewarming-exception]] — 也存在例外情况：例如 Netflix 可能会在一部新剧或电影即将爆红时，把它预先放进 RAM，只为应对最初那波用户激增流量，以提供更好的服务体验。（[39:09](https://youtu.be/Qa-7iWxDz1A?t=2349)）
- [[nginx-upstream-block]] — 该 demo 中 Nginx 配置了两个 upstream block，分别代表两组服务器，使同一个 Nginx 反向代理能够根据请求 URL 路径（如 /rr 对应 round robin，/sticky 对应 session affinity）采用不同的负载均衡策略。（[12:03](https://youtu.be/Qa-7iWxDz1A?t=723)）
- [[object-storage]] — Object storage（如 S3 bucket、Google Cloud bucket）是专门用于承载静态文件的存储方案，适合存放不常变化甚至从不变化的大体积文件，如图片和视频。（[27:06](https://youtu.be/Qa-7iWxDz1A?t=1626)）
- [[object-storage-bypass-api-server]] — 使用 presigned URL 直接上传到对象存储后，应用服务器完全不会被上传流量触及，从根本上解决了文件服务被上传请求压垮变慢的问题。（[30:07](https://youtu.be/Qa-7iWxDz1A?t=1807)）
- [[object-storage-upload-event-trigger]] — 文件上传到 bucket 后，对象存储会向内部系统发送一个事件（如「文件已上传」），用于触发诸如实时更新前端、发送推送通知等后续动作。（[30:07](https://youtu.be/Qa-7iWxDz1A?t=1807)）
- [[path-based-load-balancer-routing]] — load balancer 除了均衡负载外还能基于 API 路径做路由，例如把以上传（POST upload）开头的请求专门转发给负责文件处理的专用服务，让其余服务器只处理常规流量、保持健康状态。（[09:02](https://youtu.be/Qa-7iWxDz1A?t=542)）
- [[per-service-authorization-microservices]] — 在 microservices 架构中，每个服务可以有自己独立的授权级别，类似各自设置一套 permissions，而不是共用统一的中心化授权规则。（[27:06](https://youtu.be/Qa-7iWxDz1A?t=1626)）
- [[premature-optimization-caution]] — caching、CDN、rate limiting 这类性能优化应放在系统设计讨论的最后阶段引入，避免 premature optimization 导致过度工程化（overengineering）。（[36:09](https://youtu.be/Qa-7iWxDz1A?t=2169)）
- [[presigned-url-auth-optional]] — presigned URL 可以选择不做身份验证（unauthenticated），只要保证上传窗口很短，就是可以接受的设计。（[30:07](https://youtu.be/Qa-7iWxDz1A?t=1807)）
- [[presigned-url-direct-upload]] — 文件上传架构中，服务器可以调用对象存储生成一个 presigned URL，返回给前端后由用户直接上传文件到 bucket，而不经过应用服务器中转。（[30:07](https://youtu.be/Qa-7iWxDz1A?t=1807)）
- [[presigned-url-expiry-window]] — 生成的上传链接必须设置很小的有效期窗口（expiry date），以防止链接被滥用。（[30:07](https://youtu.be/Qa-7iWxDz1A?t=1807)）
- [[presigned-url-size-restriction]] — presigned URL 还可以限制上传文件的大小，例如只允许通过该链接上传最多50MB的文件。（[30:07](https://youtu.be/Qa-7iWxDz1A?t=1807)）
- [[private-key-token-signing]] — 认证服务使用私钥（private key）对新生成的 token 进行签名，确保该 token 的有效性与可信度。（[24:05](https://youtu.be/Qa-7iWxDz1A?t=1445)）
- [[producer-consumer-coupling-scalability]] — 如果不引入 broker，产生事件的服务就必须自己维护一份下游订阅者列表并逐个通知，这种硬编码的点对点通知方式不具备良好的可扩展性，新增订阅者就要改动生产者代码。（[33:08](https://youtu.be/Qa-7iWxDz1A?t=1988)）
- [[ram-caching-large-files-anti-pattern]] — 把整个大文件直接塞进 RAM 缓存是常见的误区，通常成本非常高，不是标准做法。（[39:09](https://youtu.be/Qa-7iWxDz1A?t=2349)）
- [[ram-cost-scarcity]] — 近年来受 AI 需求影响，RAM 价格变得昂贵且是稀缺资源，因此设计缓存时应只用它存放体积小的数据，而不是整份文件。（[39:09](https://youtu.be/Qa-7iWxDz1A?t=2349)）
- [[rate-limiting]] — 系统开始扩展规模时必须设置 rate limiting，否则恶意用户可能借机耗尽基础设施资源，造成资源浪费、增加成本并影响其他正常用户的体验。（[42:09](https://youtu.be/Qa-7iWxDz1A?t=2529)）
- [[rate-limiting-algorithms]] — rate limiting 存在多种不同的实现算法，这是一个值得单独深入的话题，而非只有一种简单计数方式。（[45:11](https://youtu.be/Qa-7iWxDz1A?t=2711)）
- [[rate-limiting-cache-based-counting]] — 因为 cache 是运行在 RAM 中的 key-value storage，读写速度快，非常适合用来实时统计每个用户在时间窗口内（如最近一分钟内发起了五次请求）的请求次数。（[45:11](https://youtu.be/Qa-7iWxDz1A?t=2711)）
- [[redis-in-ram-key-value-cache]] — Redis 是一种 key-value storage，把值缓存在 RAM 中，读取速度比访问磁盘快得多，这是缓存好用的根本原因。（[39:09](https://youtu.be/Qa-7iWxDz1A?t=2349)）
- [[redis-large-blob-limitation]] — 把几十上百 MB 的视频或图片字节直接存进 Redis 通常是错误的做法，因为这类内存很昂贵，而且 Redis 本身并不是为流式传输大体积 blob 设计的。（[39:09](https://youtu.be/Qa-7iWxDz1A?t=2349)）
- [[response-aggregation-gateway]] — API Gateway 可以将多个后端服务（例如 Auth 服务和 Profile 服务）的响应聚合后统一返回给客户端。（[21:05](https://youtu.be/Qa-7iWxDz1A?t=1265)）
- [[round-robin-load-balancing]] — round robin 算法让 load balancer 按顺序依次把新请求分配给不同服务器（例如 A 用户到 server 1，下一个用户到 server 2），使各服务器接收到数量相同的请求。（[09:02](https://youtu.be/Qa-7iWxDz1A?t=542)）
- [[separation-of-concerns-server-database]] — 服务器与数据库解耦后，服务器挂掉或被移除不会影响数据库（数据库不知道服务器的存在），体现了服务器关心服务用户、数据库关心存储数据的关注点分离。（[06:01](https://youtu.be/Qa-7iWxDz1A?t=361)）
- [[serverless-computing]] — serverless 方案意味着开发者不必关心服务器的具体 provisioning，只需提交 Docker image 或 container，由云厂商负责实际运行和管理。（[17:05](https://youtu.be/Qa-7iWxDz1A?t=1025)）
- [[service-to-service-decoupling-via-broker]] — 对象存储不需要知道系统里有哪些下游服务，它只需把上传事件发给一个统一的 broker，由 broker 负责把消息分发给实时服务、通知服务等具体消费者，这才是现实可行的服务间通信方式。（[30:07](https://youtu.be/Qa-7iWxDz1A?t=1807)）
- [[single-point-of-failure]] — 在只有单一服务器实例、且数据与逻辑都耦合其中的最初架构里，服务器宕机会导致服务不可用与数据丢失双重后果。（[03:00](https://youtu.be/Qa-7iWxDz1A?t=180)）
- [[software-architecture-cost-of-change]] — 根据 Martin Fowler 文章的观点，好的架构之所以重要，是因为如果架构设计不好，未来给系统增加新功能会变得更慢、更昂贵。（[00:00](https://youtu.be/Qa-7iWxDz1A?t=0)）
- [[stateful-server-data-coupling]] — 最初版的简单架构中，数据（如文件 ID 到位置的映射）直接以内存结构耦合存放在服务器实例内部，一旦服务器崩溃数据就会丢失。（[03:00](https://youtu.be/Qa-7iWxDz1A?t=180)）
- [[stateless-server-database-decoupling]] — 解决服务器宕机丢数据问题的关键不只是简单地添加一个数据库，而是把服务器变成无状态（stateless），让它每次请求都从独立的数据库中读写数据。（[03:00](https://youtu.be/Qa-7iWxDz1A?t=180)）
- [[sticky-sessions]] — sticky sessions 的核心动机是：如果服务器为该用户保存了某些状态（正在处理的工作），把该用户后续请求继续导向同一服务器会更合理。（[12:03](https://youtu.be/Qa-7iWxDz1A?t=723)）
- [[synchronous-downstream-call-risk]] — 若上传成功后直接同步调用缩略图服务，一旦该服务返回 404、503 或请求超时，视频会永久缺失缩略图，而系统完全不会意识到这一失败，因为上传本身已经成功返回。（[33:08](https://youtu.be/Qa-7iWxDz1A?t=1988)）
- [[token-based-usage-limiting]] — Claude Code 和 ChatGPT 的每日 token 额度本质上和 rate limiting 是同一种思路，只是把限制的资源单位从请求次数换成了 token，因为这类计算资源成本高昂。（[45:11](https://youtu.be/Qa-7iWxDz1A?t=2711)）
- [[unauthorized-401-status-code]] — 若 gateway 边缘验证发现 token 无效，会直接抛出 401 状态码拒绝该请求，而不必转发到后端服务。（[24:05](https://youtu.be/Qa-7iWxDz1A?t=1445)）
- [[uncached-file-request-path]] — 未加缓存前完整的文件获取路径是：gateway 转发请求给 files service，files service 查询 relational database 获取文件元数据，再访问 object storage 取回实际文件，最终把附带元数据的文件返回给 gateway。（[36:09](https://youtu.be/Qa-7iWxDz1A?t=2169)）
- [[understand-what-not-how-to-build]] — 作者认为在当前 AI 辅助编码普及的背景下，理解自己在构建什么（系统架构层面）比知道怎么写代码更重要。（[00:00](https://youtu.be/Qa-7iWxDz1A?t=0)）
- [[uneven-load-distribution-degraded-experience]] — 举例说明：如果大多数用户的请求都涌向其中一台服务器，而另一台还有大量空闲资源，被拥堵的那台服务器上的用户就会遭遇响应变慢等体验下降的问题，原因正是缺少合理的请求分配机制。（[06:01](https://youtu.be/Qa-7iWxDz1A?t=361)）
- [[user-existence-check-before-auth]] — 签发 token 前，系统可能先调用独立的用户服务验证该用户是否已存在于数据库中，只有确认存在后才继续颁发 token；用户服务与认证服务是否合并部署取决于具体架构设计。（[24:05](https://youtu.be/Qa-7iWxDz1A?t=1445)）
- [[vertical-scaling]] — vertical scaling 指不增加机器数量，而是把单台机器换成更强的机器（更多 RAM、CPU、存储），俗称「砸钱解决问题」。（[15:55](https://youtu.be/Qa-7iWxDz1A?t=955)）
- [[video-upload-event-driven-flow]] — 典型上传流程为：客户端经 API gateway 完成鉴权 → metadata 服务创建数据库行并返回 upload URL → 客户端直接把字节上传到 object storage bucket → 缩略图服务异步消费该上传事件，生成预览图并写回结果。（[33:08](https://youtu.be/Qa-7iWxDz1A?t=1988)）
- [[vpc-private-network-isolation]] — 引入 API Gateway 后，所有内部服务被部署在私有虚拟网络（VPC）中，不再对外暴露端口，其 IP 仅在网络内部可达。（[21:05](https://youtu.be/Qa-7iWxDz1A?t=1265)）
- [[weighted-round-robin-load-balancing]] — weighted round robin 是对基础 round robin 算法的扩展，通过权重让不同服务器承担不同比例的流量。（[12:03](https://youtu.be/Qa-7iWxDz1A?t=723)）
