---
layout: default
title: "Horizon Summary: 2026-04-10 (ZH)"
date: 2026-04-10
lang: zh
---

> From 20 items, 4 important content pieces were selected

---

1. [字节跳动发布原生全双工语音模型 Seeduplex，豆包 App 已全面上线](#item-1) ⭐️ 8.0/10
2. [FBI 从 iPhone 通知数据库提取已删除的 Signal 消息](#item-2) ⭐️ 8.0/10
3. [macOS 被曝存在 49.7 天网络故障漏洞，当前需重启修复](#item-3) ⭐️ 7.0/10
4. [OpenAI 推出 100 美元档 ChatGPT Pro 订阅，提供 5 倍于 Plus 版使用额度](#item-4) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [字节跳动发布原生全双工语音模型 Seeduplex，豆包 App 已全面上线](https://seed.bytedance.com/seeduplex) ⭐️ 8.0/10

字节跳动正式推出原生全双工语音大模型 Seeduplex，目前已在豆包 App 全面上线。这标志着全双工技术正式走出实验室，在行业内率先实现大规模落地应用，为数亿用户提供实时、高质量的语音交互体验。 这标志着全双工语音 AI 从研究走向大规模生产环境，是一项重大的行业进步，可能为自然、类人的对话式 AI 设定新标准。它直接影响数亿豆包用户，并可能加速实时语音接口在各种应用中的普及。 该模型通过语音预训练与强化学习（RL）技术，实现了真正的“边听边说”。它在保持极速响应的基础上，专注于实现精准的干扰抑制和动态端点检测。

telegram · zaihuapd · Apr 9, 05:35

**背景**: 传统的语音助手系统通常以“半双工”模式运行，即系统和用户轮流说话和聆听。相比之下，全双工模型专为实时双向交换而设计，允许语音重叠、打断和快速的来回对话，更类似于人类对话。动态端点检测是此类系统中的关键技术挑战，因为它需要准确判断用户何时结束发言，以实现自然的轮流对话。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arxiv.org/abs/2405.19487">[2405.19487] A Full-duplex Speech Dialogue Scheme Based On Large Language Models</a></li>
<li><a href="https://www.emergentmind.com/topics/full-duplex-spoken-dialogue-model">Full-Duplex Spoken Dialogue Model</a></li>
<li><a href="https://arxiv.org/abs/2210.14252">Dynamic Speech Endpoint Detection with Regression Targets</a></li>

</ul>
</details>

**标签**: `#speech-recognition`, `#generative-ai`, `#real-time-systems`, `#bytedance`, `#voice-interface`

---

<a id="item-2"></a>
## [FBI 从 iPhone 通知数据库提取已删除的 Signal 消息](https://www.404media.co/fbi-extracts-suspects-deleted-signal-messages-saved-in-iphone-notification-database-2/) ⭐️ 8.0/10

在得克萨斯州 Prairieland 拘留中心案件的庭审中，FBI 取证人员通过访问 iPhone 的内部通知数据库，提取了已从 Signal 应用中删除的传入消息。该技术从 iOS 系统存储中恢复了仅限传入消息的预览内容，而非传出消息。 这揭示了一个重大的取证漏洞：加密通讯应用的内容可能通过 iOS 通知预览持久地保留在设备上，即使在消息删除后也可能破坏用户的隐私预期。它凸显了锁屏预览等用户便利功能与端到端加密应用安全保证之间的冲突。 该漏洞具体影响的是当 Signal 在锁屏上启用了“显示预览”功能时，这会导致 iOS 将消息内容存储在其内部通知数据库中。Signal 于 3 月 12 日确认收到了置评请求但未后续回复，而苹果未回应相关询问。

telegram · zaihuapd · Apr 9, 14:05

**背景**: Signal 是一款流行的端到端加密通讯应用，通过确保只有发送方和接收方可以读取消息来承诺高隐私性。iOS 通知可以在锁屏上显示消息预览，为了实现此功能，操作系统会临时将预览内容存储在一个系统管理的数据库中。数字取证工具有时可以从该数据库中提取数据，即使源应用已删除其自身的消息副本。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://discuss.privacyguides.net/t/signal-messages-retrieved-from-ios-notification/36475">Signal messages retrieved from iOS notification - General - Privacy Guides Community</a></li>
<li><a href="https://support.signal.org/hc/en-us/articles/360049673331-Storage-Management">Storage Management - Signal Support</a></li>

</ul>
</details>

**标签**: `#digital-forensics`, `#privacy`, `#encrypted-messaging`, `#iOS-security`, `#Signal`

---

<a id="item-3"></a>
## [macOS 被曝存在 49.7 天网络故障漏洞，当前需重启修复](https://www.tomshardware.com/software/macos/macos-has-a-49-7-day-networking-time-bomb-built-in-that-only-a-reboot-fixes-comparison-operation-on-unreliable-time-value-stops-machines-dead-in-their-tracks) ⭐️ 7.0/10

macOS XNU 内核中的一个漏洞会导致系统在连续运行约 49 天 17 小时 2 分 47 秒后，TCP/IP 网络栈失效。问题根源在于一个 32 位无符号整数计时器 (`tcp_now`) 溢出，这违反了 RFC 7323 规范，导致已关闭的 TCP 连接无法被清理，最终耗尽可用的临时端口。 这是一个严重的、'定时炸弹'式的内核级漏洞，主要影响 macOS 服务器、长期运行的工作站或任何长时间不重启的系统。它暴露了核心网络组件中的一个关键缺陷，可能导致网络完全不可用，影响服务、远程访问和系统可靠性。 该漏洞位于 XNU 内核 TCP 栈中的 `tcp_now` 变量内。计时器溢出后，现有连接可能维持，但无法建立新的连接。目前唯一的缓解措施是重启系统，不过研究人员正在研究替代的修复方案。

telegram · zaihuapd · Apr 9, 12:16

**背景**: `tcp_now` 计时器是 TCP 协议栈内部的一个内核时钟，它使用一个 32 位无符号整数记录自启动以来的毫秒数。此类整数的最大值为 4,294,967,295，以毫秒计数时，大约在 49.7 天后就会溢出（归零）。RFC 7323 定义了高性能 TCP 的扩展，并包含了处理此类时间戳回绕场景以维持协议稳定性的规范。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://finance.biggo.com/news/202604080424_macos-tcp-ip-crash-49-days-uptime-bug">macOS TCP/IP Stack Crashes After 49.7 Days of Uptime Due to Kernel Timer Bug — BigGo Finance</a></li>
<li><a href="https://mjtsai.com/blog/2026/04/07/tahoe-tcp-overflow-bug/">Michael Tsai - Blog - Tahoe TCP Overflow Bug</a></li>
<li><a href="http://www.faqs.org/rfcs/rfc7323.html">RFC 7323 - TCP Extensions for High Performance ( RFC 7323 )</a></li>

</ul>
</details>

**标签**: `#macOS`, `#Networking`, `#Kernel`, `#Security`, `#TCP/IP`

---

<a id="item-4"></a>
## [OpenAI 推出 100 美元档 ChatGPT Pro 订阅，提供 5 倍于 Plus 版使用额度](https://help.openai.com/en/articles/9793128-about-chatgpt-pro-plans) ⭐️ 7.0/10

OpenAI 宣布扩展其 ChatGPT Pro 订阅体系，新增每月 100 美元的订阅档位，其使用额度是 20 美元/月的 Plus 版的 5 倍，并限时提供 10 倍的 Codex 使用额度。原有的每月 200 美元方案继续保留，提供 20 倍的使用额度，以满足高强度并行项目的工作流需求。 此次定价更新显著降低了需要高频率使用 AI 的高级用户的入门门槛，使得 GPT-5 和深度研究等高级功能更加触手可及。这代表了 OpenAI 产品策略的一次重要转变，提供了更精细的定价层级，有望吸引更广泛的专业用户和重度个人用户群体。 所有 Pro 计划均包含对 GPT-5 模型、深度研究、Codex、图像创建及文件上传等高级功能的访问权限。目前该订阅仅支持按月计费，不提供年度方案。针对部分地区 iPhone 用户因显示问题无法看到 100 美元选项的情况，OpenAI 建议用户通过 iOS 系统的 Apple Account 订阅设置进行手动选择。

telegram · zaihuapd · Apr 10, 00:35

**背景**: ChatGPT 的使用受到分级限制，这些限制规定了消息发送的频率。免费计划有严格的限制，而 Plus 等付费计划则提供更高的额度。Codex 是 OpenAI 用于代码生成和理解的模型，其使用在订阅计划中也受速率限制。深度研究是 ChatGPT 内的一个 AI 智能体，它能自主浏览网络并综合信息，为用户指定的主题创建全面的、带有引用的报告。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://help.openai.com/en/articles/9793128-what-is-chatgpt-pro">About ChatGPT Pro plans | OpenAI Help Center</a></li>
<li><a href="https://help.openai.com/en/articles/11369540-using-codex-with-your-chatgpt-plan">Using Codex with your ChatGPT plan | OpenAI Help Center</a></li>
<li><a href="https://openai.com/index/introducing-deep-research/">Introducing deep research | OpenAI</a></li>

</ul>
</details>

**标签**: `#OpenAI`, `#ChatGPT`, `#AI Pricing`, `#Subscription Models`, `#Product Updates`

---