---
layout: default
title: "Horizon Summary: 2026-03-25 (ZH)"
date: 2026-03-25
lang: zh
---

> From 31 items, 14 important content pieces were selected

---

1. [LiteLLM Python 库 1.82.7 和 1.82.8 版本在 PyPI 上被植入 forkbomb 恶意软件。](#item-1) ⭐️ 9.0/10
2. [LiteLLM PyPI 包 v1.82.8 被植入窃取凭证的 .pth 文件](#item-2) ⭐️ 9.0/10
3. [Wine 11 引入内核级重写 ntsync，为 Linux 运行 Windows 游戏带来巨大速度提升。](#item-3) ⭐️ 8.0/10
4. [社区通过流式专家技术演示在消费级硬件上运行万亿参数大语言模型](#item-4) ⭐️ 8.0/10
5. [英伟达利用 AI 巨额利润投资初创公司，构建生态系统锁定](#item-5) ⭐️ 8.0/10
6. [阿里达摩院发布玄铁 C950 RISC-V CPU，刷新全球性能纪录](#item-6) ⭐️ 8.0/10
7. [我国日均词元调用量两年增超千倍，今年 3 月突破 140 万亿](#item-7) ⭐️ 8.0/10
8. [DarkSword iOS 漏洞链披露：通过 Safari 恶意网页即可感染设备](#item-8) ⭐️ 8.0/10
9. [Google 推出基于 Gemini 的暗网情报 AI 代理，已开放公开预览](#item-9) ⭐️ 8.0/10
10. [OpenAI 计划停用 Sora AI 视频生成器，结束与迪士尼的合作](#item-10) ⭐️ 8.0/10
11. [苹果推出面向企业的 All-in-One 平台 Apple Business，但因其实现缺陷而受到批评。](#item-11) ⭐️ 7.0/10
12. [Arm 推出其首款自主设计并销售的硅产品 AGI CPU](#item-12) ⭐️ 7.0/10
13. [Claude Code 推出自动模式，配备 AI 驱动的安全分类器](#item-13) ⭐️ 7.0/10
14. [主流包管理器纷纷引入依赖冷却功能以应对供应链攻击。](#item-14) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [LiteLLM Python 库 1.82.7 和 1.82.8 版本在 PyPI 上被植入 forkbomb 恶意软件。](https://github.com/BerriAI/litellm/issues/24512) ⭐️ 9.0/10

Python 包索引 (PyPI) 上的 LiteLLM 库 1.82.7 和 1.82.8 版本被发现包含恶意代码，该代码会触发 forkbomb 行为，导致受影响的系统内存迅速耗尽。随后，PyPI 管理员将这些软件包置于隔离状态，在调查期间阻止所有下载。 此次事件是针对一个广泛使用的 AI/ML 工具的重大供应链攻击，凸显了开源生态系统在凭证泄露和自动化发布流程方面的脆弱性。它直接影响依赖 LiteLLM 进行 AI 应用开发的开发者和组织，迫使他们立即进行安全审查和依赖项更新。 恶意负载是一个添加到 `proxy_server.py` 文件中的 base64 编码数据块，它会写入并执行另一个文件，从而导致 forkbomb。维护者表示，攻击可能源于其 CI/CD 流水线中使用的 `trivy` 工具被入侵，而使用固定版本的代理 Docker 镜像的用户未受影响。

hackernews · dot_treo · Mar 24, 12:06

**背景**: LiteLLM 是一个流行的开源库，为调用各种大语言模型 (LLM) API 提供了统一接口。Forkbomb 是一种拒绝服务攻击，其中一个进程会不断自我复制以耗尽 CPU 或内存等系统资源。PyPI 的隔离功能是一项安全措施，当收到可信的恶意软件报告时，会阻止项目的下载，以便进行调查。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://blog.pypi.org/posts/2024-12-30-quarantine/">Project Quarantine - The Python Package Index Blog</a></li>
<li><a href="https://en.wikipedia.org/wiki/Fork_bomb">Fork bomb - Wikipedia</a></li>
<li><a href="https://evrimagaci.org/gpt/teampcp-supply-chain-attacks-escalate-across-open-source-534993">TeamPCP Supply Chain Attacks Escalate Across Open Source</a></li>

</ul>
</details>

**社区讨论**: 社区讨论揭示了一项正在进行的调查，一位维护者将此次攻击与更广泛的 'TeamPCP' 供应链活动联系起来。评论表达了对依赖项安全的深切担忧，呼吁采用更强的开发沙箱环境，并分享了蜜罐系统等防御工具。也有人对问题讨论串中的垃圾评论表示不满。

**标签**: `#security`, `#supply-chain`, `#ai-ml`, `#python`, `#incident-response`

---

<a id="item-2"></a>
## [LiteLLM PyPI 包 v1.82.8 被植入窃取凭证的 .pth 文件](https://simonwillison.net/2026/Mar/24/malicious-litellm/#atom-everything) ⭐️ 9.0/10

发布到 PyPI 的 LiteLLM v1.82.8 软件包被植入了一个隐藏在 base64 编码的 `litellm_init.pth` 文件中的凭证窃取程序，该文件在软件包安装时便会自动执行，无需导入该包。PyPI 管理员在大约三小时内隔离了整个项目，从而限制了暴露窗口。 此次事件是针对一个主要 AI/ML 库的复杂供应链攻击，展示了恶意代码如何仅通过安装软件包即可触发，大大降低了攻击门槛。它凸显了软件供应链中的关键漏洞，尤其是在快速发展的 AI 生态系统中广泛使用的 Python 依赖项，并强调了 CI/CD 工具被入侵所带来的风险。 恶意载荷采用了双重 base64 编码以规避静态分析工具，其目标包括 SSH 密钥、云凭证（AWS、Azure、Kubernetes、Docker）、Git 凭证、加密货币钱包和 shell 历史文件等大量敏感信息。此次攻击与之前 Trivy 安全扫描器的入侵有关，该扫描器被用于 LiteLLM 的 CI/CD 流水线，导致 PyPI 发布凭证被盗。

rss · Simon Willison · Mar 24, 15:07

**背景**: LiteLLM 是一个流行的开源 Python 库，它提供了一个统一的接口来调用来自不同供应商的各种大语言模型（LLM）。在 Python 中，`.pth`（路径）文件是一种可以放置在 site-packages 目录中以修改 Python 模块搜索路径的机制；然而，它们也可以包含任意的 Python 代码，这些代码在每次 Python 解释器启动时都会自动执行，这使其成为供应链攻击的强大载体。PyPI（Python Package Index）是 Python 软件包的主要仓库，其“隔离”功能允许管理员将项目标记为潜在有害，以防止进一步安装。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.xda-developers.com/popular-python-library-backdoor-machine/">A popular Python library just became a backdoor to your entire machine</a></li>
<li><a href="https://blog.pypi.org/posts/2024-12-30-quarantine/">Project Quarantine - The Python Package Index Blog</a></li>
<li><a href="https://github.com/BerriAI/litellm/issues/24512">[Security]: CRITICAL: Malicious litellm_init.pth in litellm 1.82.8 — credential stealer · Issue #24512 · BerriAI/litellm</a></li>

</ul>
</details>

**标签**: `#security`, `#supply-chain`, `#ai-ml`, `#python`, `#pypi`

---

<a id="item-3"></a>
## [Wine 11 引入内核级重写 ntsync，为 Linux 运行 Windows 游戏带来巨大速度提升。](https://www.xda-developers.com/wine-11-rewrites-linux-runs-windows-games-speed-gains/) ⭐️ 8.0/10

Wine 11.0 已发布，其核心特性是进行了一次重大的内核级重写，采用了新的 ntsync 驱动来模拟 Windows NT 同步原语。这一变化带来了显著的性能提升，部分基准测试显示，与未启用特定优化的旧版 Wine 相比，帧率提升了 7-8 倍。 这标志着 Wine 兼容层的效率实现了一次重大飞跃，通过让更多 Windows 游戏以更高性能运行，直接惠及 Linux 游戏生态。它标志着 Wine 向更深度的内核集成进行战略转变，以获得更好的准确性和速度，这对于 Linux 作为游戏平台的可行性至关重要。 所报告的极端性能提升（例如 7-8 倍）主要是在与未打 fsync 补丁的“原版”Wine 对比时观察到的；对于已经在使用 Proton 或打了 fsync 补丁的 Wine 的用户来说，ntsync 带来的提升更为温和，通常在个位数百分比范围内。此次发布还完成了 Wine 的 WoW64 架构，改善了 64 位系统对 32 位应用程序的支持。

hackernews · felineflock · Mar 24, 18:34

**背景**: Wine 是一个免费开源的兼容层，允许 Windows 应用程序（包括游戏）在 Linux 等类 Unix 操作系统上运行。它实时将 Windows API 调用转换为符合 POSIX 标准的调用。Proton 是 Valve Software 开发的一个工具，基于 Wine 构建，并增加了专门为在 Steam Deck 和 Linux 上运行 Windows 游戏而优化的额外补丁和组件（如 esync/fsync）。同步原语是用于协调多个线程或进程执行的底层编程构造。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://docs.kernel.org/next/userspace-api/ntsync.html">NT synchronization primitive driver — The Linux Kernel ...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Proton_(software)">Proton (software) - Wikipedia</a></li>
<li><a href="https://www.msn.com/en-us/gaming/general/wine-11-rewrites-how-linux-runs-windows-games-at-the-kernel-level-and-the-speed-gains-are-massive/ar-AA1ZgKNB">Wine 11 rewrites how Linux runs Windows games at the kernel level ...</a></li>

</ul>
</details>

**社区讨论**: 社区反应非常积极，用户们对 Wine 项目长期、细致的工作表示敬意，并对报道的性能数据感到惊讶。讨论和澄清的一个关键点是，巨大的性能提升是相对于未启用 fsync 的基线而言的，而 ntsync 相对于已经过优化的 fsync 所带来的增量改进则更为有限。社区也对 Valve 通过 Proton 对生态系统的资金投入表示赞赏。

**标签**: `#wine`, `#linux-gaming`, `#compatibility-layer`, `#performance`, `#proton`

---

<a id="item-4"></a>
## [社区通过流式专家技术演示在消费级硬件上运行万亿参数大语言模型](https://simonwillison.net/2026/Mar/24/streaming-experts/#atom-everything) ⭐️ 8.0/10

在最初实验的几天内，开发者已成功演示了在消费级硬件上使用“流式专家”技术运行巨型混合专家大语言模型，包括在配备 96GB 内存的 M2 Max MacBook Pro 上运行 1 万亿参数的 Kimi K2.5 模型，以及在 iPhone 上运行 Qwen3.5-397B-A17B 模型。该技术涉及在处理每个 token 时从 SSD 流式加载所需的专家权重，而非将整个模型加载到内存中。 这一突破极大地降低了运行最先进大语言模型的硬件门槛，有望在个人设备上实现高级 AI 能力，而无需昂贵的云基础设施或专用服务器。这代表了向普及尖端 AI 模型访问迈出的重要一步，并可能加速本地化、保护隐私的 AI 应用开发。 性能因硬件差异显著，iPhone 演示仅达到 0.6 token/秒，而配备 128GB 内存的 M4 Max MacBook Pro 运行相同的 Kimi K2.5 模型可达约 1.7 token/秒。该技术特别适用于混合专家模型，因为在任何给定的推理步骤中，只有一小部分“专家”（如 Qwen3.5 中 3970 亿参数中的 170 亿）处于激活状态。

rss · Simon Willison · Mar 24, 05:09

**背景**: 混合专家是一种大语言模型架构，它使用多个专用子网络（“专家”）和一个路由机制，该机制仅为每个输入激活相关的专家，使得模型可以拥有巨大的总参数量，同时在推理过程中保持可管理的计算成本。像 GPT-4、Mistral 的开源模型和 Qwen3.5 都使用这种架构来实现高性能且高效的推理。“流式专家”方法利用了这一特性，将完整模型存储在快速存储设备（SSD）上，并在处理每个 token 时仅加载所需的一小部分权重。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://developer.nvidia.com/blog/applying-mixture-of-experts-in-llm-architectures/">Applying Mixture of Experts in LLM Architectures | NVIDIA ...</a></li>
<li><a href="https://devblogs.co/posts/streaming-experts">Streaming experts</a></li>
<li><a href="https://qwen-ai.com/">Qwen AI — Open-Source LLMs, Vision, Audio & Coding Models (2026)</a></li>

</ul>
</details>

**标签**: `#LLM`, `#Mixture-of-Experts`, `#Model-Deployment`, `#Edge-AI`, `#Hardware-Efficiency`

---

<a id="item-5"></a>
## [英伟达利用 AI 巨额利润投资初创公司，构建生态系统锁定](https://www.wsj.com/tech/nvidia-ai-market-competition-9db60e4c) ⭐️ 8.0/10

自 2022 年以来，英伟达已向 OpenAI、CoreWeave 和 Reflection AI 等 AI 初创公司投资了数十亿美元，同时扮演供应商、投资者和债权人的多重角色。该公司还通过高价收购和灵活的交易结构，例如与芯片初创公司 Groq 达成 200 亿美元的授权协议，来获取核心技术及人才，同时据报道旨在规避监管审查。 这一策略创造了显著的财务依赖，将客户锁定在英伟达的硬件和软件生态系统中，使其难以转向 AMD 等竞争对手。这种做法已引起美国立法者的关注，他们担心此举可能违反反垄断法，并扼杀关键 AI 基础设施市场的竞争。 投资对象主要是英伟达 GPU 的主要消费者，例如专业 AI 云提供商 CoreWeave。与以独特语言处理单元（LPU）架构闻名的 Groq 达成的交易，涉及授权其技术并挖走其核心工程团队。

telegram · zaihuapd · Mar 24, 03:02

**背景**: 英伟达的图形处理器（GPU）已成为训练和运行大型 AI 模型的事实标准，在 AI 热潮中产生了巨额收入。CoreWeave 是一家专门为 AI 工作负载提供 GPU 基础设施的云计算公司。Groq 是一家芯片公司，开发了语言处理单元（LPU），这是一种专为大型语言模型提供快速、低成本推理而设计的处理器架构，在某些任务上构成了 GPU 的潜在替代方案。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/CoreWeave">CoreWeave - Wikipedia</a></li>
<li><a href="https://www.coreweave.com/">The Essential Cloud for AI | CoreWeave</a></li>
<li><a href="https://en.wikipedia.org/wiki/Groq">Groq - Wikipedia</a></li>

</ul>
</details>

**标签**: `#AI Infrastructure`, `#Antitrust`, `#Nvidia`, `#Market Competition`, `#Venture Capital`

---

<a id="item-6"></a>
## [阿里达摩院发布玄铁 C950 RISC-V CPU，刷新全球性能纪录](https://mp.weixin.qq.com/s/TTnqm8qm3Dxshj_0bxwtkw) ⭐️ 8.0/10

3 月 24 日，在上海举办的 2026 玄铁 RISC-V 生态大会上，阿里巴巴达摩院发布了新一代旗舰 CPU 玄铁 C950。官方称其在 SPECint2006 单核测试中得分超过 70 分，为目前公开 RISC-V 处理器中的较高水平。 这一发布意义重大，因为它表明开源 RISC-V 架构如今已能进入由 x86 和 ARM 主导的高性能计算领域。C950 能够原生运行 Qwen3、DeepSeek V3 等千亿参数级大模型，使其有望成为云 AI、边缘计算和高端机器人等领域的关键参与者，可能降低对专有架构的依赖。 玄铁 C950 面向云计算、生成式人工智能、高端机器人和边缘计算等领域。该芯片集成了达摩院自研的 AI 加速引擎，专门针对原生运行千亿参数级大模型进行了优化。

telegram · zaihuapd · Mar 24, 06:01

**背景**: RISC-V 是一种免费开放的指令集架构（ISA），与 x86（Intel/AMD）和 ARM 等专有架构不同。其开放性允许任何公司在无需支付许可费的情况下设计处理器，从而促进创新并减少供应商锁定。SPECint2006 是一个用于测量处理器整数计算性能的标准化基准测试套件，为不同架构间的比较提供了通用指标。Qwen3 是阿里云开发的大语言模型系列。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/RISC-V_architecture">RISC-V architecture</a></li>
<li><a href="https://en.wikipedia.org/wiki/SPECint">SPECint - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Qwen">Qwen - Wikipedia</a></li>

</ul>
</details>

**标签**: `#RISC-V`, `#Hardware`, `#AI Acceleration`, `#Semiconductors`, `#Alibaba`

---

<a id="item-7"></a>
## [我国日均词元调用量两年增超千倍，今年 3 月突破 140 万亿](http://paper.people.com.cn/rmrb/pc/content/202603/24/content_30147015.html) ⭐️ 8.0/10

国家数据局披露，我国日均词元（Token）调用量已在今年 3 月突破 140 万亿。这一指标从 2024 年初的 1000 亿，增长至 2025 年底的 100 万亿，两年内增幅超过一千倍。 这一爆炸性增长标志着中国人工智能产业正在快速规模化与商业化，因为词元调用量是衡量 AI 模型活跃度和采用率的直接指标。它也表明，围绕词元的调用、分发与结算，新的价值体系正在加速形成，并成为人工智能产业商业化的重要路径。 该数据由中国负责数据治理的关键政府部门——国家数据局正式发布。报告将这一增长与正在推进的数据要素市场化配置改革以及人工智能高质量数据供给体系的形成联系起来。

telegram · zaihuapd · Mar 24, 07:22

**背景**: 在人工智能和自然语言处理领域，词元（Token）是大模型处理信息的最小单元，可以理解为文本的碎片或 AI 的“燃料”。词元化是将连续文本切分为词元序列的过程，是几乎所有 NLP 流程的第一步。在中国的政策语境中，“数据要素”指被确认为生产要素的数据，其“市场化配置改革”是一项国家政策，旨在建立高效交易和利用数据的市场与机制。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://zh.wikipedia.org/wiki/词元_(自然语言处理)">词元 (自然语言处理) - 维基百科，自由的百科全书</a></li>
<li><a href="https://www.runoob.com/ai-agent/token-intro.html">Token (词元) - 菜鸟教程</a></li>
<li><a href="https://www.wuhan.gov.cn/zwgk/xxgk/zfwj/bgtwj/202304/P020230414574725502889.pdf">标题</a></li>

</ul>
</details>

**标签**: `#AI Infrastructure`, `#Token Economics`, `#China Tech`, `#LLM Scaling`, `#Data Elements`

---

<a id="item-8"></a>
## [DarkSword iOS 漏洞链披露：通过 Safari 恶意网页即可感染设备](https://t.me/zaihuapd/40482) ⭐️ 8.0/10

一个名为 DarkSword 的复杂 iOS 漏洞利用链被公开披露，该漏洞链串联了六个漏洞，可使运行 iOS 18.4 至 18.7 的 iPhone 在 Safari 中访问恶意网页时即被远程执行代码。该漏洞自 2025 年 11 月起被用于针对沙特阿拉伯、土耳其、马来西亚和乌克兰的定向攻击，并投放了 GHOSTBLADE 等恶意载荷。 此次披露凸显了针对移动设备的复杂多阶段漏洞利用链的持续威胁，展示了单个恶意网页如何导致设备被完全控制。它强调了及时进行软件更新的极端重要性，因为这些攻击利用了在后续 iOS 版本（包括 iOS 26.3）中已被修补的漏洞。 该漏洞利用链几乎完全由 JavaScript 编写，简化了部署过程。六个漏洞之一的 CVE-2025-43529 是 WebKit 中的一个释放后重用漏洞，已在 iOS 18.7.3 和 26.2 中修补，但在针对 iOS 18.6 至 18.7 的攻击中被利用。已知 GHOSTBLADE 载荷会针对加密货币应用程序并窃取敏感数据。

telegram · zaihuapd · Mar 24, 11:45

**背景**: DarkSword 是一个“全链”漏洞利用工具包，意味着它结合了跨不同软件层（如 WebKit 浏览器引擎和 iOS 内核）的多个漏洞，从而能够从一个远程起点（如网页）实现对设备的完全控制。“零点击”或“一键式”漏洞利用除了加载恶意内容外，几乎不需要用户进行任何交互。WebKit 是为 iOS 和 macOS 上的 Safari 提供支持的浏览器引擎。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.hklaw.com/en/insights/publications/2026/03/new-ios-exploit-darksword-and-a-new-era-of-mobile-security">New iOS Exploit "DarkSword" and a New Era of Mobile Security</a></li>
<li><a href="https://labs.cloudsecurityalliance.org/wp-content/uploads/2026/03/CSA_research_note_darksword_ios_fullchain_zeroday_multiactor_20260319-csa-styled.pdf">DarkSword: Full-Chain iOS Zero-Day Exploitation by State Actors</a></li>
<li><a href="https://nvd.nist.gov/vuln/detail/CVE-2025-43529">NVD - CVE-2025-43529</a></li>

</ul>
</details>

**标签**: `#iOS Security`, `#Browser Exploit`, `#Vulnerability Disclosure`, `#Zero-Click Exploit`, `#Cyber Threat Intelligence`

---

<a id="item-9"></a>
## [Google 推出基于 Gemini 的暗网情报 AI 代理，已开放公开预览](https://www.theregister.com/2026/03/23/google_dark_web_ai/) ⭐️ 8.0/10

Google 已推出基于 Gemini AI 模型的暗网情报服务，并在 Google Threat Intelligence 平台中以公开预览形式上线。该服务会先为客户建立组织画像，然后每天从约 800 万至 1000 万条暗网帖子中筛查与该组织相关的风险，例如初始访问中介活动、数据泄露和内部威胁，内部测试显示其准确率达到 98%。 这标志着将大语言模型应用于自动化和规模化威胁情报处理的重要进展，而这一过程传统上是手动且资源密集型的。通过以高准确率分析海量暗网数据，该服务使安全团队能够在攻击发动之前，主动发现针对其特定组织的威胁。 该服务已集成到现有的 Google Threat Intelligence 平台中，专注于识别高度具体的威胁，例如初始访问中介活动，这是勒索软件等更严重攻击的前兆。其宣称的 98% 准确率表明其重点是减少误报，这是安全团队运营效率的关键因素。

telegram · zaihuapd · Mar 24, 13:15

**背景**: 暗网是互联网中未被传统搜索引擎索引的部分，常被用于非法活动，包括出售被盗数据和访问被入侵的系统。初始访问中介是一类专门入侵网络，然后将未经授权的访问权限出售给其他威胁行为者（如勒索软件团伙）的网络犯罪分子。暗网监控服务旨在扫描这些隐藏的论坛和市场，以发现可能预示组织即将面临威胁的信息。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.theregister.com/2026/03/23/google_dark_web_ai/">Google unleashes Gemini AI agents on the dark web</a></li>
<li><a href="https://en.wikipedia.org/wiki/Initial_access_broker">Initial access broker - Wikipedia</a></li>
<li><a href="https://expertinsights.com/security-operations/the-top-dark-web-monitoring-solutions">Dark Web Monitoring: The Top Dark Web Monitoring Services 2026</a></li>

</ul>
</details>

**标签**: `#AI-Security`, `#Gemini`, `#Threat-Intelligence`, `#Dark-Web`, `#Google-Cloud`

---

<a id="item-10"></a>
## [OpenAI 计划停用 Sora AI 视频生成器，结束与迪士尼的合作](https://www.bloomberg.com/news/articles/2026-03-24/openai-plans-to-discontinue-support-for-sora-ai-video-generator?srnd=phx-technology) ⭐️ 8.0/10

OpenAI 宣布计划关闭其 Sora AI 视频生成器产品及其开发者 API，距离该独立应用高调上线仅约六个月。公司也正在逐步结束与迪士尼围绕 Sora 达成的多年合作协议。 这标志着一家领先的 AI 公司的一次重大战略转向，表明其正从面向消费者的生成式 AI 视频工具，转向其认为更具盈利性或战略性的领域，如 AI agents 和基础模型。此举将影响开发者、迪士尼等合作伙伴以及 AI 视频生成领域的竞争格局。 此次关闭是 OpenAI 精简其产品线、重新分配资源计划的一部分。公司正将重心转向开发 AI agents 和一个代号为 'Spud' 的新基础 AI 模型，同时重组部分安全与保障团队，以使其更紧密地融入开发流程。

telegram · zaihuapd · Mar 25, 00:30

**背景**: Sora 是 OpenAI 开发的一款 AI 模型，能够根据文本描述生成逼真且富有想象力的视频片段。它于 2025 年底作为独立的消费者应用推出，因其强大的功能而备受关注。AI agents 是指利用 AI 技术，代表用户自主追求目标、完成任务，并展现出推理、规划和记忆能力的软件系统。OpenAI 内部代号为 'Spud' 的新模型，代表了公司下一阶段主要的 AI 开发方向。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.nytimes.com/2026/03/24/technology/openai-shutting-down-sora.html">OpenAI Is Shutting Down Sora, Its A.I. Video Generator OpenAI shutting down Sora video-creation app - NBC News That Was Fast. OpenAI to Shut Down Sora Video Generator App OpenAI pulls the plug on Sora video generator | AP News OpenAI shutters AI video generator Sora after six-month app ... OpenAI is shutting down its Sora video generation app - Engadget OpenAI Plans to Discontinue Support for Sora AI Video Generator</a></li>
<li><a href="https://cloud.google.com/discover/what-are-ai-agents">What are AI agents? Definition, examples, and types | Google ...</a></li>
<li><a href="https://www.tomsguide.com/ai/openai-just-killed-sora-as-company-readies-ipo-and-new-spud-model">OpenAI just killed Sora as company readies IPO and new 'Spud ...</a></li>

</ul>
</details>

**标签**: `#OpenAI`, `#AI-Video-Generation`, `#Product-Strategy`, `#AI-Agents`, `#Industry-News`

---

<a id="item-11"></a>
## [苹果推出面向企业的 All-in-One 平台 Apple Business，但因其实现缺陷而受到批评。](https://www.apple.com/newsroom/2026/03/introducing-apple-business-a-new-all-in-one-platform-for-businesses-of-all-sizes/) ⭐️ 7.0/10

苹果公司宣布推出 Apple Business，这是一个面向各种规模企业的新型一体化平台，提供设备管理、商务邮箱、日历以及支持自定义域名的目录服务等集成服务。该平台免费提供，可选择付费升级存储空间，并包含预装软件管理和用户组等功能。 此举标志着苹果在企业 SaaS 市场的重大推进，直接挑战了微软 365 和 Intune 等现有厂商，尤其是针对中小型企业。一个成功的平台可能重塑商业软件生态系统，并增强苹果在企业 IT 环境中的存在感。 该平台的初始实现，特别是将现有苹果账户迁移至业务管理的“域名锁定/捕获”流程，被报告存在漏洞且用户体验不佳。主要批评包括对“自带设备”（BYOD）的支持差、更改企业名称的流程复杂，以及缺乏解决严重问题的有效支持工具。

hackernews · soheilpro · Mar 24, 15:29

**背景**: Apple Business Manager 是苹果现有的基于 Web 的管理门户，供 IT 管理员部署苹果设备、管理账户和配置设置。一体化商业平台旨在将多种 IT 服务（如设备管理、电子邮件和协作工具）整合到单一的集成产品中。众所周知，实施此类平台具有挑战性，通常会面临用户迁移、数据集成和复杂配置流程等方面的陷阱。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://klaxoon.com/insight/implementing-an-enterprise-platform-5-pitfalls-to-avoid-to-maximize-your-savings/">Implementing an all-in-one platform: 5 pitfalls to avoid</a></li>
<li><a href="https://www.forbes.com/councils/forbestechcouncil/2024/06/28/tech-consolidation-how-all-in-one-solutions-are-shaping-modern-business-operations/">How All-In-One Tech Solutions Are Shaping Modern Business ... Businesses are being 'locked in' to all-in-one platforms ... The Complete Guide to Software Implementation: Challenges ... Top 10 ERP Implementation Challenges & How to Solve Them</a></li>

</ul>
</details>

**社区讨论**: Hacker News 的讨论揭示了对该平台当前实现的重大批评，用户描述其设置过程“漏洞百出”且令人沮丧，尤其是在域名迁移方面。虽然一些人看到了它对新兴小型企业的战略潜力，但另一些人则认为这证实了苹果在企业 IT 体验方面一贯不佳的历史。此外，也有关于该平台免费定价模式可能阻碍其对必要改进进行投资的讨论。

**标签**: `#apple`, `#business-software`, `#enterprise`, `#saas`, `#product-launch`

---

<a id="item-12"></a>
## [Arm 推出其首款自主设计并销售的硅产品 AGI CPU](https://newsroom.arm.com/blog/introducing-arm-agi-cpu) ⭐️ 7.0/10

Arm 宣布了其首款直接销售的硅产品 Arm AGI CPU，这标志着其经营模式发生了历史性转变，从超过 35 年的 IP 授权模式转向自主设计、制造和销售芯片。这款 136 核的 CPU 专为数据中心设计，将由台积电制造，Meta 被宣布为首个主要客户，将于今年晚些时候开始部署。 此举代表了 Arm 一次根本性的战略转向，可能为其带来数十亿美元的年收入，并重塑数据中心和 AI 硬件市场的竞争格局。通过销售自有芯片，Arm 现在直接与其被授权方（如高通和英伟达）竞争，同时也为构建智能体 AI 基础设施的公司提供了一个新选择。 产品名称中的 "AGI" 代表 "Agentic AI Infrastructure"（智能体 AI 基础设施），指的是其目标工作负载是支持自主 AI 智能体，而非 "Artificial General Intelligence"（通用人工智能）。该 CPU 基于 Arm 的 Neoverse 架构，并宣称在 AI 数据中心工作负载上，其性能是同类 x86 处理器的两倍。

hackernews · RealityVoid · Mar 24, 17:30

**背景**: Arm Holdings 是一家英国公司，主要以为大多数智能手机以及越来越多的服务器和其他设备设计 CPU 架构（Arm 架构）而闻名。几十年来，Arm 的商业模式一直是将其 CPU 设计和知识产权授权给其他公司（如苹果、高通、三星），然后由这些公司制造和销售芯片。智能体 AI 指的是新一代半自主或全自主的 AI 系统，能够独立感知、推理和行动，这需要专门且可扩展的计算基础设施。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://newsroom.arm.com/blog/introducing-arm-agi-cpu">Announcing Arm AGI CPU: The silicon foundation for the ...</a></li>
<li><a href="https://mitsloan.mit.edu/ideas-made-to-matter/agentic-ai-explained">Agentic AI, explained - MIT Sloan</a></li>
<li><a href="https://www.reuters.com/business/media-telecom/arm-unveils-new-ai-chip-expects-it-add-billions-annual-revenue-2026-03-24/">Arm unveils new AI chip, expects it to add billions in annual ...</a></li>

</ul>
</details>

**社区讨论**: 社区讨论凸显了对产品命名的强烈质疑，用户批评 "AGI" 是误导性营销，利用了围绕通用人工智能的热度。一些评论指出，这种向销售芯片的战略转变在高通诉 Arm 的诉讼中已有预兆，当时高通指控 Arm 有此计划，而 Arm 当时的 CEO 予以否认。社区情绪复杂，一方面承认其商业模式的歷史性转变，另一方面质疑产品的新颖性和营销策略。

**标签**: `#arm`, `#semiconductors`, `#ai-hardware`, `#business-strategy`, `#cpu`

---

<a id="item-13"></a>
## [Claude Code 推出自动模式，配备 AI 驱动的安全分类器](https://simonwillison.net/2026/Mar/24/auto-mode-for-claude-code/#atom-everything) ⭐️ 7.0/10

Claude Code 推出了全新的“自动模式”权限系统，AI 助手可代表用户做出权限决策，取代了之前的 --dangerously-skip-permissions 标志。该系统使用 Claude Sonnet 4.6 作为分类器模型，在每次操作运行前审查对话，阻止超出任务范围、针对不可信基础设施或看似由恶意内容驱动的操作。 这代表了 AI 辅助开发的重大进步，它在保持保护的同时自动化了安全决策，可能消除开发人员生产力与安全性之间的权衡。它解决了一个主要痛点，即开发人员以前必须在手动权限提示和完全绕过安全保护的危险跳过标志之间做出选择。 该系统包含广泛的默认过滤器，涵盖本地文件管理、只读 API 调用以及从已声明的清单安装依赖等操作，同时阻止诸如强制推送到 Git、执行外部代码下载或安装任意包等操作。用户可以进一步自定义这些规则，且分类器始终在 Claude Sonnet 4.6 上运行，与主会话模型无关，从而提供一致的安全评估。

rss · Simon Willison · Mar 24, 23:57

**背景**: Claude Code 是一款 AI 驱动的编码助手，此前要求开发人员配置细粒度权限或使用 --dangerously-skip-permissions 标志来完全绕过提示。该跳过标志专为容器化环境设计，但尽管存在安全风险，仍因能实现不间断的工作流程而流行。Claude Sonnet 4.6 是 Anthropic 的中端 AI 模型，具有增强的编码、推理能力和 100 万 token 的上下文窗口，使其适合复杂的分类任务。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://code.claude.com/docs/en/permissions">Configure permissions - Claude Code Docs</a></li>
<li><a href="https://www.anthropic.com/news/claude-sonnet-4-6">Introducing Claude Sonnet 4.6 - Anthropic</a></li>
<li><a href="https://www.ksred.com/claude-code-dangerously-skip-permissions-when-to-use-it-and-when-you-absolutely-shouldnt/">Claude Code --dangerously-skip-permissions: Safe Usage Guide ...</a></li>

</ul>
</details>

**标签**: `#AI-assisted-development`, `#developer-tools`, `#code-safety`, `#Claude`, `#permissions`

---

<a id="item-14"></a>
## [主流包管理器纷纷引入依赖冷却功能以应对供应链攻击。](https://simonwillison.net/2026/Mar/24/package-managers-need-to-cool-down/#atom-everything) ⭐️ 7.0/10

在近期 LiteLLM 供应链攻击事件后，一项分析显示，自 2025 年底以来，多个主流包管理器已迅速实现了依赖冷却机制。这包括 pnpm 的 `minimumReleaseAge`、npm 的 `min-release-age`、Bun 的 `minimumReleaseAge`、Deno 的 `--minimum-dependency-age`、uv 增强的 `--exclude-newer` 以及 pip 的 `--uploaded-prior-to` 标志。 这标志着软件供应链安全领域一次重要且协同的转变，从事后修补转向主动风险缓解。通过延迟自动安装新发布的软件包，这些功能为安全社区提供了检测和响应恶意更新的时间窗口，从而有可能在恶意更新被广泛采用之前阻止类似 LiteLLM 攻击的大规模事件。 具体实现各有不同：大多数工具允许设置相对时间延迟（例如 1440 分钟代表一天），并且许多工具包含针对受信任包的覆盖机制。一个显著的局限是 pip 26.0 目前其 `--uploaded-prior-to` 标志仅支持绝对时间戳，不过存在使用 cron 作业的变通方案。

rss · Simon Willison · Mar 24, 21:11

**背景**: 依赖冷却是一种安全实践，它在软件包发布到注册中心（如 npm 或 PyPI）与包管理器自动安装或更新到该新版本之间引入一个等待期。这一概念作为抵御软件供应链攻击的一种防御手段而受到关注，在这种攻击中，攻击者会入侵合法的软件包并发布恶意更新。近期对每月下载量达 9500 万次的流行 AI 网关库 LiteLLM 的攻击就是此类威胁的一个典型例子，攻击者利用被入侵的维护者账户来分发恶意代码。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://blog.yossarian.net/2025/11/21/We-should-all-be-using-dependency-cooldowns">We should all be using dependency cooldowns - blog.yossarian.net</a></li>
<li><a href="https://docs.litellm.ai/blog/security-update-march-2026">Security Update: Suspected Supply Chain Incident - liteLLM</a></li>
<li><a href="https://pnpm.io/blog/releases/10.16">pnpm 10.16 | pnpm</a></li>

</ul>
</details>

**标签**: `#package-management`, `#security`, `#supply-chain`, `#devops`, `#software-engineering`

---