---
video_id: G_7AmjfSRQ8
title: 最新软路由代理 Open-Box 发布！全图形极简配置，超越 OpenClash/Nikki/Passwall + SubStore + Zashboard？
source: '[[2026-09-07-最新软路由代理-open-box-发布全图形极简配置超越-openclashnikkipasswal]]'
tags:
- summary
_gen:
  prompt_hash: 209b52739480c30c61b7dcc0392dfa4aa0deb99654ee921af5e045409c961f85
  task_hash: 2b8c0fe0ab215cfb5d2248edb8a173dfc3c82ae7074cc824dbdcb52e5973a541
  schema_version: 1
  model: sonnet
  generated_at: '2026-09-09T00:28:05+00:00'
---

## 一句话总结

[[open-box-router-system]] 是一款一体化软路由代理系统,用图形界面和"规则路由 vs 真实路由"对照诊断,一次性解决了传统 OpenClash/Nikki/Passwall + Sub-Store + Zashboard 组合中长期存在的黑箱、流量黑洞和配置复杂问题。

## 核心内容

### 传统软路由的三大痛点

视频开篇([00:00])直指传统软路由系统的核心缺陷。首先是 [[software-router-configuration-complexity]]:配置前需要先理解 DNS、网络栈、TUN、FakeIP 等一堆专业概念,而且很多系统设计前后矛盾、功能重叠,一不小心配置错误就可能导致路由器变砖,只能重新刷机。其次是 [[software-router-fragmented-toolchain]]:光是搭起一套可用系统就要装 OpenClash/Nikki 做代理内核、Sub-Store/Sub-Web 做订阅聚合、再单独配一个面板(如 Ange-Board),工具链非常碎片化。最后也是最致命的是 [[software-router-black-box-problem]]:流量怎么走、经过哪些路由、节点是否可用全是黑箱,出问题时根本无从排查。此外 [[software-router-ui-complexity]] 也让用户面对无数开关和选项无所适从。

Open-Box 采用 [[open-box-dual-component-architecture]],由 sing-box 内核和 Open-Box 面板两部分构成,均可独立启停并设置开机自启([03:00])。它作为 [[open-box-openwrt-plugin]] 安装,LuCI 里只保留极简启停控制,真正的管理都在独立 Web 面板中完成。面板前端复用了 [[open-box-zashboard-frontend]] 的 UI 设计,但后端已全部替换为自有实现。资源消耗方面,[[open-box-memory-usage-comparison]] 显示 Open-Box 常驻内存约 45MB,而作者此前用 OpenClash 实现同等功能内存轻松突破 200MB,不到其 1/5。

### 用"真实路由"打破黑洞:诊断能力是最大卖点

针对 [[software-router-blackhole-problem]](站点访问规则黑洞,DNS 解析方式和实际出口难以追溯)与 [[traffic-blackhole-problem]](流量去向不明、机场按流量计费却说不清花在哪),Open-Box 给出了系统性的解决方案([06:03]、[09:05])。

核心武器是 [[rule-routing-vs-real-routing]]:在规则页面输入任意域名,系统会同时展示"规则路由"(理论上应匹配的规则集/DNS/出口)和"真实路由"(路由器真实执行后的结果),两者对比即可验证有无黑洞。视频用两个案例验证:[[open-box-baidu-routing-case]] 显示百度确实走直连 DNS + 国内出口,返回 HTTP 200,规则与真实完全一致;[[open-box-google-routing-case]] 则验证谷歌确实通过美国节点发出 DNS 请求,与预期一致。配合 [[openbox-url-diagnosis-tool]],可直接输入域名或粘贴 URL,返回真实 IP、是否命中 CDN、出站节点、解析 IP 和 HTTP 状态码,方便排查具体站点问题。

流量可见性方面,[[openbox-traffic-overview-dashboard]] 提供实时流量和按日统计柱状图(可回看上月数据);[[openbox-hourly-traffic-chart]] 按小时统计,视频中观察到上午 10-11 点是流量高峰([09:05]);在此基础上可以做三维钻取——[[openbox-traffic-drilldown-by-device]] 按终端设备查看消耗占比(某设备当天 2.6GB、占 42% 排第一,还能继续看它访问了哪些网站);[[openbox-traffic-drilldown-by-node]] 按出站节点查看承载的站点流量(如 ChatGPT 消耗 1.5GB);[[openbox-traffic-drilldown-by-time-period]] 则支持选定某个时段(如 10-11 点)后再按设备/节点/目标继续下钻。

### 节点与分流:全图形化,支持按服务精细分流

