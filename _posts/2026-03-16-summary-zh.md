---
layout: default
title: "Horizon Summary: 2026-03-16 (ZH)"
date: 2026-03-16
lang: zh
---

> From 28 items, 11 important content pieces were selected

---

1. [加拿大 C-22 号法案提议扩大执法部门无需授权令即可获取数字元数据的权限。](#item-1) ⭐️ 8.0/10
2. [Chrome DevTools 集成 Model Context Protocol，支持 AI 驱动浏览器调试](#item-2) ⭐️ 8.0/10
3. [华虹集团旗下华力微电子拟量产 7 纳米芯片，或成中国第二家掌握该技术的厂商。](#item-3) ⭐️ 8.0/10
4. [月之暗面发布 Attention Residuals 技术，48B 模型训练效率提升至 1.25 倍](#item-4) ⭐️ 8.0/10
5. [阿里通义实验室开源影视级配音大模型 Fun-CineForge，首次引入时间模态](#item-5) ⭐️ 8.0/10
6. [一份详细指南：如何将 LLM 作为架构师、开发者和评审员来编写软件。](#item-6) ⭐️ 7.0/10
7. [分析揭示新闻网页达 49MB，因广告脚本产生 422 个网络请求](#item-7) ⭐️ 7.0/10
8. [编码代理如何作为 LLM 的“缰绳”，通过隐形提示和可调用工具工作](#item-8) ⭐️ 7.0/10
9. [Simon Willison 将 'Agentic Engineering' 定义为使用 Coding Agents 开发软件](#item-9) ⭐️ 7.0/10
10. [鸿海四季度利润不及预期，引发 AI 需求担忧](#item-10) ⭐️ 7.0/10
11. [阿里巴巴推行全面'AI 化'战略，将 2025 年绩效与 AI 驱动增长挂钩。](#item-11) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [加拿大 C-22 号法案提议扩大执法部门无需授权令即可获取数字元数据的权限。](https://www.michaelgeist.ca/2026/03/a-tale-of-two-bills-lawful-access-returns-with-changes-to-warrantless-access-but-dangerous-backdoor-surveillance-risks-remains/) ⭐️ 8.0/10

加拿大政府提出了 C-22 号法案，旨在更新合法访问法律，赋予警察和安全机构更快、更明确地获取数字数据的权限，这些数据包括来自电信和在线服务提供商的用户信息、传输数据和追踪数据。该法案还建立了一个要求电子服务提供商支持此类访问请求的框架。 这项立法意义重大，因为它扩大了无需授权令的监控范围，允许执法部门在没有司法监督的情况下访问大量元数据，可能影响所有加拿大人的隐私。它引发了关于数字时代国家安全与公民自由之间平衡的关键问题。 该法案中一个值得注意的条款是，如果法官认为理由正当，可以免除向相关人员提供授权令副本的要求，这为通知义务创造了一个潜在的例外。该法案还旨在强制外国公司和服务提供商遵守加拿大的数据访问请求。

hackernews · opengrass · Mar 15, 21:22

**背景**: 数字元数据指的是关于通信的信息，例如通话或信息的时间、时长、发送者和接收者，但不包括其实际内容。在许多法律框架中，包括美国的第三方原则，与服务提供商共享的元数据历史上受到的保护比内容要少，这使其成为执法部门收集的目标。像 C-22 这样的法案通常被称为“合法访问”立法，旨在使法律适应数字时代，这一过程受到过去关于大规模监控披露的影响。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.cbc.ca/news/politics/lawfull-access-legislation-liberal-9.7125891">New lawful access bill would give police, CSIS more powers to ...</a></li>
<li><a href="https://docs.reclaimthenet.org/canada-bill-c-22-lawful-access-act-2026.pdf">Bill C-22 451 An Act respecting lawful access | Projet de loi ...</a></li>
<li><a href="https://www.numberanalytics.com/blog/metadata-surveillance-guide">Metadata Surveillance Guide - numberanalytics.com</a></li>

</ul>
</details>

**社区讨论**: 社区评论表达了对隐私和民主规范受到侵蚀的强烈担忧，一些人将该法案比作奥威尔式的监控。一位用户指出了法案中一个具体的、可能存在问题例外条款，该条款允许法官免除提供授权令副本的要求。其他人则将这个问题置于更广泛的地缘政治紧张局势和 perceived 的国家监控加强的全球趋势中，质疑外国影响和国际联盟的未来。

**标签**: `#privacy`, `#surveillance`, `#legislation`, `#civil-liberties`, `#canada`

---

<a id="item-2"></a>
## [Chrome DevTools 集成 Model Context Protocol，支持 AI 驱动浏览器调试](https://developer.chrome.com/blog/chrome-devtools-mcp-debug-your-browser-session) ⭐️ 8.0/10

Chrome DevTools 团队宣布集成 Model Context Protocol (MCP)，使 AI 代理能够以编程方式调试和控制浏览器会话。这包括在 chrome-devtools-mcp 项目的 v0.20.0 版本中最新发布的独立 CLI 工具。 这项集成意义重大，因为它标准化了 AI 代理与浏览器调试工具的交互方式，有望自动化复杂的 Web 测试、监控和交互任务。这标志着在让 AI 驱动的工作流更易于进行浏览器自动化方面迈出了一大步，并可能加速自动化质量保证和网络抓取等领域的发展。 一个关键细节是该项目现在包含一个独立的 CLI，这有助于缓解人们对通过某些 AI 助手使用 MCP 所产生的高令牌成本的担忧。同样值得注意的是，通过 Chrome DevTools Protocol (CDP) 让 AI 代理控制浏览器的类似功能已在社区项目（例如 'chrome-cdp-skill'）中存在。

hackernews · xnx · Mar 15, 19:12

**背景**: Chrome DevTools 是直接内置于 Google Chrome 浏览器中的一套 Web 开发者工具，用于调试、性能分析和编辑网页。Model Context Protocol (MCP) 是 Anthropic 于 2024 年底推出的一个开放标准，旨在标准化像 LLM 这样的 AI 系统与外部工具和数据源的连接方式。面向 AI 代理的浏览器自动化是一个不断发展的领域，其中的工具允许 AI 模型以编程方式控制 Web 浏览器来执行数据提取或交互等任务。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Model_Context_Protocol">Model Context Protocol - Wikipedia</a></li>
<li><a href="https://developer.chrome.com/docs/devtools">Chrome DevTools | Chrome for Developers</a></li>

</ul>
</details>

**社区讨论**: 社区讨论呈现出兴奋与批评并存的状态。开发者们分享了实际用例，例如使用类似工具与 Claude 配合来自动化与 YouTube Music 等网站的交互。人们对 MCP 相关的高令牌成本表示明显担忧，而新的 CLI 被视为一种潜在的缓解方案。一些评论者还指出，许多 MCP 实现只是简单的封装，不过设计良好的实现能提供安全优势。

**标签**: `#devtools`, `#browser-automation`, `#ai-agents`, `#mcp`, `#web-development`

---

<a id="item-3"></a>
## [华虹集团旗下华力微电子拟量产 7 纳米芯片，或成中国第二家掌握该技术的厂商。](https://www.reuters.com/world/asia-pacific/chinas-no-2-chipmaker-readies-7-nm-production-beijing-ramps-up-self-suffiency-2026-03-16/) ⭐️ 8.0/10

华虹集团旗下的华力微电子已开发出可用于人工智能芯片的先进制造技术，目前正准备在其上海工厂量产 7 纳米芯片。若消息属实，华虹将成为继中芯国际之后，中国第二家具备 7 纳米芯片生产能力的代工厂。 这一进展是中国推动半导体自给自足过程中的一个重要里程碑，有助于减少对国外先进芯片制造技术的依赖。它将使国内能够生产更强大的人工智能和计算芯片，对全球科技供应链和半导体产业的地缘政治格局产生影响。 据悉，华为已与华虹就该技术展开合作，国内设备供应商昇维旭也提供了相关支持。华力微电子计划在今年年底前实现每月数千片晶圆的 7 纳米初始产能，并设定了后续扩产目标。

telegram · zaihuapd · Mar 16, 06:50

**背景**: 7 纳米（nm）工艺节点是一种先进的半导体制造技术，能够制造出更小、更快、更节能的芯片，对于高性能计算和人工智能应用至关重要。在晶圆代工（Foundry）模式下，像华虹这样的公司专门为其他“无晶圆厂”（Fabless）半导体公司制造芯片。中芯国际（SMIC）是中国目前领先的晶圆代工厂，也是国内首家实现 7 纳米生产能力的厂商。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.edn.com/smic-at-7-nm-semiconductor-process-node-a-shanghai-surprise/">SMIC at 7 - nm semiconductor process node : A Shanghai... - EDN</a></li>
<li><a href="https://en.wikipedia.org/wiki/Foundry_model">Foundry model - Wikipedia</a></li>

</ul>
</details>

**标签**: `#semiconductors`, `#manufacturing`, `#china-tech`, `#ai-hardware`, `#geopolitics`

---

<a id="item-4"></a>
## [月之暗面发布 Attention Residuals 技术，48B 模型训练效率提升至 1.25 倍](https://github.com/MoonshotAI/Attention-Residuals/blob/master/Attention_Residuals.pdf) ⭐️ 8.0/10

月之暗面（Moonshot AI）推出了 Attention Residuals 技术，这是一种对 Transformer 架构的改进，使每一层能够选择性地关注此前各层的输出，而非统一求和。该技术已应用于其 480 亿参数的 Kimi Linear 模型，在达到相同性能时所需算力比基线减少约 20%，同时在 GPQA-Diamond 推理基准上提升了 7.5 分。 这项技术之所以重要，是因为它为大型语言模型提供了一条更高效的训练路径，有可能降低开发尖端 AI 所需的海量计算成本。通过改进信息在层间的流动方式，它可能催生出能力更强且训练成本更低的模型，这对于 AI 系统的可持续扩展至关重要。 据论文介绍，该技术的训练额外开销低于 4%，推理延迟增加不超过 2%。该技术还通过改善梯度流，缓解了'PreNorm 稀释'问题。值得注意的是，前 OpenAI 研究科学家 Andrej Karpathy 对此给予了正面评价，称其更字面地践行了'Attention is All You Need'的理念。

telegram · zaihuapd · Mar 16, 09:05

**背景**: Transformer 架构是大多数现代大型语言模型的基础，其核心思想源自论文《Attention is All You Need》。在标准的 Transformer 中，每一层的输出通常通过简单的残差连接（相加）与前面层的输出结合。Attention Residuals 对此进行了改进，它允许模型的注意力机制动态决定'关注'或整合来自任何先前层的信息的程度，从而创建了一条更灵活、可能更强大的信息通路。GPQA-Diamond 基准是 GPQA 数据集中一个极具挑战性的子集，包含 198 个问题，即使是博士专家在该测试上的准确率也只有 65%，因此它是检验高级推理能力的严格测试。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://nerdschalk.com/moonshot-ais-attention-residuals-for-kimi-could-change-how-ai-models-use-layers/">Moonshot AI’s Attention Residuals for Kimi Could Change How AI Models Use Layers</a></li>
<li><a href="https://artificialanalysis.ai/evaluations/gpqa-diamond">GPQA Diamond Benchmark Leaderboard - Artificial Analysis</a></li>

</ul>
</details>

**标签**: `#transformer-architecture`, `#model-efficiency`, `#large-language-models`, `#attention-mechanism`, `#ai-research`

---

<a id="item-5"></a>
## [阿里通义实验室开源影视级配音大模型 Fun-CineForge，首次引入时间模态](https://mp.weixin.qq.com/s/MylZJGEYgYiBS6fq53v2XQ) ⭐️ 8.0/10

阿里通义实验室发布并开源了首个支持影视级多场景配音的多模态大模型 Fun-CineForge。该模型的核心创新在于首次将“时间模态”引入配音模型，使其在说话人面部缺失等复杂场景下仍可实现音画同步，并在独白场景的对比测试中，在词错率、唇部同步等多个指标上超越了 DeepDubber-V1 和 InstructDubber。 这项发布意义重大，因为它通过引入专门的时间模态，解决了自动视频配音中保持精确口型同步和时间对齐的关键挑战。作为一个来自主要实验室的开源模型，它有望降低媒体制作、本地化和内容创作领域实现高质量自动配音的门槛，可能对影视、广告和在线视频等行业产生影响。 该模型基于 CosyVoice3 语音合成底层能力构建，当前支持对 30 秒以内的视频片段进行推理，适用于独白、旁白、对话及多说话人等多种影视配音场景。模型已在 GitHub、HuggingFace 及 ModelScope 三平台同步开源。

telegram · zaihuapd · Mar 16, 11:20

**背景**: 多模态 AI 模型旨在单一架构内理解和生成跨不同感官输入（如文本、图像、音频和视频）的内容。视频配音模型的具体目标是合成与视频中角色口型动作和时间相匹配的语音，这项任务要求音频流和视频流之间的精确对齐。CosyVoice3 是一个基于大语言模型的先进文本转语音系统，以其在说话人相似度和韵律自然度上相对于前代模型的改进而闻名。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://blog.gopenai.com/from-sora-to-imagebind-how-7-multi-modal-ai-models-are-quietly-replacing-5m-creative-teams-026a11b9fb91">From Sora to ImageBind: How 7 Multi- Modal AI Models Are... | GoPenAI</a></li>
<li><a href="https://funaudiollm.github.io/cosyvoice3/">CosyVoice3.0</a></li>

</ul>
</details>

**标签**: `#speech-synthesis`, `#multimodal-ai`, `#video-dubbing`, `#open-source`, `#time-modality`

---

<a id="item-6"></a>
## [一份详细指南：如何将 LLM 作为架构师、开发者和评审员来编写软件。](https://www.stavros.io/posts/how-i-write-software-with-llms/) ⭐️ 7.0/10

作者发布了一份实用指南，详细介绍了其使用大语言模型（LLM）编写软件的具体工作流程，该流程为不同模型分配了不同的角色（架构师、开发者、评审员），并为每个阶段采用了针对性的提示工程技术。 这很重要，因为它提供了一个结构化、可重复的框架，超越了简单的代码生成，旨在提高 AI 辅助开发的质量和可靠性，因为这些工具正成为现代软件工程不可或缺的一部分。 该工作流程明确为不同角色使用不同的模型，例如使用 Claude 3.5 Sonnet 进行架构设计，使用 GPT-4 进行开发，并强调了对 AI 生成代码进行人工监督和严格评审的重要性。

hackernews · indigodaddy · Mar 16, 01:24

**背景**: LLM 辅助编程涉及使用像 GPT-4 或 Claude 这样的大语言模型作为生成、解释或评审代码的工具。提示工程是指设计输入（提示词）来引导这些模型产生期望输出的实践，其中角色扮演（例如“扮演一名高级架构师”）是常用技术。有效使用需要清晰的方向和上下文，将 LLM 更多地视为一个强大的结对编程伙伴，而非自主代理。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://medium.com/@addyosmani/my-llm-coding-workflow-going-into-2026-52fe1681325e">My LLM coding workflow going into 2026 | by Addy Osmani | Medium</a></li>
<li><a href="https://en.wikipedia.org/wiki/Prompt_engineering">Prompt engineering - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: 社区讨论揭示了不同的观点。一些人质疑多角色流程的必要性，认为不如使用一个强大的模型并给予清晰指令。另一些人则对可能存在的开源代码许可证被“洗白”的伦理问题表示担忧，尤其是对于闭源产品。还有评论指出，结果的质量可能更依赖于评审者的经验，而非提示词的“技巧”。

**标签**: `#llm-programming`, `#developer-workflow`, `#ai-tools`, `#prompt-engineering`, `#software-development`

---

<a id="item-7"></a>
## [分析揭示新闻网页达 49MB，因广告脚本产生 422 个网络请求](https://thatshubham.com/blog/news-audit) ⭐️ 7.0/10

一项针对新闻网页的技术审计显示，该页面通过 422 个网络请求加载了 49MB 数据，主要原因是广告和追踪脚本通过 Google Tag Manager 等工具被添加。分析表明，非技术人员如何逐步添加脚本，在没有开发者监督的情况下造成严重的性能膨胀。 这个案例体现了系统性网页性能退化问题，尤其影响移动设备和较慢网络连接的用户体验，同时揭示了业务对追踪和广告的需求如何与性能目标直接冲突。它提出了现代网页开发中责任与治理的重要问题，即营销工具如何绕过工程监督。 作者指出，当分析报告广泛传播时，Cloudflare 的边缘缓存处理了 19.24GB 流量，缓存命中率达 98.5%，避免了服务器过载。审计特别指出标签管理系统是脚本不受控制扩散的主要入口，非技术用户可以直接向生产环境添加追踪脚本而无需开发者审核。

hackernews · kermatt · Mar 15, 19:25

**背景**: 网页性能优化专注于通过减少网络请求、压缩资源、优化渲染等技术来缩短页面加载时间。广告和追踪脚本是添加到网页中的 JavaScript 代码片段，用于收集用户数据、衡量转化率和投放定向广告，但它们经常会产生额外的 HTTP 请求，从而拖慢页面加载。网络请求瀑布图可视化这些请求的顺序和持续时间，帮助识别脚本延迟页面渲染的性能瓶颈。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.debugbear.com/docs/waterfall">How to Read a Request Waterfall Chart | DebugBear</a></li>
<li><a href="https://sopriza.com/delaying-gtm-4-tracking-script-impact/">Delaying Gtm 4 Tracking Script Impact – Sopriza</a></li>

</ul>
</details>

**社区讨论**: 社区讨论强调，开发者通常只实现初始的标签管理器脚本，而非技术人员随后会添加大量追踪脚本而不考虑性能影响。几位评论者指出，像 Pi-hole 这样的 DNS 级屏蔽工具对于获得干净浏览体验变得必要，这实际上将性能优化的负担从发布者转移到了终端用户。讨论还透露了对《纽约时报》等新闻网站因页面膨胀而变得难以使用的沮丧，一些用户已完全放弃这些网站。

**标签**: `#web-performance`, `#advertising`, `#tracking`, `#developer-practices`, `#network-optimization`

---

<a id="item-8"></a>
## [编码代理如何作为 LLM 的“缰绳”，通过隐形提示和可调用工具工作](https://simonwillison.net/guides/agentic-engineering-patterns/how-coding-agents-work/#atom-everything) ⭐️ 7.0/10

Simon Willison 发布了一份详细指南，解释了编码代理是大型语言模型（LLM）的软件“缰绳”，通过隐形提示和可调用工具来扩展其能力。该指南分解了核心组件，包括 LLM 如何处理 token、如何使用聊天模板提示来模拟对话，以及“缰绳”在管理状态和执行工具方面的作用。 理解编码代理的架构对于开发者和工程师有效构建、部署和调试 AI 驱动的软件系统至关重要。随着“代理式工程”成为主流的开发范式，掌握这些基础模式有助于在工具选择、成本管理和系统设计方面做出明智的决策。 该指南阐明，LLM 是无状态的，并且处理的是 token 而非单词，这直接影响成本和上下文长度限制。它还强调，是代理“缰绳”（而非 LLM 本身）负责维护对话状态、执行工具以及处理引导代理行为的隐形系统提示。

rss · Simon Willison · Mar 16, 14:01

**背景**: 像 GPT-4 和 Claude 这样的大型语言模型（LLM）是预测序列中下一个 token 的机器学习模型，使它们能够生成文本和代码。“代理缰绳”是管理 LLM 与外部世界交互的周边软件基础设施，处理工具执行、记忆和状态持久化等 LLM 自身无法完成的任务。“隐形提示”指的是“缰绳”在用户可见输入之前添加的系统指令或上下文，用于在用户不知情的情况下引导 LLM 的行为。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.firecrawl.dev/blog/what-is-an-agent-harness">What Is an Agent Harness ? The Infrastructure That Makes AI Agents...</a></li>
<li><a href="https://simonwillison.net/2026/Feb/23/agentic-engineering-patterns/">Writing about Agentic Engineering Patterns | Simon Willison’s Weblog</a></li>

</ul>
</details>

**标签**: `#AI Agents`, `#LLM`, `#Software Engineering`, `#AI Development`, `#Technical Explanation`

---

<a id="item-9"></a>
## [Simon Willison 将 'Agentic Engineering' 定义为使用 Coding Agents 开发软件](https://simonwillison.net/guides/agentic-engineering-patterns/what-is-agentic-engineering/#atom-everything) ⭐️ 7.0/10

Simon Willison 发布了一份指南，将 'agentic engineering' 定义为在 coding agents 的辅助下开发软件的实践，这些 AI agents 能够以循环方式编写和执行代码以实现目标。他通过强调人类在提供工具、明确问题和验证结果方面的作用，将这一概念与 'vibe coding' 区分开来。 这很重要，因为它为 AI 辅助软件开发这一新兴范式建立了一个正式的框架和术语体系，超越了简单的代码生成，转向一个更具协作性和迭代性的过程。它强调了软件工程师角色的转变：从编写代码转向编排和指导 AI agents，以更雄心勃勃、更有效地解决复杂问题。 Willison 的定义关键在于 agent 执行代码的能力，他认为这是实现迭代改进和产出可验证工作软件的核心能力。他指出，此类 coding agents 的流行示例包括 Claude Code、OpenAI Codex 和 Gemini CLI。

rss · Simon Willison · Mar 15, 22:41

**背景**: 在大型语言模型（LLM）的语境中，'agent' 通常被定义为一种软件：它使用提示词和一组工具定义来调用 LLM，然后执行 LLM 请求的任何工具，并将结果反馈回循环中以实现目标。这与传统的聊天机器人或自动化工具不同，后者遵循预定义的脚本或规则，缺乏自主适应和推理多步骤任务的能力。Coding agents 是 LLM agent 的一种特定类型，其可用工具中包含代码执行功能。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://simonwillison.net/guides/agentic-engineering-patterns/">Agentic Engineering Patterns - Simon Willison's Weblog</a></li>
<li><a href="https://www.atscale.com/glossary/llm-agents/">What is an LLM Agent ? Definition, Examples | AtScale</a></li>

</ul>
</details>

**标签**: `#AI-assisted-development`, `#software-engineering`, `#LLM-agents`, `#coding-agents`

---

<a id="item-10"></a>
## [鸿海四季度利润不及预期，引发 AI 需求担忧](https://www.bloomberg.com/news/articles/2026-03-16/nvidia-partner-hon-hai-s-profit-miss-raises-ai-demand-fears?srnd=phx-technology) ⭐️ 7.0/10

作为英伟达 AI 服务器的核心组装商，鸿海精密（富士康）最新披露的财报利润意外低于预期。去年 12 月的季度净利润为新台币 452 亿元，同比下滑 2.4%，远低于分析师平均预期的新台币 599 亿元。 作为 AI 硬件供应链的关键一环，鸿海的业绩爆冷引发了投资者对 AI 算力硬件爆炸性需求是否已见顶的担忧。这让人质疑，科技巨头们数千亿美元的巨额投入，能否顺利转化为整个产业链的实质性利润。 这份财报凸显了科技巨头高昂的资本支出（今年在 AI 领域投入超 6500 亿美元）与硬件供应链即时盈利能力之间可能存在的脱节。作为 AI 基础设施需求的关键风向标，鸿海的业绩被视为观察行业健康状况的重要先行指标。

telegram · zaihuapd · Mar 16, 12:50

**背景**: AI 服务器是用于训练和运行大型 AI 模型的高性能计算机。英伟达等公司设计关键的 GPU 芯片，而鸿海（富士康）这类合同制造商则负责组装完整的服务器系统。此前的 AI 硬件热潮由云服务和科技公司为构建算力基础设施而进行的大规模投资所驱动。目前，行业正密切关注市场是否正从初期的“抢卡圈地、拼硬件规模”阶段，转向注重运营效率和投资回报的下半场。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://xueqiu.com/1994378695/378836099">算力下半场投资逻辑 算力下半场投资逻辑算力投资已从上半场的抢卡圈地...</a></li>
<li><a href="https://xueqiu.com/6704595592/347315189">鸿海集团与英伟达合作及旗下公司分工布局 首先鸿海集团有两个子公司，...</a></li>

</ul>
</details>

**标签**: `#AI Hardware`, `#Market Analysis`, `#Supply Chain`, `#Investment`, `#Nvidia`

---

<a id="item-11"></a>
## [阿里巴巴推行全面'AI 化'战略，将 2025 年绩效与 AI 驱动增长挂钩。](https://t.me/zaihuapd/40303) ⭐️ 7.0/10

阿里巴巴 CEO 吴泳铭已下令在全公司推行'AI 化'转型，所有部门 2025 年的绩效评估都将与其利用 AI 驱动增长的效果挂钩。公司还在开发一系列新的 AI 原生应用，其中一些可能会在今年推出。 这标志着中国最大科技公司之一的深刻战略转变，表明 AI 不再仅仅是实验性工具，而是未来商业价值和竞争优势的核心驱动力。这一举措迫使整个组织进行 AI 创新，并可能加速开发出能与抖音等主要平台竞争的面向消费者的 AI 应用。 淘宝和天猫等核心电商部门被鼓励采用更多 AI 技术，各团队正与通义千问大模型的工程师密切合作。公司内部相信，基于成熟 AI 技术的'杀手级应用'可能很快就会出现，甚至可能比抖音更受欢迎。

telegram · zaihuapd · Mar 16, 14:45

**背景**: 阿里巴巴的'通义千问'（Qwen）是阿里云开发的一系列大语言模型，在概念上类似于 GPT-4 等模型。根据行业定义，'AI 原生'应用是指从零开始构建、将 AI 作为其架构和价值主张核心组成部分的应用，而不是在现有产品上添加 AI 功能。'AI 优先'战略则是指将 AI 作为业务运营和产品开发的核心支柱。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Qwen">Qwen - Wikipedia</a></li>
<li><a href="https://www.producttalk.org/glossary-ai-ai-native/">AI Native | Definition and Overview | Product Talk</a></li>
<li><a href="https://www.padiso.co/blog/ai-first-strategy">AI - First Strategy : Everything Sydney Business Owners... | PADISO</a></li>

</ul>
</details>

**标签**: `#AI Strategy`, `#Enterprise AI`, `#Business Transformation`, `#Alibaba`, `#Tech Industry`

---