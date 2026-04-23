---
layout: default
title: "Horizon Summary: 2026-04-23 (ZH)"
date: 2026-04-23
lang: zh
---

> From 24 items, 12 important content pieces were selected

---

1. [谷歌发布第八代 TPU 与 Gemini Enterprise 平台，构建 AI 智能体全栈基础设施](#item-1) ⭐️ 9.0/10
2. [苹果修复 iOS 漏洞，该漏洞曾允许警方从通知缓存中恢复已删除的聊天信息](#item-2) ⭐️ 8.0/10
3. [Firefox 和 Tor 浏览器漏洞暴露跨隐私会话的稳定标识符](#item-3) ⭐️ 8.0/10
4. [Qwen3.6-27B：270 亿参数稠密模型实现旗舰级编程性能](#item-4) ⭐️ 8.0/10
5. [Mozilla 使用 Claude Mythos Preview 发现并修复了 Firefox 150 中的 271 个漏洞。](#item-5) ⭐️ 8.0/10
6. [腾讯与阿里巴巴洽谈投资 DeepSeek，估值超 200 亿美元](#item-6) ⭐️ 8.0/10
7. [AI 编程助手'过度编辑'问题分析及提示策略探讨](#item-7) ⭐️ 7.0/10
8. [GitHub Copilot 个人版计划调整：限制收紧、暂停注册、Claude Opus 分级访问。](#item-8) ⭐️ 7.0/10
9. [长江存储一季度收入超 200 亿元，加速扩产拟实现产能翻番](#item-9) ⭐️ 7.0/10
10. [特斯拉中国车机语音服务将接入字节跳动豆包大模型](#item-10) ⭐️ 7.0/10
11. [FBI 从 iPhone 通知数据库提取已删除 Signal 消息，案件发生在得州](#item-11) ⭐️ 7.0/10
12. [法国国家安全证件署（ANTS）确认发生数据泄露，或影响 1900 万公民。](#item-12) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [谷歌发布第八代 TPU 与 Gemini Enterprise 平台，构建 AI 智能体全栈基础设施](https://blog.google/innovation-and-ai/infrastructure-and-cloud/google-cloud/eighth-generation-tpu-agentic-era/) ⭐️ 9.0/10

在 Google Cloud Next 大会上，谷歌发布了采用训练（TPU 8t）与推理（TPU 8i）双架构设计的第八代定制张量处理器（TPU），并将 Gemini Enterprise 升级为端到端的智能体系统。TPU 8t 的单集群算力提升至 3 倍，TPU 8i 的性价比和能效比分别提升 80%和 2 倍，两款芯片均搭载谷歌自研的 Axion 处理器，预计于今年晚些时候正式商用。 此次发布标志着 AI 基础设施的范式转变，为新兴的'智能体时代'提供了软硬件全栈支持，旨在让 AI 智能体执行复杂的多步骤任务。通过为 AI 生命周期的不同阶段提供专用芯片，以及一个具备智能体身份、测试和长期记忆功能的统一平台，谷歌正致力于引领下一代企业级 AI 的大规模开发与部署。 TPU 8t 专为前沿模型训练设计，可构建由 9600 个芯片组成的超级集群；TPU 8i 则针对大规模推理和强化学习优化，以实现快速的智能体推理。升级后的 Gemini Enterprise 平台（现称为 Agent Platform）引入了智能体治理、模拟测试功能，并集成了长期记忆系统，使智能体能够在不同会话间保留信息。

telegram · zaihuapd · Apr 22, 14:38

**背景**: 张量处理器（TPU）是谷歌定制开发的专用集成电路（ASIC），用于加速机器学习工作负载。AI 智能体是能够自主推理、规划并执行多步骤工作流以实现复杂目标的高级 AI 系统，超越了简单的问答功能。AI 智能体的长期记忆是一项关键能力，使其能够持久保存信息、从过去的交互中学习并维持上下文，通常通过向量嵌入和知识图谱等技术实现。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://cloud.google.com/blog/products/compute/tpu-8t-and-tpu-8i-technical-deep-dive">TPU 8t and TPU 8i technical deep dive | Google Cloud Blog</a></li>
<li><a href="https://blog.google/innovation-and-ai/infrastructure-and-cloud/google-cloud/tpus-8t-8i-cloud-next/">Google introduces new TPUs at Cloud Next ‘26 - The Keyword</a></li>
<li><a href="https://mem0.ai/blog/long-term-memory-ai-agents">Long-Term Memory for AI Agents: The What, Why and How</a></li>

</ul>
</details>

**标签**: `#AI Infrastructure`, `#TPU`, `#AI Agents`, `#Google Cloud`, `#Hardware Acceleration`

---

<a id="item-2"></a>
## [苹果修复 iOS 漏洞，该漏洞曾允许警方从通知缓存中恢复已删除的聊天信息](https://techcrunch.com/2026/04/22/apple-fixes-bug-that-cops-used-to-extract-deleted-chat-messages-from-iphones/) ⭐️ 8.0/10

苹果公司已修复 iOS 中的一个安全漏洞，该漏洞曾允许执法机构从 iPhone 中提取已删除的聊天信息。该漏洞涉及操作系统的通知系统将消息内容缓存在本地数据库中，即使在 Signal 等应用内删除消息后，这些缓存内容仍然存在。 此次修复意义重大，因为它堵住了一个破坏端到端加密承诺的后门，用户原本相信已删除的信息会永久消失。它影响了数百万 iPhone 用户的隐私，并改变了执法部门调查的数字取证环境。 缓存数据存在于一个由 iOS 管理的 SQLite 数据库中，不受单个应用删除协议的控制。值得注意的是，仅仅删除像 Signal 这样的应用可能并未清除其缓存的通知，这正是本次补丁要解决的具体行为。用户可以通过在系统通知设置中禁用消息预览来降低类似风险。

hackernews · cdrnsf · Apr 22, 20:27

**背景**: iOS 上的推送通知通常会经过苹果的服务器，并且操作系统会在本地缓存通知内容（如消息预览）以在锁屏上显示。执法部门使用的取证工具，如 Cellebrite 的 UFED，可以进行完整的文件系统提取以访问这些缓存数据，即使在应用内原始内容已被删除之后。像 Signal 这样的端到端加密消息应用会对消息内容进行加密，但由操作系统生成的通知预览可能会创建一个持久的、未加密的记录。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://spacedaily.com/sd-n-the-push-notification-backdoor-how-ios-architecture-undermines-end-to-end-encryption-by-design/">The Push Notification Backdoor: How iOS Architecture Undermines End-to-End Encryption by Design</a></li>
<li><a href="https://blog.elcomsoft.com/2021/11/the-five-ways-to-recover-iphone-deleted-data/">The Five Ways to Recover iPhone Deleted Data | ElcomSoft blog</a></li>
<li><a href="https://cellebrite.com/en/products/ufed/">Cellebrite UFED | Mobile Device Extraction Tool for iOS</a></li>

</ul>
</details>

**社区讨论**: 评论者指出，核心问题在于 iOS 架构默认缓存通知内容，且不受应用控制。他们提到 Signal 提供了“通用通知”设置来隐藏内容，一些人对苹果整体的安全叙事表示怀疑。讨论强调，“已删除”并不总是意味着从所有系统缓存中擦除。

**标签**: `#privacy`, `#security`, `#apple`, `#law-enforcement`, `#encryption`

---

<a id="item-3"></a>
## [Firefox 和 Tor 浏览器漏洞暴露跨隐私会话的稳定标识符](https://fingerprint.com/blog/firefox-tor-indexeddb-privacy-vulnerability/) ⭐️ 8.0/10

Fingerprint.com 的研究人员发现，基于 Firefox 的浏览器（包括 Firefox 隐私浏览模式和 Tor 浏览器）存在一个隐私漏洞。该漏洞允许网站通过 IndexedDB `databases()` API 返回条目的顺序，推导出一个稳定的、进程作用域的标识符。只要 Firefox 进程保持运行，该标识符就会持续存在，从而将单个浏览器会话内的所有隐私浏览窗口和 Tor 身份链接起来。 该漏洞从根本上破坏了 Firefox 隐私浏览和 Tor 浏览器“新建身份”功能的隐私保证，使得那些自认为匿名的用户面临跨域追踪和指纹识别的风险。这标志着隐私关键应用程序在进程隔离方面存在重大缺陷，可能影响数百万依赖这些工具获取安全和匿名性的用户。 该漏洞是进程作用域的，而非源作用域，这意味着只要浏览器进程未重启，该标识符在不同的源（网站）和隐私窗口之间保持稳定。在 Tor 浏览器中，这破坏了“新建身份”功能在单个运行进程内预期的隔离性，使得网站能够链接本应完全分离的会话。

hackernews · danpinto · Apr 22, 17:35

**背景**: 浏览器指纹识别是一种追踪技术，通过收集浏览器和设备属性的组合（如屏幕分辨率、已安装字体和 API 行为）来为用户创建唯一标识符。IndexedDB 是一种 Web API，用于在用户浏览器中存储大量结构化数据。Tor 浏览器是一款注重隐私的网络浏览器，它通过 Tor 网络路由流量以匿名化用户的位置和使用情况，其“新建身份”功能旨在创建一个全新的、无法关联的浏览会话。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://fingerprint.com/blog/firefox-tor-indexeddb-privacy-vulnerability/">We Found a Stable Firefox Identifier Linking All Your Private Tor ...</a></li>
<li><a href="https://support.mozilla.org/en-US/kb/firefox-protection-against-fingerprinting">Firefox's protection against fingerprinting | Firefox Help Firefox is blocking more fingerprinting methods to improve ... We found a stable Firefox identifier linking all your private ... We found a stable Firefox identifier linking all your... Mozilla Firefox gets new anti-fingerprinting defenses Firefox 145 Brings Major Privacy Upgrade to Defend Against ...</a></li>
<li><a href="https://support.torproject.org/tor-browser/features/managing-identities/">Managing identities - Features - Tor Browser — Tor</a></li>

</ul>
</details>

**社区讨论**: 讨论围绕该漏洞的进程作用域性质展开了技术辩论，一位用户提到了 Mozilla 之前关于“每站点一进程”架构的工作，并质疑其为何未能防止此问题。另一位用户指出，该标识符在浏览器重启后不会持续存在，他们认为这降低了其对攻击者的实用性。此外，还讨论了指纹识别公司披露此漏洞的伦理问题，一些人对其动机表示惊讶和好奇。

**标签**: `#privacy`, `#security-vulnerability`, `#firefox`, `#tor`, `#fingerprinting`

---

<a id="item-4"></a>
## [Qwen3.6-27B：270 亿参数稠密模型实现旗舰级编程性能](https://qwen.ai/blog?id=qwen3.6-27b) ⭐️ 8.0/10

阿里通义千问团队开源了 Qwen3.6-27B 模型，这是一个拥有 270 亿参数的稠密语言模型，在 SWE-bench Verified 等核心编程基准测试中超越了其前代 3970 亿参数的 MoE 旗舰模型 Qwen3.5-397B-A17B，实现了旗舰级的编程性能。 这具有重要意义，因为它证明了一个相对小巧、高效的稠密模型可以匹配甚至超越更庞大、更复杂模型的编程能力，使得高性能的 AI 编程助手能够在消费级硬件上进行本地部署。它显著缩小了开源/本地模型与 Claude Opus 等顶级专有模型在实际编程任务上的性能差距。 该模型采用稠密架构，避免了混合专家模型的路由复杂性，从而简化了部署。据报道，经过量化后，它可以在拥有约 20-32GB 内存的硬件上高效运行，这使得许多使用现代消费级机器的开发者能够实际使用它。

hackernews · mfiguiere · Apr 22, 13:19

**背景**: 大语言模型主要有两种架构类型：稠密模型和混合专家模型。稠密模型对每个输入都使用其全部参数，而 MoE 模型对每个 token 只激活一部分专门的“专家”子集，旨在实现超大规模下的更高效率。一个 270 亿参数的模型被认为是中等规模，通常旨在为本地或高性价比的云端部署寻求性能与效率的平衡。旗舰级编程性能指的是在 SWE-bench 等基准测试中取得与现有最佳专有模型相竞争的结果。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://maximilian-schwarzmueller.com/articles/understanding-mixture-of-experts-moe-llms/">Mixture of Experts (MoE) vs Dense LLMs</a></li>
<li><a href="https://epoch.ai/gradient-updates/moe-vs-dense-models-inference">MoE vs AI dense models: How do they compare in inference? | Epoch AI</a></li>
<li><a href="https://www.morphllm.com/best-ai-model-for-coding">Best AI for Coding (2026): Every Model Ranked by Real Benchmarks</a></li>

</ul>
</details>

**社区讨论**: 社区参与度很高，注意到了该模型令人印象深刻的性能和实际效率。用户分享了在 M5 Pro Mac（32GB 内存）等硬件上本地运行的良好体验，认为对于大多数编程需求它都很有竞争力，同时也承认像 Opus 这样的顶级专有模型在可靠性上仍有优势。讨论还强调了开源模型与专有模型之间成本效益差距的缩小，一些人质疑闭源模型的长期竞争优势。

**标签**: `#llm`, `#open-source`, `#coding-assistant`, `#model-efficiency`, `#ai-hardware`

---

<a id="item-5"></a>
## [Mozilla 使用 Claude Mythos Preview 发现并修复了 Firefox 150 中的 271 个漏洞。](https://simonwillison.net/2026/Apr/22/bobby-holley/#atom-everything) ⭐️ 8.0/10

Mozilla 与 Anthropic 合作，将 Claude Mythos Preview AI 模型的早期版本应用于 Firefox 代码库，从而识别出 271 个漏洞。这些漏洞已在本周发布的 Firefox 150 中得到修复。 这展示了前沿 AI 模型在主动网络安全防御方面的重要实际应用，可能将平衡转向防御者一方。这表明 AI 可以成为组织在安全漏洞被利用之前，系统性地发现并修补它们的强大工具。 此次合作是 Mozilla 与 Anthropic 持续合作伙伴关系的一部分；之前使用 Claude Opus 4.6 的努力发现了 22 个漏洞。已修复的漏洞详情载于 Mozilla 安全公告 MFSA2026-30 中，且这项工作需要团队以 "不懈且专注" 的精神重新调整工作优先级。

rss · Simon Willison · Apr 22, 05:40

**背景**: Claude Mythos Preview 是 Anthropic 迄今为止能力最强的 AI 模型，旨在阅读、编写代码和进行研究。零日漏洞是攻击者可在开发者提供补丁之前利用的、先前未知的软件缺陷，因此特别危险。AI 辅助漏洞检测涉及使用大语言模型分析代码以寻找潜在的安全弱点，这种方法正变得越来越复杂。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www-cdn.anthropic.com/8b8380204f74670be75e81c820ca8dda846ab289.pdf">Claude Mythos Preview System Card - www-cdn.anthropic.com</a></li>
<li><a href="https://www.anthropic.com/news/mozilla-firefox-security">Partnering with Mozilla to improve Firefox’s security \ Anthropic</a></li>
<li><a href="https://en.wikipedia.org/wiki/Zero-day_vulnerability">Zero-day vulnerability - Wikipedia</a></li>

</ul>
</details>

**标签**: `#AI Security`, `#Vulnerability Detection`, `#Firefox`, `#Mozilla`, `#Anthropic`

---

<a id="item-6"></a>
## [腾讯与阿里巴巴洽谈投资 DeepSeek，估值超 200 亿美元](https://www.cls.cn/detail/2352468) ⭐️ 8.0/10

据报道，中国科技巨头腾讯控股和阿里巴巴集团正在洽谈投资人工智能初创公司 DeepSeek，该公司正寻求以超过 200 亿美元的估值进行融资。这是 DeepSeek 成立以来的首次重大融资活动。 这笔潜在投资标志着中国最大的科技公司为确保在快速演变的人工智能格局中的地位而采取的重大战略举措，可能加速与 OpenAI 等全球领先者的竞争。超过 200 亿美元的估值将立即使 DeepSeek 成为全球最有价值的人工智能初创公司之一，重塑全球人工智能投资格局。 此次洽谈涉及 DeepSeek 的首次融资轮，据报道该公司正寻求以超过 200 亿美元的估值筹集资金。DeepSeek 由中国对冲基金幻方量化所有，因其高效的模型训练方法而受到关注，据报道其训练成本仅为同类模型的十分之一。

telegram · zaihuapd · Apr 22, 12:23

**背景**: DeepSeek 是一家开发大型语言模型的中国人工智能公司。该公司在其应用程序登上下载排行榜榜首并于 2024 年 1 月发布最新模型 DeepSeek R1 后，在全球范围内成为头条新闻。DeepSeek 的旗舰 V3 模型采用混合专家架构，该架构通过仅为每个任务咨询相关的专家而非整个模型，从而实现更高效的处理。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/DeepSeek">DeepSeek - Wikipedia</a></li>
<li><a href="https://www.bbc.com/news/articles/c5yv5976z9po">What is DeepSeek - and why is everyone talking about it?</a></li>
<li><a href="https://medium.com/@ahdustechnology/technical-comparison-between-deepseek-chatgpt-llm-models-how-a-young-chinese-firm-developed-5c34aeb35089">Technical Comparison between DeepSeek & ChatGPT LLM Models ...</a></li>

</ul>
</details>

**标签**: `#artificial-intelligence`, `#venture-capital`, `#chinese-tech`, `#startups`, `#investment`

---

<a id="item-7"></a>
## [AI 编程助手'过度编辑'问题分析及提示策略探讨](https://nrehiew.github.io/blog/minimal_editing/) ⭐️ 7.0/10

一篇详细分析探讨了 AI 编程助手中的'过度编辑'现象，即模型对现有代码进行了超出请求所需的不必要修改。讨论包含了社区分享的用于缓解此问题的提示策略，并探讨了进行最小化更改与改进代码质量之间的权衡。 这很重要，因为过度编辑会引入不必要的复杂性、破坏现有功能并降低开发人员对 AI 工具的信任，直接影响生产力和代码库的稳定性。由于编码被广泛认为是生成式 AI 的关键应用场景，理解并控制这种行为对于这些助手在实际软件开发中的有效采用至关重要。 讨论中提到的一个关键提示策略是明确指示模型进行'最小化更改'，并精确指定要添加或修改的内容，同时声明哪些部分应保持不变。分析表明，过度编辑的倾向可能与模型被训练来生成'完整'或'改进'解决方案的方式有关，这可能与在成熟代码库中进行精准、保持上下文的编辑需求相冲突。

hackernews · pella · Apr 22, 17:51

**背景**: AI 编程助手，如 Claude Code 和 Gemini Code Assist，是集成到开发环境中的生成式 AI 工具，用于帮助完成代码生成、解释和修改等任务。提示工程涉及设计具体的指令来引导这些 AI 模型产生期望的输出，是有效使用的关键技能。讨论的核心挑战在于平衡 AI 重构和改进代码的能力与它对现有工作代码进行不稳定、不必要修改的风险。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://hackr.io/blog/ai-coding-assistants">7 Best AI Coding Assistants In 2026 [Free + Paid]</a></li>
<li><a href="https://www.promptingguide.ai/applications/coding">Generating Code | Prompt Engineering Guide</a></li>
<li><a href="https://medium.com/no-time/antigravity-vs-claude-code-which-ai-coding-assistant-should-you-actually-use-8337d9233582">Antigravity vs Claude Code : Which AI Coding Assistant ... | Medium</a></li>

</ul>
</details>

**社区讨论**: 开发者的情绪是复杂的，反映了不同的工作流程和项目背景。一些用户（如 hathawsh）表示高度满意，他们将过度编辑视为可纠正的错误，并使用项目特定的'技能'文件供 AI 学习。另一些用户（如 jstanley）则认为助手可能过于保守，有时更需要积极的改进，尤其是在新项目中。包括 rcvassallo83 在内的几位评论者分享了实用的提示技巧，例如指定"添加一个函数……其他保持不变"，以成功限制修改范围。

**标签**: `#AI-coding-assistants`, `#software-engineering`, `#prompt-engineering`, `#developer-tools`

---

<a id="item-8"></a>
## [GitHub Copilot 个人版计划调整：限制收紧、暂停注册、Claude Opus 分级访问。](https://simonwillison.net/2026/Apr/22/changes-to-github-copilot/#atom-everything) ⭐️ 7.0/10

GitHub 宣布对其 Copilot 个人版计划进行重大调整，包括收紧使用限制、暂停个人版新用户注册，并将最新的 Claude Opus 4.7 模型访问权限限制在更昂贵的 39 美元/月的 "Pro+" 套餐中，同时取消了旧版 Opus 模型。这些调整是由于智能体工作流带来的计算需求激增，并且计费模式从按请求计费转向了基于令牌的使用限制系统。 此次公告标志着 AI 辅助开发经济模式的一次重大转变，高级编码智能体的高昂计算成本正迫使平台提供商重构定价策略。这将影响数百万依赖 Copilot 进行日常编码的开发者，并可能影响其他 AI 编码工具供应商设计其定价和资源分配模式。 此次调整具体涉及包含 CLI、云端智能体、GitHub.com 上的代码审查功能以及 VS Code、Zed 和 JetBrains 等 IDE 集成的 GitHub Copilot 产品。新的基于令牌的限制同时适用于单次会话和每周总量，旨在解决消耗大量令牌的单个智能体请求所带来的利润压力。

rss · Simon Willison · Apr 22, 03:30

**背景**: GitHub Copilot 是由 GitHub 开发、基于 OpenAI 模型的广泛使用的 AI 代码补全和辅助工具。智能体工作流指的是能够自主执行复杂、多步骤开发任务（如代码审查或依赖管理）以响应事件的 AI 系统，而不仅仅是响应用户提示。Claude Opus 是 Anthropic 最先进的大语言模型，Opus 4.7 是其最新版本，具有 100 万令牌的上下文窗口和高分辨率图像支持功能。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.deployhq.com/blog/agentic-workflows-explained-ai-agents-cicd-pipelines">Agentic Workflows Explained: How AI Agents Are Changing CI/CD ...</a></li>
<li><a href="https://platform.claude.com/docs/en/about-claude/models/whats-new-claude-4-7">What's new in Claude Opus 4.7 - Claude API Docs</a></li>

</ul>
</details>

**标签**: `#github-copilot`, `#ai-coding-assistants`, `#pricing-changes`, `#developer-tools`, `#anthropic-claude`

---

<a id="item-9"></a>
## [长江存储一季度收入超 200 亿元，加速扩产拟实现产能翻番](https://www.guancha.cn/economy/2026_04_20_814211.shtml) ⭐️ 7.0/10

长江存储（YMTC）2026 年第一季度收入突破 200 亿元人民币，同比翻倍，其全球 NAND 闪存市场份额已超过 10%。公司正加速产能扩张，武汉三期晶圆厂预计年内投产，并计划新建两座晶圆厂，目标是将总产能提升一倍以上，单厂月产能达 10 万片。 这一快速增长和雄心勃勃的扩张计划标志着 YMTC 在全球存储市场的地位正在加强，可能对美光等现有厂商构成挑战。其新产线国产设备占比首次突破 50%，也标志着中国在推动半导体供应链自主化、减少对外国技术依赖方面取得了显著进展。 长江存储三期产线的国产设备占比首次突破 50%，这一供应链自主化程度显著优于行业平均水平。与此同时，国产 DRAM 主要生产商长鑫存储（CXMT）2025 年前三季度收入也接近翻倍，并拟募资 295 亿元用于扩产。

telegram · zaihuapd · Apr 22, 06:18

**背景**: 长江存储（YMTC）是一家中国半导体制造商，2016 年成立于武汉，专注于 NAND 闪存芯片的制造，这是固态硬盘（SSD）和智能手机等设备中用于数据存储的关键部件。NAND 闪存是一种断电后仍能保留数据的非易失性存储器，全球市场主要由三星、铠侠、西部数据和 SK 海力士等公司主导。中国一直通过政策和投资积极追求半导体自主化，近期有政策要求芯片制造商新增产能中至少使用 50%的国产设备。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Yangtze_Memory_Technologies">Yangtze Memory Technologies - Wikipedia</a></li>
<li><a href="https://www.astutegroup.com/news/general/china-accelerates-semiconductor-self-sufficiency-with-mandatory-local-equipment-use/">China accelerates semiconductor self-sufficiency with mandatory local equipment use - Astute Group</a></li>

</ul>
</details>

**标签**: `#semiconductors`, `#supply-chain`, `#china-tech`, `#manufacturing`, `#memory`

---

<a id="item-10"></a>
## [特斯拉中国车机语音服务将接入字节跳动豆包大模型](https://www.chinastarmarket.cn/detail/2351905) ⭐️ 7.0/10

特斯拉中国的车载语音大模型服务于 4 月 20 日完成备案，其车机语音服务将接入字节跳动的豆包大模型。此前特斯拉中国官网披露，Model Y L 车型将搭载豆包大模型和 DeepSeek 模型，两者均通过火山引擎平台接入。 这标志着特斯拉在中国市场的重要本土化战略，通过与国内领先的 AI 提供商合作，在遵守本地法规的同时提升车辆智能化水平。这种集成展示了汽车制造商如何越来越多地为不同的车内功能采用专门的 AI 模型，可能为其他在中国运营的国际汽车制造商树立趋势。 豆包大模型将专门负责语音命令，包括导航设置、媒体播放控制、空调调节和车主手册查询，而 DeepSeek 模型则提供更广泛的 AI 互动服务。两个模型都通过字节跳动的火山引擎平台接入，该平台作为云和 AI 服务平台，将特斯拉车辆与这些中国 AI 系统连接起来。

telegram · zaihuapd · Apr 22, 06:53

**背景**: 豆包是字节跳动自主研发的大语言模型，已通过 50 多个内部业务场景验证，每日处理千亿级 tokens。DeepSeek 是一家专注于大语言模型开发的中国 AI 公司，以其深度分析能力而闻名。火山引擎是字节跳动旗下的云与 AI 服务平台，为企业提供 AI 转型服务，包括模型部署和智能体开发。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.volcengine.com/product/doubao-dy">豆包大模型-火山引擎</a></li>
<li><a href="https://en.wikipedia.org/wiki/DeepSeek">DeepSeek - Wikipedia</a></li>
<li><a href="https://www.volcengine.com/">volcengine.com - 火山引擎-你的AI云</a></li>

</ul>
</details>

**标签**: `#automotive-ai`, `#voice-assistants`, `#china-tech`, `#tesla`, `#llm-integration`

---

<a id="item-11"></a>
## [FBI 从 iPhone 通知数据库提取已删除 Signal 消息，案件发生在得州](https://t.me/zaihuapd/41013) ⭐️ 7.0/10

在得克萨斯州 Prairieland 拘留中心的一起案件庭审中，FBI 通过访问嫌疑人 iPhone 的系统通知数据库，提取出了已从 Signal 应用中删除的传入消息。证词和庭审记录显示，只恢复了传入消息，没有传出消息。 这揭示了一个重大的隐私漏洞：被认为已消失或删除的加密消息，可能持久保存在一个系统级数据库中，并可被取证工具访问。它影响了用户对安全通讯应用的隐私期望，并突显了一种适用于任何开启了锁屏预览功能应用的取证技术。 之所以能够恢复，是因为 iOS 系统（而非 Signal 应用本身）会生成锁屏通知预览并将其存储在一个内部数据库中。据报道，即使 Signal 应用被卸载，该技术仍然有效，但仅限于已显示过预览的传入消息。

telegram · zaihuapd · Apr 22, 23:10

**背景**: Signal 是一款流行的端到端加密通讯应用，以用户隐私为首要考虑。在 iPhone 上，当通知到达时，iOS 操作系统会生成消息内容的预览以显示在锁屏上。这些预览存储在一个由系统管理的通知数据库中，该数据库与应用自身的加密存储是分开的，这正是本次取证发现的焦点。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://9to5mac.com/2026/04/09/fbi-used-iphone-notification-data-to-retrieve-deleted-signal-messages/">FBI used iPhone notification data to retrieve deleted Signal ...</a></li>
<li><a href="https://cybernews.ae/fbi-recovers-deleted-signal-messages-via-iphone-notifications/">FBI recovers deleted Signal messages via iPhone notifications</a></li>
<li><a href="https://www.macobserver.com/news/fbi-finds-deleted-signal-messages-on-iphone-via-notification-storage-heres-how-to-protect-your-privacy/">FBI Finds Deleted Signal Messages on iPhone via Notification ...</a></li>

</ul>
</details>

**标签**: `#digital-forensics`, `#privacy`, `#encryption`, `#iOS`, `#Signal`

---

<a id="item-12"></a>
## [法国国家安全证件署（ANTS）确认发生数据泄露，或影响 1900 万公民。](https://techcrunch.com/2026/04/22/france-confirms-data-breach-at-government-agency-that-manages-citizens-ids/) ⭐️ 7.0/10

法国负责管理身份证、护照及移民文件的国家安全证件署（ANTS）确认发生数据泄露，该机构于 4 月 15 日监测到攻击。已有黑客在论坛声称持有包含 1900 万条记录的数据库，被盗数据涵盖公民姓名、出生日期、出生地、联系地址及电话等个人隐私信息。 此次泄露事件影响重大，因为 ANTS 是核心的政府身份管理系统，被暴露的个人信息高度敏感，对数百万公民构成身份盗窃和欺诈的重大风险。这也对负责公民身份识别的关键国家基础设施的安全态势提出了严重质疑。 官方尚未公布受影响的具体人数，对攻击原因及影响范围的调查仍在进行中。作为应对程序的一部分，ANTS 已开始通知可能受影响的公民。

telegram · zaihuapd · Apr 23, 00:08

**背景**: 法国国家安全证件署（ANTS）是一个政府机构，负责管理车辆注册、驾驶执照以及护照和国民身份证等安全身份证件的在线申请流程。像 ANTS 运营的这类身份和访问管理（IAM）系统是关键基础设施，它们集中管理大量人口的身份数据，因此成为网络攻击的高价值目标。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://ants.gouv.fr/">Accueil - France Titres (ANTS)</a></li>
<li><a href="https://www.bleepingcomputer.com/news/security/french-govt-agency-confirms-breach-as-hacker-offers-to-sell-data/">French govt agency confirms breach as hacker offers to sell data</a></li>

</ul>
</details>

**标签**: `#cybersecurity`, `#data-breach`, `#privacy`, `#government`, `#identity-management`

---