Open-Box 支持 [[open-box-node-grouping]],把节点按地区自动分组(如香港自动、日本自动、美国自动),分流策略可直接引用分组而非逐个指定节点。在此基础上做 [[open-box-per-service-routing-policy]] 和 [[app-specific-traffic-routing-policy]]:视频示例中 Google 走美国自动、Microsoft 走直连、Apple/GitHub/YouTube 走香港自动、TikTok 走台湾节点、AI 相关流量单独指定美国手动节点([03:00]、[06:03])。

节点组配置([18:07])完全通过 [[no-code-config-ui]] 完成,不需要写一行 YAML/JSON。[[node-group-auto-generation-by-country]] 默认生成港/台/新/日/韩/美六个分组,若节点池里还有其他国家节点,可用 [[node-group-country-expansion]] 一键扩展到 14 个分组。也支持 [[node-group-manual-creation]](选图标、填名称、设规则、选节点)和 [[node-group-reorder]](如把"拒绝"组调到列表末尾)。每个分组可设 [[node-group-selection-mode]]:自动优选或手动指定。

目标分流层面,[[target-routing-domain-set]] 本质是域名集管理。新建 [[custom-site-set-manual-build]] 时可用关键字联想内置图标、选规则类型([[geosite-geoip-builtin-support]] 可直接用内置 Geosite/GeoIP,无需手写匹配规则)、逐个添加域名;大批量域名则可整理成 .list 文件,通过 [[rule-set-list-file-import]] 粘贴 Raw 链接批量导入。每个 [[site-set-category-types]] 条目内部含域名后缀、关键字、IP、域名集、规则集链接等多种分类,支持 [[site-set-detail-preview]] 查看具体域名列表。配置好的每个域名集都能在 [[openbox-policy-per-domain-set]] 中单独指定节点策略([21:08])。

### 节点质量追踪与可用性验证

传统工具缺乏 [[open-box-node-history-tracking]],用户无法判断哪些节点稳定。Open-Box 的 [[open-box-speed-test-visualization]] 悬停节点测速可看最近 10 次检测及趋势折线图([12:05]),并用 [[open-box-node-color-coding]] 直观区分:全绿=可用性好,部分超时=一般,全红=基本不可用。策略页面区分 [[open-box-manual-vs-auto-policy]](手动节点固定 vs 自动节点自行切换),悬停自动策略组还能看 [[open-box-policy-group-switch-history]](如"日本自动"从日本07→日本02→日本01 的实际切换记录)。

网络质量的用户侧验证用了三个实测:[[gpt-voice-network-quality-test]](ChatGPT 语音是否秒开顺畅)、[[tiktok-loading-network-quality-test]](TikTok 视频秒开、切换是否丝滑)、[[youtube-loading-latency-user-test]](手机连 Wi-Fi 后 YouTube 秒开、拖进度条秒切)。另外用 [[dns-leak-test]] 配合 [[node-region-switching-ip-dns-consistency-test]] 验证:切换港/日/美自动节点后,DNS 泄露检测显示的 IP 和 DNS 地区与所切节点完全一致([03:00])。手机端还有 [[open-box-pwa-mobile-support]],可添加到桌面以 PWA 形式使用,外出时也能远程改家里路由器的分流规则。

### 安装与订阅配置流程

安装前提是准备好 [[openwrt-x86-requirement]](x86 架构 OpenWrt 固件)。配置设备须满足 [[open-box-same-subnet-requirement]],通过 [[hexhub-ssh-tool]] 建立 SSH 连接,登录凭证遵循 [[openwrt-ssh-login-credentials]](默认地址 10.0.0.1、用户名 root、密码为刷机时自设密码)([12:05])。固件下载走 [[open-box-firmware-download-channels]](阿里云盘或 GitHub,有外网建议直接上 GitHub),安装脚本按 [[open-box-install-script-network-branch]] 分两条命令(能上外网用第一条,纯国内网络用镜像版第二条),[[open-box-github-proxy-install-speed]] 提示直连 GitHub 会比走代理更快。[[open-box-panel-installation]] 全程只是在 OpenWrt 里粘贴命令回车,无需手写配置文件;首次打开面板要按 [[open-box-panel-password-setup]] 设置两遍密码(至少 4 位)。

