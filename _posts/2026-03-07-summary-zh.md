---
layout: default
title: "Horizon Summary: 2026-03-07 (ZH)"
date: 2026-03-07
lang: zh
---

> From 32 items, 11 important content pieces were selected

---

1. [Andrej Karpathy 启动 'autoresearch' 项目，利用 AI 智能体自动化单 GPU 训练实验。](#item-1) ⭐️ 8.0/10
2. [60 岁开发者表示 Claude Code AI 助手重新点燃了他的编程热情](#item-2) ⭐️ 8.0/10
3. [Anthropic 发布 Claude Code Security 预览版，检出 500 余个陈年漏洞，网络安全板块下跌 8%](#item-3) ⭐️ 8.0/10
4. [Proton Mail 向瑞士当局提供付款数据，FBI 借此识别匿名抗议者](#item-4) ⭐️ 8.0/10
5. [Anthropic 将对美国国防部的供应链风险认定提起法律挑战](#item-5) ⭐️ 8.0/10
6. [黄仁勋预测软件公司将从授权模式转向出租 AI 代理](#item-6) ⭐️ 8.0/10
7. [vLLM v0.17.0 发布，支持 PyTorch 2.10 和 FlashAttention 4，Model Runner V2 迎来重大升级。](#item-7) ⭐️ 7.0/10
8. [Go 标准库将包含 UUID 包](#item-8) ⭐️ 7.0/10
9. [Anthropic 五角大楼合同被分析为商品化 AI 市场中的品牌战略](#item-9) ⭐️ 7.0/10
10. [谷歌、微软、亚马逊将继续提供 Anthropic AI，但排除国防项目](#item-10) ⭐️ 7.0/10
11. [谷歌 AI Overviews 吞噬媒体流量，部分科技网站来自谷歌的访问量暴跌超 90%](#item-11) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [Andrej Karpathy 启动 'autoresearch' 项目，利用 AI 智能体自动化单 GPU 训练实验。](https://github.com/karpathy/autoresearch) ⭐️ 8.0/10

Andrej Karpathy 在 GitHub 上创建了一个名为 'autoresearch' 的新分支和代码库，这是一个让 AI 智能体自主进行研究的框架，专门用于在单 GPU 上训练 nanochat 模型。该系统旨在以最少的人工干预，在夜间自动运行实验。 这个项目之所以重要，是因为它旨在通过自动化实验流程，在低成本、易获取的硬件上实现 AI 研究的民主化和加速。如果成功，它将使个人研究者和小型团队能够在无需庞大计算资源或持续人工监督的情况下，系统性地进行模型训练的夜间优化。 该框架专门针对 'nanochat' 训练，这是 Karpathy 的一个项目，旨在用大约 100 美元的成本训练出一个类似 ChatGPT 的可用模型。'autoresearch' 系统实现了一个自主优化循环，AI 智能体可以根据用户提供的高级指令文件来设计、运行和分析实验。

github · karpathy · Mar 6, 22:01

**背景**: Andrej Karpathy 是一位著名的 AI 研究员，曾任特斯拉 AI 总监，以创建 'nanochat' 等教育性和极简主义的 AI 项目而闻名。'Nanochat' 是一个专注于在单 GPU 节点上端到端训练一个可用语言模型的项目，目标是创造出 '100 美元能买到的最好的 ChatGPT'。AI 智能体是能够感知环境、做出决策并采取行动以实现特定目标的自主系统，将其应用于自动化科学研究是一个新兴且活跃的发展领域。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/karpathy/autoresearch">GitHub - karpathy/autoresearch: AI agents running research on ...</a></li>
<li><a href="https://github.com/karpathy/nanochat">GitHub - karpathy/nanochat: The best ChatGPT that $100 can buy. · GitHub</a></li>
<li><a href="https://deepwiki.com/karpathy/autoresearch">karpathy/autoresearch | DeepWiki</a></li>

</ul>
</details>

**标签**: `#AI-agents`, `#automated-research`, `#single-GPU-training`, `#nanochat`, `#Karpathy`

---

<a id="item-2"></a>
## [60 岁开发者表示 Claude Code AI 助手重新点燃了他的编程热情](https://news.ycombinator.com/item?id=47282777) ⭐️ 8.0/10

一位 60 岁的开发者在 Hacker News 上分享，使用 AI 驱动的编程助手 Claude Code 重新点燃了他对编程的热情，让他感受到了几十年前接触 Active Server Pages 和 COM 组件等技术时的兴奋与动力。他描述自己熬夜使用该工具工作，这让他想起了职业生涯早期的热情。 这个个人故事凸显了 AI 编程助手如何能重新激发经验丰富的开发者对技术的参与度，可能延长他们的生产性职业生涯，并改变各年龄段开发者与编程的互动方式。这表明 AI 有潜力减轻开发者跟上复杂现代技术栈的认知负担，并将精力重新聚焦于创造性解决问题。 这位开发者特别提到 Claude Code 是产生这种效果的工具，并将其与他职业生涯中早期变革性技术相比较。他提到熬夜使用该工具工作，这表明了与他过去体验服务器端编程突破时类似的深度参与。

hackernews · shannoncc · Mar 7, 00:05

**背景**: Claude Code 是由 Anthropic 开发的 AI 驱动编程助手，通过自然语言交互帮助开发者编写、调试和改进代码。Active Server Pages (ASP)是微软在 20 世纪 90 年代末期创建动态网页的首个服务器端脚本技术，而 COM（组件对象模型）是微软创建可重用二进制软件组件的技术，是 Windows 开发的基础。开发者提到的 VB6、COM 组件和 ASP 将其早期职业生涯定位在 20 世纪 90 年代末/21 世纪初的微软生态系统中。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://claude.com/product/claude-code">Claude Code by Anthropic | AI Coding Agent, Terminal, IDE</a></li>
<li><a href="https://en.wikipedia.org/wiki/Active_Server_Pages">Active Server Pages - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Component_Object_Model">Component Object Model - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: 讨论显示出复杂但投入的回应，许多年长开发者对现代 Web 技术栈带来的压力感同身受，并发现 AI 工具具有 rejuvenating 效果。一些评论者分享了 AI 重新点燃他们编程热情的类似经历，而另一些人则表达了对 AI 潜在就业市场影响的担忧，以及有 AI 辅助与无 AI 辅助编程的不同体验。

**标签**: `#AI-assisted-programming`, `#developer-experience`, `#career-reflection`, `#technology-adoption`, `#hacker-news`

---

<a id="item-3"></a>
## [Anthropic 发布 Claude Code Security 预览版，检出 500 余个陈年漏洞，网络安全板块下跌 8%](https://t.me/zaihuapd/40077) ⭐️ 8.0/10

2026 年 2 月 20 日，Anthropic 推出了 Claude Code Security 的限量研究预览版，该功能内置于网页版 Claude Code 中，可自动扫描代码库漏洞并建议补丁。官方数据显示，Claude Opus 4.6 在生产环境的开源代码中发现了 500 多个此前未被察觉的漏洞。 这表明先进 AI 模型在规模化自动化和增强安全审计方面具有巨大潜力，可能颠覆传统的网络安全工具市场。据报道网络安全板块下跌 8%，这表明投资者认识到 AI 驱动的代码分析对现有安全厂商构成了颠覆性威胁。 该工具目前仅向企业和团队客户开放，所有补丁建议在应用前均需经过人工审核。这是一个限量预览版，表明它还不是一个完全发布的产品，其功能正在由特定用户进行测试。

telegram · zaihuapd · Mar 7, 00:23

**背景**: Claude Code 是 Anthropic 的 AI 驱动编码助手，Claude Opus 4.6 是其底层的大型语言模型架构，以处理复杂、长时间运行的任务而闻名。静态应用程序安全测试（SAST）工具通过分析源代码来发现漏洞，而无需执行程序，它是 DevSecOps（将安全实践集成到软件开发生命周期中）的核心组成部分。AI 正越来越多地被应用于增强这些安全分析任务。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://claude.com/solutions/coding">Coding | Claude</a></li>
<li><a href="https://www.aikido.dev/blog/top-10-ai-powered-sast-tools-in-2025">Top 10 AI - powered SAST tools in 2026</a></li>
<li><a href="https://levelact.com/ai-enhanced-devsecops-securing-code-to-cloud/">AI-Enhanced DevSecOps: Securing Code to Cloud with AI</a></li>

</ul>
</details>

**标签**: `#AI Security`, `#Code Analysis`, `#Vulnerability Detection`, `#Anthropic`, `#DevSecOps`

---

<a id="item-4"></a>
## [Proton Mail 向瑞士当局提供付款数据，FBI 借此识别匿名抗议者](https://www.404media.co/proton-mail-helped-fbi-unmask-anonymous-stop-cop-city-protestor/) ⭐️ 8.0/10

法庭记录显示，加密邮件服务 Proton Mail 应瑞士当局的法律请求，提供了与邮箱地址 defendtheatlantaforest@protonmail.com 相关的付款数据。美国联邦调查局（FBI）随后利用这些信息，识别出与该匿名账号有关联的个人，该账号与亚特兰大的 Stop Cop City 抗议运动有关。 这一事件揭示了加密服务隐私保护的一个关键局限：即使受瑞士严格隐私法约束的服务提供商，在法律压力下也可能被迫披露用户的元数据，如付款信息。它为注重隐私的用户和安全专业人士提供了一个重要的现实案例，表明当执法部门通过其他渠道获取身份识别数据时，仅靠加密并不能保证完全的匿名性。 被披露的数据是具体的付款信息，而非 Proton Mail 声称其无法访问的加密邮件内容本身。涉事账号与 'Defend the Atlanta Forest' 团体有关，该团体是反对警察训练中心的去中心化 Stop Cop City 运动的一部分。值得注意的是，与该抗议活动相关的、针对 60 多人的指控此后已被撤销。

telegram · zaihuapd · Mar 7, 01:10

**背景**: Proton Mail 是一家以其端到端加密和强硬隐私立场而闻名的电子邮件服务，总部位于瑞士，受瑞士隐私法管辖。'Stop Cop City' 运动，也称为 'Defend the Atlanta Forest'，是佐治亚州亚特兰大一场去中心化的抗议运动，反对建设一个名为亚特兰大公共安全培训中心的大型警察和消防员训练设施。瑞士法律允许处理国际执法请求，像 Proton 这样的服务商有处理此类请求的法律程序，这可能迫使其披露某些用户数据，即使邮件内容本身仍处于加密状态。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://proton.me/legal/law-enforcement">Information for law enforcement - Proton</a></li>
<li><a href="https://en.wikipedia.org/wiki/Stop_Cop_City">Stop Cop City - Wikipedia</a></li>
<li><a href="https://itsfoss.com/news/swiss-privacy-bill-controversy/">No More Safe Haven for Privacy? Switzerland Drifts Toward a ...</a></li>

</ul>
</details>

**标签**: `#privacy`, `#encryption`, `#law-enforcement`, `#digital-rights`, `#security`

---

<a id="item-5"></a>
## [Anthropic 将对美国国防部的供应链风险认定提起法律挑战](https://t.me/zaihuapd/40080) ⭐️ 8.0/10

3 月 5 日，Anthropic 首席执行官 Dario Amodei 发表声明称，公司于前一日收到美国国防部信函，被认定为国家安全供应链风险。Anthropic 表示不相信该行动具备法律依据，将在法庭上提出挑战。 此次法律挑战可能为 AI 公司在国家安全框架下的监管方式开创重要先例，并界定政府以供应链风险为由将供应商排除在国防合同之外的权力边界。其结果将影响新兴的 AI 产业与美国国家安全采购之间的关系，并左右未来对其他 AI 公司的监管和市场准入。 据声明指出，该认定的适用范围狭窄，仅适用于客户将 Claude 直接用于与国防部合同相关的用途。Anthropic 表示将在过渡期内以名义成本继续向国防部和国家安全社区提供模型及工程师支持。

telegram · zaihuapd · Mar 7, 02:48

**背景**: 美国国防部可根据《美国法典》第 10 编第 3252 条等授权，将公司认定为供应链风险，从而将其排除在某些国防采购之外，以降低对特定系统的风险。Anthropic 是一家领先的 AI 公司，以其 Claude 大语言模型闻名，这些模型是使用人类反馈强化学习（RLHF）等技术训练的生成式 AI 系统。相关的法律框架包括《联邦采购供应链安全法》（FASCSA）等法规，它们规定了政府如何基于供应链安全考虑来限制承包商参与。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.justsecurity.org/132851/anthropic-supply-chain-risk-designation/">What Hegseth’s “Supply Chain Risk” Designation of Anthropic Does and Doesn’t Mean</a></li>
<li><a href="https://www.lawfaremedia.org/article/pentagon's-anthropic-designation-won't-survive-first-contact-with-legal-system">Pentagon’s Anthropic Designation Won’t Survive First Contact with Legal System | Lawfare</a></li>
<li><a href="https://en.wikipedia.org/wiki/Claude_(language_model)">Claude (language model) - Wikipedia</a></li>

</ul>
</details>

**标签**: `#AI Regulation`, `#National Security`, `#Legal Challenge`, `#Anthropic`, `#Government Policy`

---

<a id="item-6"></a>
## [黄仁勋预测软件公司将从授权模式转向出租 AI 代理](https://www.constellationr.com/insights/news/nvidias-huang-all-software-will-be-agentic) ⭐️ 8.0/10

英伟达 CEO 黄仁勋在摩根士丹利科技、媒体与电信大会上表示，未来几乎所有软件都将具备'智能代理'能力。他预测软件公司的主要收入模式将从销售许可证转向出租专门处理任务的 AI 代理和基于 token 的服务，而企业将混合使用自有和租用的模型。 这位行业关键领袖的愿景预示着软件构建、销售和消费方式的根本性转变，可能颠覆传统的 SaaS 商业模式。如果实现，经济力量将向提供专业 AI 代理和基于 token 的基础设施的供应商转移，同时迫使所有软件公司调整其战略。 黄仁勋特别将这一模式与当前的 SaaS 模式进行了对比，认为'智能代理 AI'代表了一种新范式，软件将自主行动而非作为被动工具。他强调，随着 AI 代理的兴起，软件的重要性将会增加而非降低，企业将像管理员工和承包商一样管理模型——混合使用自有和租用的资源。

telegram · zaihuapd · Mar 7, 10:55

**背景**: '智能代理 AI'指的是旨在自主行动以实现特定目标的人工智能系统，超越了被动的聊天机器人，成为主动完成任务的主体。基于 token 的计费是 AI API 服务的常见定价模式，客户根据模型处理的'token'（文本单位）数量付费。微调是指使用专有数据，针对特定任务调整一个预训练的（通常是开源的）基础模型的过程，这与使用完全专有的、以服务形式提供的闭源模型形成对比。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Intelligent_agent">Intelligent agent - Wikipedia</a></li>
<li><a href="https://cdn.medevel.com/understanding-tokens-and-token-based-billing/">How AI API Services Charge You: Understanding Tokens and...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Fine-tuning_(deep_learning)">Fine-tuning (deep learning) - Wikipedia</a></li>

</ul>
</details>

**标签**: `#AI Agents`, `#Software Business Models`, `#NVIDIA`, `#SaaS`, `#Future of Software`

---

<a id="item-7"></a>
## [vLLM v0.17.0 发布，支持 PyTorch 2.10 和 FlashAttention 4，Model Runner V2 迎来重大升级。](https://github.com/vllm-project/vllm/releases/tag/v0.17.0) ⭐️ 7.0/10

vLLM v0.17.0 已发布，其特性包括强制升级至 PyTorch 2.10.0、集成 FlashAttention 4 后端以提升注意力计算性能，以及 Model Runner V2 架构的重大成熟，新增了流水线并行和基于 CUDA 图的 Eagle3 推测解码等功能。该版本还新增了对 Qwen3.5 模型家族的完整支持、一个新的 `--performance-mode` 性能模式标志，以及对 Anthropic API 的兼容性。 此次发布意义重大，因为 vLLM 是一个被广泛使用的高性能大语言模型推理引擎，升级其核心依赖（PyTorch 2.10）和注意力计算内核（FlashAttention 4）将直接影响生产环境中运行大语言模型的速度、效率和成本。Model Runner V2 的成熟以及弹性专家并行等新功能，使得更复杂、可扩展的部署成为可能，特别是对于混合专家模型，这确保了 vLLM 保持在推理优化技术的前沿。 升级到 PyTorch 2.10 是一个破坏性变更，会改变环境依赖，要求用户更新其配置。使用 CUDA 12.9+ 的用户可能会因库不匹配而遇到 `CUBLAS_STATUS_INVALID_VALUE` 错误，发布说明中提供了具体的解决方法，例如修改 `LD_LIBRARY_PATH` 或使用特定的 pip 安装命令。

github · khluu · Mar 7, 00:46

**背景**: vLLM 是一个专为大语言模型设计的高吞吐、内存高效的推理和服务引擎，因此在生产部署中非常流行。FlashAttention 是用于计算 Transformer 模型中注意力机制的优化算法，FlashAttention 4 是其最新版本，专为在 NVIDIA Blackwell 等新一代 GPU 上获得更好性能而重新设计。Model Runner 是 vLLM 执行模型推理的核心架构，其 V2 版本代表了一次重大的重新设计，旨在支持更先进的并行技术和部署场景。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://vllm.ai/">vLLM</a></li>
<li><a href="https://www.theneuron.ai/explainer-articles/flashattention-4-explained-the-software-that-makes-every-ai-chatbot-fast-just-got-a-massive-upgrade-tri-dao-blackwell/">FlashAttention-4, Explained: What it is & Why it Matters</a></li>
<li><a href="https://github.com/vllm-project/vllm/releases">Releases · vllm-project/vllm</a></li>

</ul>
</details>

**标签**: `#llm-inference`, `#gpu-optimization`, `#pytorch`, `#machine-learning`, `#performance`

---

<a id="item-8"></a>
## [Go 标准库将包含 UUID 包](https://github.com/golang/go/issues/62026) ⭐️ 7.0/10

Go 编程语言正在其标准库中添加一个 UUID 包，这由 GitHub issue #62026 中被接受的提案所表明。这一新增功能将提供对生成和处理 UUID 的原生支持，无需依赖第三方库。 这很重要，因为 UUID 是分布式系统、数据库主键和 API 设计的基础，将其纳入标准库对 Go 开发者来说是一个显著的生活质量改进。它减少了依赖管理的开销，并为这一关键工具建立了一个规范的、经过充分审查的实现。 社区讨论揭示了关于支持哪些 UUID 版本的重大争论，评论强调了纯随机的 v4 和更新的、基于时间排序的 v7 之间的权衡。一些开发者还表达了对 UUID 在调试时不友好以及存在像 `github.com/gofrs/uuid` 这样积极维护的第三方替代方案的担忧。

hackernews · soypat · Mar 7, 02:03

**背景**: UUID（通用唯一识别码）是一个 128 位的标签，用于在计算机系统中唯一地标识信息。存在不同的版本，例如 v4（随机）和 v7（基于时间排序），每个版本都有特定的用例以及对数据库和分布式系统的性能影响。Go 标准库是由 Go 团队维护的核心包集合，向其中添加一个包是一个重大决定，意味着长期的维护支持和广泛的实用性。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://jrxcodes.com/uuidv4-vs-uuidv7-a-comprehensive-comparison">UUIDv4 vs UUIDv7: Key Differences Explained - JRX Codes UUID v4 vs v7: What Changed and Why It Matters - DEV Community UUID Versions Explained: V1 vs V4 vs V7 - CreateUUID.com Choosing The Right UUID Version: v1, v4, v6, Or v7 - Authgear Which UUID version to use? - Stack Overflow TIL: 8 versions of UUID and when to use them | nicole@web GUID / UUID V4 vs V7 - Comparison and Migration Guide</a></li>
<li><a href="https://dev.to/santacruz/uuid-v4-vs-v7-what-changed-and-why-it-matters-2bj6">UUID v4 vs v7: What Changed and Why It Matters - DEV Community</a></li>
<li><a href="https://pkg.go.dev/std">Standard library - Go Packages</a></li>

</ul>
</details>

**社区讨论**: 社区表现出浓厚兴趣，讨论集中在 UUID 版本的选择上，一些人主张 v4 的简单性，另一些人则主张 v7 的可排序性。情绪复杂，既有对 Go 务实添加功能的赞扬，也有对 UUID 在调试时不友好的批评，以及关于在现有第三方包的情况下标准库实现是否必要的争论。

**标签**: `#go`, `#uuid`, `#standard-library`, `#programming-languages`, `#backend-development`

---

<a id="item-9"></a>
## [Anthropic 五角大楼合同被分析为商品化 AI 市场中的品牌战略](https://simonwillison.net/2026/Mar/6/anthropic-and-the-pentagon/#atom-everything) ⭐️ 7.0/10

Bruce Schneier 和 Nathan E. Sanders 发表了对 Anthropic 近期及正在进行的五角大楼合同的分析，强调了该公司如何在顶级 AI 模型已变得商品化的市场中实现差异化。Simon Willison 引述了他们的分析，指出 Anthropic 及其 CEO Dario Amodei 正将公司定位为'道德且可信赖'的 AI 提供商，以获取市场价值。 这很重要，因为它揭示了在技术性能趋同的竞争性 AI 格局中的一项关键企业战略。Anthropic 在追求军事合同的同时，以道德和安全为品牌定位，可能会影响政府和企业如何选择 AI 合作伙伴，并可能为高风险领域的'基于价值观'的采购开创先例。 分析指出，Anthropic、OpenAI 和谷歌的最新模型往往'每隔几个月在质量上小幅超越对方'，这使得性能成为一个不那么有效的差异化因素。这种商品化迫使公司在其他因素上竞争，例如品牌、信任和感知到的道德一致性。

rss · Simon Willison · Mar 6, 17:26

**背景**: Anthropic 是一家 AI 安全和研究公司，由前 OpenAI 研究副总裁 Dario Amodei 共同创立并领导。其旗舰模型 Claude 以其'宪法 AI'方法而闻名，该方法使用一套原则（宪法）来指导和约束模型输出，强调安全性和对齐性。在企业 AI 市场中，'商品化'指的是产品变得标准化，主要基于价格或非技术属性而非独特功能进行竞争的趋势。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Claude_(language_model)">Claude (language model) - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Dario_Amodei">Dario Amodei - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Commodity">Commodity - Wikipedia</a></li>

</ul>
</details>

**标签**: `#ai-ethics`, `#military-ai`, `#corporate-strategy`, `#ai-market`

---

<a id="item-10"></a>
## [谷歌、微软、亚马逊将继续提供 Anthropic AI，但排除国防项目](https://www.cnbc.com/2026/03/06/google-says-anthropic-remains-available-outside-of-defense-projects.html) ⭐️ 7.0/10

继微软之后，谷歌和亚马逊宣布将继续通过其云平台向客户提供 Anthropic 的 AI 技术，但明确排除国防相关项目。此举背景是美国国防部将 Anthropic 列为“供应链风险”，原因是该公司拒绝了特定的政府使用条款。 这一决定凸显了 AI 公司的伦理护栏与国家安全利益之间日益紧张的关系，可能为云服务提供商如何在敏感领域管理先进 AI 模型的访问开创先例。它影响了依赖商业云平台获取 AI 能力的国防承包商和政府机构，同时保护了 Claude 模型更广泛的商业可用性。 尽管特朗普政府已指示联邦机构停用该公司技术，但 Anthropic 的 Claude 模型在谷歌 Vertex AI 等平台上仍可获取。Anthropic 首席执行官 Dario Amodei 表示，公司将就国防部的风险认定提起法律诉讼，该认定可能导致合作在六个月内终止。

telegram · zaihuapd · Mar 7, 05:17

**背景**: Anthropic 是一家 AI 安全初创公司，开发了以信息论先驱克劳德·香农命名的 Claude 系列大语言模型。Claude 模型是先进的 AI 系统，可用于软件开发和企业工作流等多种应用。Vertex AI 是谷歌云用于构建、训练和部署机器学习模型及生成式 AI 应用的统一平台。美国国防部的“供应链风险”认定是一种正式分类，可能限制或终止公司与军方合作的能力。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Claude_(language_model)">Claude (language model) - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Vertex_AI">Vertex AI - Wikipedia</a></li>
<li><a href="https://www.politico.com/news/2026/03/05/pentagon-tells-anthropic-it-has-designated-the-company-a-supply-chain-risk-00814758">Pentagon formally designates Anthropic a supply-chain risk</a></li>

</ul>
</details>

**标签**: `#AI Governance`, `#Cloud Computing`, `#Anthropic`, `#Defense Technology`, `#Regulatory Compliance`

---

<a id="item-11"></a>
## [谷歌 AI Overviews 吞噬媒体流量，部分科技网站来自谷歌的访问量暴跌超 90%](https://futurism.com/artificial-intelligence/google-ai-overviews-media) ⭐️ 7.0/10

一项研究显示，10 家美国科技媒体来自谷歌的月访问量已从高峰时的 1.12 亿次骤降至不足 5000 万次，其中部分媒体的跌幅超过 90%。该分析认为，谷歌 AI Overviews（搜索结果中的 AI 摘要）的扩张、Reddit 内容权重的上升，以及用户转向 AI 聊天机器人，是抽空媒体搜索流量的三大原因。 这标志着在线信息发现和消费方式的根本性转变，威胁到许多出版商赖以获取收入和触达受众的传统搜索驱动流量模式。它凸显了 AI 集成搜索的颠覆性力量，以及平台算法可能彻底重塑网络流量格局和媒体生态。 报道中引用的一个显著例子是 Digital Trends，据称其在两年内来自谷歌的访问量暴跌了 97%。谷歌已公开否认该流量分析结论，但具体反驳理由在提供的内容中未详细说明。

telegram · zaihuapd · Mar 7, 13:24

**背景**: 谷歌的 AI Overviews 是集成在谷歌搜索中的一项功能，它利用人工智能直接在搜索结果页面上生成搜索结果的简明摘要。其目的是更快地回答用户查询，而无需用户点击进入源网站。与此同时，谷歌的搜索算法似乎更倾向于展示来自 Reddit 等论坛的内容，因为这些内容因其一手经验和讨论而受到重视。这些变化正伴随着 ChatGPT 等独立 AI 聊天机器人的日益普及而发生，这些工具也提供直接答案。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/AI_Overviews">AI Overviews - Wikipedia</a></li>
<li><a href="https://www.search.google/ways-to-search/ai-overviews/">Google AI Overviews - Search anything, effortlessly</a></li>
<li><a href="https://www.theredditmarketingagency.com/post/the-reddit-algorithm">How Does the Reddit Algorithm Work? (With Action Items)</a></li>

</ul>
</details>

**标签**: `#AI`, `#Search-Engines`, `#Media`, `#Traffic-Analytics`, `#Google`

---