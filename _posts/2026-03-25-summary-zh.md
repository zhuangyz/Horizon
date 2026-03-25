---
layout: default
title: "Horizon Summary: 2026-03-25 (ZH)"
date: 2026-03-25
lang: zh
---

> From 27 items, 12 important content pieces were selected

---

1. [Arm 将首次销售自研芯片，Meta 成首个主要客户，台积电代工](#item-1) ⭐️ 9.0/10
2. [Swift 6.3 正式发布，提供官方 Android SDK，支持原生 Android 应用开发](#item-2) ⭐️ 9.0/10
3. [Apifox 桌面端遭供应链投毒攻击，窃取 SSH 密钥与 Git 凭证](#item-3) ⭐️ 9.0/10
4. [谷歌推出 TurboQuant，用于大语言模型 KV 缓存的极致压缩。](#item-4) ⭐️ 8.0/10
5. [OpenAI 计划停用 Sora AI 视频生成器，并逐步结束与迪士尼的合作](#item-5) ⭐️ 8.0/10
6. [腾讯撤销 AI Lab，密集引入字节 Seed 骨干推进混元模型升级](#item-6) ⭐️ 8.0/10
7. [NASA 暂停月球轨道站，转向 2029 年前建立月球基地目标](#item-7) ⭐️ 8.0/10
8. [中国计算机学会反对 NeurIPS 制裁政策，呼吁抵制投稿](#item-8) ⭐️ 8.0/10
9. [OpenAI 关闭 Sora AI 视频生成应用](#item-9) ⭐️ 7.0/10
10. [Claude Code 推出自动模式，作为危险权限绕过的更安全替代方案](#item-10) ⭐️ 7.0/10
11. [主流包管理器纷纷引入依赖冷却功能以应对供应链攻击。](#item-11) ⭐️ 7.0/10
12. [Claude Code 推出自动模式：AI 自主决策权限，内置安全审查](#item-12) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [Arm 将首次销售自研芯片，Meta 成首个主要客户，台积电代工](https://www.bloomberg.com/news/articles/2026-03-24/arm-to-sell-its-own-chips-for-first-time-in-bid-for-ai-revenue) ⭐️ 9.0/10

Arm Holdings 宣布将首次开始销售自研芯片，首款产品是针对 AI 数据中心工作负载的新型'AGI CPU'。Meta Platforms 是该芯片的首个主要客户，这款芯片最高可配置 136 个核心，功耗为 300 瓦，将由台积电（TSMC）负责制造。 这标志着 Arm 的重大战略转变，从纯粹的知识产权（IP）授权模式转向直接参与芯片销售市场竞争。此举加剧了数据中心 CPU 领域，特别是 AI 工作负载领域的竞争，并可能重塑芯片设计公司、晶圆代工厂和 Meta 等大型云客户之间的格局。 这款 Arm AGI CPU 设计用于与英伟达等公司的加速器芯片协同工作，并声称在能效方面优于英特尔和 AMD 的传统 CPU 设计。基于该芯片的现成系统已由广达电脑和超微电脑等厂商推出，预计将在 2026 年下半年扩大供货量。

telegram · zaihuapd · Mar 25, 02:45

**背景**: Arm Holdings 是一家英国公司，主要以设计 CPU 架构并将其知识产权（IP）授权给苹果、高通、三星等其他公司而闻名，这些公司随后制造自己的芯片。'AGI CPU'基于 Arm 的 Neoverse V3 架构构建，该架构专为云和数据中心应用而设计。台积电（TSMC）是全球最大的半导体合约制造商，为苹果、英伟达、AMD 等公司生产芯片。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://newsroom.arm.com/blog/introducing-arm-agi-cpu">Announcing Arm AGI CPU: The silicon foundation for the agentic AI cloud era - Arm Newsroom</a></li>
<li><a href="https://www.arm.com/products/cloud-datacenter/arm-agi-cpu">Arm AGI CPU – Arm®</a></li>
<li><a href="https://www.cnbc.com/2026/03/24/arm-launches-its-own-cpu-with-meta-as-first-customer.html">Arm launches its own CPU, with Meta as first customer</a></li>

</ul>
</details>

**标签**: `#semiconductors`, `#artificial-intelligence`, `#data-center`, `#hardware`, `#arm-architecture`

---

<a id="item-2"></a>
## [Swift 6.3 正式发布，提供官方 Android SDK，支持原生 Android 应用开发](https://swift.org/blog/swift-6.3-released/) ⭐️ 9.0/10

Swift 6.3 于 2026 年 3 月 25 日正式发布，其中包含了首个官方发布的 Swift SDK for Android。这使得开发者能够使用 Swift 编写原生 Android 应用程序，或通过 Swift Java 互操作性插件将 Swift 代码集成到现有的 Kotlin/Java 应用中。 这标志着一个重大的范式转变，显著扩展了 Swift 在苹果平台之外的生态系统，并可能重塑跨平台移动开发的工作流程。它允许 iOS 开发者利用他们的 Swift 专业知识进行 Android 开发，有可能增加代码复用率，并降低为两大主要移动平台构建应用的门槛。 Swift Java 插件通过将 Java 类包装在相应的 Swift 类型中，允许 Swift 程序调用 Java 库。开发者可以通过查阅官方的 'Getting Started with the Swift SDK for Android' 指南并探索 swift-android-examples 代码库中的示例项目，开始尝试这项新功能。

telegram · zaihuapd · Mar 25, 03:45

**背景**: Swift 是苹果公司开发的一种通用编程语言，于 2014 年首次发布，是开发苹果各平台（iOS、macOS、watchOS、tvOS）应用程序的主要语言。传统的原生 Android 开发使用 Java 或 Kotlin，其中 Kotlin 自 2019 年起成为谷歌推荐的语言。使用 Swift 开发 Android 应用的概念在社区项目中早已存在，但 Swift 6.3 标志着 Swift 项目本身首次提供了官方的、第一方的支持。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.swift.org/blog/swift-6.3-released/">Swift 6.3 Released | Swift .org</a></li>
<li><a href="https://github.com/swiftlang/swift-java">GitHub - swiftlang/swift-java: Java interopability support for Swift · GitHub</a></li>
<li><a href="https://en.wikipedia.org/wiki/Swift_(programming_language)">Swift (programming language) - Wikipedia</a></li>

</ul>
</details>

**标签**: `#swift`, `#android`, `#cross-platform`, `#mobile-development`, `#programming-languages`

---

<a id="item-3"></a>
## [Apifox 桌面端遭供应链投毒攻击，窃取 SSH 密钥与 Git 凭证](http://apifox.it.xn--comcdn-kr3e.openroute.xn--devupgrade-eh3i.feishu.it.com/) ⭐️ 9.0/10

Apifox 桌面端遭遇供应链投毒攻击，攻击者篡改了其内容分发网络（CDN）上的事件统计脚本，注入了恶意代码。该代码会窃取受害主机上的 SSH 密钥、Git 凭证、Shell 历史记录及进程列表等敏感信息，并可进一步植入后门、发起横向攻击。 此事影响重大，因为它直接针对使用流行 API 开发工具的开发者，可能危及无数软件项目及其底层基础设施的安全。它凸显了针对开发者工具的供应链攻击所带来的严重风险，这类攻击可能导致大范围的凭证窃取以及对源代码仓库和服务器的未授权访问。 该攻击自 3 月 4 日起活跃，影响了 Windows、macOS 和 Linux 三平台用户。安全研究员 phith0n 已独立还原恶意载荷并公开了分析代码。用户可通过检查本地特定文件（如 'Network Persistent State' 文件或 LevelDB 中的键值）是否包含 'apifox.it.com' 等恶意域名痕迹来排查是否受影响。

telegram · zaihuapd · Mar 25, 11:10

**背景**: 软件供应链攻击是指将恶意代码注入合法应用程序或其更新机制，以感染其所有用户。SSH 密钥是用于安全远程访问服务器和系统的加密凭证。Git 凭证用于在 GitHub 或 GitLab 等版本控制系统中进行身份验证。LevelDB 是一个快速的键值存储库，应用程序常用来存储本地数据，本次攻击中的恶意脚本就在其结构中搜索敏感信息。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.crowdstrike.com/en-us/cybersecurity-101/cyberattacks/supply-chain-attack/">What Is a Supply Chain Attack? - CrowdStrike</a></li>
<li><a href="https://martin.kleppmann.com/2013/05/24/improving-security-of-ssh-private-keys.html">Improving the security of your SSH private key files — Martin Kleppmann’s blog</a></li>
<li><a href="https://en.wikipedia.org/wiki/LevelDB">LevelDB - Wikipedia</a></li>

</ul>
</details>

**标签**: `#security`, `#supply-chain-attack`, `#api-tools`, `#developer-tools`, `#incident-response`

---

<a id="item-4"></a>
## [谷歌推出 TurboQuant，用于大语言模型 KV 缓存的极致压缩。](https://research.google/blog/turboquant-redefining-ai-efficiency-with-extreme-compression/) ⭐️ 8.0/10

谷歌研究院推出了 TurboQuant，这是一种结合随机旋转和量化的新方法，可在无需重新训练的情况下将大语言模型（LLM）的 KV 缓存压缩至 3 比特。该技术及相关方法 QJL 和 PolarQuant 已在一篇博客文章中公布，并将在 ICLR 2026 和 AISTATS 2026 会议上展示。 这很重要，因为 KV 缓存是大语言模型推理过程中的主要内存瓶颈，尤其是在长上下文任务中，限制了模型的部署和效率。通过大幅减少 KV 缓存内存占用（例如 6 倍或更多），TurboQuant 可以实现更长的上下文窗口、更高的吞吐量和更低的推理成本，使先进的大语言模型更易于使用。 在测试中，与 32 位未量化键相比，4 比特 TurboQuant 在 H100 GPU 上计算注意力 logits 的速度最高提升了 8 倍。该方法在高维向量搜索召回率上也优于 PQ 和 RabbiQ 等现有技术，并且在长上下文“大海捞针”评估中保持了下游任务性能。

hackernews · ray__ · Mar 25, 05:00

**背景**: 在推理过程中，大语言模型会将注意力机制中过去的键（K）和值（V）向量存储在“KV 缓存”中以避免重复计算，但该缓存会消耗大量内存，且随上下文长度增加而增加。KV 缓存压缩技术旨在减少这种内存占用，以提高推理效率。量化是一种常见的压缩方法，它降低了这些存储向量的数值精度（例如，从 32 位降至 4 位）。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arxiv.org/html/2508.06297v1">KV Cache Compression for Inference Efficiency in LLMs: A Review</a></li>
<li><a href="https://research.google/blog/turboquant-redefining-ai-efficiency-with-extreme-compression/">TurboQuant: Redefining AI efficiency with extreme compression</a></li>

</ul>
</details>

**社区讨论**: 社区表现出积极的技术参与，一位用户指出可能遗漏了一项基础旋转技术的引用。另一位用户请求对随机旋转概念进行更简单的解释，而其他人则强调了在 llama.cpp 和 PyTorch 中快速出现的独立实现。另有一条评论批评该博客文章的解释对普通读者而言不够清晰。

**标签**: `#AI Efficiency`, `#Model Compression`, `#KV Cache`, `#LLM Inference`, `#Quantization`

---

<a id="item-5"></a>
## [OpenAI 计划停用 Sora AI 视频生成器，并逐步结束与迪士尼的合作](https://www.bloomberg.com/news/articles/2026-03-24/openai-plans-to-discontinue-support-for-sora-ai-video-generator?srnd=phx-technology) ⭐️ 8.0/10

OpenAI 计划停用其 AI 视频生成产品 Sora 的独立应用及面向开发者的 API，距离该应用高调上线仅约六个月。与 Sora 相关的迪士尼合作也在逐步收尾，公司将资源转向 AI agents 和一款内部代号为 'Spud' 的新模型。 这一决定标志着一家领先的 AI 公司进行了重大的战略转向，从一款旗舰级生成式视频产品转向专注于自主 AI 智能体和下一代基础模型。这凸显了 AI 行业激烈的竞争和快速的演变，即使是备受瞩目的产品也可能昙花一现，因为公司们都在追逐新的技术前沿。 此次停用是 OpenAI 精简其 AI 产品线整体方向的一部分。与此同时，公司正在重组部分安全与保障团队，以便将相关工作更紧密地纳入其新优先事项的开发流程中。

telegram · zaihuapd · Mar 25, 00:30

**背景**: Sora 是 OpenAI 开发的一款文生视频模型及应用，可根据文本提示生成简短、逼真的视频片段。AI agents（智能体），例如 OpenAI 的 Codex，是旨在自主完成复杂任务（如软件工程）的系统。新模型 'Spud' 代表了 OpenAI 的下一个主要 AI 计划，其 CEO Sam Altman 暗示它可能产生重大的经济影响。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Sora_(text-to-video_model)">Sora (text-to- video model) - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/OpenAI_Codex_(AI_agent)">OpenAI Codex (AI agent) - Wikipedia</a></li>
<li><a href="https://www.theinformation.com/articles/openai-ceo-shifts-responsibilities-preps-spud-ai-model">OpenAI CEO Shifts Responsibilities, Preps ‘Spud’ AI Model</a></li>

</ul>
</details>

**标签**: `#OpenAI`, `#AI-Strategy`, `#Video-Generation`, `#Product-Discontinuation`, `#Industry-News`

---

<a id="item-6"></a>
## [腾讯撤销 AI Lab，密集引入字节 Seed 骨干推进混元模型升级](https://mp.weixin.qq.com/s/24ZWs8JFP6seQSSIhU6mOw) ⭐️ 8.0/10

腾讯近期正式撤销了其 AI Lab，并对大模型研发体系进行了重组，同时集中引入了多位原字节跳动 Seed 团队的技术骨干。公司计划于 2026 年 4 月发布新一代的混元基础模型。 此举标志着腾讯在 AI 战略上的重大调整，将其研究力量整合到更偏向产品化、以大模型为中心的路径上，以应对中国日益激烈的生成式 AI 竞争。从字节跳动先进的 Seed 团队引进核心人才，是腾讯为快速增强其技术能力和基础设施所做的直接努力。 引入的关键人才包括原字节 Seed 视觉 AI 平台团队负责人肖学锋，现任腾讯 AI Infra 部助理负责人，以及来自字节 Seed 的黄启，担任训练 Infra 组负责人。重组还包括将原 AI Lab 的部分人员转入大语言模型部。

telegram · zaihuapd · Mar 25, 03:00

**背景**: 腾讯的混元（Hunyuan）是一个基于 Transformer 架构、参数规模达万亿的自研大语言模型，于 2023 年 9 月首次发布。字节跳动的 Seed 团队成立于 2023 年，致力于探索通用人工智能的新方法，研究领域涵盖大语言模型、视觉、语音和 AI 基础设施。'AI Infra'（人工智能基础设施）部门通常专注于大规模开发和部署 AI 模型所需的底层计算系统、工具和平台。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.tencent.com/en-us/articles/2201685.html">Tencent Unveils Hunyuan, its Proprietary Large Foundation ...</a></li>
<li><a href="https://seed.bytedance.com/en/">ByteDance Seed</a></li>

</ul>
</details>

**标签**: `#AI-Industry`, `#Organizational-Strategy`, `#Large-Language-Models`, `#Tencent`, `#Talent-Mobility`

---

<a id="item-7"></a>
## [NASA 暂停月球轨道站，转向 2029 年前建立月球基地目标](https://www.nasa.gov/news-release/nasa-unveils-initiatives-to-achieve-americas-national-space-policy/) ⭐️ 8.0/10

NASA 宣布了一项战略调整，暂停了 Lunar Gateway 月球轨道站的现有方案，将重点转向在 2029 年前建立一个月球表面永久基地。该机构还计划在 2028 年前发射其首个核动力星际飞船 Space Reactor-1 Freedom 前往火星，以验证核电力推进技术。 这标志着 NASA 阿尔忒弥斯计划内部资源的一次重大重新分配，从轨道中转站转向直接、持续的月面作业，可能加速在月球建立长期人类存在的时间表。同时推进核动力技术对于实现更快、能力更强的载人火星任务至关重要，标志着深空探索的一次重大技术飞跃。 新计划的目标是初期每年至少实施一次月面着陆，并计划在 Artemis V 任务之后，通过引入更多商业采购和可重复使用硬件，将载人登月任务频率提升至每六个月一次。NASA 还预计从 2027 年起，通过其商业月球载荷服务计划实施 30 次机器人登月着陆。

telegram · zaihuapd · Mar 25, 04:30

**背景**: Lunar Gateway 是一个原计划绕月运行的小型空间站，旨在作为阿尔忒弥斯计划下宇航员前往月球表面的中转站。阿尔忒弥斯计划是 NASA 的旗舰月球探索计划，于 2017 年正式确立，目标是让人类重返月球并最终执行载人火星任务。核电力推进是一种利用核反应堆发电，然后为高效电推进器提供动力的技术，与用于深空旅行的传统化学火箭相比，它能提供更高的效率和任务灵活性。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Lunar_Gateway">Lunar Gateway - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Artemis_program">Artemis program - Wikipedia</a></li>
<li><a href="https://www.insightsonindia.com/2026/03/25/space-reactor-1-sr-1-freedom-spacecraft/">NASA Space Reactor 1 Freedom : Nuclear Spacecraft & Mars Mission...</a></li>

</ul>
</details>

**标签**: `#space-exploration`, `#nasa`, `#lunar-base`, `#nuclear-propulsion`, `#artemis-program`

---

<a id="item-8"></a>
## [中国计算机学会反对 NeurIPS 制裁政策，呼吁抵制投稿](https://www.ccf.org.cn/Focus/2026-03-25/865918.shtml) ⭐️ 8.0/10

中国计算机学会（CCF）于 2026 年 3 月 25 日发表正式声明，强烈反对 NeurIPS 2026 在其投稿指南中禁止受美国制裁机构投稿的政策。CCF 呼吁中国学者抵制该会议，拒绝投稿或提供学术服务，并警告若 NeurIPS 不及时纠正，将考虑将其从《中国计算机学会推荐国际学术会议和期刊目录》中移除。 这标志着全球 AI 研究政治化的重大升级，一个国家级重要学术机构直接挑战顶级会议的决策。CCF 的推荐目录对中国研究者的投稿选择和职业评估有重大影响，因此其可能将 NeurIPS 除名的举动，将显著重塑全球最大 AI 研究群体之一的参与模式和合作网络。 争议源于 NeurIPS 2026 在其官方投稿指南中明确禁止"美国制裁名单中的部分组织"投稿。CCF 威胁将 NeurIPS 除名的影响尤为重大，因为其《推荐目录》是中国评估研究影响力和学术声誉的广泛认可的标准。

telegram · zaihuapd · Mar 25, 14:07

**背景**: NeurIPS（神经信息处理系统大会）是全球人工智能和机器学习领域最负盛名的年度顶级会议之一。中国计算机学会《推荐国际学术会议和期刊目录》是中国计算机学界极具影响力的排名体系，指导研究者的投稿选择并影响机构评估。美国制裁名单，例如商务部实体清单，包含了受出口管制和限制的外国大学与研究机构，这些限制现在正被延伸至学术会议参与。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Conference_on_Neural_Information_Processing_Systems">Conference on Neural Information Processing Systems - Wikipedia</a></li>
<li><a href="https://www.iconf.com/news/820">CCF Recommended Conference List and How to Understand Computer Science Conference Rankings丨ICONF</a></li>
<li><a href="https://researchpolicy.caltech.edu/research-security/export-compliance/restricted-party-screening/foreign-universities-sanctioned-by-the-us-government">Foreign Universities Sanctioned by the U.S. Government</a></li>

</ul>
</details>

**标签**: `#academic-policy`, `#ai-research`, `#geopolitics`, `#research-ethics`, `#conferences`

---

<a id="item-9"></a>
## [OpenAI 关闭 Sora AI 视频生成应用](https://twitter.com/soraofficialapp/status/2036532795984715896) ⭐️ 7.0/10

OpenAI 正在关闭其 Sora AI 视频生成应用，该应用推出时曾引起巨大关注。这一决定是在该应用未能将用户留存期延长至短暂的新奇感驱动阶段之后做出的。 此次关闭凸显了即使是领先的 AI 公司在实现产品市场契合度以及维持超越初期炒作后的用户参与度方面所面临的挑战。这标志着 OpenAI 产品策略的潜在转变，即从依赖新奇感的独立消费级应用，转向更集成化或更注重实用性的产品。 就在 OpenAI 发布了一份关于 Sora 安全措施的入门指南后不久，关闭公告便随之而来，这表明要么是内部沟通不畅，要么是战略方向的突然转变。据报道，该应用在用户留存方面存在困难，许多用户在经历了初期的创作热潮后，发现没有持续使用的强烈理由。

hackernews · mikeocool · Mar 24, 20:01

**背景**: Sora 是 OpenAI 开发的一款 AI 模型和应用，能够根据文本提示生成逼真的短视频。它是生成式 AI 工具浪潮的一部分，标志着 AI 从生成静态图像向动态视频内容的迈进。该应用允许用户创建和分享这些 AI 生成的视频，将自己定位为一个创意表达平台。

**社区讨论**: 社区情绪复杂，用户分享了个人体验和战略批评。一些用户，如 meken，深情地回忆了最初的创作乐趣，但确认新奇感很快消退，导致应用被弃用。另一些用户，如 johnfn，批评 Sora 缺乏像 GPT 这样的 OpenAI 其他产品所具有的实用性和对用户时间的尊重。评论者还指出了关闭时机相对于近期安全出版物发布的尴尬之处，并对该应用作为专用 AI 视频流的核心价值主张提出了质疑。

**标签**: `#AI`, `#OpenAI`, `#product-strategy`, `#video-generation`, `#startup-failure`

---

<a id="item-10"></a>
## [Claude Code 推出自动模式，作为危险权限绕过的更安全替代方案](https://simonwillison.net/2026/Mar/24/auto-mode-for-claude-code/#atom-everything) ⭐️ 7.0/10

Anthropic 为 Claude Code 推出了自动模式，这是一种新的权限模式，Claude 代表用户做出权限决策，并在执行前通过安全措施监控操作。该模式使用 Claude Sonnet 4.6 作为分类器模型来审查对话，并阻止超出任务范围、针对不受信任的基础设施或似乎由恶意内容驱动的潜在有害操作。 这一进展意义重大，因为它为 --dangerously-skip-permissions 标志提供了一个更安全的替代方案，该标志允许在没有安全措施的情况下完全无人值守执行。自动模式通过在权限决策中引入内置安全检查，代表了 AI 辅助编码安全性的重要进步，可能减少破坏性操作、供应链攻击和未经授权的系统修改等风险。 自动模式包含广泛的默认过滤器，涵盖测试工件、项目范围内的本地操作、只读操作和已声明的依赖项等领域，同时阻止诸如强制推送到 Git、直接推送到默认分支以及执行外部源代码等操作。用户可以通过运行 'claude auto-mode defaults' 查看完整的默认规则，并可以根据特定的安全需求使用自己的规则自定义这些过滤器。

rss · Simon Willison · Mar 24, 23:57

**背景**: Claude Code 是一款 AI 辅助编码工具，之前包含一个 --dangerously-skip-permissions 标志，该标志启用了 'Safe YOLO 模式'，系统在该模式下会绕过所有权限提示以实现不间断执行。Claude Sonnet 4.6 是 Anthropic 最新的 Sonnet 模型，在编码、计算机使用、长上下文推理和智能体规划方面具有增强的能力，支持 100 万 token 的上下文窗口。随着研究表明人工编写和 AI 生成的代码中都可能出现漏洞，AI 生成代码的安全性变得越来越重要，这需要在开发工作流程中建立更好的安全措施。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.anthropic.com/news/claude-sonnet-4-6">Introducing Claude Sonnet 4.6</a></li>
<li><a href="https://blog.promptlayer.com/claude-dangerously-skip-permissions/">claude -- dangerously - skip - permissions</a></li>
<li><a href="https://link.springer.com/article/10.1007/s10664-024-10590-1">How secure is AI-generated code: a large-scale comparison of ...</a></li>

</ul>
</details>

**标签**: `#AI-assisted-coding`, `#developer-tools`, `#code-security`, `#claude-ai`, `#permissions`

---

<a id="item-11"></a>
## [主流包管理器纷纷引入依赖冷却功能以应对供应链攻击。](https://simonwillison.net/2026/Mar/24/package-managers-need-to-cool-down/#atom-everything) ⭐️ 7.0/10

受 2026 年 3 月 LiteLLM 供应链攻击事件启发，近期分析显示，大多数主流包管理器现已实现依赖冷却机制。这包括 pnpm (10.16)、Yarn (4.10.0)、Bun (1.3)、Deno (2.6)、uv (0.9.17)、pip (26.0) 和 npm (11.10.0)，这些工具均在 2025 年末至 2026 年初新增了延迟安装新发布软件包的功能。 这种广泛采用标志着软件供应链安全策略的重大转变，从被动检测转向主动延迟防御。通过为社区提供审查新版本的时间，这些冷却期可以阻止大部分供应链攻击，有研究表明 7 天的冷却期可以预防 80%的此类事件。 具体实现各有不同：大多数工具使用如 `minimumReleaseAge` 或 `--exclude-newer` 等设置来指定延迟期（例如 7 天），并且许多工具为受信任的包提供了豁免机制。一个显著的局限是，pip 26.0 目前其 `--uploaded-prior-to` 标志仅支持绝对时间戳，需要变通方案来实现相对时长。

rss · Simon Willison · Mar 24, 21:11

**背景**: 依赖冷却是一种安全实践，有意将新发布的软件包版本延迟安装一段设定时间（例如 24 小时到 7 天）。这创造了一个软件包已公开但未被自动采用的窗口期，让安全研究人员和自动化工具有时间检测其是否包含通过供应链攻击引入的恶意代码。供应链攻击针对软件开发和分发过程，通常通过入侵合法软件包的发布者账户或构建系统来注入恶意软件，进而传播给所有下游用户。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://blog.yossarian.net/2025/11/21/We-should-all-be-using-dependency-cooldowns">We should all be using dependency cooldowns - blog.yossarian.net</a></li>
<li><a href="https://christian-schneider.net/blog/dependency-cooldowns-supply-chain-defense/">Dependency cooldowns: a simple supply chain fix</a></li>
<li><a href="https://securitylabs.datadoghq.com/articles/litellm-compromised-pypi-teampcp-supply-chain-campaign/">LiteLLM compromised on PyPI: Tracing the March 2026 TeamPCP...</a></li>

</ul>
</details>

**标签**: `#package-management`, `#security`, `#supply-chain`, `#devops`, `#software-engineering`

---

<a id="item-12"></a>
## [Claude Code 推出自动模式：AI 自主决策权限，内置安全审查](https://claude.com/blog/auto-mode) ⭐️ 7.0/10

Anthropic 为 Claude Code 推出了“自动模式”，该功能允许 AI 在执行任务时自主决定权限。该模式通过安全分类器在每次工具调用前审查操作，自动放行安全动作，同时拦截批量删除文件、敏感数据外泄等高危行为。 这代表了 AI 辅助编程领域的一项重要进步，在提升工作流效率和保障安全之间取得了平衡。它让开发者能够以更少的人工中断运行更长、更复杂的任务，同时避免了完全禁用权限检查可能带来的灾难性错误风险。 该功能目前以研究预览形式向 Team 计划用户开放，未来数日内将覆盖 Enterprise 及 API 用户，并支持 Claude Sonnet 4.6 与 Opus 4.6 模型。官方提示，虽然此模式比 `--dangerously-skip-permissions` 参数更安全，但并非零风险，建议在隔离环境中使用，且可能轻微增加 Token 消耗与延迟。

telegram · zaihuapd · Mar 25, 01:15

**背景**: Claude Code 是由 Anthropic 开发的 AI 编程助手。此前，用户面临一个两难选择：要么手动批准每一个操作（这会中断工作流），要么使用 `--dangerously-skip-permissions` 参数（这会赋予 AI 对文件系统、Shell 命令和网络操作的无限制访问权，带来重大安全风险）。自动模式引入了一个由分类器驱动的中间层，旨在自动执行安全决策，同时拦截危险操作。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://claude.com/blog/auto-mode">Auto mode for Claude Code | Claude</a></li>
<li><a href="https://www.zdnet.com/article/claude-code-auto-mode/">How Claude Code's new auto mode prevents AI coding disasters - without slowing you down | ZDNET</a></li>
<li><a href="https://aiwiki.ai/wiki/Claude_--dangerously-skip-permissions">Claude --dangerously-skip-permissions - AI Wiki - Artificial Intelligence Wiki</a></li>

</ul>
</details>

**标签**: `#AI-Assisted Coding`, `#Developer Tools`, `#AI Safety`, `#Claude`, `#Automation`

---