---
video_id: G_7AmjfSRQ8
url: https://www.youtube.com/watch?v=G_7AmjfSRQ8
title: 最新软路由代理 Open-Box 发布！全图形极简配置，超越 OpenClash/Nikki/Passwall + SubStore + Zashboard？
channel: 安格视界
published: '2026-09-07'
duration: '24:24'
transcript_origin: subs
tags:
- video
---

# 最新软路由代理 Open-Box 发布！全图形极简配置，超越 OpenClash/Nikki/Passwall + SubStore + Zashboard？

摘要: [[2026-09-07-最新软路由代理-open-box-发布全图形极简配置超越-openclashnikkipasswal-summary|完整摘要]]

## 知识点

- [[anger-supermarket]] — 如果没有机场订阅，可以通过安格超市购买 VPS 自建节点，也可以直接在机场中挑选购买现成的订阅服务。（[15:07](https://youtu.be/G_7AmjfSRQ8?t=907)）
- [[app-specific-traffic-routing-policy]] — Open-Box 面板左侧栏提供策略功能，可以为 AI、Google、Microsoft、Apple 等不同应用/服务分别配置走哪个代理节点，例如作者把 AI 相关流量单独指定走美国的手动节点。（[03:00](https://youtu.be/G_7AmjfSRQ8?t=180)）
- [[custom-site-set-manual-build]] — 新建站点集时可通过关键字（如「test」）联想匹配内置图标，再设置站点集名称、选择规则类型（如 Geosite 域名集），最后逐个手动添加相关域名。（[18:07](https://youtu.be/G_7AmjfSRQ8?t=1087)）
- [[dns-leak-test]] — DNS 泄露是用户使用软路由系统时普遍关心的问题，视频中演示了 Open-Box 在这方面的实测表现。（[00:00](https://youtu.be/G_7AmjfSRQ8?t=0)）
- [[geosite-geoip-builtin-support]] — 创建站点集的规则时可以直接选用内置的 Geosite 域名集或 GeoIP 规则，无需自己手写匹配规则。（[18:07](https://youtu.be/G_7AmjfSRQ8?t=1087)）
- [[gpt-voice-network-quality-test]] — 点击 ChatGPT 的语音功能，如果能很快加载出来并顺畅响应，就说明当前代理网络质量接近原生网络，可以用这个方法快速验证外网连接质量。（[03:00](https://youtu.be/G_7AmjfSRQ8?t=180)）
- [[hexhub-ssh-tool]] — 配置 Open-Box 需要先在 HexHub 上建立到 OpenWrt 路由器的 SSH 连接，才能进行后续的命令行安装操作。（[12:05](https://youtu.be/G_7AmjfSRQ8?t=725)）
- [[no-code-config-ui]] — Open-Box 的节点组配置全程通过图形界面点选完成，不需要手写一行 YAML 或 JSON 代码。（[18:07](https://youtu.be/G_7AmjfSRQ8?t=1087)）
- [[node-group-auto-generation-by-country]] — Open-Box 支持自动按国家规则生成节点组，默认会生成香港、台湾、新加坡、日本、韩国、美国六个节点组。（[18:07](https://youtu.be/G_7AmjfSRQ8?t=1087)）
- [[node-group-country-expansion]] — 若节点池中还存在默认六国之外的其他国家节点，可点击「添加国家」把节点组一次性扩展到14个分组。（[18:07](https://youtu.be/G_7AmjfSRQ8?t=1087)）
- [[node-group-manual-creation]] — 手动添加节点组时需要依次选择图标、填写名称、设定节点分组的规则，再选择具体节点添加进组。（[18:07](https://youtu.be/G_7AmjfSRQ8?t=1087)）
- [[node-group-reorder]] — 已建好的节点组支持重新排序，例如可以把「拒绝」这个节点组调整到列表末尾。（[18:07](https://youtu.be/G_7AmjfSRQ8?t=1087)）
- [[node-group-selection-mode]] — 每个自动生成的节点组都可以设置为自动优选（系统自动挑选最优节点）或手动选择（用户自行指定节点）两种模式。（[18:07](https://youtu.be/G_7AmjfSRQ8?t=1087)）
- [[node-region-switching-ip-dns-consistency-test]] — 把代理站点集分别切换为香港、日本、美国的自动节点后，用 DNS 泄露检测工具刷新验证，IP 和 DNS 显示的地区均与所切换的节点地区完全一致，说明没有出现 DNS 泄露。（[03:00](https://youtu.be/G_7AmjfSRQ8?t=180)）
- [[open-box-add-subscription-modes]] — Open-Box 添加订阅支持两种模式：一种是填写机场的订阅地址，另一种是逐行粘贴单个节点信息直接添加节点。（[15:07](https://youtu.be/G_7AmjfSRQ8?t=907)）
- [[open-box-baidu-routing-case]] — 以百度为例：规则路由按域名后缀 baidu.com 匹配到「国内」规则集，对应直连 DNS 和国内直连出口；真实路由验证显示确实用直连 DNS 解析出百度真实 IP，并通过国内直连节点访问，返回 HTTP 200，规则路由与真实路由完全一致，没有黑洞。（[06:03](https://youtu.be/G_7AmjfSRQ8?t=363)）
- [[open-box-dual-component-architecture]] — Open-Box 由 sing-box 内核和 Open-Box 面板两个组件构成，两者都可以分别启动、停止、重启，并可设置是否开机自启。（[03:00](https://youtu.be/G_7AmjfSRQ8?t=180)）
- [[open-box-firmware-download-channels]] — Open-Box 固件可从阿里云盘或 GitHub 下载，阿里云盘速度可能较慢，有外网环境的用户建议直接去 GitHub 下载。（[12:05](https://youtu.be/G_7AmjfSRQ8?t=725)）
- [[open-box-github-proxy-install-speed]] — 安装 Open-Box 时若通过代理 GitHub 下载会比较慢，若能直连 GitHub 则安装速度会更快。（[15:07](https://youtu.be/G_7AmjfSRQ8?t=907)）
- [[open-box-google-routing-case]] — 以谷歌为例：规则路由匹配到谷歌站点集后应通过代理 DNS 访问、出口为美国节点；真实路由验证显示 DNS 请求确实是通过美国节点发出的，与规则路由预期一致。（[06:03](https://youtu.be/G_7AmjfSRQ8?t=363)）
- [[open-box-install-script-network-branch]] — Open-Box 的安装文档提供两条安装命令，设备能访问外网时复制第一条，仅有国内网络环境时复制第二条（镜像版本）。（[12:05](https://youtu.be/G_7AmjfSRQ8?t=725)）
- [[open-box-manual-vs-auto-policy]] — Open-Box 的策略页面区分手动策略（如“日本手动”，节点固定不变）与自动策略（如“日本自动”，节点会自动切换），两者均可通过鼠标悬停查看其历史表现。（[12:05](https://youtu.be/G_7AmjfSRQ8?t=725)）
- [[open-box-memory-usage-comparison]] — Open-Box 平时运行内存占用极低，约为 45MB，而作者此前使用 OpenClash 实现同样功能时内存轻松突破 200MB，即 Open-Box 的内存占用不到 OpenClash 的 1/5。（[03:00](https://youtu.be/G_7AmjfSRQ8?t=180)）
- [[open-box-multi-subscription-support]] — Open-Box 支持同时添加多条订阅地址，例如一条机场订阅和一条自建节点的订阅，互不冲突。（[15:07](https://youtu.be/G_7AmjfSRQ8?t=907)）
- [[open-box-node-auto-rename]] — Open-Box 解析订阅后会自动为每个节点加上对应订阅名称前缀进行重命名，用户如不满意也可手动修改节点名称。（[15:07](https://youtu.be/G_7AmjfSRQ8?t=907)）
- [[open-box-node-color-coding]] — 节点测速历史全绿表示可用性很好，出现部分超时表示可用性一般，全红并有超时则表示该节点基本不可用。（[12:05](https://youtu.be/G_7AmjfSRQ8?t=725)）
- [[open-box-node-grouping]] — Open-Box 支持把节点按地区做分组（如香港自动、日本自动、美国自动），分流策略可以直接引用这些分组，而不必逐个指定单个节点。（[06:03](https://youtu.be/G_7AmjfSRQ8?t=363)）
- [[open-box-node-history-tracking]] — 传统路由器代理工具没有节点历史数据追踪功能，用户无法直观判断哪些代理节点稳定可靠、哪些不可用。（[12:05](https://youtu.be/G_7AmjfSRQ8?t=725)）
- [[open-box-node-keyword-filter-rule]] — 在 Open-Box 的规则设置页面，将某关键词（如 VM）加入特征关键词栏后，节点名称中带有该关键词的节点会被自动纳入对应筛选组。（[15:07](https://youtu.be/G_7AmjfSRQ8?t=907)）
- [[open-box-openwrt-plugin]] — Open-Box 作为 OpenWrt 的插件安装后，在 LuCI 界面里只提供极简的启停控制，真正的管理功能都在其独立的 Web 面板中，面板入口链接可直接从 LuCI 页面跳转。（[03:00](https://youtu.be/G_7AmjfSRQ8?t=180)）
- [[open-box-outbound-node-groups]] — Open-Box 的出站节点设置实际上是定义节点组，例如“美国自动”节点组或“香港手动”节点组，用于组织不同地区、不同切换策略的节点。（[15:07](https://youtu.be/G_7AmjfSRQ8?t=907)）
- [[open-box-panel-installation]] — Open-Box 面板安装流程是在软路由的 OpenWrt 环境中粘贴指令并回车执行，无需手动编写 YAML 或 JSON 配置文件。（[15:07](https://youtu.be/G_7AmjfSRQ8?t=907)）
- [[open-box-panel-password-setup]] — Open-Box 面板首次打开需要设置两遍密码进行确认，密码长度至少为 4 位。（[15:07](https://youtu.be/G_7AmjfSRQ8?t=907)）
- [[open-box-per-service-routing-policy]] — Open-Box 的分流策略可针对具体服务单独指定出口，例如示例中 Google 走美国自动、Microsoft 走直连、Apple/GitHub/油管走香港自动、TikTok 走台湾节点，且可灵活切换。（[06:03](https://youtu.be/G_7AmjfSRQ8?t=363)）
- [[open-box-policy-group-switch-history]] — 鼠标悬停在自动切换的策略组（如“日本自动”）上，可以看到该策略组实际经历过的节点切换记录，例如从日本07依次切换到日本02、日本01。（[12:05](https://youtu.be/G_7AmjfSRQ8?t=725)）
- [[open-box-project-version]] — Open-Box 项目托管在 GitHub 上，视频录制时的版本号已迭代到 v0.1.131。（[12:05](https://youtu.be/G_7AmjfSRQ8?t=725)）
- [[open-box-pwa-mobile-support]] — Open-Box 做了手机端适配，可以在手机桌面以 PWA（网站应用）形式添加入口，操作逻辑与电脑网页版基本相同，用户外出时也能远程修改家中路由器的分流规则。（[06:03](https://youtu.be/G_7AmjfSRQ8?t=363)）
- [[open-box-router-system]] — Open-Box 定位为一款可以替代 OpenClash、Nikki、Passwall、Sub-Store、Zashboard 组合使用的一体化软路由系统。（[00:00](https://youtu.be/G_7AmjfSRQ8?t=0)）
- [[open-box-same-subnet-requirement]] — 用来配置 Open-Box 的设备网络环境必须和刷入 OpenWrt 的路由器处于同一网段，否则无法建立 SSH 连接。（[12:05](https://youtu.be/G_7AmjfSRQ8?t=725)）
- [[open-box-site-set-domain-lookup]] — Open-Box 提供域名穿透功能，可以查看某个站点集（如 AI 站点集）具体包含哪些域名或 IP。（[06:03](https://youtu.be/G_7AmjfSRQ8?t=363)）
- [[open-box-speed-test-visualization]] — 在 Open-Box 中，进入代理-订阅-展开订阅后，鼠标悬停在测速上会显示该节点最近10次检测结果和对应的趋势折线图。（[12:05](https://youtu.be/G_7AmjfSRQ8?t=725)）
- [[open-box-subscription-self-built-node]] — Open-Box 中的「订阅」对应机场（第三方代理服务商），此外系统也支持接入用户自建的节点。（[06:03](https://youtu.be/G_7AmjfSRQ8?t=363)）
- [[open-box-subscription-setup]] — Open-Box 配置流程中，订阅设置页面用于输入机场的订阅地址，是获取代理节点的核心步骤。（[15:07](https://youtu.be/G_7AmjfSRQ8?t=907)）
- [[open-box-zashboard-frontend]] — Open-Box 的真正主界面前端 UI 复用了 Zashboard 的设计，但后端已经全部替换为 Open-Box 自己的实现，不是简单套壳 Zashboard 原有后台。（[03:00](https://youtu.be/G_7AmjfSRQ8?t=180)）
- [[openbox-first-boot-geosite-geoip-download]] — Open-Box 第一次启动时会自动去下载 Geosite 和 GeoIP 数据库，如果这两个数据库下载不下来，程序就会启动失败。（[21:08](https://youtu.be/G_7AmjfSRQ8?t=1268)）
- [[openbox-hourly-traffic-chart]] — Open-Box 提供按小时统计的流量消耗图表，可用于识别一天中流量使用的高峰时段，例如观察到上午10点到11点为流量高峰。（[09:05](https://youtu.be/G_7AmjfSRQ8?t=545)）
- [[openbox-list-file-fetch-failure-blocks-startup]] — 如果自建域名集配置的 .list 规则文件链接拉取不到，会导致 Open-Box 启动时报错，需要先到目标分流里删掉该规则集的链接，才能让程序继续完成数据库下载并正常启动。（[21:08](https://youtu.be/G_7AmjfSRQ8?t=1268)）
- [[openbox-policy-per-domain-set]] — 在代理的策略页面中，可以为每一个已经建立好的域名集分别定义其对应使用的节点策略，具体分配可根据自己的实际需求来设定。（[21:08](https://youtu.be/G_7AmjfSRQ8?t=1268)）
- [[openbox-post-config-connectivity-verification]] — 完成所有分流规则配置并启动 Open-Box 后，可以打开一个新的浏览器窗口访问外部网站（如 Google 搜索）来验证网络是否已经调通、规则是否生效。（[21:08](https://youtu.be/G_7AmjfSRQ8?t=1268)）
- [[openbox-rule-display-order-vs-hit-order]] — 在设置窗口里可以单独调整规则集的显示排序（例如把某条规则拖到列表下方以避免显得突兀），但这只影响界面展示顺序，右侧实际命中规则的判定顺序并不会因此改变。（[21:08](https://youtu.be/G_7AmjfSRQ8?t=1268)）
- [[openbox-rule-top-down-matching]] — 规则命中是从上往下匹配的，如果某个域名集规则排在后面、而前面的规则已经包含了相同的域名或 IP，那么这条规则可能永远不会被命中，因此需要把它拖到最上面确保生效。（[21:08](https://youtu.be/G_7AmjfSRQ8?t=1268)）
- [[openbox-terminal-traffic-splitting]] — 终端分流功能允许按局域网内设备的 IP 单独指定网络策略，可选择让该 IP 走某个具体节点、走直连，或者直接拒绝联网。（[21:08](https://youtu.be/G_7AmjfSRQ8?t=1268)）
- [[openbox-traffic-drilldown-by-device]] — Open-Box 支持按终端设备维度钻取当天流量明细，可看到各设备的流量消耗量及占比排名（如某设备当天消耗2.6GB、占比42%排第一），并可继续下钻查看该设备访问的具体网站及各网站消耗的流量、所使用的出站节点。（[09:05](https://youtu.be/G_7AmjfSRQ8?t=545)）
- [[openbox-traffic-drilldown-by-node]] — Open-Box 支持按出站节点维度查看当天流量消耗分布，并可继续钻取该节点承载的具体访问站点及各站点消耗的流量（如显示 ChatGPT 消耗了1.5GB流量）。（[09:05](https://youtu.be/G_7AmjfSRQ8?t=545)）
- [[openbox-traffic-drilldown-by-time-period]] — 除按整天维度统计外，Open-Box 还支持选定具体时间段（如10点到11点），并在该时间段内继续按终端设备、出站节点、访问目标三个维度进行钻取分析。（[09:05](https://youtu.be/G_7AmjfSRQ8?t=545)）
- [[openbox-traffic-overview-dashboard]] — Open-Box 的流量概览页面同时展示实时流量信息和按日统计的流量消耗柱状图，每个柱子可点击切换查看不同日期（含上个月）的具体流量数值。（[09:05](https://youtu.be/G_7AmjfSRQ8?t=545)）
- [[openbox-url-diagnosis-tool]] — Open-Box 支持直接输入域名或粘贴完整 URL 进行诊断，返回实际访问的真实 IP、是否命中 CDN 缓存、出站所走的节点（如美国节点）、域名解析出的 IP 以及 HTTP 状态码，用于排查站点访问规则问题。（[09:05](https://youtu.be/G_7AmjfSRQ8?t=545)）
- [[openwrt-ssh-login-credentials]] — 通过 SSH 连接 OpenWrt 路由器时，默认地址通常是 10.0.0.1，用户名为 root，密码为安装 OpenWrt 时自行设置的密码。（[12:05](https://youtu.be/G_7AmjfSRQ8?t=725)）
- [[openwrt-x86-requirement]] — 安装配置 Open-Box 前，需要先准备一台已刷好 x86 架构 OpenWrt 固件的路由器。（[12:05](https://youtu.be/G_7AmjfSRQ8?t=725)）
- [[passwall-shared-network-transparent-proxy]] — 共享网络（Passwall 服务端功能）可以把整台路由器透明代理到某个节点上，之后用 Karing 等软件连接该路由器节点，就能直接享受路由器上已配置好的分流规则。（[21:08](https://youtu.be/G_7AmjfSRQ8?t=1268)）
- [[rule-routing-vs-real-routing]] — 在 Open-Box 的规则页面输入域名（如 www.baidu.com）后，系统会同时展示「规则路由」（理论上应匹配的规则集、DNS 和出口）与「真实路由」（路由器真实执行一遍得到的结果），两者对比即可验证是否存在黑洞。（[06:03](https://youtu.be/G_7AmjfSRQ8?t=363)）
- [[rule-set-list-file-import]] — 自定义域名可以整理成 .list 文件，复制该文件的 Raw 链接后粘贴到「规则集链接」字段，即可批量导入为规则集，无需逐条手动添加。（[18:07](https://youtu.be/G_7AmjfSRQ8?t=1087)）
- [[shared-network-requires-public-ip]] — 共享网络功能能否发挥实际作用的前提是路由器需要拥有公网 IP，如果没有公网 IP，这个功能基本没有意义。（[21:08](https://youtu.be/G_7AmjfSRQ8?t=1268)）
- [[site-set-category-types]] — 一个站点集条目内部通常包含域名后缀、域名关键字、IP、域名集以及规则集链接等多种分类信息。（[18:07](https://youtu.be/G_7AmjfSRQ8?t=1087)）
- [[site-set-detail-preview]] — 每个站点集条目旁会显示一个数字详情入口，点击后可以查看该站点集具体包含的域名列表，例如 YouTube 站点集的详情。（[18:07](https://youtu.be/G_7AmjfSRQ8?t=1087)）
- [[software-router-black-box-problem]] — 传统软路由系统流量怎么走、经过哪些路由、节点是否可用都是黑箱状态，出问题时无从排查，被认为是最可怕的缺陷。（[00:00](https://youtu.be/G_7AmjfSRQ8?t=0)）
- [[software-router-blackhole-problem]] — 传统软路由（如 OpenClash、Nikki）存在多种「黑洞」，其中之一是站点访问规则黑洞：站点的 DNS 解析方式与实际出口难以追溯，排查非常复杂。（[06:03](https://youtu.be/G_7AmjfSRQ8?t=363)）
- [[software-router-configuration-complexity]] — 配置传统软路由系统前需要先理解 DNS、网络栈、TUN、FakeIP、分流策略等一大堆专业概念，门槛很高。（[00:00](https://youtu.be/G_7AmjfSRQ8?t=0)）
- [[software-router-fragmented-toolchain]] — 配置好 OpenClash 或 Nikki 之后仍需单独配一个面板（如原版 Zashboard），若功能不够全还得换成作者自制的 Ange-Board。（[00:00](https://youtu.be/G_7AmjfSRQ8?t=0)）
- [[software-router-ui-complexity]] — 很多软路由系统把无数选项和开关全部甩给用户，用户只能一个一个去试，配置失误同样可能导致设备变砖。（[00:00](https://youtu.be/G_7AmjfSRQ8?t=0)）
- [[target-routing-domain-set]] — Open-Box 的「目标分流」本质上就是域名集管理，即维护一组组预先定义好的域名或 IP 集合，供分流规则调用。（[18:07](https://youtu.be/G_7AmjfSRQ8?t=1087)）
- [[tiktok-loading-network-quality-test]] — 打开 TikTok 直接测试视频加载速度和切换流畅度，如果视频秒开、切换如同刷抖音一样丝滑，说明代理外网质量良好，这是常用的外网质量测试方法之一。（[03:00](https://youtu.be/G_7AmjfSRQ8?t=180)）
- [[traffic-blackhole-problem]] — 传统路由器用户往往完全不清楚自己的流量到底去了哪里、是否浪费、是否存在异常流量，而机场和节点流量通常都是按流量计费的，这构成所谓的「流量黑洞」问题。（[09:05](https://youtu.be/G_7AmjfSRQ8?t=545)）
- [[youtube-loading-latency-user-test]] — 手机连接家里 Wi-Fi 后打开 YouTube，视频一下就能加载出来，切换视频也很快，拖动进度条同样能秒切，说明经过 Open-Box 代理后手机端访问外网视频的体验流畅。（[03:00](https://youtu.be/G_7AmjfSRQ8?t=180)）
