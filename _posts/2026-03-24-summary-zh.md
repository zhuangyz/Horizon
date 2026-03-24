---
layout: default
title: "Horizon Summary: 2026-03-24 (ZH)"
date: 2026-03-24
lang: zh
---

> From 27 items, 11 important content pieces were selected

---

1. [LiteLLM Python 软件包因 CI/CD 工具被入侵而遭受供应链攻击](#item-1) ⭐️ 9.0/10
2. [LiteLLM v1.82.8 PyPI 软件包被植入自动执行的凭据窃取程序](#item-2) ⭐️ 9.0/10
3. [Ripgrep 在 2016 年基准测试中性能超越 Grep 及其他搜索工具](#item-3) ⭐️ 8.0/10
4. [从 SSD 流式加载专家权重，实现消费级硬件运行万亿参数模型](#item-4) ⭐️ 8.0/10
5. [美国联邦通信委员会以安全风险为由全面禁止新型外国造消费级路由器](#item-5) ⭐️ 8.0/10
6. [英伟达利用 AI 热潮现金投资初创公司，将客户锁定在其生态系统中](#item-6) ⭐️ 8.0/10
7. [阿里达摩院发布玄铁 C950 RISC-V CPU，宣称刷新全球性能纪录](#item-7) ⭐️ 8.0/10
8. [我国日均词元调用量两年增超千倍，今年 3 月突破 140 万亿](#item-8) ⭐️ 8.0/10
9. [DarkSword iOS 漏洞利用链被披露，利用 6 个漏洞通过 Safari 感染用户](#item-9) ⭐️ 8.0/10
10. [Google 推出基于 Gemini 的暗网情报与安全运营 AI 代理，已开放公开预览。](#item-10) ⭐️ 8.0/10
11. [批评微软对 Windows 11 的修复仅为表面改进](#item-11) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [LiteLLM Python 软件包因 CI/CD 工具被入侵而遭受供应链攻击](https://github.com/BerriAI/litellm/issues/24512) ⭐️ 9.0/10

LiteLLM Python 软件包遭受了一次供应链攻击，其源头是用于 CI/CD 流水线中的 Trivy 安全扫描工具的一个被入侵版本。该软件包现已在 PyPI 上被隔离，所有下载均被阻止，相关调查正在进行中。 这一事件凸显了开源供应链的严重脆弱性，开发流水线中一个受信任的安全工具（Trivy）竟能成为攻击媒介，进而危及像 LiteLLM 这样作为访问多种 AI 模型网关的广泛使用的软件包。这迫使整个软件行业重新评估对依赖项和 CI/CD 安全实践的信任。 此次攻击与近期的 'TeamPCP' 恶意活动有关，维护者确认使用固定版本的代理 Docker 镜像的用户未受影响。PyPI 上的隔离是一项保护性措施，旨在解决问题期间阻止受损软件包的进一步分发。

hackernews · theanonymousone · Mar 24, 12:36

**背景**: LiteLLM 是一个流行的 Python SDK 和代理服务器，充当应用程序与来自 OpenAI、Anthropic 等提供商的各种大语言模型（LLM）交互的统一网关。Trivy 是一个广泛使用的开源漏洞扫描器，通常集成到 CI/CD 流水线中，用于对代码和容器进行安全检查。PyPI（Python Package Index）是 Python 软件的官方仓库，'隔离'是一种阻止软件包下载的状态，通常用于控制安全事件。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/BerriAI/litellm">GitHub - BerriAI/ litellm : Python SDK, Proxy Server (AI Gateway) to...</a></li>
<li><a href="https://0x1.gitlab.io/security/Trivy/">Trivy</a></li>
<li><a href="https://pypi.org/project/remove-quarantine/">remove- quarantine · PyPI</a></li>

</ul>
</details>

**社区讨论**: 讨论揭示了对依赖项信任和 CI/CD 安全的深切担忧。LiteLLM 维护者提供了时间线并确认了 Trivy 这一攻击媒介。社区成员呼吁在开发环境中采用更强的隔离措施（如沙箱和出口过滤器），并建议进行架构更改，例如将软件包发布与公共代码仓库解耦以减少攻击面。

**标签**: `#security`, `#supply-chain-attack`, `#python`, `#ci-cd`, `#open-source`

---

<a id="item-2"></a>
## [LiteLLM v1.82.8 PyPI 软件包被植入自动执行的凭据窃取程序](https://simonwillison.net/2026/Mar/24/malicious-litellm/#atom-everything) ⭐️ 9.0/10

发布到 Python 包索引 (PyPI) 的 LiteLLM v1.82.8 软件包被植入一个隐藏在 `litellm_init.pth` 文件中的凭据窃取程序，该程序在安装软件包时自动执行，无需任何导入语句。PyPI 随后隔离了该软件包，将暴露窗口限制在数小时内。 此次事件是针对一个广泛使用的 AI/ML 库的复杂供应链攻击，展示了恶意行为者如何利用受信任的分发渠道自动入侵开发者系统。它凸显了开源生态系统中的关键漏洞，即单个被入侵的软件包可能导致云服务、版本控制和加密货币钱包的大规模凭据失窃。 恶意负载在 `.pth` 文件中进行了双重 base64 编码，难以通过简单的源代码检查发现。该窃取程序针对广泛的敏感文件和目录，包括 SSH 密钥、Git 凭据、云服务配置（AWS、Azure、Docker、Kubernetes）、数据库凭据、Shell 历史记录和加密货币钱包数据。

rss · Simon Willison · Mar 24, 15:07

**背景**: LiteLLM 是一个流行的开源库，为调用各种大语言模型 API 提供了统一接口。在 Python 中，放置在 `site-packages` 目录中的 `.pth`（路径）文件是扩展模块搜索路径的合法机制。然而，自 Python 3.5 起，`.pth` 文件中以 'import' 开头的行会在 Python 解释器启动时自动执行，这使其成为恶意代码潜在的隐蔽持久化机制。PyPI 的隔离功能是一项安全措施，在收到可信的恶意软件报告时限制对项目的访问。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://blog.pypi.org/posts/2024-12-30-quarantine/">Project Quarantine - The Python Package Index Blog</a></li>
<li><a href="https://dfir.ch/posts/publish_python_pth_extension/">Analysis of Python 's . pth files as a persistence mechanism | dfir.ch</a></li>
<li><a href="https://github.com/BerriAI/litellm/issues/24512">[Security]: CRITICAL: Malicious litellm_init. pth in litellm...</a></li>

</ul>
</details>

**标签**: `#security`, `#supply-chain-attack`, `#ai-ml`, `#python`, `#pypi`

---

<a id="item-3"></a>
## [Ripgrep 在 2016 年基准测试中性能超越 Grep 及其他搜索工具](https://burntsushi.net/ripgrep/) ⭐️ 8.0/10

2016 年 9 月，Andrew Gallant 发表了一篇详细的技术博客文章，介绍了用 Rust 编写的新命令行搜索工具 ripgrep (rg)。该文章提供了全面的基准测试，证明 ripgrep 的性能超越了多个成熟工具，包括 GNU grep、The Silver Searcher (ag)、git grep、Universal Code Grep (ucg)、The Platinum Searcher (pt) 和 sift。 这一性能突破之所以重要，是因为类 grep 工具是开发者搜索代码库工作流的基础。一个显著更快的工具能直接提升开发者的生产力，尤其是在处理大型现代代码仓库时。这篇文章还促进了社区协作，最终推动了 `.ignore` 文件支持在不同工具间的标准化。 Ripgrep 的关键性能优化包括并行、多线程搜索（与单线程的 GNU grep 不同）、利用 SIMD 指令进行高效模式匹配，以及智能的默认行为，如遵守 `.gitignore` 规则。该工具专为搜索代码而设计，优先考虑软件开发常见场景下的速度。

hackernews · jxmorris12 · Mar 24, 06:31

**背景**: `grep` 是一个经典的 Unix 命令行工具，用于使用正则表达式搜索纯文本数据。随着时间的推移，出现了许多替代工具以解决其在搜索代码方面的局限性：`ack` 和 `The Silver Searcher (ag)` 增加了诸如默认忽略版本控制文件等功能。`git grep` 用于在 Git 仓库内搜索。像 `ucg`、`pt` 和 `sift` 这样的工具是创建更快、功能更丰富的 grep 替代品的其他尝试，通常使用 Go 或 C++ 等现代语言编写。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://burntsushi.net/ripgrep/">ripgrep is faster than {grep, ag, git grep, ucg, pt, sift} - Andrew Gallant's Blog</a></li>
<li><a href="https://github.com/ggreer/the_silver_searcher">GitHub - ggreer/the_silver_searcher: A code-searching tool ...</a></li>
<li><a href="https://www.codeant.ai/blogs/ripgrep-vs-grep-performance">Ripgrep vs Grep Performance: Why rg Is 10x Faster for Modern Codebases</a></li>

</ul>
</details>

**社区讨论**: 社区讨论强调了这篇文章作为性能工程和技术写作典范的持久影响力。评论者指出，它在推动 `.ignore` 文件支持在不同工具间标准化方面的影响，以及它作为优化其他搜索工具的参考价值。具体例子包括开发者借鉴其“搜索最少见字节”的技术，并指出其已被 Claude Code 等 AI 编程助手采用。

**标签**: `#ripgrep`, `#systems-programming`, `#performance`, `#developer-tools`, `#rust`

---

<a id="item-4"></a>
## [从 SSD 流式加载专家权重，实现消费级硬件运行万亿参数模型](https://simonwillison.net/2026/Mar/24/streaming-experts/#atom-everything) ⭐️ 8.0/10

在短短五天内，通过从 SSD 流式加载专家权重以在有限 RAM 的硬件上运行大规模混合专家模型的技术取得了显著进展：从在 48GB RAM 上运行 3970 亿参数模型，发展到在配备 96GB RAM 的 MacBook Pro 上运行具有 320 亿活跃权重的 1 万亿参数模型（Kimi K2.5）。同一款 397B 模型也已在 iPhone 上成功运行，尽管速度较慢，仅为每秒 0.6 个 token。 这一突破极大地降低了运行最先进、大规模 AI 模型的硬件门槛，使得万亿参数模型能够在高端消费级设备上运行，而不再需要庞大的服务器集群。这代表着在普及强大 AI 能力、实现更高效、更具成本效益的本地推理方面迈出了重要一步。 该技术特别利用了 MoE 模型的稀疏激活特性，即每个 token 只需要一部分'专家'，使得系统能够从更大、更慢的 SSD 存储中即时地将所需权重加载到 RAM/VRAM 中。目前在 iPhone 上的实现显示出显著的性能权衡，速度仅为每秒 0.6 个 token，这表明在移动设备上实现实际可用性，速度仍然是一个关键挑战。

rss · Simon Willison · Mar 24, 05:09

**背景**: 混合专家模型是一种机器学习架构，其中一个大型模型由许多称为'专家'的较小子网络组成。对于每个输入（如文本生成中的一个 token），一个路由机制仅选择少数相关的专家进行激活，使得模型在计算上是稀疏的。这使得模型的总参数量（例如 1 万亿）可以远大于每次计算实际使用的参数量（例如 320 亿）。传统上，运行此类模型需要将所有参数加载到快速但昂贵且容量有限的 GPU 显存或系统 RAM 中。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Mixture_of_experts">Mixture of experts - Wikipedia</a></li>
<li><a href="https://www.nvidia.com/en-us/glossary/mixture-of-experts/">What Is Mixture of Experts (MoE) and How It Works? | NVIDIA Glossary</a></li>
<li><a href="https://developer.nvidia.com/blog/applying-mixture-of-experts-in-llm-architectures/">Applying Mixture of Experts in LLM Architectures | NVIDIA Technical Blog</a></li>

</ul>
</details>

**标签**: `#LLM`, `#Mixture-of-Experts`, `#Model-Inference`, `#Hardware`, `#Optimization`

---

<a id="item-5"></a>
## [美国联邦通信委员会以安全风险为由全面禁止新型外国造消费级路由器](https://www.bloomberg.com/news/articles/2026-03-23/fcc-bans-all-foreign-made-routers-citing-security-risks?embedded-checkout=true) ⭐️ 8.0/10

2026 年 3 月 23 日，美国联邦通信委员会（FCC）正式宣布，出于对网络安全和供应链漏洞的担忧，全面禁止所有新型外国制造的消费级路由器进口至美国市场。FCC 将这些路由器列入了其'受管辖实体名单'，这意味着新型号将无法获得在美销售的设备授权，除非获得国防部等机构的豁免批准。 这项政策将显著重塑美国消费级网络硬件市场，在旨在降低外国制造硬件带来的国家安全风险的同时，可能会限制消费者选择并提高成本。它标志着技术供应链安全措施的显著升级，并可能影响网络设备的全球贸易政策和制造策略。 该禁令仅适用于规定发布后寻求授权的新型路由器型号；已获批准销售的现有型号以及消费者当前正在使用的路由器不受影响。制造商若想获得豁免，必须向美国国防部或国土安全部等国家安全机构申请批准。

telegram · zaihuapd · Mar 24, 01:17

**背景**: FCC 的'受管辖实体名单'是根据《安全网络法》制定的，列出了被认为对美国国家安全构成不可接受风险的通信设备和服务清单。消费级路由器是管理互联网流量并连接多台设备的关键家庭网络设备；它们容易受到供应链攻击，即在制造过程中被植入恶意硬件或固件。此前，FCC 在此框架下的关注点更多集中在特定公司的电信运营商设备上。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.fcc.gov/faqs-recent-updates-fcc-covered-list-regarding-routers-produced-foreign-countries">FAQs on Recent Updates to FCC Covered List Regarding Routers ...</a></li>
<li><a href="https://www.pcmag.com/news/fcc-just-banned-the-sale-of-new-wi-router-models-made-outside-us">The FCC Just Banned the Sale of New Wi-Router Models Made ...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Supply_chain_attack">Supply chain attack - Wikipedia</a></li>

</ul>
</details>

**标签**: `#cybersecurity`, `#trade-policy`, `#networking`, `#supply-chain`, `#regulation`

---

<a id="item-6"></a>
## [英伟达利用 AI 热潮现金投资初创公司，将客户锁定在其生态系统中](https://www.wsj.com/tech/nvidia-ai-market-competition-9db60e4c) ⭐️ 8.0/10

英伟达正利用其在 AI 热潮中积累的巨额现金储备，自 2022 年以来向 OpenAI、CoreWeave 及 Reflection AI 等初创公司投资了数十亿美元并提供信贷支持。此外，该公司还通过一项与芯片初创公司 Groq 达成的 200 亿美元授权协议等交易获取核心技术与人才，其交易结构已引发美国参议员的担忧，认为其可能旨在规避反垄断审查。 这一策略通过扮演供应商、投资者和债权人的多重角色，巩固了英伟达在 AI 基础设施市场的统治地位，使得客户难以转向 AMD 等竞争对手。这引发了关于市场竞争、潜在的反垄断违规行为以及 AI 创新生态系统长期健康的重大担忧，因为单一参与者可能通过财务手段巩固其地位。 由于转换计算供应商的成本高昂，这些投资和信贷安排实际上将客户锁定在英伟达的生态系统中。与 Groq 的交易（涉及挖走其核心团队）被引为利用灵活交易结构以规避监管审查的例证。

telegram · zaihuapd · Mar 24, 03:02

**背景**: 英伟达的 GPU 是训练和运行大型 AI 模型的主导硬件，在 AI 热潮中创造了巨大的需求和利润。像 CoreWeave 这样的初创公司专门为 AI 工作负载提供基于 GPU 的云基础设施，而像 Groq 这样的公司则开发专门的 AI 加速芯片（LPU）作为 GPU 的替代品。像 Reflection AI 这样的 AI 实验室获得的巨额融资，突显了尖端 AI 开发的高度资本密集型特性。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/CoreWeave">CoreWeave - Wikipedia</a></li>
<li><a href="https://techcrunch.com/2025/10/09/reflection-raises-2b-to-be-americas-open-frontier-ai-lab-challenging-deepseek/">Reflection AI raises $2B to be America's open frontier AI lab ...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Groq">Groq - Wikipedia</a></li>

</ul>
</details>

**标签**: `#AI Infrastructure`, `#Business Strategy`, `#Antitrust`, `#Nvidia`, `#Market Competition`

---

<a id="item-7"></a>
## [阿里达摩院发布玄铁 C950 RISC-V CPU，宣称刷新全球性能纪录](https://mp.weixin.qq.com/s/TTnqm8qm3Dxshj_0bxwtkw) ⭐️ 8.0/10

2026 年 3 月 24 日，在上海举办的玄铁 RISC-V 生态大会上，阿里巴巴达摩院发布了基于开源 RISC-V 架构的新一代旗舰 CPU 玄铁 C950。官方宣称其在 SPECint2006 单核测试中得分超过 70 分，为目前公开 RISC-V 处理器中的最高水平。 此次发布意义重大，它表明开源指令集架构 RISC-V 如今已能进军传统上由 ARM 和 x86 主导的高性能计算领域。C950 能够原生运行 Qwen3、DeepSeek V3 等千亿参数大模型，使其成为云 AI、边缘计算和机器人等领域的一个可行选择，有望加速 RISC-V 在数据中心和高端 AI 硬件市场的采用。 该芯片集成了达摩院自研的 AI 加速引擎，这是其宣称能够原生运行千亿参数大模型而不依赖软件仿真的关键。该产品明确面向高端算力场景，包括云计算、生成式人工智能、高端机器人和边缘计算。

telegram · zaihuapd · Mar 24, 06:01

**背景**: RISC-V 是一种开放标准的指令集架构，为 ARM 和 x86 等专有架构提供了免费的替代选择。SPECint2006 是标准性能评估公司（SPEC）设计的一套基准测试套件（现已退役但历史上很重要），用于测试 CPU 的整数计算性能。所谓在 CPU 上“原生运行”大模型，是指不重度依赖外部 GPU 或软件仿真，而是在硬件层面针对 AI 工作负载进行了优化，这是一个重大的技术挑战。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.wevolver.com/article/risc-v-vs-arm">RISC-V vs ARM: A Comprehensive Comparison of Processor ... ARM vs. RISC-V: Is one better than the other? - Digital Trends RISC-V, ARM, and x86: The Battle for Dominance in ... - Medium RISC-V vs ARM vs x86: Which Processor Reigns Supreme? - DFRobot Choose Wisely: RISC-V vs. ARM - Architectures of the Future</a></li>
<li><a href="https://en.wikipedia.org/wiki/SPECint">SPECint - Wikipedia</a></li>
<li><a href="https://awesomeagents.ai/news/alibaba-xuantie-c950-risc-v-llm-inference/">Alibaba's C950 - First RISC-V CPU with Native ... | Awesome Agents</a></li>

</ul>
</details>

**标签**: `#RISC-V`, `#Semiconductors`, `#AI Hardware`, `#High-Performance Computing`, `#Alibaba`

---

<a id="item-8"></a>
## [我国日均词元调用量两年增超千倍，今年 3 月突破 140 万亿](http://paper.people.com.cn/rmrb/pc/content/202603/24/content_30147015.html) ⭐️ 8.0/10

国家数据局披露，我国日均词元（Token）调用量已在今年 3 月突破 140 万亿。这一指标从 2024 年初的 1000 亿增长至 2025 年底的 100 万亿，两年内增幅超过一千倍。 这一爆炸性增长标志着中国人工智能产业正在快速规模化与商业化，因为词元是大模型可计量、可定价、可交易的基本操作单位。这表明一个围绕词元调用、分发与结算的新价值体系正在加速形成，并成为人工智能产业商业化的重要路径。 该数据由中国国家数据局官方发布。'词元'已被确立为 AI 语境中'Token'的标准中文译名，这反映了其作为大模型调用量的评估标准和 API 服务计费单位的关键地位。

telegram · zaihuapd · Mar 24, 07:22

**背景**: 在人工智能和大型语言模型（LLM）中，词元（Token）是处理文本的最小单位，例如一个词或词的一部分。它是 GPT 等大模型操作的基本单位，将人类文字转化为模型可计算的数字序列。词元数量是 AI 时代衡量价值的关键度量，因为 API 调用费和模型推理成本通常以词元消耗量来计算。例如，在中文中，通常一个字对应一个词元。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.wangxiansheng.com/what-is-a-token/">词 元 （ Token ）是什么？ 大型语言模型的核心文本处理解析 - 王先生</a></li>
<li><a href="https://cloud.tencent.com/developer/article/2585723">大模型API的token是如何计算的？-腾讯云开发者社区-腾讯云</a></li>
<li><a href="https://m.163.com/dy/article/KOQDOCPN05534KO1.html?spss=news-hotlist-wap-index">Token 中文名定了： 词 元 | token |中文名|全模态|翻译| 词 元 _手机网易网</a></li>

</ul>
</details>

**标签**: `#AI Infrastructure`, `#Token Economics`, `#China Tech`, `#Data Metrics`, `#AI Commercialization`

---

<a id="item-9"></a>
## [DarkSword iOS 漏洞利用链被披露，利用 6 个漏洞通过 Safari 感染用户](https://t.me/zaihuapd/40482) ⭐️ 8.0/10

安全研究人员披露了名为 'DarkSword' 的漏洞利用链，该攻击链自 2025 年 11 月起被用于针对沙特阿拉伯、土耳其、马来西亚和乌克兰用户的攻击。该链利用了 iOS 18.4 至 18.7 版本中的六个漏洞（包括三个零日漏洞），用户只需在 Safari 中访问恶意网页即可被植入 GHOSTBLADE 等恶意软件。 此次披露突显了一种复杂的现实威胁，它能通过一次点击无声地入侵 iPhone，进行有针对性的数据窃取，尤其针对加密货币资产。这凸显了基于浏览器的攻击带来的持续风险，以及多样化的威胁行为者如何快速将多个漏洞武器化，用于攻击高价值目标。 相关漏洞，包括 CVE-2025-43529（WebKit 中的一个释放后重用漏洞），已在 iOS 26.3 及更早的 iOS 18.7.3 等更新中修复。GHOSTBLADE 载荷是一种基于 JavaScript 的恶意软件，专为快速窃取数据而设计，会专门扫描并窃取 Coinbase、Binance 等加密货币交易应用中的信息。

telegram · zaihuapd · Mar 24, 11:45

**背景**: 漏洞利用链是指将多个软件漏洞按顺序组合使用，以达到比单个漏洞更深层次的系统入侵。零日漏洞是软件厂商尚不知晓的漏洞，在补丁发布前为攻击者提供了优势。WebKit 是为苹果设备上 Safari 浏览器提供动力的引擎。释放后重用漏洞是一种内存破坏问题，指程序在释放了某块内存后仍继续使用指向它的指针，这可能导致任意代码执行。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://cloud.google.com/blog/topics/threat-intelligence/darksword-ios-exploit-chain">The Proliferation of DarkSword: iOS Exploit Chain Adopted by ...</a></li>
<li><a href="https://thehackernews.com/2026/03/darksword-ios-exploit-kit-uses-6-flaws.html">DarkSword iOS Exploit Kit Uses 6 Flaws, 3 Zero-Days for Full ...</a></li>
<li><a href="https://nvd.nist.gov/vuln/detail/CVE-2025-43529">NVD - CVE-2025-43529</a></li>

</ul>
</details>

**标签**: `#cybersecurity`, `#vulnerability`, `#ios`, `#safari`, `#exploit`

---

<a id="item-10"></a>
## [Google 推出基于 Gemini 的暗网情报与安全运营 AI 代理，已开放公开预览。](https://www.theregister.com/2026/03/23/google_dark_web_ai/) ⭐️ 8.0/10

Google 已将基于 Gemini 的暗网情报服务集成到 Google Threat Intelligence 中，并以公开预览形式上线。该服务会先为客户建立组织画像，然后每天从约 800 万至 1000 万条暗网帖子中筛查与该组织相关的风险，识别初始访问中介活动、数据泄露和内部威胁等信息。 这代表了生成式 AI 在自动化和规模化威胁情报方面的重要应用，可能使安全团队能够以声称的高准确率，从庞大且难以监控的暗网中主动识别风险。它标志着利用大语言模型对抗由初始访问中介等推动的复杂、不断演变的网络威胁迈出了重要一步。 Google 表示，基于内部测试，该系统在分析每日数百万外部事件时准确率达到 98%。该服务旨在处理来自暗网来源（包括传统搜索引擎未索引的论坛和市场）的海量非结构化数据。

telegram · zaihuapd · Mar 24, 13:15

**背景**: 暗网监控涉及持续扫描互联网的隐藏部分（如 TOR 网络和加密通道），以查找被盗凭证或企业数据等信息。初始访问中介（IABs）是威胁行为者，他们入侵企业网络并将未经授权的访问权限出售给其他网络犯罪分子，通常用于推动勒索软件攻击。威胁情报服务旨在收集和分析此类信息，以向组织发出潜在安全风险的警告。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.crowdstrike.com/en-us/cybersecurity-101/threat-intelligence/dark-web-monitoring/">What is Dark Web Monitoring? [Beginner's Guide] | CrowdStrike</a></li>
<li><a href="https://cyble.com/dark-web-intelligence-monitoring-guide/">Dark Web Intelligence: Why Monitoring Matters In 2026</a></li>
<li><a href="https://cybernews.com/security/initial-access-broker-threat-corporate-network-breach/">They hack to sell: corporate access traded in shadows | Cybernews Researchers Uncover Data Leak Site Linked To Active Initial ... Initial Access Brokers How They’re Changing Cybercrime - CIS A Deep-Dive Into Initial Access Brokers: Trends, Statistics ... Initial access brokers involved in more ... - Cybersecurity Dive Initial Access Brokers Plays a Vital Role Modern Ransomware ... Initial Access Brokers—Everything You Need To Know</a></li>

</ul>
</details>

**标签**: `#AI Security`, `#Threat Intelligence`, `#Google Gemini`, `#Dark Web Monitoring`, `#Cybersecurity`

---

<a id="item-11"></a>
## [批评微软对 Windows 11 的修复仅为表面改进](https://www.sambent.com/microsofts-plan-to-fix-windows-11-is-gaslighting/) ⭐️ 7.0/10

一篇批评文章指出，微软近期对 Windows 11 的更改，例如添加视觉装饰，只是表面改进，并未解决操作系统中根本性的、对用户不友好的设计选择。该批评将这些更改定性为在实施激进策略后提供微小修复，是对用户的'煤气灯操纵'。 这很重要，因为它凸显了软件供应商的商业策略与用户自主权之间日益增长的紧张关系，对数亿 Windows 用户具有重大影响。如果表面修复成为常态，可能会使整个行业日益侵入式的软件设计正常化，从而削弱用户对自己设备的控制权。 文章特别批评了诸如强制更新、难以永久禁用的侵入式功能，以及微软测试用户容忍度的渐进式方法。文章指出，核心问题是微软做出了战略选择，优先考虑用户参与度和数据收集，而非提供干净、尊重用户的体验。

hackernews · h0ek · Mar 24, 09:36

**背景**: Windows 11 是微软继 Windows 10 之后最新的主要操作系统版本。软件批评中的'用户不友好设计'一词指的是以牺牲用户的便利性、控制权或隐私为代价而使公司受益的功能，例如难以卸载的臃肿软件、激进的更新提示或有利于数据收集的默认设置。'煤气灯操纵'是一个心理学术语，在此用作隐喻，描述通过提供微小、分散注意力的修复来让用户怀疑自己合理投诉的行为。

**社区讨论**: 社区情绪 largely 批评微软，用户将其策略比作渐进式测试用户容忍极限。一些评论将其与历史上的'浏览器大战'等做法相提并论，而另一些则指出苹果也存在类似趋势。提到的具体不满包括已禁用功能（如 Microsoft Start 新闻）的顽固重现和侵入式的升级提示。

**标签**: `#windows-11`, `#microsoft`, `#user-experience`, `#software-criticism`, `#tech-policy`

---