订阅方面,[[open-box-subscription-setup]] 是获取节点的核心步骤,[[open-box-add-subscription-modes]] 支持两种方式:填机场订阅地址,或逐行粘贴单个节点。[[open-box-multi-subscription-support]] 允许同时添加多条订阅(如一条机场+一条自建节点)互不冲突。没有订阅的话可通过 [[anger-supermarket]] 购买 VPS 自建节点或直接买机场订阅。[[open-box-subscription-self-built-node]] 说明"订阅"对应机场,系统同时也支持自建节点接入。解析后 [[open-box-node-auto-rename]] 会自动加订阅名前缀重命名节点(可手动改);[[open-box-node-keyword-filter-rule]] 支持按关键词(如 VM)自动把匹配节点纳入筛选组;[[open-box-outbound-node-groups]] 实质是定义节点组(如"美国自动""香港手动")来组织节点。[[open-box-site-set-domain-lookup]] 可查看某站点集(如 AI)具体包含的域名/IP。

### 首次启动排错与进阶功能

[[openbox-first-boot-geosite-geoip-download]] 提示 Open-Box 首次启动会自动下载 Geosite/GeoIP 数据库,下载失败则程序启动失败;若自建的 [[openbox-list-file-fetch-failure-blocks-startup]] 规则文件链接拉取不到,也会导致报错,需先去目标分流里删掉该规则集链接才能让数据库下载完成、程序正常启动([21:08])。

规则生效有个重要细节——[[openbox-rule-display-order-vs-hit-order]]:设置窗口里调整规则集显示排序只影响界面展示,不影响右侧实际命中顺序;而 [[openbox-rule-top-down-matching]] 才是真正的判定逻辑——规则从上往下匹配,如果某域名集规则排在后面而前面规则已包含相同域名/IP,这条规则可能永远不会命中,需要拖到最上面确保生效。

配置完成后建议做 [[openbox-post-config-connectivity-verification]]:开新浏览器窗口访问 Google 等外网站点验证是否调通、规则是否生效。进阶功能还有 [[openbox-terminal-traffic-splitting]](按局域网设备 IP 单独指定走某节点/直连/拒绝联网)和 [[passwall-shared-network-transparent-proxy]](共享网络,把整台路由器透明代理到某节点,配合 Karing 等软件连接后直接复用路由器分流规则),但后者有前提条件 [[shared-network-requires-public-ip]]——没有公网 IP 这个功能基本没意义。

## 值得记住的细节

- [00:00] 传统组合需要 OpenClash/Nikki + Sub-Store/Sub-Web + 独立面板(如 Ange-Board)才能凑齐功能,Open-Box 一体化替代。
- [03:00] Open-Box 内存占用约 45MB,OpenClash 实现同等功能超 200MB(不到 1/5)。
- [06:03] 百度案例:直连 DNS + 国内直连出口,HTTP 200,规则与真实路由一致;谷歌案例:DNS 请求经美国节点发出,与预期一致。
- [09:05] 上午 10-11 点为流量高峰时段;某设备当天消耗 2.6GB 占 42% 排第一;ChatGPT 单项消耗 1.5GB。
- [12:05] SSH 默认地址 10.0.0.1,用户名 root,密码为刷 OpenWrt 时自设;视频录制时 Open-Box 版本为 v0.1.131。
- [12:05] 节点测速悬停显示最近 10 次检测结果+趋势折线图;全绿=可用性好,部分超时=一般,全红=基本不可用。
- [15:07] Open-Box 面板首次打开需设置两遍密码,至少 4 位。
- [15:07] 安装 Open-Box 时通过代理下 GitHub 较慢,直连 GitHub 更快。
- [18:07] 默认自动生成 6 个国家节点组(港/台/新/日/韩/美),可通过"添加国家"扩展到 14 个。
- [21:08] 陷阱:规则展示排序≠实际命中顺序,展示顺序调整只是界面显示;真正生效要靠把规则拖到匹配列表最上面(从上往下匹配)。
- [21:08] 陷阱:自建 .list 规则链接拉取失败会直接阻塞 Open-Box 启动(因为要先下载完 Geosite/GeoIP),需先删掉该链接才能让程序启动。
- [21:08] 共享网络(类 Passwall 透明代理整机)功能生效前提是路由器必须有公网 IP。

## 这个视频适合谁 / 可以跳过什么

**适合**:正在用 OpenClash/Nikki/Passwall + Sub-Store + Zashboard 拼凑软路由、苦于配置复杂和"黑箱排障"的用户;想要图形化无代码配置、并且关心流量和节点历史可追溯性的用户;已有 x86 OpenWrt 路由器、准备迁移到更省内存方案的用户。

**可跳过**:如果只是想快速了解 Open-Box 是什么,可跳过 [12:05]-[18:07] 的详细安装/SSH/订阅配置操作步骤,直接看 [00:00]-[09:05] 的痛点对比与诊断功能演示即可抓住核心卖点;已经很熟悉 Geosite/GeoIP 概念的用户也可以跳过 [18:07] 里域名集/规则集导入的基础讲解部分。
