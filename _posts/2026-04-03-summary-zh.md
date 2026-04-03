---
layout: default
title: "Horizon Summary: 2026-04-03 (ZH)"
date: 2026-04-03
lang: zh
---

> From 26 items, 13 important content pieces were selected

---

1. [Google DeepMind 发布 Gemma 4，这是一个具备视觉和音频能力的高效开源模型家族。](#item-1) ⭐️ 9.0/10
2. [Google 发布 Gemma 4 开放模型家族，提供四种规格覆盖手机到工作站](#item-2) ⭐️ 9.0/10
3. [vLLM v0.19.0 发布，支持 Gemma 4、零气泡异步调度及多项性能升级。](#item-3) ⭐️ 8.0/10
4. [前 Azure 核心工程师详述侵蚀微软云平台信任度的决策](#item-4) ⭐️ 8.0/10
5. [Axios 供应链攻击使用针对维护者的高度定向社交工程](#item-5) ⭐️ 8.0/10
6. [Simon Willison 在 Lenny 播客中探讨 AI 拐点与智能体工程](#item-6) ⭐️ 8.0/10
7. [工信部通报苹果设备高危漏洞风险：涉及 iOS 17.2.1 及以下版本](#item-7) ⭐️ 8.0/10
8. [Blogosphere：一个社区策展的个人博客首页聚合器发布，提供极简版和标准版。](#item-8) ⭐️ 7.0/10
9. [Cursor 发布 Cursor 3，主打面向 AI 代理的软件开发统一工作区。](#item-9) ⭐️ 7.0/10
10. [Google Vids 接入 Veo 3.1，普通用户可免费生成 AI 视频](#item-10) ⭐️ 7.0/10
11. [美国人形机器人依赖中国技术提供关键内部组件](#item-11) ⭐️ 7.0/10
12. [调查指 LinkedIn 扫描用户浏览器扩展并向第三方共享数据](#item-12) ⭐️ 7.0/10
13. [逆向工程揭示如何绕过 Claude Code 基于 Bun 的 API 签名，从而开启快速模式](#item-13) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [Google DeepMind 发布 Gemma 4，这是一个具备视觉和音频能力的高效开源模型家族。](https://simonwillison.net/2026/Apr/2/gemma-4/#atom-everything) ⭐️ 9.0/10

Google DeepMind 发布了 Gemma 4，这是一个包含四个新模型的开源推理模型家族，采用 Apache 2.0 许可证，模型规模包括 2B、4B、31B 以及一个 26B-A4B 的混合专家（MoE）变体。这些模型具备视觉能力，其中较小的 E2B 和 E4B 模型还具备原生音频输入功能，可用于语音识别和理解。 此次发布代表了在创建小型、高性能模型方面的重大进展，推动了'单位参数智能'效率的边界，这对于设备端和具有成本效益的 AI 部署至关重要。Apache 2.0 许可证和多模态能力（视觉、音频）使这些模型对广大开发者和超越纯文本的各类应用而言，变得高度可访问且实用。 较小的模型（E2B, E4B）使用了一种称为逐层嵌入（Per-Layer Embeddings, PLE）的新技术，以最大化设备端使用的参数效率，其中'E'代表'有效'参数规模。虽然 2B、4B 和 26B-A4B 模型已经可以通过 LM Studio 等工具在本地运行，但作者指出 31B 模型的输出存在问题，并且本地音频输入支持在常用工具中尚未广泛可用。

rss · Simon Willison · Apr 2, 18:28

**背景**: 逐层嵌入（Per-Layer Embeddings, PLE）是一种参数高效技术，它为每个解码器层提供自己的小型词元嵌入表，使得大型嵌入表可以存储在速度较慢但容量更大的 CPU 内存中，而非稀缺的 GPU 显存中，从而显著降低了设备端模型的内存占用。混合专家（Mixture-of-Experts, MoE）架构用于 26B-A4B 变体，这种设计将每个输入仅路由到一小部分专门的子网络（'专家'），使得模型可以拥有庞大的总参数量以具备知识容量，同时保持每个词元的计算成本较低，从而实现更快、更便宜的推理。在小型语言模型（SLM）中追求'参数效率'是一个关键的研究领域，旨在弥合巨型模型与适用于边缘设备的紧凑、可部署版本之间的能力差距。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://huggingface.co/blog/rishiraj/matformer-in-gemma-3n">Understanding Gemma 3n: How MatFormer Gives You Many Models in One</a></li>
<li><a href="https://arxiv.org/abs/2507.11181">[2507.11181] Mixture of Experts in Large Language Models</a></li>
<li><a href="https://newsletter.maartengrootendorst.com/p/a-visual-guide-to-mixture-of-experts">A Visual Guide to Mixture of Experts (MoE) What is mixture of experts? - IBM What Is Mixture of Experts (MoE)? How Modern LLMs Get ... Mixture of Experts Explained - Hugging Face What Is Mixture of Experts (MoE)? How It Works (2026)</a></li>

</ul>
</details>

**标签**: `#llm`, `#open-source`, `#model-efficiency`, `#computer-vision`, `#google-deepmind`

---

<a id="item-2"></a>
## [Google 发布 Gemma 4 开放模型家族，提供四种规格覆盖手机到工作站](https://blog.google/innovation-and-ai/technology/developers-tools/gemma-4/) ⭐️ 9.0/10

Google 发布了 Gemma 4 开放模型家族，包含 E2B、E4B、26B MoE 和 31B Dense 四种规格，覆盖从 Android 设备、笔记本 GPU、开发工作站到加速器的部署场景，并以 Apache 2.0 许可证开放。 此次发布通过提供一系列针对不同硬件（从边缘设备到高性能服务器）优化的模型，并在商业友好的许可下，显著推进了高性能、易获取的 AI 技术发展。31B 模型在 Arena AI 文本榜单的开放模型中排名第 3，加之 Gemma 家族累计下载量已超 40 亿次，这证明了其巨大的社区采用度，并有望加速整个生态系统的 AI 应用开发。 该系列模型主打高级推理和 Agent 工作流，支持函数调用、结构化 JSON 输出、代码生成以及图像和视频处理，其中 E2B 和 E4B 还支持原生音频输入。较小的 E2B 和 E4B 模型面向端侧离线运行，支持 128K 上下文窗口，而较大的模型最高支持 256K 上下文。

telegram · zaihuapd · Apr 2, 16:12

**背景**: Gemma 是 Google 开发的一个开放、轻量级的大语言模型（LLM）家族。其中 26B 规格采用的 Mixture of Experts (MoE) 架构是一种神经网络设计，它将计算分割到多个“专家”子网络中，从而在推理时以更低的计算成本获得更强的性能。Apache 2.0 许可证是一种宽松的自由软件许可证，允许广泛的商业和开源使用，但要求保留版权声明和免责声明。Arena AI 是一个通过众包、并排比较模型响应来对大语言模型进行基准测试的流行平台。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://developer.nvidia.com/blog/applying-mixture-of-experts-in-llm-architectures/">Applying Mixture of Experts in LLM Architectures | NVIDIA ...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Apache_License">Apache License - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Arena_(AI_platform)">Arena ( AI platform) - Wikipedia</a></li>

</ul>
</details>

**标签**: `#open-source-ai`, `#llm`, `#google-research`, `#model-deployment`, `#apache-license`

---

<a id="item-3"></a>
## [vLLM v0.19.0 发布，支持 Gemma 4、零气泡异步调度及多项性能升级。](https://github.com/vllm-project/vllm/releases/tag/v0.19.0) ⭐️ 8.0/10

vLLM v0.19.0 已发布，该版本引入了对 Google Gemma 4 模型架构的完整支持、结合推测解码的零气泡异步调度系统，以及对 Model Runner V2 引擎的重大增强。此版本还包括 ViT 全 CUDA 图捕获、通用的 CPU KV 缓存卸载机制，以及对 NVIDIA B300/GB300 GPU 的支持。 此次发布意义重大，因为它直接提升了大规模语言模型服务的吞吐量和效率，这是实际 AI 应用的关键瓶颈。结合推测解码的零气泡异步调度以及通用的 CPU KV 缓存卸载，能够实现更高的请求并发度，并更好地利用 GPU 和 CPU 内存，从而降低大规模推理的成本和延迟。 零气泡异步调度功能专门消除了在推测解码激活时处理批次之间的空闲时间（气泡），这是一项新颖的性能优化。此外，新的 CPU KV 缓存卸载机制被描述为“通用”的，并具有可插拔的缓存策略和块级抢占处理，使其比之前的实现更加灵活。

github · khluu · Apr 3, 02:19

**背景**: vLLM 是一个用于大规模语言模型的高吞吐、内存高效的推理和服务引擎。推测解码是一种推理加速技术，由一个更小、更快的“草案”模型提议几个潜在的下一个 token，然后由更大的目标模型并行验证，从而降低总体延迟。CUDA 图是 NVIDIA 的一项技术，通过将一系列 GPU 操作捕获到一个单一、可重放的图中，以减少内核启动开销。KV（键-值）缓存卸载涉及将模型的工作内存部分从昂贵的 GPU 内存移动到更大、更便宜的 CPU 内存，以处理更长的上下文或更多的并发请求。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://deepwiki.com/npuichigo/vllm/8.1-speculative-decoding">Speculative Decoding | npuichigo/vllm | DeepWiki</a></li>
<li><a href="https://docs.vllm.ai/en/stable/design/cuda_graphs/">CUDA Graphs - vLLM</a></li>
<li><a href="https://blog.vllm.ai/2026/01/08/kv-offloading-connector.html">Inside vLLM’s New KV Offloading Connector: Smarter Memory Transfer for Maximizing Inference Throughput | vLLM Blog</a></li>

</ul>
</details>

**标签**: `#llm-inference`, `#performance-optimization`, `#model-serving`, `#gpu-acceleration`, `#open-source`

---

<a id="item-4"></a>
## [前 Azure 核心工程师详述侵蚀微软云平台信任度的决策](https://isolveproblems.substack.com/p/how-microsoft-vaporized-a-trillion) ⭐️ 8.0/10

微软 Azure 核心团队的一名前工程师发表了一份详细报告，指控公司内部特定的技术和组织决策系统性地破坏了 Azure 的可靠性和开发文化。该工程师声称，在公开之前，他曾在内部（包括向 CEO）提出过担忧，但未得到任何回应。 这一内部视角罕见地揭示了全球最大云服务提供商之一的系统性问题，可能证实了用户对 Azure 复杂性和可靠性的普遍不满。如果这些指控属实，则表明其存在根深蒂固的技术债务和文化问题，可能影响这一关键全球数字基础设施的长期竞争力和可信度。 报告引述的一个具体例子是，工程团队变得过于规避风险，以至于连基本的代码重构和错误修复（例如采用智能指针）都因担心破坏现有功能而被拒绝。署名的作者表示，这是在内部报告渠道失效后不得已采取的最后手段。

hackernews · axelriet · Apr 2, 16:00

**背景**: Microsoft Azure 是全球第二大云计算平台，提供用于构建、部署和管理应用程序的广泛服务。技术债务指的是现在选择一种简单、有限或快速的解决方案，而非需要更长时间但更好的方法，所导致的未来返工的隐含成本。在大型云平台中，管理技术债务并维护一种优先考虑可靠性和可持续工程的文化，是其长期成功的关键挑战。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Microsoft_Azure">Microsoft Azure - Wikipedia</a></li>
<li><a href="https://www.gartner.com/en/infrastructure-and-it-operations-leaders/topics/technical-debt">Reduce and Manage Technical Debt - Gartner</a></li>

</ul>
</details>

**社区讨论**: 社区评论反映了认同、担忧和分析的混合情绪。一些用户表示，他们使用 Azure 时遇到的界面卡顿、文档质量差和服务复杂等问题，与这位工程师的指控相符。另一些人则争论微软的核心能力究竟在于软件工程，还是在于商业合同和销售。此外，也有关于消息来源可信度以及工程文化变得过于恐惧而无法进行必要改进所带来的严重后果的讨论。

**标签**: `#cloud-computing`, `#microsoft`, `#software-engineering`, `#technical-debt`, `#industry-critique`

---

<a id="item-5"></a>
## [Axios 供应链攻击使用针对维护者的高度定向社交工程](https://simonwillison.net/2026/Apr/3/supply-chain-social-engineering/#atom-everything) ⭐️ 8.0/10

Axios 团队发布了一份事后分析报告，揭示最近一次导致恶意软件通过版本发布的供应链攻击，是通过一次针对特定维护者的、高度定制化的复杂社交工程活动执行的。攻击者冒充一家公司的创始人，将维护者诱骗到一个逼真的虚假 Slack 工作区和 Microsoft Teams 会议中，并诱使其安装了远程访问木马。 这一事件凸显了威胁行为者策略的重大升级，从利用技术漏洞转向对开源生态系统中关键个人进行高度个性化的心理操纵。它揭示了一个广泛使用的项目所面临的严重脆弱性：单个维护者被攻陷就可能影响数百万下游用户和应用程序。 安全研究人员已将此攻击归因于 UNC1069，这是一个具有经济动机、疑似与朝鲜有关的威胁行为者。攻击者精心克隆了一家真实的公司及其创始人的网络形象，创建了一个人员齐备、看起来活跃的 Slack 工作区，其中甚至包含其他开源维护者的虚假资料以增强可信度，并利用加入预定会议的时间压力来绕过受害者的警惕。

rss · Simon Willison · Apr 3, 13:54

**背景**: 软件供应链攻击针对用于开发和分发软件的流程和工具，旨在破坏源代码、构建过程或更新机制，从而感染下游用户。社交工程通过欺骗等手段操纵人们泄露机密信息或执行危害安全的操作。Axios 是一个基于 Promise、非常流行的 JavaScript HTTP 客户端，下载量达数十亿次，因其庞大的用户基础而成为此类攻击的主要目标。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://cloud.google.com/blog/topics/threat-intelligence/unc1069-targets-cryptocurrency-ai-social-engineering">UNC 1069 Targets Cryptocurrency Sector with... | Google Cloud Blog</a></li>
<li><a href="https://www.securityweek.com/axios-npm-package-breached-in-north-korean-supply-chain-attack/">Axios NPM Package Breached in North Korean Supply... - SecurityWeek</a></li>
<li><a href="https://blog.dreamfactory.com/five-supply-chain-attacks-in-twelve-days-how-march-2026-broke-open-source-trust-and-what-comes-next">Five Supply Chain Attacks in Twelve Days: How March 2026 ...</a></li>

</ul>
</details>

**标签**: `#security`, `#supply-chain-attack`, `#social-engineering`, `#axios`, `#open-source`

---

<a id="item-6"></a>
## [Simon Willison 在 Lenny 播客中探讨 AI 拐点与智能体工程](https://simonwillison.net/2026/Apr/2/lennys-podcast/#atom-everything) ⭐️ 8.0/10

Simon Willison 分享了他做客 Lenny Rachitsky 播客的要点，他们讨论了以 GPT-5.1 和 Claude Opus 4.5 为标志的 2025 年 11 月 AI 拐点、智能体工程的兴起，以及用于自动化软件生产的“暗工厂”概念。 这次对话很重要，因为它捕捉到了一个关键转折点：AI 编码智能体已经跨越了可靠性门槛，从根本上改变了软件开发工作流程，并预示着将影响工程师以外更广泛信息工作者的自动化趋势。 Willison 指出，2025 年 11 月的拐点将 AI 生成的代码从“大部分能用但需要密切关注”转变为“几乎总是能完成你的指令”。他还强调，开发中的主要瓶颈现已从编写代码转移到测试代码。

rss · Simon Willison · Apr 2, 20:40

**背景**: 智能体工程指的是借助能够编写和执行代码的自主编码智能体（如 Claude Code 或 OpenAI Codex）来开发软件的实践。在软件语境中，“暗工厂”一词描述了高度自动化、AI 驱动的流水线，它接收软件规格说明并以最少的人力参与产出可运行的代码。“拐点”则标志着技术能力或采用率发生剧变的时刻。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://simonwillison.net/guides/agentic-engineering-patterns/what-is-agentic-engineering/">What is agentic engineering? - Agentic Engineering Patterns - Simon Willison's Weblog</a></li>
<li><a href="https://www.mindstudio.ai/blog/what-is-a-dark-factory-ai-agent">What Is a Dark Factory AI Agent? How to Build Fully ...</a></li>
<li><a href="https://startup.whatfinger.com/2026/04/02/an-ai-state-of-the-union-weve-passed-the-inflection-point-dark-factories-are-coming/">An AI state of the union: We’ve passed the inflection point & dark factories are coming - Whatfinger Startup And Small Business</a></li>

</ul>
</details>

**标签**: `#AI`, `#Agentic Engineering`, `#Automation`, `#Software Engineering`, `#Podcast`

---

<a id="item-7"></a>
## [工信部通报苹果设备高危漏洞风险：涉及 iOS 17.2.1 及以下版本](https://www.nvdb.org.cn/publicAnnouncement/2040008892420247553) ⭐️ 8.0/10

工业和信息化部网络安全威胁和漏洞信息共享平台（NVDB）近日发布通报，警告苹果 iOS 和 iPadOS 系统存在一个高危漏洞。该漏洞影响 iOS 13.0 至 17.2.1 版本，攻击者可通过短信、邮件或网页投毒诱导用户访问恶意网页，从而植入远程控制木马并获取最高系统权限。 来自国家网络安全主管部门的官方警告，表明一个已被利用的关键漏洞对数百万 iPhone 和 iPad 用户构成了直接的数据窃取和完全设备控制风险。该通报凸显了针对广泛使用的消费级设备的复杂网络钓鱼攻击的持续威胁，以及及时进行软件更新的重要性。 该漏洞允许远程代码执行，使攻击者能够安装一个授予其最高系统权限的远程控制木马。工信部 NVDB 平台明确建议受影响的用户立即将系统升级到最新的已修复版本，并对点击来源不明的链接保持警惕。

telegram · zaihuapd · Apr 3, 11:23

**背景**: 工业和信息化部网络安全威胁和漏洞信息共享平台（NVDB）是于 2021 年 9 月上线的官方平台，负责收集、验证和共享网络安全漏洞信息。远程控制木马（RAT）是一种恶意软件，能让攻击者获得对受感染设备的完全控制权，常用于监视和数据窃取。攻击向量是指攻击者利用系统漏洞入侵的具体路径或方法，例如本次事件中通过恶意链接进行攻击。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://baike.baidu.com/item/工信部网络安全威胁和漏洞信息共享平台/58438279">工信部网络安全威胁和漏洞信息共享平台_百度百科</a></li>
<li><a href="https://zh.wikipedia.org/zh-hans/攻擊媒介">攻击媒介 - 维基百科，自由的百科全书</a></li>

</ul>
</details>

**标签**: `#cybersecurity`, `#vulnerability`, `#apple`, `#ios`, `#government-alert`

---

<a id="item-8"></a>
## [Blogosphere：一个社区策展的个人博客首页聚合器发布，提供极简版和标准版。](https://text.blogosphere.app/) ⭐️ 7.0/10

一位开发者推出了名为“Blogosphere”的社区策展聚合器，它从各个类别的个人博客中抓取并展示最新文章。该项目提供两个不同的界面：一个快速、静态、受 Hacker News 启发的极简版本，以及一个功能更丰富的标准版本。 该工具解决了在 AI 生成内容和企业媒体饱和的背景下，发现优质独立内容日益增长的挑战。它为独立网络提供了一个实用的、人工策展的发现层，帮助作者获得可见性，并让读者在算法平台之外找到真实的声音。 该平台依赖社区提交来发现博客，用户可以添加博客供创建者审核和批准。“极简”版本被明确设计为快速和静态的，优先考虑速度和以文本为中心的体验，让人联想到早期的网络聚合器。

hackernews · ramkarthikk · Apr 3, 12:33

**背景**: “独立网络”是一场倡导将个人、自托管的网站作为主要在线身份的运动，旨在对抗企业社交媒体平台的主导地位。博客聚合器和“网络环”等工具历来被用于连接和推广独立内容。“受 HN 启发”指的是由新闻聚合和讨论网站 Hacker News 推广的极简、重文本的设计美学。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/IndieWeb">IndieWeb - Wikipedia</a></li>
<li><a href="https://indieweb.org/">IndieWeb</a></li>

</ul>
</details>

**社区讨论**: 社区反响非常积极，用户赞扬了其轻量级的设计以及项目与独立网络价值观的一致性。评论将其与“网络环”和“星球”等历史概念进行比较，认为该项目是在搜索质量下降和 AI 内容饱和的背景下，向人工策展的必要回归。一些用户表达了希望有更多特定主题聚合器的愿望，并讨论了算法推荐与策展发现各自的优点。

**标签**: `#indie-web`, `#content-discovery`, `#blog-aggregator`, `#community-curation`, `#web-preservation`

---

<a id="item-9"></a>
## [Cursor 发布 Cursor 3，主打面向 AI 代理的软件开发统一工作区。](https://cursor.com/blog/cursor-3) ⭐️ 7.0/10

Cursor 发布了 Cursor 3，这是一个重大更新，将该工具重新定位为面向 AI 代理的软件开发统一工作区。新版本采用围绕代理重构的全新界面，支持多仓库工作区，并允许用户从移动端、网页、桌面端以及 Slack、GitHub、Linear 等平台发起会话。 此次发布标志着 Cursor 将 AI 辅助编码的碎片化工作流程整合到一个以代理为中心的单一环境中的战略举措。这很重要，因为它旨在通过允许 AI 代理在多个仓库和上下文中工作来简化开发流程，从而可能提高开发者的生产力，并支持更复杂、更自主的编码任务。 一个关键特性是能够在云端和本地环境之间快速切换代理会话，允许在本地进行修改和测试，而云端会话可以在离线或切换任务时继续运行。该更新还引入了用于更快编辑和审查变更的 diff 视图，并集成了对暂存、提交和管理 Pull Request 的支持。

telegram · zaihuapd · Apr 3, 02:00

**背景**: Cursor 是一款 AI 驱动的代码编辑器，集成了大型语言模型（LLM）来协助完成编码任务，范围从自动补全到自主代理功能。在此语境下，“AI 代理”指的是能够根据高级指令自主规划和执行一系列编码任务的 AI。多仓库支持对于处理由多个相互关联的代码库组成的复杂项目的开发者来说是一个重要特性。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://cursor.com/">Cursor: The best way to code with AI</a></li>
<li><a href="https://dev.to/katya_pavlopoulos/how-i-built-an-app-with-cursor-ai-agent-for-the-first-time-the-good-the-bad-and-the-drama-168o">How I Built an App with Cursor AI Agent for the First Time (the Good, the Bad, and the Drama) - DEV Community</a></li>
<li><a href="https://www.wired.com/story/cusor-launches-coding-agent-openai-anthropic/">Cursor Launches a New AI Agent Experience to Take On Claude Code and Codex | WIRED</a></li>

</ul>
</details>

**标签**: `#AI-assisted development`, `#developer-tools`, `#software-engineering`, `#product-announcement`, `#AI-agents`

---

<a id="item-10"></a>
## [Google Vids 接入 Veo 3.1，普通用户可免费生成 AI 视频](https://www.techradar.com/ai-platforms-assistants/google-is-pushing-ai-video-into-ordinary-life-just-as-openai-pulls-sora-back) ⭐️ 7.0/10

Google 更新了其浏览器端 AI 视频制作工具 Google Vids，新增了 Veo 3.1 视频生成模型，并向所有 Google 账号持有者开放免费月度生成额度。此次更新还引入了可自定义外观、语音和道具的数字化身功能，并集成了 Lyria 3 音乐模型用于生成配乐。 此举通过提供基础免费额度，极大地普及了高质量 AI 视频生成技术的使用，直接与 OpenAI 限制更多的 Sora 模型展开竞争。这代表了 Google 将先进 AI 视频能力嵌入主流创意工作流和日常平台的战略推进，可能会加速 AI 辅助内容创作的普及。 个人用户每月可获得 10 次免费视频生成额度，而 Google AI Ultra 和 Workspace AI Ultra 订阅用户的额度则提升至每月最多 1,000 条。用于生成 30 秒到 3 分钟配乐的 Lyria 3 和 Lyria 3 Pro 音乐生成功能，仅向 Google AI Pro 和 Ultra 订阅用户开放。

telegram · zaihuapd · Apr 3, 05:23

**背景**: Google Vids 是 Google Workspace 内一款基于浏览器的、由 AI 驱动的视频创作和编辑工具，旨在简化视频制作流程。Veo 是 Google 先进的生成式 AI 模型，用于根据文本提示创建高质量、逼真的视频，Veo 3.1 是其最新版本。Lyria 是 Google 专注于生成高质量音乐和音频的 AI 模型。AI 视频生成领域竞争激烈，OpenAI 的 Sora 等模型也在争夺主导地位。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://workspace.google.com/products/vids/">Google Vids: AI-Powered Video Creator and Editor | Google ...</a></li>
<li><a href="https://blog.google/products-and-platforms/products/workspace/google-vids-updates-lyria-veo/">Google Vids updates include high-quality video generation at ...</a></li>

</ul>
</details>

**标签**: `#AI Video Generation`, `#Google AI`, `#Creative Tools`, `#Generative AI`, `#Product Announcement`

---

<a id="item-11"></a>
## [美国人形机器人依赖中国技术提供关键内部组件](https://www.wsj.com/tech/under-the-skin-of-americas-humanoid-robots-chinese-technology-27dd4fdf) ⭐️ 7.0/10

《华尔街日报》报道披露，包括迪士尼和特斯拉在内的美国人形机器人，在电机、关节、磁体和传感器等关键部件上越来越依赖中国供应链。报道指出，中国计划在 2025 年推出 28 款人形机器人，数量接近美国企业的 3 倍，且中国供应链最多可将相关制造成本压低三分之二。 这种依赖性在尖端领域为美国的技术竞争力和国家安全创造了战略脆弱性，可能使中国在未来先进机器人技术的发展和制造上获得显著优势。这也突显了一个更广泛的趋势：美国在 AI 和软件方面的创新，正依赖于外国（尤其是中国）在关键硬件组件制造方面的实力。 具体案例包括迪士尼的“奥拉夫”机器人使用了中国宇树科技（Unitree Robotics）的部件，以及特斯拉正与中国供应商合作推进其 Optimus 机器人的量产准备。针对这些担忧，美国国会两党议员已于今年 2 月提出一项法案，旨在评估美国机器人产业的竞争力及供应链风险。

telegram · zaihuapd · Apr 3, 08:55

**背景**: 人形机器人是模仿人类形态和运动的复杂机器，需要精密的执行器（控制运动的电机）和传感器。其中，实现肢体运动的关节执行器尤为关键，可占机器人总物料成本（BOM）的 30-50%，直接影响其性能、精度和成本。全球人形机器人的竞争不仅涉及软件和 AI，还包括对这些高性能、高可靠性硬件组件生产能力的掌控。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://interactanalysis.com/insight/joint-actuators-the-fundamental-component-for-humanoid-robots-power-and-dexterity/">Joint Actuators: Powering the Future of Humanoid Robotics</a></li>

</ul>
</details>

**标签**: `#robotics`, `#supply-chain`, `#geopolitics`, `#manufacturing`, `#ai-hardware`

---

<a id="item-12"></a>
## [调查指 LinkedIn 扫描用户浏览器扩展并向第三方共享数据](https://cybernews.com/privacy/linkedin-surveillance-browsergate/?utm_source=flipboard&amp;utm_content=CyberNews_com%2Fmagazine%2FLatest+cybersecurity+news) ⭐️ 7.0/10

由 Fairlinked 组织发起的 'BrowserGate' 调查指控 LinkedIn 在网站中部署代码，扫描用户浏览器已安装的扩展程序和软件，并将加密后的数据发回其服务器。调查还声称，这些数据在未获得用户明确同意或进行披露的情况下，被共享给包括 HUMAN Security 在内的第三方公司。 这一做法可能影响约 4.05 亿用户，涉及扫描超过 6000 个扩展程序，包括竞品工具和可能揭示宗教信仰、政治倾向、健康状况及求职状态等敏感信息的应用。这引发了重大的隐私担忧，并可能违反欧盟《通用数据保护条例》(GDPR)，因为该条例通常要求此类数据处理必须获得用户的明确同意。 被扫描的数据可能用于推断用户的敏感属性，并覆盖了超过 200 款竞品工具。调查仍在进行中，监管机构的回应以及 LinkedIn 的官方立场正受到密切关注。

telegram · zaihuapd · Apr 3, 12:09

**背景**: 浏览器扩展是用于定制和增强浏览体验的小型软件程序。'BrowserGate' 调查是由 Fairlinked（数字公平联盟，代表商业版 LinkedIn 用户的组织）进行的一个研究项目和宣传活动。GDPR 是欧盟一项全面的数据保护法规，为公司如何处理欧盟境内个人的个人数据制定了严格规则。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://piunikaweb.com/2026/04/03/linkedin-chrome-extension-scan-investigation/">Investigation says LinkedIn scans extensions that reveal ...</a></li>
<li><a href="https://gigazine.net/gsc_news/en/20260403-linkedin-browsergate/">BrowserGate is a research project that claims that every time ...</a></li>
<li><a href="https://browsergate.eu/credits/">Credits | BrowserGate</a></li>

</ul>
</details>

**标签**: `#privacy`, `#data-protection`, `#gdpr`, `#surveillance`, `#browser-security`

---

<a id="item-13"></a>
## [逆向工程揭示如何绕过 Claude Code 基于 Bun 的 API 签名，从而开启快速模式](https://a10k.co/b/reverse-engineering-claude-code-cch.html) ⭐️ 7.0/10

一项技术分析逆向工程揭示了 Anthropic 的编码助手 Claude Code 如何使用其私有的 Bun 运行时，通过 xxHash64 和 SHA-256 算法对 API 请求进行签名。这一发现使得创建一个无需 Bun 二进制文件的 Python 概念验证成为可能，该验证可以伪造有效的请求签名，从而可能解锁诸如“快速模式”等受控功能。 这很重要，因为它揭示了 Anthropic 在 Claude Code 内部用于功能门控和计费归因的机制，表明其更像是一种弱控制，而非严格的安全屏障。它为开发者和研究人员提供了关于商业 AI 工具如何实现基于运行时的功能控制的见解，并可能导致访问高级功能的非官方方法出现。 签名涉及两部分：`cch` 头部值由 Bun 运行时使用 xxHash64 算法对包含占位符的请求体进行计算得出；而 `cc_version` 末尾的 3 位后缀，则是通过 SHA-256 算法，根据用户第一条消息中的指定字符、内置盐值和版本号计算得出。分析指出，该机制主要用于功能门控和归因，而非强访问控制。

telegram · zaihuapd · Apr 3, 15:00

**背景**: Claude Code 是 Anthropic 推出的编码助手，需与其 API 通信。Bun 是一个现代的一体化 JavaScript 运行时（类似于 Node.js），包含打包、转译和哈希等工具。xxHash64 是一种速度极快的非加密哈希算法，设计初衷是追求速度而非安全性；而 SHA-256 是一种标准的加密哈希函数。API 请求签名是验证请求完整性和来源的常用方法。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Bun_(software)">Bun (software) - Wikipedia</a></li>
<li><a href="https://github.com/Cyan4973/xxHash">xxHash - Extremely fast hash algorithm - GitHub</a></li>
<li><a href="https://code.claude.com/docs/en/authentication">Authentication - Claude Code Docs</a></li>

</ul>
</details>

**标签**: `#reverse-engineering`, `#api-security`, `#anthropic-claude`, `#authentication-bypass`, `#runtime-analysis`

---