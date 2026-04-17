---
layout: default
title: "Horizon Summary: 2026-04-17 (ZH)"
date: 2026-04-17
lang: zh
---

> From 21 items, 11 important content pieces were selected

---

1. [IETF 发布 IPv8 草案协议，采用 64 位地址并完全向后兼容 IPv4](#item-1) ⭐️ 9.0/10
2. [Anthropic 发布 Claude Opus 4.7，引入自适应思考能力并更新分词器。](#item-2) ⭐️ 8.0/10
3. [OpenAI 发布 Codex 重大更新，支持自动操作电脑与长期任务自动化](#item-3) ⭐️ 8.0/10
4. [通义千问发布专为智能体编码任务优化的开源 35B 参数模型。](#item-4) ⭐️ 8.0/10
5. [OpenAI、Anthropic 和 Google 罕见联手，遏制中国竞争对手未经授权蒸馏美国 AI 模型。](#item-5) ⭐️ 8.0/10
6. [苹果据传计划每年支付 10 亿美元，授权谷歌 1.2 万亿参数 Gemini AI，用于在 iOS 26.4 中对 Siri 进行重大重构](#item-6) ⭐️ 8.0/10
7. [阿里腾讯同日发布 3D 内容生成 AI 模型](#item-7) ⭐️ 8.0/10
8. [DeepSeek 发布 DeepGEMM 重大更新：推出 Mega MoE 融合算子并支持 FP4 精度](#item-8) ⭐️ 8.0/10
9. [Qwen3.6-35B-A3B 开源发布：一款仅激活 3B 参数的稀疏 MoE 代理式编程模型](#item-9) ⭐️ 8.0/10
10. [Anthropic 发布 Claude Opus 4.6，支持 200K 上下文窗口和自适应思考模式](#item-10) ⭐️ 8.0/10
11. [俄罗斯多款流行安卓应用被曝检测 VPN 使用并扫描外国应用](#item-11) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [IETF 发布 IPv8 草案协议，采用 64 位地址并完全向后兼容 IPv4](https://www.ietf.org/archive/id/draft-thain-ipv8-00.html) ⭐️ 9.0/10

互联网工程任务组（IETF）发布了互联网协议第 8 版（IPv8）的初始草案，该协议采用 64 位地址空间，并将 IPv4 视为其子集，实现了 100% 的向后兼容性。草案还引入了“区域服务器”架构来统一管理服务，并提出了基于 OAuth2 的强制授权和“成本因子”路由算法等新机制。 这代表了互联网基础设施一次潜在的范式转变，它从根本上解决了 IPv4 地址枯竭问题，同时避免了 IPv6 复杂的迁移挑战。如果被采纳，IPv8 可以简化网络管理，增强路由安全，并为未来的互联网提供一个更具可扩展性和安全性的基础。 该协议为每个自治系统号（ASN）分配超过 42.9 亿个主机地址，从结构上将全局 BGP8 路由表的大小限制为 ASN 的数量而非前缀数量。它强制要求 WHOIS8 路由验证和 /16 最小注入前缀规则以防止 BGP 劫持，并使用基于 HTTPS 封装的 8to4 隧道技术进行分阶段迁移。

telegram · zaihuapd · Apr 16, 08:43

**背景**: 当前的互联网主要依赖 IPv4，其 32 位地址空间有限，导致了地址枯竭。IPv6 拥有 128 位地址空间，是作为继任者开发的，但由于缺乏向后兼容性和复杂的过渡机制，其采用速度缓慢。IETF 是负责制定构成互联网协议套件（包括 TCP/IP）技术标准的标准组织。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.ietf.org/archive/id/draft-thain-ipv8-00.html">Internet Protocol Version 8 (IPv8) - ietf.org</a></li>
<li><a href="https://datatracker.ietf.org/doc/draft-thain-ipv8/">draft-thain-ipv8-01 - Internet Protocol Version 8 (IPv8)</a></li>
<li><a href="https://en.wikipedia.org/wiki/IPv6">IPv6 - Wikipedia</a></li>

</ul>
</details>

**标签**: `#networking`, `#protocols`, `#ietf`, `#ipv8`, `#internet-infrastructure`

---

<a id="item-2"></a>
## [Anthropic 发布 Claude Opus 4.7，引入自适应思考能力并更新分词器。](https://www.anthropic.com/news/claude-opus-4-7) ⭐️ 8.0/10

Anthropic 发布了 Claude Opus 4.7，这是一个重要更新，引入了自适应思考能力并更新了分词器。该模型现已在其所有产品和 API 中上线，定价与 4.6 版本保持一致。 此次发布标志着大语言模型向更高效、更具上下文感知的推理方式转变，有望在不进行手动调优的情况下提升复杂任务的处理性能。分词器的更新虽然增加了相同输入的 token 数量，但其目标是改进文本处理能力，这是影响模型理解和效率的基础组件。 自适应思考功能取代了手动设置思考 token 预算的模式，允许模型根据请求的复杂度动态决定推理力度。一个关键的注意事项是，新的分词器会使相同输入的 token 数量增加约 1.0 到 1.35 倍（取决于内容类型），这可能影响基于 token 计费的 API 成本。

hackernews · meetpateltech · Apr 16, 14:23

**背景**: Claude 是由 Anthropic 开发的大语言模型系列。'思考'或'思维链'能力允许模型在生成最终答案前，在内部逐步推理问题，这通常能带来更好的推理结果。分词器是大语言模型的核心组件，它将文本分解成更小的单元进行处理；其设计直接影响模型对语言的理解和计算效率。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://platform.claude.com/docs/en/build-with-claude/adaptive-thinking">Adaptive thinking - Claude API Docs</a></li>
<li><a href="https://www.anthropic.com/news/claude-opus-4-7">Introducing Claude Opus 4.7 \ Anthropic</a></li>
<li><a href="https://en.wikipedia.org/wiki/Large_language_model">Large language model - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: 社区讨论显示，用户对此次 API 变更感到困惑和沮丧，特别是转向自适应思考以及默认不再输出可读的推理摘要。部分用户对前一个版本（4.6）的性能表示不满，并指出 4.7 版本增强了网络安全过滤器，可能会阻止一些合法的技术请求。分词器更新及其对成本的影响也是技术讨论的焦点。

**标签**: `#llm`, `#anthropic`, `#claude`, `#ai-models`, `#api`

---

<a id="item-3"></a>
## [OpenAI 发布 Codex 重大更新，支持自动操作电脑与长期任务自动化](https://openai.com/index/codex-for-almost-everything/) ⭐️ 8.0/10

OpenAI 宣布为其开发者工具 Codex 推出重大更新，使其能够像人类一样通过视觉、点击和输入来操作电脑应用程序。此次更新引入了在 macOS 上并行工作的后台模式，新增了内置浏览器、图像生成、SSH 支持，并整合了包括 GitHub 和 Slack 在内的 90 多个新插件。 此次更新将 Codex 从一个代码助手转变为一个能够自动化复杂、多步骤工作流的通用 AI 智能体，覆盖了完整的软件开发周期及其他领域。这标志着 AI 在直接理解并执行用户对电脑的高级意图方面迈出了一大步，可能重塑人机交互和生产力工具的未来。 电脑操作功能目前仅面向登录 ChatGPT 桌面端的 macOS 用户开放。新版 Codex 增强了记忆和上下文感知能力，支持调度并自动执行跨越数日或数周的长期任务，并且它在任务执行期间运行在一个安全的、隔离的云容器中，并禁用互联网访问以确保安全。

hackernews · mikeevans · Apr 16, 17:12

**背景**: OpenAI Codex 是一系列专门为编程和编码任务微调的大型语言模型。在此次更新之前，它的主要功能是基于自然语言提示，通过生成、解释或重构代码来协助开发人员。'AI 智能体'的概念指的是一个能够感知环境、做出决策并采取行动以实现特定目标的系统，这标志着从纯粹的对话或代码生成模型的重要演进。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://openai.com/index/introducing-codex/">Introducing Codex | OpenAI</a></li>
<li><a href="https://openai.com/codex/">Codex | AI Coding Partner from OpenAI | OpenAI</a></li>

</ul>
</details>

**社区讨论**: 社区情绪复杂，部分用户对安全性表示怀疑，并指出类似功能已存在于 Claude Desktop 等竞争对手的产品中。另一些用户则对开发出强大的图形界面版本以彻底改变非专家用户使用电脑方式的潜力感到兴奋。反复出现的讨论主题包括：这究竟是真正的创新还是对现有工具的追赶，以及对 AI 直接控制个人电脑的担忧。

**标签**: `#AI`, `#automation`, `#OpenAI`, `#productivity`, `#human-computer-interaction`

---

<a id="item-4"></a>
## [通义千问发布专为智能体编码任务优化的开源 35B 参数模型。](https://qwen.ai/blog?id=qwen3.6-35b-a3b) ⭐️ 8.0/10

通义千问团队发布了 Qwen3.6-35B-A3B，这是一个拥有 350 亿参数的开源模型，专门针对智能体编码任务进行了优化。该模型的权重已在宽松许可下公开，并迅速被量化成 GGUF 格式，便于本地部署。 此次发布意义重大，它为开发者构建自主编码智能体提供了一个强大的开源选择，尤其是在金融和医疗等因数据隐私和监管合规而限制使用云端闭源模型的行业。这彰显了在行业整合趋势下，对开源权重 AI 模型的持续投入。 该模型基于 Qwen3.6 系列的混合架构，结合了线性注意力与稀疏专家混合路由机制，以实现高效扩展。它支持 256K 上下文长度和 201 种语言，早期社区反馈显示其在文本描述生成图像等创意任务上表现优异。

hackernews · cmitsakis · Apr 16, 13:36

**背景**: 智能体编码指的是超越简单代码补全的 AI 系统，它能够通过推理、选择工具和观察结果，自主规划和执行多步骤的软件开发任务。开源权重模型是指训练好的参数在宽松许可下公开发布的模型，允许检查、修改和本地部署，这与仅提供 API 访问的闭源模型不同。通义千问模型系列由阿里巴巴开发，以其在各种基准测试中的强劲表现而闻名。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://cloud.google.com/discover/what-is-agentic-coding">What is agentic coding? How it works and use cases</a></li>
<li><a href="https://help.openai.com/en/articles/11870455-openai-open-weight-models-gpt-oss">OpenAI open - weight models (gpt-oss) | OpenAI Help Center</a></li>
<li><a href="https://unsloth.ai/docs/models/qwen3.6">Run the new Qwen 3 . 6 -35-A3B model locally! | Unsloth Documentation</a></li>

</ul>
</details>

**社区讨论**: 社区反响非常积极，通过 GGUF 量化实现本地使用的即时实践已被注意到。评论者对通义千问在面临内部挑战时仍坚持开源权重的承诺表示欣慰和赞赏。此外，社区还讨论了该模型在受监管行业的特殊价值，并观察了它与其他基础模型相比的独特性能特征。

**标签**: `#open-source-ai`, `#coding-assistants`, `#llm`, `#model-release`, `#agentic-ai`

---

<a id="item-5"></a>
## [OpenAI、Anthropic 和 Google 罕见联手，遏制中国竞争对手未经授权蒸馏美国 AI 模型。](https://t.me/zaihuapd/40889) ⭐️ 8.0/10

OpenAI、Anthropic 和 Google（Alphabet）已开始通过 Frontier Model Forum 进行罕见协作，共享有关“对抗性蒸馏”的信息，旨在遏制中国竞争对手未经授权提取其前沿 AI 模型的输出并复制其能力。OpenAI 已确认参与这一信息共享行动，并提到了其近期提交给美国国会的相关备忘录。 此次合作意义重大，它代表了美国主要 AI 公司在应对其视为经济威胁和潜在国家安全风险的行为上达成了战略一致。这凸显了全球 AI 竞争的加剧，以及保护知识产权和模型安全作为核心资产的关注度日益提升。 此次合作是在 Frontier Model Forum 的框架内进行的，这是一个关注 AI 安全与安全风险的行业支持的非营利组织。具体的担忧在于“对抗性蒸馏”，即未经授权使用模型的输出来训练竞争模型，这可能绕过原始模型的安全护栏并导致重大的经济损失。

telegram · zaihuapd · Apr 16, 04:06

**背景**: 模型蒸馏是一种合法的机器学习技术，较小的“学生”模型学习模仿较大、较复杂的“教师”模型的行为，通常是为了提高效率。Frontier Model Forum 由 OpenAI、Anthropic、Google 和 Microsoft 于 2023 年创立，旨在协调先进“前沿”AI 模型的安全最佳实践。“对抗性蒸馏”指的是竞争对手未经授权使用该技术来复制专有模型能力，引发了关于知识产权盗窃和创建缺乏适当安全控制模型的担忧。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.frontiermodelforum.org/">Frontier Model Forum</a></li>
<li><a href="https://www.frontiermodelforum.org/issue-briefs/issue-brief-adversarial-distillation/">Adversarial Distillation - Frontier Model Forum</a></li>
<li><a href="https://oecd.ai/en/incidents/2026-04-06-1282">US AI Firms Collaborate to Counter Unauthorized Model Distillation ...</a></li>

</ul>
</details>

**标签**: `#AI Ethics & Safety`, `#AI Competition`, `#Model Security`, `#Geopolitics`

---

<a id="item-6"></a>
## [苹果据传计划每年支付 10 亿美元，授权谷歌 1.2 万亿参数 Gemini AI，用于在 iOS 26.4 中对 Siri 进行重大重构](https://t.me/zaihuapd/40891) ⭐️ 8.0/10

据报道，苹果正在敲定一项协议，授权使用谷歌开发的 1.2 万亿参数 Gemini AI 模型，以支持对 Siri 语音助手进行全面升级，年授权费约为 10 亿美元。新版 Siri 代号为 Linwood，计划于 2026 年春季作为 iOS 26.4 的一部分发布。 这笔潜在交易对苹果而言是一次重大的战略转变（苹果历来开发自己的 AI 模型），通过将苹果庞大的设备生态系统与谷歌尖端的大语言模型相结合，可能极大地重塑 AI 助手领域的竞争格局。成功的整合将使 Siri 成为对抗其他先进 AI 助手时能力强大得多的竞争者。 据报道，1.2 万亿参数的 Gemini 模型将远超苹果目前使用的 1500 亿参数模型，预计将处理 Siri 的摘要和规划任务。然而，有报道称此次重构在内部测试中遇到了障碍，且 iOS 26.4 中的 Siri 将不具备完整的聊天机器人功能，苹果计划保留部分设备端处理，并使用 Private Cloud Compute 来维护隐私。

telegram · zaihuapd · Apr 16, 05:18

**背景**: 像 Gemini 这样的大语言模型（LLM）是拥有数十亿或数万亿参数的机器学习模型，在海量数据集上训练，用于自然语言处理。谷歌的 Gemini 是一个多模态 AI 模型系列，采用 Transformer 架构，并在其 1.5 版本中使用了混合专家（Mixture of Experts, MoE）方法以提高效率。Siri 是苹果的语音助手，其表现被认为落后于谷歌助手等竞争对手，这一直是批评的焦点，也促使苹果努力进行由 AI 驱动的大规模重构。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/List_of_large_language_models">List of large language models - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Gemini_(language_model)">Gemini (language model) - Wikipedia</a></li>
<li><a href="https://theoutpost.ai/news-story/apple-s-i-os-26-4-siri-overhaul-powered-by-google-gemini-promises-bigger-upgrade-than-expected-23609/">Apple Siri Delay: AI Assistant Pushed to Late 2026</a></li>

</ul>
</details>

**标签**: `#AI-Models`, `#Apple`, `#Google`, `#Voice-Assistants`, `#Industry-News`

---

<a id="item-7"></a>
## [阿里腾讯同日发布 3D 内容生成 AI 模型](https://www.bloomberg.com/news/articles/2026-04-16/alibaba-releases-new-ai-model-for-gaming-development) ⭐️ 8.0/10

阿里巴巴发布了名为“Happy Oyster”的 AI 模型，可生成三维、可交互的视频内容，主要面向游戏开发及影视制作。腾讯同日发布并开源了“混元 3D 世界模型 2.0”，支持根据文字、图片、视频生成、重建和模拟 3D 世界，并可导出 Mesh、3DGS、点云等资产，接入现有游戏工作流。 两家中国科技巨头同日发布相关模型，标志着 AI 驱动的 3D 内容创作正加速走向工业化，有望极大提升游戏、影视及数字孪生应用的生产效率。模型强调与 Unity、UE 等行业标准工具的集成，表明其目标已超越技术演示，旨在提供可直接用于生产流程的实用解决方案。 腾讯的开源模型特别支持导出 Mesh 和 3D 高斯泼溅（3DGS）等格式的资产，这对于在游戏引擎中进行实时渲染和编辑至关重要。两款模型都强调了从真实空间视频或多视角图片构建数字孪生场景的能力，拓展了其在纯内容生成之外的实用性。

telegram · zaihuapd · Apr 16, 07:58

**背景**: 3D 内容生成是 AI 的前沿领域，旨在从文本或图像等简单输入中创建三维模型和场景。Mesh（由顶点和多边形定义的表面）和 3D 高斯泼溅（3DGS，一种从图像生成高质量、实时新视角合成的技术）是游戏和模拟中常用的 3D 资产表示格式。数字孪生是物理对象、系统或空间的虚拟复制品，常用于分析、监控或模拟。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Gaussian_splatting">Gaussian splatting - Wikipedia</a></li>
<li><a href="https://imerit.net/resources/blog/3d-point-cloud-vs-mesh/">3 D Point Cloud vs Mesh : What’s the Difference?</a></li>
<li><a href="https://arxiv.org/html/2509.17647">VideoArtGS: Building Digital Twins of Articulated Objects from Monocular Video</a></li>

</ul>
</details>

**标签**: `#3D-Generation`, `#AI-Models`, `#Game-Development`, `#Multimodal-AI`, `#Computer-Vision`

---

<a id="item-8"></a>
## [DeepSeek 发布 DeepGEMM 重大更新：推出 Mega MoE 融合算子并支持 FP4 精度](https://github.com/deepseek-ai/DeepGEMM/tree/public-release-260416) ⭐️ 8.0/10

2026 年 4 月 16 日，DeepSeek 对其高性能算子库 DeepGEMM 发布了重大更新，正式推出了名为 Mega MoE 的融合算子，该算子通过将 dispatch、SwiGLU 等多个计算步骤与 NVLink 通信重叠，实现了计算与通信的高效融合。此外，本次更新还新增了 FP8xFP4 GEMM 算子、FP4 Indexer 以及程序化依赖启动（PDL）支持，并显著提升了即时编译（JIT）速度。 此次更新对于大型语言模型的推理和训练，尤其是日益流行的混合专家（MoE）架构，是一次重大的性能优化。通过融合算子操作并实现计算与通信的重叠，该技术可以显著提升硬件利用率和降低延迟，使得运行大规模 AI 模型变得更加高效。 DeepGEMM 库专为现代大模型设计，支持 NVIDIA SM90 和 SM100 GPU 架构，其核心优势在于轻量化设计与运行时即时编译，无需在安装阶段进行复杂编译。Mega MoE 算子通过对称内存技术，进一步优化了多专家模型在推理和训练中的性能表现。

telegram · zaihuapd · Apr 16, 09:57

**背景**: DeepGEMM 是 DeepSeek-AI 发布的高性能 CUDA 内核库，最初以支持 FP8 精度的通用矩阵乘法（GEMM）运算来加速模型训练而闻名。融合 MoE 算子解决了混合专家模型中的一个关键瓶颈，它将多个小型独立操作（如将令牌路由到专家、计算专家输出）合并为一个大规模的内核。这种融合能更好地利用 GPU 为大型连续数据块设计的并行处理能力，从而减少开销并提升性能。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/deepseek-ai/DeepGEMM">GitHub - deepseek-ai/ DeepGEMM : DeepGEMM : clean and efficient...</a></li>
<li><a href="https://medium.com/@datenlord/from-loops-to-fusion-understanding-the-principles-of-the-fused-moe-operator-part1-203767168166">From Loops to Fusion: Understanding the Principles of the Fused MoE Operator (Part1) | by DatenLord | Nov, 2025 | Medium</a></li>

</ul>
</details>

**标签**: `#AI-Infrastructure`, `#GPU-Computing`, `#Model-Optimization`, `#CUDA`, `#Mixture-of-Experts`

---

<a id="item-9"></a>
## [Qwen3.6-35B-A3B 开源发布：一款仅激活 3B 参数的稀疏 MoE 代理式编程模型](https://qwenlm.github.io/blog/qwen3.6-35b-a3b/) ⭐️ 8.0/10

Qwen 团队开源了 Qwen3.6-35B-A3B，这是一款稀疏专家混合模型，总参数量为 350 亿，但每次推理仅激活 30 亿参数。该模型专为代理式编程和多模态推理设计，官方称其在 SWE-bench、MCPMark 等编码与工具使用基准上的表现显著优于前代模型，并可媲美部分规模更大的稠密模型。 此次发布是迈向更高效、更强大 AI 智能体（Agent）的重要一步。该模型仅用少量激活参数就实现了强大的性能，降低了开发能够理解代码、使用工具和处理多模态输入的复杂智能体系统的计算成本和门槛，有望加速现实世界 AI 应用的开发进程。 该模型保留了多模态理解能力，在多项视觉语言评测中表现接近甚至超过部分闭源强模型。它已提供开放权重供自托管，并提供了兼容 OpenAI/Anthropic 风格接口的 API，便于接入 OpenClaw、Qwen Code 等开发者工作流。

telegram · zaihuapd · Apr 16, 13:59

**背景**: 稀疏专家混合模型是一种神经网络架构，旨在不按比例增加计算成本的前提下提升模型容量。其原理是拥有多个“专家”子网络，但对于每个输入，只激活和使用一小部分专家进行计算。SWE-bench 是一个用于评估大语言模型解决现实世界软件工程问题能力的基准，其中的问题收集自 GitHub，要求模型生成能解决所述问题的代码补丁。MCPMark 则是一个综合性基准，旨在压力测试模型和智能体在真实 Model Context Protocol 使用场景下的能力。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arxiv.org/abs/2604.13761">Design and Behavior of Sparse Mixture-of-Experts Layers in ...</a></li>
<li><a href="https://github.com/swe-bench/SWE-bench">GitHub - SWE-bench/SWE-bench: SWE-bench: Can Language Models ...</a></li>
<li><a href="https://arxiv.org/abs/2509.24002">[2509.24002] MCPMark : A Benchmark for Stress-Testing Realistic...</a></li>

</ul>
</details>

**标签**: `#AI`, `#Large Language Models`, `#Mixture-of-Experts`, `#Code Generation`, `#Open Source`

---

<a id="item-10"></a>
## [Anthropic 发布 Claude Opus 4.6，支持 200K 上下文窗口和自适应思考模式](https://t.me/zaihuapd/40903) ⭐️ 8.0/10

Anthropic 发布了新一代 Claude Opus 4.6 模型，将上下文窗口提升至 200K token（测试版提供 100 万 token），并将最大输出 token 数翻倍至 128K。该模型引入了自适应思考模式，可根据问题复杂度动态调整思考深度，并新增最高级别的 'max effort' 参数，同时还推出了上下文压缩功能以实现近乎无限长度的对话。 此次发布标志着 AI 模型能力的一次重大飞跃，通过提供更大的上下文窗口和更复杂的推理机制，直接与其他领先模型展开竞争。自适应思考模式和上下文压缩功能有望实现更高效、更自然的长时间交互，可能彻底改变用户在处理复杂任务和进行长时间对话时与 AI 助手互动的方式。 200K 上下文窗口在测试版中提供实验性的 100 万 token 容量，而标准版本则为 200K。上下文压缩功能会在对话接近窗口限制时自动总结早期内容，形成一个滚动的记忆系统，在保持对话连续性的同时不丢失关键上下文。

telegram · zaihuapd · Apr 16, 14:28

**背景**: Claude 是 Anthropic 的旗舰大型语言模型，直接与 OpenAI 的 GPT 系列和 Google 的 Gemini 等模型竞争。上下文窗口指的是模型在处理时一次性能考虑的文本量（以 token 计量），本质上相当于其工作记忆。上下文压缩是一种通过总结或有选择地保留信息来优化对话历史的技术，使模型能够处理更长的对话而不超出 token 限制，同时保持对话状态和连贯性。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://blog.mycal.net/infinite-ai-chat-windows/">Make Your Chat Context Feel Infinite: Rolling Compression for GPT...</a></li>
<li><a href="https://particula.tech/blog/prompt-compression-context-window-optimization">Prompt Compression : Making Context Windows Work for You</a></li>

</ul>
</details>

**标签**: `#AI`, `#LLM`, `#Anthropic`, `#Claude`, `#Natural Language Processing`

---

<a id="item-11"></a>
## [俄罗斯多款流行安卓应用被曝检测 VPN 使用并扫描外国应用](https://files.rks.global/russian_apps_search_for_vpn_en.pdf) ⭐️ 7.0/10

RKS Global 的一项研究发现，30 款流行的俄罗斯安卓应用中有 22 款具备 VPN 检测功能，其中 19 款会将 VPN 状态数据发送至其服务器。此外，Avito 应用还被发现会扫描设备上是否安装了超过 200 种外国应用，包括银行、加密货币钱包和即时通讯应用。 主流应用这种系统性的、侵犯隐私的数据收集行为，标志着用户监控的显著升级，很可能是为了遵守即将到来的政府限制而实施的。它直接影响数百万用户的数字隐私和自由，可能基于用户使用规避工具而阻止其访问基本服务。 该研究特别指出 Avito 市场应用会扫描大量外国软件。这种广泛的检测和上报行为与俄罗斯数字发展部的一项指令直接相关，该部已指示大型企业从 2026 年 4 月 15 日起，对启用 VPN 的用户限制相关服务。

telegram · zaihuapd · Apr 16, 04:38

**背景**: 虚拟专用网络（VPN）会加密用户的互联网流量，并通过位于另一地点的服务器进行路由，可用于绕过地理限制或增强隐私。近年来，俄罗斯政府日益寻求控制互联网访问并封锁 Telegram 等服务，导致对 VPN 这一常见规避工具的打击。数字发展部已公开声明其目标是减少俄罗斯人使用 VPN。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.themoscowtimes.com/2026/03/31/russias-digital-ministry-declares-war-on-vpns-a92384">Russia’s Digital Ministry Declares War on VPNs</a></li>
<li><a href="https://tarkalabs.com/blogs/vpn-detection-guide-ios-android/">The ultimate VPN detection guide for iOS and Android ... - Tarka Labs</a></li>

</ul>
</details>

**标签**: `#privacy`, `#android-security`, `#vpn`, `#government-surveillance`, `#app-analysis`

---