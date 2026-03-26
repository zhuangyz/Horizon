---
layout: default
title: "Horizon Summary: 2026-03-26 (ZH)"
date: 2026-03-26
lang: zh
---

> From 35 items, 10 important content pieces were selected

---

1. [苹果与谷歌宣布达成多年合作，Gemini AI 将为下一代 Apple Foundation Models 提供支持。](#item-1) ⭐️ 9.0/10
2. [谷歌宣布在 Android 17 中引入后量子加密](#item-2) ⭐️ 9.0/10
3. [欧洲议会否决 Chat Control 1.0，阻止强制扫描私人信息。](#item-3) ⭐️ 8.0/10
4. [洛杉矶陪审团裁定 Instagram 和 YouTube 故意使儿童上瘾，判赔 600 万美元](#item-4) ⭐️ 8.0/10
5. [LiteLLM PyPI 攻击事件：46 分钟内 4.7 万次恶意下载，88%的依赖包未锁定版本](#item-5) ⭐️ 8.0/10
6. [Apifox 桌面端遭供应链投毒攻击，CDN 脚本被篡改](#item-6) ⭐️ 8.0/10
7. [中科院发布“香山”开源处理器和“如意”原生操作系统，启动下一代联合研发](#item-7) ⭐️ 8.0/10
8. [行业资深人士警告 AI 智能体开发速度失控，呼吁关注代码质量而非数量。](#item-8) ⭐️ 7.0/10
9. [英特尔和 AMD 通知中国客户服务器 CPU 交付周期将延长](#item-9) ⭐️ 7.0/10
10. [GitHub 更新 Copilot 数据政策：免费与个人付费版默认纳入 AI 模型训练，可手动退出](#item-10) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [苹果与谷歌宣布达成多年合作，Gemini AI 将为下一代 Apple Foundation Models 提供支持。](https://t.me/zaihuapd/40506) ⭐️ 9.0/10

苹果与谷歌宣布达成一项多年合作协议，谷歌的 Gemini AI 模型及云技术将成为下一代 Apple Foundation Models 的基础。这些增强后的模型将为今年推出的苹果智能功能提供支持，包括更个性化的 Siri，同时相关功能将继续在设备端和私有云计算环境中运行。 此次合作代表了 AI 领域的范式转变，将两大科技巨头联合起来，可能重塑移动 AI 助手和行业竞争格局。这使苹果能立即获得谷歌先进的 Gemini 模型，同时让谷歌的 AI 技术深度嵌入 iOS 生态系统，可能影响数十亿用户，并为移动设备的 AI 功能设定新标准。 苹果强调，通过此次合作实现的 AI 功能将继续在设备端和其私有云计算（Private Cloud Compute）基础设施上运行，维持现有的隐私标准。此次合作具体涉及谷歌的 Gemini 模型为苹果的基础模型提供底层技术支持，而非将 Gemini 直接集成到苹果设备中。

telegram · zaihuapd · Mar 25, 16:32

**背景**: Apple Foundation Models 指的是苹果专有的大型语言模型，为其跨设备的'Apple Intelligence'功能提供支持。这些模型包括紧凑的设备端模型（约 30 亿参数）和使用混合专家架构的、更大的基于服务器的模型。谷歌的 Gemini 是一个多模态 AI 模型系列，以其强大能力闻名，例如 Gemini 1.5 具备一百万 token 的上下文窗口。行业正在隐私/速度优先的设备端 AI 和处理复杂任务的云端 AI 之间寻求平衡，苹果的私有云计算代表了一种混合方法，在卸载密集型计算的同时保持隐私。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arxiv.org/pdf/2507.13575">Apple Intelligence Foundation Language Models : Tech Report 2025</a></li>
<li><a href="https://en.wikipedia.org/wiki/Gemini_(language_model)">Gemini (language model) - Wikipedia</a></li>
<li><a href="https://www.theverge.com/news/818364/google-private-ai-compute">Google is introducing its own version of Apple’s private AI cloud compute | The Verge</a></li>

</ul>
</details>

**标签**: `#AI-Partnerships`, `#Mobile-AI`, `#Tech-Giants`, `#Siri`, `#Gemini`

---

<a id="item-2"></a>
## [谷歌宣布在 Android 17 中引入后量子加密](https://security.googleblog.com/2026/03/post-quantum-cryptography-in-android.html) ⭐️ 9.0/10

谷歌宣布将在 Android 17 中引入后量子加密标准，具体方案包括在引导加载程序中加入具备量子抗性的数字签名，并将 Android 密钥库系统迁移至符合 PQC 标准的架构。 这是对数十亿 Android 设备的一次基础性安全升级，旨在主动防范未来量子计算可能破解当前加密体系的攻击。它为整个行业向量子抗性安全过渡树立了一个关键先例。 此次升级针对两个关键安全组件：引导加载程序的签名链（防止设备启动阶段被篡改）和密钥库（保障身份验证和敏感数据传输的安全）。该实现遵循了美国国家标准与技术研究院于 2024 年 8 月发布的最终版后量子加密标准。

telegram · zaihuapd · Mar 26, 07:09

**背景**: 后量子加密指的是设计用于抵御经典计算机和量子计算机攻击的加密算法。当前广泛使用的公钥密码学（如 RSA 和 ECC）容易受到足够强大的量子计算机利用肖尔算法的攻击。为此，像 NIST 这样的标准化机构一直在努力最终确定新的 PQC 算法。Android 密钥库是一个在设备上安全存储加密密钥的系统，可防止密钥被提取。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.nist.gov/news-events/news/2024/08/nist-releases-first-3-finalized-post-quantum-encryption-standards">NIST Releases First 3 Finalized Post-Quantum Encryption Standards</a></li>
<li><a href="https://developer.android.com/privacy-and-security/keystore">Android Keystore system | Security | Android Developers</a></li>

</ul>
</details>

**标签**: `#post-quantum-cryptography`, `#android-security`, `#quantum-computing`, `#cryptography`, `#mobile-security`

---

<a id="item-3"></a>
## [欧洲议会否决 Chat Control 1.0，阻止强制扫描私人信息。](https://bsky.app/profile/tuta.com/post/3mhxkfowv322c) ⭐️ 8.0/10

欧洲议会投票否决了备受争议的'Chat Control 1.0'提案，该提案本将强制要求扫描私人信息以查找儿童性虐待材料。这一决定阻止了一个要求科技公司扫描加密通信的系统的实施。 这是欧盟数字隐私和加密技术的一次重大胜利，因为它阻止了一个会破坏端到端加密的大规模监控系统的建立。该决定维护了基本的隐私权，并拒绝了一个被安全专家广泛批评的技术上存在问题的方案。 此次投票明确否决了无差别扫描的提案，但斗争尚未结束，关于'Chat Control 2.0'法规的谈判仍在继续。此外，允许科技公司自愿扫描儿童性虐待材料的临时规则已延长至 2026 年 4 月，这为 Gmail 等服务设定了合规期限。

hackernews · lemoncookiechip · Mar 26, 12:30

**背景**: 欧盟的'Chat Control'提案是一项旨在打击网络儿童性虐待材料的立法倡议。它提议使用'客户端扫描'技术，即在信息加密前在用户设备上进行分析，批评者认为这种方法从根本上破坏了端到端加密并制造了安全漏洞。该提案引发了关于儿童保护与隐私权及技术可行性之间平衡的重大辩论。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.webpronews.com/inside-the-eus-encryption-war-how-chat-control-became-europes-most-dangerous-surveillance-proposal/">Inside the EU 's Encryption War: How ' Chat Control ' Became...</a></li>
<li><a href="https://www.eff.org/deeplinks/2019/11/why-adding-client-side-scanning-breaks-end-end-encryption">Why Adding Client-Side Scanning Breaks End-To-End Encryption</a></li>
<li><a href="https://www.euractiv.com/news/commission-proposes-two-year-extension-to-csam-chat-scanning-rules/">Commission proposes two-year extension to CSAM chat-scanning ...</a></li>

</ul>
</details>

**社区讨论**: 社区评论澄清了投票涉及多个程序步骤，并警告称关于'Chat Control 2.0'的谈判意味着斗争仍在继续。一些用户对现有的扫描做法表示困惑，而另一些则讽刺地指出'保护儿童'常被用来为监控措施辩护。讨论中还提到了支持该提案的政治游说活动。

**标签**: `#privacy`, `#eu-regulation`, `#surveillance`, `#policy`, `#encryption`

---

<a id="item-4"></a>
## [洛杉矶陪审团裁定 Instagram 和 YouTube 故意使儿童上瘾，判赔 600 万美元](https://www.latimes.com/california/story/2026-03-25/social-media-lawsuit-trial-meta-google-verdict) ⭐️ 8.0/10

2026 年 3 月 25 日，洛杉矶一个陪审团作出了一项里程碑式的裁决，认定 Meta 旗下的 Instagram 和 Google 旗下的 YouTube 被故意设计成具有使儿童上瘾的功能。陪审团裁定这两家科技巨头需支付 600 万美元的赔偿金。 这一裁决确立了一个关键的法律先例，可能使社交媒体平台因其以参与度为导向的设计所造成的危害而面临广泛的赔偿责任。它标志着一种转变，即法院可能要求公司对其算法和产品功能造成的心理影响直接负责，这可能会引发一波类似的诉讼，并迫使平台设计发生重大改变。 该裁决特别关注了使儿童上瘾的故意设计选择，而不仅仅是对社交媒体的普遍批评。此案紧随新墨西哥州另一项针对 Meta 的 3.75 亿美元裁决之后，据报道，Meta 的保险公司已被免除对此类索赔的承保责任，这意味着未来的赔付可能直接影响公司的资产负债表。

hackernews · 1vuio0pswjnm7 · Mar 26, 12:15

**背景**: 社交媒体平台通常使用复杂的算法来最大化用户参与度和应用使用时间。这些算法由自然语言处理和聚类等机器学习技术驱动，通过分析用户行为来个性化内容推送。其设计通常融入了行为心理学的原理，例如可变奖励（如不可预测的'点赞'），这可能会激活大脑中与动机和成瘾相关的多巴胺通路。多年来，关于科技公司对这些设计选择所应承担的伦理责任的争论一直在持续。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://pmc.ncbi.nlm.nih.gov/articles/PMC11804976/">Social Media Algorithms and Teen Addiction: Neurophysiological Impact and Ethical Considerations - PMC</a></li>
<li><a href="https://hai.stanford.edu/news/psychiatrists-perspective-social-media-algorithms-and-mental-health">A Psychiatrist's Perspective on Social Media Algorithms and ...</a></li>

</ul>
</details>

**社区讨论**: 社区评论提出了技术和监管解决方案，例如立法强制允许用户选择第三方推荐算法。一些用户质疑任何吸引儿童并使用 A/B 测试或自学习算法的平台如何能避免类似责任，而另一些人则强调了短视频和'愤怒诱饵'内容的特殊效力。此外，也有讨论认为，如果更多州提起类似诉讼，这些裁决的财务规模可能会影响公司的资产负债表。

**标签**: `#social-media`, `#regulation`, `#tech-ethics`, `#addiction`, `#legal`

---

<a id="item-5"></a>
## [LiteLLM PyPI 攻击事件：46 分钟内 4.7 万次恶意下载，88%的依赖包未锁定版本](https://simonwillison.net/2026/Mar/25/litellm-hack/#atom-everything) ⭐️ 8.0/10

对 BigQuery PyPI 数据集的分析显示，在 LiteLLM Python 包于 PyPI 上被攻击的 46 分钟内，其恶意版本 1.82.7 和 1.82.8 被下载了 46,996 次。分析还发现，在 2,337 个依赖 LiteLLM 的软件包中，有 88% 没有采用正确的版本锁定机制，这导致它们无法避免安装受攻击的版本。 此事件凸显了 Python 生态系统中供应链攻击的严重性和快速影响，表明一个流行库的短暂被攻击如何在几分钟内影响数万次下载。依赖包中缺乏正确版本锁定的高比例，暴露了依赖管理实践中普遍存在的漏洞，使许多项目面临类似攻击的风险。 该分析使用了 Google BigQuery 的公共 PyPI 数据集，该数据集将 PyPI 的下载日志流式传输以供分析。受攻击的软件包仅在线上存在了 46 分钟，却获得了近 4.7 万次下载，这显示了 LiteLLM 库的高使用量。

rss · Simon Willison · Mar 25, 17:21

**背景**: LiteLLM 是一个开源 Python 库，它提供了一个统一的接口，使用 OpenAI 格式来调用超过 100 种不同的大型语言模型（LLM）API（如 OpenAI、Anthropic 和 Vertex AI）。PyPI（Python 包索引）是 Python 软件包的官方仓库，开发者在此发布和安装库。版本锁定是一种安全和可复现的实践，项目通过它明确指定所需依赖的确切版本（或一个狭窄的兼容范围），从而防止自动安装新的、可能受攻击的版本。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.litellm.ai/">LiteLLM</a></li>
<li><a href="https://kindatechnical.com/python/lesson-46-pip-and-pypi.html">pip and PyPI: Installing, Upgrading, and Pinning Packages - kindatechnical() | A Guide to Learning and Mastering Python</a></li>
<li><a href="https://docs.pypi.org/api/bigquery/">BigQuery Datasets - PyPI Docs</a></li>

</ul>
</details>

**标签**: `#security`, `#supply-chain`, `#python`, `#pypi`, `#packaging`

---

<a id="item-6"></a>
## [Apifox 桌面端遭供应链投毒攻击，CDN 脚本被篡改](https://t.me/zaihuapd/40514) ⭐️ 8.0/10

Apifox 桌面端遭受供应链投毒攻击，攻击者篡改了其官方 CDN 上托管的事件统计脚本，注入了高度混淆的恶意 JavaScript 代码。该恶意载荷自 3 月 4 日起活跃，会窃取受影响 Windows、macOS 和 Linux 系统中的 SSH 密钥、Git 凭证、Shell 历史记录及进程列表等敏感信息。 此事影响重大，因为 Apifox 是一款广泛使用的 API 开发工具，如此规模的供应链攻击直接针对开发者和企业，可能导致大规模的凭证泄露、对代码仓库的未授权访问以及在网络内的横向渗透。这凸显了在开发工具中依赖外部 CDN 提供可执行代码所带来的关键安全风险。 知名安全研究员 phith0n 已独立分析并确认了此次攻击，并公开分享了恶意载荷的分析代码。被篡改的脚本是一个前端事件追踪文件，此次攻击向量表明，篡改单个 CDN 托管的资源就足以危及一个跨所有主流操作系统广泛分发的桌面应用程序。

telegram · zaihuapd · Mar 26, 04:19

**背景**: 供应链攻击是指针对软件开发或分发流程中安全性较弱的环节进行攻击，从而危害最终产品。CDN（内容分发网络）用于托管和快速全球分发脚本等静态文件，但一旦被攻破，就可能向所有用户提供恶意代码。SSH 密钥和 Git 凭证是用于认证访问服务器和 GitHub 等版本控制系统的关键凭据；窃取这些凭据将使攻击者能够访问敏感的基础设施和源代码。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.binance.com/en/square/post/03-26-2026-apifox-desktop-client-faces-supply-chain-attack-with-malicious-code-injection-305605946597617">Apifox Desktop Client Faces Supply Chain Attack with Malicious...</a></li>
<li><a href="https://httptoolkit.com/blog/public-cdn-risks/">Public CDNs Are Useless and Dangerous</a></li>
<li><a href="https://docs.github.com/en/authentication/connecting-to-github-with-ssh/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent">Generating a new SSH key and adding it to the ssh -agent - GitHub Docs</a></li>

</ul>
</details>

**标签**: `#security`, `#supply-chain-attack`, `#developer-tools`, `#credentials-theft`, `#malware`

---

<a id="item-7"></a>
## [中科院发布“香山”开源处理器和“如意”原生操作系统，启动下一代联合研发](https://h.xinhuaxmt.com/vh512/share/13024070?docid=13024070) ⭐️ 8.0/10

3 月 26 日，在中关村论坛年会的 RISC-V 生态科技论坛上，中国科学院集中发布了“香山”开源高性能 RISC-V 处理器和“如意”原生操作系统。同时，论坛现场启动了下一代“昆明湖”架构与“如意”操作系统的联合开发项目，中国移动、中国电信、中兴、阿里、腾讯、字节跳动等数十家单位将参与协同攻关。 此举标志着中国在构建自主开源硬件与软件生态方面迈出重要一步，有助于减少对专有架构的依赖。“香山”处理器性能达到国际先进水平，并已获得多家芯片公司的商业采用，这表明 RISC-V 生态正在成熟，未来有望在特定市场对 ARM 和 x86 等传统架构构成挑战。 “香山”处理器的关键细节在于，它同步推出了全球首个开源的片上互连网络（NoC）IP，这是多核处理器设计中的关键组件。目前，基于“香山”的高性能开源芯片已实现规模化产业落地，进迭时空、蓝芯算力、芯动科技、奕斯伟计算等企业已推出商用芯片，表明其已从研究阶段进入产业部署。

telegram · zaihuapd · Mar 26, 10:08

**背景**: RISC-V 是一种开放标准的处理器指令集架构（ISA），允许任何人设计、制造和销售 RISC-V 芯片而无需支付授权费，这与 ARM 和 x86 等专有架构形成对比。片上互连网络（NoC）是集成电路上的通信子系统，通常用于系统级芯片（SoC）中各个 IP 核之间的连接。“原生”操作系统是指为特定硬件架构从头构建的操作系统，而非从现有系统移植或适配，这通常能带来更好的性能和集成度。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://link.springer.com/article/10.1007/s11432-014-5248-8">Reliability-aware mapping for various NoC topologies and routing ...</a></li>
<li><a href="https://www.ithome.com/0/931/668.htm">阿里达摩院官宣 2026 玄铁 RISC - V 生态大会，有“重磅发布”环节 - IT之家</a></li>

</ul>
</details>

**标签**: `#RISC-V`, `#Open-Source Hardware`, `#Operating Systems`, `#Computer Architecture`, `#Semiconductors`

---

<a id="item-8"></a>
## [行业资深人士警告 AI 智能体开发速度失控，呼吁关注代码质量而非数量。](https://simonwillison.net/2026/Mar/25/thoughts-on-slowing-the-fuck-down/#atom-everything) ⭐️ 7.0/10

OpenClaw 所使用的 Pi 智能体框架的创建者 Mario Zechner 发表评论，认为当前 AI 智能体开发的狂热浪潮已导致工程纪律的丧失，优先考虑海量代码生成而非深思熟虑的设计与审查。他警告称，这种不受控制的速度会让错误迅速累积，在代码库中造成不可持续的技术债务和认知债务。 这一批评之所以重要，是因为它揭示了 AI 辅助软件开发这一快速演进领域中的系统性风险，即代码生成能力已远超人类理解和维护的能力。如果不加以解决，这一趋势可能导致脆弱、难以管理的软件系统激增，从而损害 AI 驱动工程工具的长期价值和可靠性。 Zechner 特别建议对 AI 智能体每日生成的代码量设置上限，使其与团队的审查能力相匹配，并坚持核心架构和 API 决策必须手工编写。博客文章作者 Simon Willison 赞同关于速度与严谨性之间失衡的核心担忧，但并不完全认同手工编码是定义系统架构的最佳解决方案。

rss · Simon Willison · Mar 25, 21:47

**背景**: 智能体工程（Agentic Engineering）是一门新兴学科，专注于设计能够自主规划、使用工具并以最少人力干预完成复杂任务的 AI 智能体。Pi 框架是一个用于构建此类 AI 智能体的 TypeScript 工具包，被开源个人 AI 助手 OpenClaw 所使用。“认知债务”这一概念指的是当系统演进到超出我们完全理解的能力时，所累积的心智负担和复杂性。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/badlogic/pi-mono">GitHub - badlogic/pi-mono: AI agent toolkit: coding agent CLI ...</a></li>
<li><a href="https://grokipedia.com/page/Agentic_Engineering">Agentic Engineering</a></li>
<li><a href="https://en.wikipedia.org/wiki/OpenClaw">OpenClaw - Wikipedia</a></li>

</ul>
</details>

**标签**: `#AI Agents`, `#Software Engineering`, `#Technical Debt`, `#Code Quality`, `#Industry Trends`

---

<a id="item-9"></a>
## [英特尔和 AMD 通知中国客户服务器 CPU 交付周期将延长](https://t.me/zaihuapd/40507) ⭐️ 7.0/10

英特尔和 AMD 已通知其中国客户服务器 CPU 供应紧张，其中英特尔部分 CPU 的交付周期最长达到 6 个月，AMD 部分产品的交付周期则被拉长至 8 至 10 周。英特尔还对其第四代和第五代至强（Xeon）处理器在华进行限量供货，并导致其服务器产品在中国的整体价格上涨超过 10%。 此次供应中断直接影响中国的数据中心、云计算和 AI 基础设施建设，可能延缓关键的数字化转型和计算项目。这凸显了全球半导体供应链持续存在的脆弱性，并可能加速中国在高性能计算组件领域追求更大程度自给自足的努力。 英特尔将部分供需失衡归因于 AI 的快速采用带动了"传统计算"的需求，并预计其库存将在 2026 年第一季度达到最低点，之后在第二季度开始改善。这些供应限制不仅限于中国，而是影响全球 PC 和服务器制造商的更广泛供应链问题的一部分。

telegram · zaihuapd · Mar 26, 00:03

**背景**: 服务器 CPU，如英特尔的至强（Xeon）和 AMD 的霄龙（EPYC）处理器，是专为服务器和数据中心设计的中央处理器，负责处理云服务、数据库和企业应用的关键工作负载。第四代和第五代英特尔至强可扩展处理器代表了这些高性能芯片的最新代际。根据行业分析，全球服务器需求一直在增长，戴尔、HPE 和联想等企业 OEM 厂商在 2024 年第二季度至第三季度显示出显著的出货量增长。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.trendforce.com/presscenter/news/20240701-12213.html">Upstream Supply Chain Replenishment and Increased Demand ...</a></li>
<li><a href="https://asianmorning.com/2026/03/25/intel-and-amd-supply-constraints-threaten-global-pc-market-stabilization-efforts/">Intel and AMD Supply Constraints Threaten Global PC Market ...</a></li>
<li><a href="https://www.gurufocus.com/news/8743019/intel-amd-supply-constraints-weigh-on-pc-and-server-manufacturers?r=4bf001661e6fdd88d0cd7a5659ff9748?r=4bf001661e6fdd88d0cd7a5659ff9748?r=4bf001661e6fdd88d0cd7a5659ff9748?r=4bf001661e6fdd88d0cd7a5659ff9748">Intel, AMD Supply Constraints Weigh on PC and Server ...</a></li>

</ul>
</details>

**标签**: `#semiconductors`, `#supply-chain`, `#china-tech`, `#server-hardware`, `#geopolitics`

---

<a id="item-10"></a>
## [GitHub 更新 Copilot 数据政策：免费与个人付费版默认纳入 AI 模型训练，可手动退出](https://github.blog/news-insights/company-news/updates-to-github-copilot-interaction-data-usage-policy/) ⭐️ 7.0/10

GitHub 宣布更新 Copilot 交互数据使用政策：自 4 月 24 日起，Copilot Free、Pro 和 Pro+ 用户的输入、输出、代码片段及相关上下文将默认用于训练和改进其 AI 模型，用户可在“隐私”设置中选择退出；此前已关闭相关数据收集选项的用户，其偏好将继续保留。 这一变更对数百万个人开发者影响重大，他们的编码模式和反馈现在默认成为 GitHub AI 的训练资源，这在使用广泛的开发者工具中引发了关于数据隐私和所有权的重要问题。它突显了一个日益增长的行业趋势，即利用用户与 AI 助手的交互来改进模型，而企业客户则保留更严格的数据控制权。 该政策明确排除了 Copilot Business 和 Copilot Enterprise 用户以及企业私有代码库的代码。可用于训练的数据包括光标附近的代码上下文、注释与文档、文件名、仓库结构、导航模式及对建议的反馈；相关数据可与包括 Microsoft 在内的关联公司共享，但不会提供给第三方 AI 模型提供商。

telegram · zaihuapd · Mar 26, 00:47

**背景**: GitHub Copilot 是由 GitHub 和 OpenAI 开发的 AI 代码补全工具，集成在代码编辑器中。它根据开发者的当前上下文建议整行或整块的代码。该服务提供多个层级：免费版、个人付费计划（Pro, Pro+）以及按用户按月收费的商业/企业计划，后者提供定制化和全平台聊天等功能。AI 模型在庞大的数据集上进行训练，“选择退出机制”是允许用户要求其数据不用于此目的的功能，尽管其实施和有效性有时存在争议。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/features/copilot/plans">GitHub Copilot · Plans & pricing · GitHub</a></li>
<li><a href="https://dev.to/tiamatenity/the-ai-training-data-opt-out-lie-why-your-prompts-are-being-used-anyway-pa6">The AI Training Data Opt - Out Lie: Why Your... - DEV Community</a></li>

</ul>
</details>

**标签**: `#GitHub Copilot`, `#AI Ethics`, `#Data Privacy`, `#Developer Tools`, `#Microsoft`

---