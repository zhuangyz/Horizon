---
layout: default
title: "Horizon Summary: 2026-04-04 (ZH)"
date: 2026-04-04
lang: zh
---

> From 29 items, 13 important content pieces were selected

---

1. [AI 智能体将很快自动化大部分漏洞研究](#item-1) ⭐️ 9.0/10
2. [vLLM v0.19.0 发布，支持 Gemma 4、零气泡异步调度及多项性能优化。](#item-2) ⭐️ 8.0/10
3. [AI 生成的安全漏洞报告涌入 Linux 内核安全列表，维护者不堪重负](#item-3) ⭐️ 8.0/10
4. [Linux 内核维护者称 AI 生成的安全报告已变得有用](#item-4) ⭐️ 8.0/10
5. [Axios 供应链攻击采用针对维护者的定向社交工程手段](#item-5) ⭐️ 8.0/10
6. [工信部通报苹果设备高危漏洞风险，建议用户尽快升级](#item-6) ⭐️ 8.0/10
7. [马斯克据称要求参与 SpaceX IPO 的银行购买 Grok 订阅](#item-7) ⭐️ 8.0/10
8. [病毒式传播片段引发对 AI 编程助手认知成本的讨论](#item-8) ⭐️ 7.0/10
9. [Cursor 发布 3.0 版本，定位为面向 AI 代理的软件开发统一工作区](#item-9) ⭐️ 7.0/10
10. [Google Vids 接入 Veo 3.1，向所有用户提供免费 AI 视频生成](#item-10) ⭐️ 7.0/10
11. [美国人形机器人“机体内部”依赖中国技术](#item-11) ⭐️ 7.0/10
12. [调查指 LinkedIn 扫描用户浏览器扩展并向第三方共享数据](#item-12) ⭐️ 7.0/10
13. [研究成功逆向 Claude Code 请求签名机制，脱离 Bun 运行时伪造认证头部](#item-13) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [AI 智能体将很快自动化大部分漏洞研究](https://simonwillison.net/2026/Apr/3/vulnerability-research-is-cooked/#atom-everything) ⭐️ 9.0/10

安全专家 Thomas Ptacek 认为，前沿 AI 模型将很快导致漏洞研究发生阶跃式变化，使 AI 智能体能够通过暴力分析源代码来自动化发现零日漏洞。这一转变预计将在几个月内发生，从根本上改变漏洞利用开发的实践和经济模式。 这很重要，因为它代表了网络安全领域的范式转变，AI 自动化可能大幅降低发现关键漏洞的门槛，可能导致零日漏洞充斥市场，并迫使人们彻底重新思考软件安全实践。无论是攻击性安全研究还是防御性补丁开发的经济模式都将被根本性颠覆。 分析强调，LLM 特别适合漏洞研究，因为它们编码了大量关于代码关联性和已记录漏洞类别的知识，例如悬垂指针和整数处理错误。这种基于智能体的方法将这种内置知识与暴力模式匹配和约束求解能力相结合，可以无限期运行而不会疲劳。

rss · Simon Willison · Apr 3, 23:59

**背景**: 漏洞研究涉及在攻击者之前发现软件中的安全缺陷，其中零日漏洞尤其有价值，因为供应商尚不知晓它们的存在，也没有补丁。LLM 智能体是能够通过将复杂任务分解为步骤、使用工具和做出决策来自主执行任务的 AI 系统。前沿模型指的是当前最先进的 AI 系统，其能力显著超越前几代。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://sockpuppet.org/blog/2026/03/30/vulnerability-research-is-cooked/">Vulnerability Research Is Cooked — Quarrelsome</a></li>
<li><a href="https://en.wikipedia.org/wiki/Zero-day_vulnerability">Zero-day vulnerability - Wikipedia</a></li>
<li><a href="https://github.com/NVISOsecurity/cyber-security-llm-agents">GitHub - NVISOsecurity/ cyber - security - llm - agents : A collection of...</a></li>

</ul>
</details>

**标签**: `#ai-security`, `#vulnerability-research`, `#llm-agents`, `#exploit-development`, `#cybersecurity`

---

<a id="item-2"></a>
## [vLLM v0.19.0 发布，支持 Gemma 4、零气泡异步调度及多项性能优化。](https://github.com/vllm-project/vllm/releases/tag/v0.19.0) ⭐️ 8.0/10

vLLM v0.19.0 已发布，该版本全面支持 Google 的 Gemma 4 模型架构，并通过零气泡异步调度与推测解码相结合实现了显著的性能提升。此次发布还标志着 Model Runner V2 的成熟，支持用于流水线并行的分段 CUDA 图，并引入了一个通用的 CPU KV 缓存卸载机制。 此次发布意义重大，因为它直接提升了大型语言模型服务的吞吐量和效率，这是生产级 AI 应用的关键因素。零气泡调度与推测解码的结合减少了 GPU 空闲时间，而更广泛的模型支持和架构增强使 vLLM 成为生态系统中更通用、更强大的推理引擎。 零气泡异步调度功能通过允许调度器在 GPU 繁忙时准备下一个批次，专门减少了高吞吐量服务中的“GPU 气泡”。新的 CPU KV 缓存卸载是一个可插拔的机制，它将 KV 缓存从 GPU 内存移动到 CPU 内存，从而可能实现更多的缓存命中，并支持处理更大的模型或上下文。

github · khluu · Apr 3, 02:19

**背景**: vLLM 是一个用于大型语言模型的高吞吐量、内存高效的推理和服务引擎。推测解码是一种技术，由一个更小、更快的“草案”模型提出 token，并由一个更大的“目标”模型进行验证，旨在降低延迟。CUDA 图是 NVIDIA CUDA 中的一种性能优化技术，它将一系列内核启动捕获到一个单一、可重放的单元中，以减少启动开销。流水线并行是一种模型并行技术，它将模型的层拆分到多个 GPU 上。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://docs.vllm.ai/en/latest/features/speculative_decoding/">Speculative Decoding - vLLM</a></li>
<li><a href="https://agentnativedev.medium.com/vllm-v0-14-0-async-scheduling-grpc-and-deployability-b042bbe40312">vLLM v0.14.0: Async Scheduling, gRPC, and Deployability | by Agent Native | Medium</a></li>
<li><a href="https://docs.sglang.io/advanced_features/piecewise_cuda_graph.html">Piecewise CUDA Graph — SGLang</a></li>

</ul>
</details>

**标签**: `#llm-inference`, `#performance-optimization`, `#vllm`, `#model-serving`, `#gpu-acceleration`

---

<a id="item-3"></a>
## [AI 生成的安全漏洞报告涌入 Linux 内核安全列表，维护者不堪重负](https://simonwillison.net/2026/Apr/3/willy-tarreau/#atom-everything) ⭐️ 8.0/10

首席开发人员兼 Linux 内核维护者 Willy Tarreau 报告称，提交给内核安全列表的 AI 生成安全漏洞报告数量已从两年前的每周 2-3 份激增至 2026 年的每天 5-10 份，迫使团队引入更多维护者。现在每天都会出现针对同一漏洞的重复报告，这很可能来自不同的 AI 工具，这是一种新现象。 AI 生成报告的急剧增加代表了漏洞披露领域的重大转变，为关键的开源基础设施创造了新的运营瓶颈。这突显出，虽然 AI 驱动的安全工具能有效发现漏洞，但可能会无意中给支撑软件安全的人工审查流程带来巨大压力。 Tarreau 指出，虽然大多数 AI 生成的报告是正确的，但庞大的数量和新出现的重复发现是主要挑战。报告涌入量如此之大，以至于需要扩大维护者团队规模来处理分类和验证的工作量。

rss · Simon Willison · Apr 3, 21:48

**背景**: Linux 内核安全列表是一个专门用于报告和讨论 Linux 内核安全漏洞的邮件列表。Willy Tarreau 是广泛使用的开源负载均衡器 HAProxy 的首席开发人员，同时也是一位活跃的 Linux 内核维护者。AI 驱动的漏洞扫描工具使用机器学习和大型语言模型来自动分析代码中的潜在安全缺陷，这种做法已变得越来越普遍。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://lwn.net/Articles/566123/">Opening up kernel security bug handling [LWN.net]</a></li>
<li><a href="https://www.haproxy.com/company/careers">Open Positions - HAProxy Technologies Careers</a></li>

</ul>
</details>

**标签**: `#security`, `#linux-kernel`, `#ai`, `#vulnerability-management`, `#maintenance`

---

<a id="item-4"></a>
## [Linux 内核维护者称 AI 生成的安全报告已变得有用](https://simonwillison.net/2026/Apr/3/greg-kroah-hartman/#atom-everything) ⭐️ 8.0/10

Linux 内核的关键维护者 Greg Kroah-Hartman 表示，提交给开源项目的 AI 生成安全报告最近在质量上发生了巨大转变。他指出，虽然这些报告以前是低质量的 'AI slop'，但现在它们在所有开源项目中都变得准确且真正有用。 这一转变很重要，因为它标志着 AI 工具正在从一种噪音来源，成熟为保护关键软件基础设施的合法辅助工具。如果 AI 能够可靠地识别真正的漏洞，它将能显著扩大安全审计的规模，并减轻工作过度的开源维护者的负担。 Kroah-Hartman 指出这一变化发生在他 2026 年 3 月发表言论的大约一个月前。他强调，这种改进并非孤立现象，而是在整个开源生态系统中被一致观察到。

rss · Simon Willison · Apr 3, 21:44

**背景**: Greg Kroah-Hartman 是 Linux 内核的主要维护者之一，负责监督部分代码库、审查补丁并确保稳定性。'AI slop' 是指 AI 大量生成的、通常无意义的低质量内容，随着 AI 代理向项目提交大量错误报告，这已成为软件开发中日益严重的问题。开源项目传统上依赖社区漏洞披露来提高安全性。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://linuxvox.com/blog/linux-kernal-maintainers/">Linux Kernel Maintainers: A Comprehensive Guide - linuxvox.com</a></li>
<li><a href="https://en.wikipedia.org/wiki/AI_slop">AI slop - Wikipedia</a></li>
<li><a href="https://www.axios.com/2026/03/10/ai-agents-spam-the-volunteers-securing-open-source-software">AI agents are flooding open-source maintainers with security reports</a></li>

</ul>
</details>

**标签**: `#ai-security`, `#open-source`, `#linux-kernel`, `#generative-ai`

---

<a id="item-5"></a>
## [Axios 供应链攻击采用针对维护者的定向社交工程手段](https://simonwillison.net/2026/Apr/3/supply-chain-social-engineering/#atom-everything) ⭐️ 8.0/10

Axios 团队发布了一份事件分析报告，揭示最近一次导致发布恶意软件版本的供应链攻击，是通过一次专门针对项目维护者的复杂社交工程活动执行的。攻击者模仿 UNC1069 威胁组织的策略，创建了一个逼真的虚假公司，并利用 Slack 工作区和 Microsoft Teams 会议诱骗维护者安装了远程访问木马。 这一事件凸显了软件供应链攻击的一个关键转变：威胁行为体现在直接针对广泛使用的开源库的人类维护者，而不仅仅是利用技术漏洞。它表明，即使是技术安全性强的项目，也可能通过复杂的社交工程被攻破，从而使数百万下游用户和应用程序面临风险。 这次攻击是高度定制的，涉及一个克隆的公司（带有虚假的创始人资料）、一个逼真的 Slack 工作区（包含频道和虚假的团队成员资料），以及一次协调好的 MS Teams 会议，在会议中远程访问木马被伪装成必需的更新。恶意 npm 包在活跃了大约 3 小时后才被检测并撤下。

rss · Simon Willison · Apr 3, 13:54

**背景**: 软件供应链攻击是指攻击者通过入侵第三方组件（如开源库）来间接攻击其所有用户。威胁行为体组织 UNC1069 疑似与朝鲜有关联，以出于经济动机的攻击而闻名，并且最近已发展为使用 AI 增强的社交工程手段。Axios 是一个流行的 JavaScript HTTP 客户端库，被全球数百万开发者使用。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://thehackernews.com/2026/04/unc1069-social-engineering-of-axios.html">UNC1069 Social Engineering of Axios Maintainer Led to npm ...</a></li>
<li><a href="https://cloud.google.com/blog/topics/threat-intelligence/unc1069-targets-cryptocurrency-ai-social-engineering">UNC 1069 Targets Cryptocurrency Sector with... | Google Cloud Blog</a></li>
<li><a href="https://onymos.com/blog/how-vulnerable-are-you-to-a-supply-chain-attack/">How Vulnerable Are You to a Supply Chain Attack ? - Onymos</a></li>

</ul>
</details>

**标签**: `#security`, `#supply-chain-attack`, `#social-engineering`, `#open-source`, `#axios`

---

<a id="item-6"></a>
## [工信部通报苹果设备高危漏洞风险，建议用户尽快升级](https://www.nvdb.org.cn/publicAnnouncement/2040008892420247553) ⭐️ 8.0/10

工业和信息化部网络安全威胁和漏洞信息共享平台（NVDB）近日通报，有攻击者正在利用苹果公司终端产品中的一个高危漏洞实施网络攻击。该漏洞影响运行 iOS 13.0 至 17.2.1 版本的 iPhone 和 iPad 等产品，可导致攻击者植入远程控制木马并获取系统最高权限。 此次官方通报揭示了一个紧急且影响广泛的重大安全威胁，可能导致数百万用户的数据被窃取和设备被完全控制。国家网络安全权威机构的介入，凸显了该漏洞的严重性和已被实际利用的现实，要求个人用户和企业管理员必须立即采取行动。 攻击者通过短信、邮件或网页投毒等方式诱导用户访问恶意网页，进而利用漏洞静默植入远程控制木马。NVDB 明确建议相关用户立即通过系统升级或安装补丁修复漏洞，并提高安全意识，避免点击来源不明的链接。

telegram · zaihuapd · Apr 3, 11:23

**背景**: 工信部网络安全威胁和漏洞信息共享平台（NVDB）是中国官方发布网络安全威胁和漏洞信息的平台，其职能类似于 CVE 等漏洞数据库。远程控制木马（RAT）是一种恶意软件，能让攻击者获得对受感染设备的完全控制权，从而进行数据窃取、监控等操作。网页投毒是一种攻击技术，攻击者通过篡改合法网站或创建恶意网页来传播恶意代码。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.itiger.com/news/2566671621">防范苹果公司iOS/iPadOS/macOS越界写入高危漏洞 - Tiger Brokers</a></li>
<li><a href="https://zhuanlan.zhihu.com/p/655411571">远控木马详解与防御及APT攻击中的远控 - 知乎 木马程序原理与远程执行技术全解析-CSDN博客 工信部紧急提醒苹果用户_信息化_漏洞_网页 远控木马详解及APT攻击中的远控和防御-百度开发者中心 RAT (Remote Access Trojan ）远程控制木马专题一 | CN-SEC 中文网</a></li>
<li><a href="https://www.163.com/dy/article/KPK1OE650534P59R.html">工信部：有攻击者用短信、邮件或网页投毒等方式，向苹果公司终端产品...</a></li>

</ul>
</details>

**标签**: `#cybersecurity`, `#vulnerability`, `#apple`, `#ios`, `#government-alert`

---

<a id="item-7"></a>
## [马斯克据称要求参与 SpaceX IPO 的银行购买 Grok 订阅](https://arstechnica.com/tech-policy/2026/04/elon-musk-insists-banks-working-on-spacex-ipo-must-buy-grok-subscriptions/) ⭐️ 8.0/10

据熟悉保密谈判的匿名人士透露，埃隆·马斯克要求参与 SpaceX IPO 的银行、律师事务所、审计机构等顾问方购买其人工智能公司 xAI 的聊天机器人 Grok 的订阅服务。据报道，部分银行已同意为此投入数千万美元，并已开始将 Grok 接入其 IT 系统。 此举引发了关于重大金融交易中潜在利益冲突以及捆绑销售无关服务的严重质疑。这可能为科技创始人如何利用高风险的重大企业事件，在其商业帝国内部交叉销售其他产品开创先例，并可能影响市场惯例和监管审查。 据报道，SpaceX 已于本周向美国证券交易委员会提交了 IPO 文件，距离其收购 xAI 仅过去两个月。与马斯克此前提出的要求相关银行在其社交平台 X 上投放广告相比，购买 Grok 订阅的要求似乎被更坚决地执行。

telegram · zaihuapd · Apr 4, 00:07

**背景**: SpaceX 是埃隆·马斯克的航空航天公司，目前已秘密提交了首次公开募股申请，这是私人公司首次向公众发售股票的过程。xAI 是马斯克的人工智能公司，开发了 Grok 聊天机器人；SpaceX 近期通过一项历史性交易收购了 xAI。Grok 是一个先进的人工智能模型，以其实时网络访问和推理能力等特性而闻名。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.investopedia.com/spacex-filed-to-go-public-every-step-between-now-and-when-you-can-buy-shares-11940905">SpaceX Filed to Go Public—Here's Every Step Between Now and When You Can Buy Shares</a></li>
<li><a href="https://markets.financialcontent.com/stocks/article/marketminute-2026-3-30-the-galactic-merger-spacex-consolidates-xai-in-125-trillion-deal">The Galactic Merger: SpaceX Consolidates xAI in $1.25 ...</a></li>
<li><a href="https://guptadeepak.com/research/grok-ai-fundamentals/">Grok AI - Core Concepts, Capabilities, Technical Foundation</a></li>

</ul>
</details>

**标签**: `#business`, `#tech-policy`, `#artificial-intelligence`, `#ipo`, `#elon-musk`

---

<a id="item-8"></a>
## [病毒式传播片段引发对 AI 编程助手认知成本的讨论](https://simonwillison.net/2026/Apr/3/cognitive-cost/#atom-everything) ⭐️ 7.0/10

Simon Willison 在 Lenny Rachitsky 播客节目中一段讨论 AI 编程助手认知成本的 48 秒片段在 Twitter/X 上病毒式传播，获得了超过 110 万次观看。这段片段是从长达 1 小时 40 分钟的完整对话中剪辑出来的。 这一讨论很重要，因为随着 GitHub Copilot、Cursor 和 Claude Code 等 AI 编程助手在软件开发中变得无处不在，理解它们对开发者的认知影响对于长期生产力和技能发展至关重要。病毒式的关注表明开发者普遍担忧这些工具可能如何影响批判性思维和问题解决能力。 这段病毒式传播的片段特别讨论了'认知债务'或'认知成本'的概念——即过度依赖 AI 编程辅助可能导致开发者自身的问题解决和批判性思维能力随时间推移而退化。这一讨论是关于 AI 伦理和软件开发中智能体工程长期影响的更广泛对话的一部分。

rss · Simon Willison · Apr 3, 23:57

**背景**: AI 编程助手是使用大语言模型来生成、补全或调试代码以协助开发者的工具。流行的例子包括 GitHub Copilot、Cursor、Claude Code 和 Devin。这些工具已经彻底改变了开发者的工作流程，但也引发了关于其认知影响的疑问。'认知成本'这一术语指的是过度依赖 AI 辅助可能对人类认知能力产生的负面影响，类似于哈佛大学教授 Avi Loeb 提出的关于 AI 工具导致批判性思维能力退化的担忧。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://artificialanalysis.ai/agents/coding">Coding Agents Comparison: Cursor, Claude Code, GitHub Copilot ...</a></li>
<li><a href="https://futurism.com/artificial-intelligence/harvard-avi-loeb-ai">Harvard Professor Says AI Users Are Losing Cognitive Abilities - Futurism</a></li>
<li><a href="https://www.media.mit.edu/publications/your-brain-on-chatgpt/">Your Brain on ChatGPT: Accumulation of Cognitive Debt when Using an ...</a></li>

</ul>
</details>

**标签**: `#ai-ethics`, `#coding-agents`, `#developer-productivity`, `#ai-tools`, `#software-engineering`

---

<a id="item-9"></a>
## [Cursor 发布 3.0 版本，定位为面向 AI 代理的软件开发统一工作区](https://cursor.com/blog/cursor-3) ⭐️ 7.0/10

Cursor 正式发布了 Cursor 3，这是一个重大版本更新，将该工具重新定位为一个专为 AI 代理设计的统一工作区。新版本采用了完全重新设计的、以代理为中心的界面，引入了多仓库工作区支持，并实现了混合工作流，允许在本地和基于云的代理会话之间无缝切换。 此次发布意义重大，因为它标志着 Cursor 从主要是一个 AI 辅助代码编辑器，转变为一个用于在软件开发中编排 AI 代理的综合性平台。它直接应对了日益增长的需求：需要能够管理复杂的多仓库项目，并支持在不同环境中工作的持久性、长时间运行的 AI 代理，这是 AI 代理开发领域的一个关键趋势。 其混合工作流允许开发者在本地启动代理会话进行编辑和测试，然后将其移至云端，以便在离线或切换任务时继续运行。此次更新还包括一个新的 diff 视图，用于更快地编辑和审查变更，并保留了暂存、提交和管理拉取请求等核心 Git 操作。

telegram · zaihuapd · Apr 3, 02:00

**背景**: Cursor 是一个 AI 驱动的集成开发环境（IDE），旨在通过 AI 代码补全、基于聊天的辅助和自动化编辑等功能来提高开发者的生产力。它常被与集成了 GitHub Copilot 的 VS Code 进行比较。此处的 AI 代理指的是更具自主性的 AI 助手，能够执行复杂的、多步骤的开发任务，例如在整个代码库中实现功能或修复错误。模型上下文协议（MCP）是一个开放标准，使这些 AI 代理能够安全地连接和使用外部工具及数据源，Cursor 将其视为一项核心能力。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://cursor.com/">Cursor : The best way to code with AI</a></li>
<li><a href="https://www.devtoolsacademy.com/blog/cursor-vs-claudecode/">Cursor vs Claude Code: A Comprehensive Comparison</a></li>
<li><a href="https://howaiworks.ai/blog/cursor-3-unified-workspace-agents">Introducing Cursor 3: A Unified Agentic Workspace - howaiworks.ai</a></li>

</ul>
</details>

**标签**: `#AI-assisted-development`, `#developer-tools`, `#software-engineering`, `#cursor`, `#AI-agents`

---

<a id="item-10"></a>
## [Google Vids 接入 Veo 3.1，向所有用户提供免费 AI 视频生成](https://www.techradar.com/ai-platforms-assistants/google-is-pushing-ai-video-into-ordinary-life-just-as-openai-pulls-sora-back) ⭐️ 7.0/10

谷歌已将其先进的 Veo 3.1 AI 视频生成模型集成到其基于浏览器的视频创作工具 Google Vids 中，并向所有谷歌账户持有者提供每月 10 次视频生成的免费额度。此次更新还增加了用于创建 30 秒至 3 分钟配乐的 Lyria 3 音乐生成模型，并引入了可定制的数字化身功能，但音乐功能仅限于付费的 AI Pro 和 Ultra 订阅用户。 此举极大地普及了高质量 AI 视频生成的获取途径，将强大的创意工具免费提供给普通公众，这与 OpenAI 对其 Sora 模型采取的更严格限制方法形成对比。通过将这些功能嵌入到 Google Vids 这样广泛可访问的平台中，谷歌正在将 AI 视频从专业工具推向日常创意工作流，用于演示文稿、社交媒体和个人项目。 个人用户的免费层级每月上限为 10 次生成，而付费的 Google AI Ultra 和 Workspace AI Ultra 订阅者每月可获得高达 1000 次 Veo 生成的显著更高额度。集成的 Lyria 3 和 Lyria 3 Pro 模型可以生成带人声和歌词的音乐，但这一高级功能仍然是付费客户的专属权益。

telegram · zaihuapd · Apr 3, 05:23

**背景**: Google Veo 3.1 是谷歌最新、最先进的 AI 视频生成模型，能够根据文本或图像生成带声音的高质量 8 秒视频，并支持高达 4K 分辨率及多种宽高比的输出。Lyria 3 是 Google DeepMind 的旗舰 AI 音乐生成模型系列，能够根据文本、图像或视频提示创建专业级音频片段，包括具有逼真人声和自动生成歌词的曲目。Google Vids 是 Google Workspace 内一个基于网络的 AI 辅助视频创作工具，旨在帮助用户快速制作用于演示文稿和其他内容的视频。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://aistudio.google.com/models/veo-3">Veo 3 | Google AI Studio</a></li>
<li><a href="https://deepmind.google/models/lyria/">Lyria 3 — Google DeepMind</a></li>

</ul>
</details>

**标签**: `#AI Video Generation`, `#Google AI`, `#Veo 3.1`, `#Creative Tools`, `#AI Democratization`

---

<a id="item-11"></a>
## [美国人形机器人“机体内部”依赖中国技术](https://www.wsj.com/tech/under-the-skin-of-americas-humanoid-robots-chinese-technology-27dd4fdf) ⭐️ 7.0/10

《华尔街日报》报道指出，美国人形机器人，包括迪士尼的“奥拉夫”机器人和特斯拉的 Optimus，在电机、关节、磁体和传感器等关键部件上越来越依赖中国供应商。报道还提到，中国计划在 2025 年推出 28 款人形机器人，数量接近美国企业的 3 倍，且中国供应链最多可将相关制造成本压低三分之二。 这种依赖性在代表未来自动化和 AI 战略前沿的关键技术领域，造成了重大的供应链脆弱性。它凸显了美国技术发展的一个战略弱点，并已促使美国国会两党议员提出法案，旨在评估美国机器人竞争力及供应链风险。 具体案例包括迪士尼的“奥拉夫”机器人使用了中国宇树科技(Unitree Robotics)的部件，以及特斯拉正与中国供应商合作推进 Optimus 的量产准备。关节执行器这类关键部件可占人形机器人物料成本(BOM)的 30-50%，这使得其成本和供应至关重要。

telegram · zaihuapd · Apr 3, 08:55

**背景**: 人形机器人是旨在模仿人类形态和运动的先进机器，其应用范围从制造业到客户服务。其功能的核心在于内部组件，如执行器（为关节提供运动）和传感器（提供感知）。特斯拉（凭借 Optimus）和宇树科技(Unitree Robotics)等公司是开发这类机器人的主要参与者。所需精密组件的供应链是全球性且复杂的。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Unitree_Robotics">Unitree Robotics - Wikipedia</a></li>
<li><a href="https://interactanalysis.com/insight/joint-actuators-the-fundamental-component-for-humanoid-robots-power-and-dexterity/">Joint Actuators: Powering the Future of Humanoid Robotics</a></li>

</ul>
</details>

**标签**: `#robotics`, `#supply-chain`, `#geopolitics`, `#manufacturing`, `#ai-hardware`

---

<a id="item-12"></a>
## [调查指 LinkedIn 扫描用户浏览器扩展并向第三方共享数据](https://cybernews.com/privacy/linkedin-surveillance-browsergate/?utm_source=flipboard&amp;utm_content=CyberNews_com%2Fmagazine%2FLatest+cybersecurity+news) ⭐️ 7.0/10

一份名为“BrowserGate”的新报告指控，微软旗下的 LinkedIn 在其网站上使用隐藏的 JavaScript 脚本，扫描访问者浏览器中安装的超过 6000 个扩展程序并收集设备数据。这些可能揭示宗教信仰或求职状态等敏感信息的数据被加密后发送至 LinkedIn 服务器，可能影响 4.05 亿用户，并在未获得用户适当同意的情况下与 HUMAN Security 等第三方公司共享。 这种做法构成了严重的隐私侵犯，因为扫描到的数据可用于在未经明确许可的情况下，构建推断敏感个人属性的详细用户画像。这引发了关于企业监控以及可能违反 GDPR 等数据保护法规的严重担忧，因为此类处理通常需要用户的明确同意。 扫描目标涵盖超过 6000 个浏览器扩展和 200 多款竞品工具，收集的数据可能指向用户的宗教信仰、政治倾向、健康状况或求职活动。LinkedIn 未向用户披露此做法，也未获得欧盟《通用数据保护条例》(GDPR) 要求的、与第三方共享此类数据所需的明确同意。

telegram · zaihuapd · Apr 3, 12:09

**背景**: 浏览器扩展是用于为网页浏览器添加功能或修改其功能的小型软件程序。虽然有用，但它们可能带来安全和隐私风险，因为用户安装的扩展可以揭示个人兴趣、习惯甚至敏感属性。GDPR 是一项全面的欧盟法规，管辖数据保护和隐私，要求组织在处理个人数据（尤其是用于用户画像分析或与第三方共享等目的）之前，必须获得个人明确且肯定的同意。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.bleepingcomputer.com/news/security/linkedin-secretely-scans-for-6-000-plus-chrome-extensions-collects-data/">LinkedIn secretely scans for 6,000+ Chrome extensions ...</a></li>
<li><a href="https://appleinsider.com/articles/26/04/03/microsofts-linkedin-is-scanning-installed-browser-extensions-without-user-permission">Microsoft's LinkedIn is scanning installed browser extensions ...</a></li>

</ul>
</details>

**标签**: `#privacy`, `#data-protection`, `#gdpr`, `#linkedin`, `#browser-security`

---

<a id="item-13"></a>
## [研究成功逆向 Claude Code 请求签名机制，脱离 Bun 运行时伪造认证头部](https://a10k.co/b/reverse-engineering-claude-code-cch.html) ⭐️ 7.0/10

一篇于 2026 年 4 月 2 日发布的技术分析文章详细介绍了研究人员如何逆向工程 Anthropic 旗下 Claude Code 使用的专有请求签名机制。他们发现完整性校验头 `cch` 是由内嵌的 Bun 运行时使用 xxHash64 算法对特定 JSON 结构计算得出的，并成功创建了一个不依赖 Bun 的 Python 概念验证程序来伪造这些签名。 此事意义重大，因为它揭示了一个主流 AI 编程助手中关键的安全与功能门控机制的内部原理。伪造签名的能力可能让开发者绕过既定限制，例如开启'快速模式'或其他受控功能，同时也突显了该机制的设计初衷更多是用于计费归因和功能控制，而非强访问安全。 `cch` 哈希值由 Bun 运行时的原生 fetch 函数对包含 `cch=00000` 占位符的完整 JSON 请求体进行计算得出。`cc_version` 的后缀则通过对首条用户消息中的指定字符、内置盐值和版本号进行 SHA-256 哈希运算得到。分析指出，该方案并非强健的访问控制，而更像是一种用于追踪使用情况和控制高级功能的机制。

telegram · zaihuapd · Apr 3, 15:00

**背景**: Claude Code 是由 Anthropic 开发的 AI 编程助手。它通过专有的头部与 Anthropic 的后端 API 进行通信，用于认证和请求完整性校验。Bun 是一个用 Zig 语言编写的高性能 JavaScript 运行时。`cch` 头部是一个请求完整性校验值，错误的校验值会导致 API 请求被拒绝。xxHash64 是一种速度极快的非加密哈希算法，常用于校验和计算。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://rexai.top/en/ai/claude-code/2026-04-02-reverse-engineering-claude-code-cch/">Reverse Engineering Claude Code's API Request Signing</a></li>
<li><a href="https://bun.com/docs/runtime">Bun Runtime - Bun</a></li>
<li><a href="https://github.com/Cyan4973/xxHash">xxHash - Extremely fast hash algorithm - GitHub What's cch? Reverse Engineering Claude Code's Request Signing XXHash Algorithm Implementation | ceph/xxHash | DeepWiki pyspark.sql.functions.xxhash64 — PySpark 4.1.1 documentation XxHash64 Class (System.IO.Hashing) | Microsoft Learn XXHash Algorithm Implementation | ceph/xxHash | DeepWiki xxHash : XXH64 family XXHash Algorithm Implementation | ceph/xxHash | DeepWiki XXH64 family - xxHash</a></li>

</ul>
</details>

**标签**: `#reverse-engineering`, `#api-security`, `#anthropic`, `#claude-code`, `#authentication`

---