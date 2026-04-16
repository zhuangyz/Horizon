---
layout: default
title: "Horizon Summary: 2026-04-16 (ZH)"
date: 2026-04-16
lang: zh
---

> From 24 items, 12 important content pieces were selected

---

1. [IETF 发布 IPv8 草案：采用 64 位地址，实现与 IPv4 的完全向后兼容](#item-1) ⭐️ 9.0/10
2. [DeepSeek 发布 DeepGEMM 重大更新：推出 Mega MoE 融合算子并支持 FP4 精度](#item-2) ⭐️ 9.0/10
3. [Anthropic 发布 Claude Opus 4.7，引入自适应思考与更新分词器。](#item-3) ⭐️ 8.0/10
4. [通义千问发布开源权重 35B 代码模型 Qwen3.6-35B-A3B，专为智能体应用设计](#item-4) ⭐️ 8.0/10
5. [谷歌发布采用 Swift 原生开发的 macOS 版 Gemini 应用，支持快捷键并宣布与苹果达成多年合作](#item-5) ⭐️ 8.0/10
6. [OpenAI、Anthropic 和 Google 罕见联手，遏制中国竞争对手的对抗性蒸馏行为。](#item-6) ⭐️ 8.0/10
7. [苹果据称计划授权谷歌 1.2 万亿参数 Gemini AI 模型，以全面重构 Siri。](#item-7) ⭐️ 8.0/10
8. [阿里腾讯同日发布 3D 内容生成 AI 模型](#item-8) ⭐️ 8.0/10
9. [Qwen3.6-35B-A3B 开源发布：一款仅激活 3B 参数的稀疏 MoE 代理式编程模型](#item-9) ⭐️ 8.0/10
10. [Anthropic 发布 Claude Opus 4.6，支持 200K 上下文窗口和自适应思考模式。](#item-10) ⭐️ 8.0/10
11. [谷歌发布 Gemini 3.1 Flash TTS，支持场景化提示控制](#item-11) ⭐️ 7.0/10
12. [俄罗斯多款流行安卓应用被曝检测 VPN 状态并扫描外国应用，或响应政府限制指令](#item-12) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [IETF 发布 IPv8 草案：采用 64 位地址，实现与 IPv4 的完全向后兼容](https://www.ietf.org/archive/id/draft-thain-ipv8-00.html) ⭐️ 9.0/10

互联网工程任务组（IETF）发布了互联网协议第 8 版（IPv8）的初始草案，该草案引入了 64 位地址空间，并将 IPv4 视为其子集，实现了 100%的向后兼容性。草案提议将 DHCP、DNS 和身份验证等服务整合到统一的“区域服务器”架构中，并引入了新的安全与路由效率机制。 该提案通过直接解决 IPv4 长期存在的地址枯竭问题，同时避免了 IPv6 复杂的双栈部署挑战，代表了一种潜在的范式转变。如果被采纳，它可以简化互联网基础设施管理，增强路由安全性，并实现从传统 IPv4 网络更平滑的过渡。 草案规定每个自治系统号（ASN）将被分配超过 42 亿个主机地址，并提议基于 OAuth2 的强制授权和名为“成本因子”的算法用于最优路径选择。它还包括用于迁移期间互操作性的 8to4 隧道技术，以及诸如/16 最小注入前缀等规则，以防止 BGP 劫持和全球路由表膨胀。

telegram · zaihuapd · Apr 16, 08:43

**背景**: 当前的互联网主要运行在两种协议上：IPv4 使用 32 位地址，其可用空间已耗尽；IPv6 使用 128 位地址以提供巨大容量，但需要双栈方法来实现兼容性，这使部署变得复杂。IETF 是负责定义核心互联网协议的标准机构，其草案代表了供社区评审和讨论的早期提案。像 6to4 这样的过渡机制已被用于连接 IPv4 和 IPv6 网络。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.ietf.org/archive/id/draft-thain-ipv8-00.html">Internet Protocol Version 8 (IPv8)</a></li>
<li><a href="https://cybernews.com/tech/ipv8-proposal-slammed-by-tech-professionals/">Tech pros slam new IPv8 proposal as AI slop | Cybernews</a></li>
<li><a href="https://lowendtalk.com/discussion/216334/internet-protocol-version-8-ipv8-proposal">Internet Protocol Version 8 (IPv8) proposal — LowEndTalk</a></li>

</ul>
</details>

**社区讨论**: 该提案发布后不久，便在技术专业人士中引发了重大争议和批评。社区中的许多人持怀疑态度，将该草案标记为不切实际的“AI 垃圾”，并鉴于 IPv6 正在持续（尽管缓慢）部署，质疑新协议的必要性。

**标签**: `#networking`, `#protocols`, `#ietf`, `#ipv8`, `#internet-infrastructure`

---

<a id="item-2"></a>
## [DeepSeek 发布 DeepGEMM 重大更新：推出 Mega MoE 融合算子并支持 FP4 精度](https://github.com/deepseek-ai/DeepGEMM/tree/public-release-260416) ⭐️ 9.0/10

2026 年 4 月 16 日，DeepSeek 对其高性能算子库 DeepGEMM 发布了重大更新，正式推出了 Mega MoE 融合算子，该算子将 dispatch、SwiGLU 等多个计算步骤与 NVLink 通信进行重叠。此外，本次更新还新增了 FP8xFP4 GEMM 算子、FP4 Indexer 以及程序化依赖启动（PDL）支持，并显著提升了即时编译（JIT）速度。 此次更新通过优化计算和通信模式，解决了大型混合专家（MoE）模型在训练和推理中的关键瓶颈。引入 FP4 精度支持使得模型部署更加内存高效，有望让更大的模型在现有硬件上运行，或为 AI 公司降低基础设施成本。 DeepGEMM 库专为现代大模型设计，支持 NVIDIA SM90 和 SM100 架构，其核心优势在于轻量化设计与运行时即时编译，无需在安装阶段进行复杂编译。Mega MoE 算子特别采用了对称内存技术，进一步优化了多专家模型在推理和训练中的性能表现。

telegram · zaihuapd · Apr 16, 09:57

**背景**: 混合专家（MoE）模型是一种神经网络架构，其中不同的专用子网络（专家）处理不同的输入，从而允许更大的模型容量而无需按比例增加计算量。融合算子将多个计算步骤合并到单个 GPU 内核中，以减少内存传输并提高效率。NVLink 是 NVIDIA 的高速 GPU 互连技术，与传统 PCIe 连接相比，可实现 GPU 之间更快的数据传输。FP4（4 位浮点）量化通过降低模型权重的数值精度来节省内存，但如果实施不当可能会影响模型精度。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://medium.com/@datenlord/from-loops-to-fusion-understanding-the-principles-of-the-fused-moe-operato-part2-1ff65a17cd56">From Loops to Fusion: Understanding the Principles of the Fused MoE ...</a></li>
<li><a href="https://stevenfoerster.com/tutorials/efficient-fine-tuning-with-lora-and-quantization/">Efficient Fine-Tuning with LoRA and Quantization · Steven Foerster</a></li>
<li><a href="https://uvation.com/articles/unlocking-ultra-fast-gpu-communication-with-nvidia-nvlink-nvlink-switch">NVIDIA NVLink and NVLink Switch: Redefining GPU Interconnects</a></li>

</ul>
</details>

**标签**: `#AI-Infrastructure`, `#High-Performance-Computing`, `#CUDA-Optimization`, `#Mixture-of-Experts`, `#Quantization`

---

<a id="item-3"></a>
## [Anthropic 发布 Claude Opus 4.7，引入自适应思考与更新分词器。](https://www.anthropic.com/news/claude-opus-4-7) ⭐️ 8.0/10

Anthropic 发布了 Claude Opus 4.7，引入了新的“自适应思考”能力并更新了分词器。此次发布还弃用了之前的手动思考预算模式，并更改了默认输出，不再包含人类可读的推理摘要。 这是对领先 AI 模型的一次重大更新，从根本上改变了开发者与其推理能力的交互方式，有望提升复杂任务的处理性能。分词器的更新虽然增加了相同输入的 token 数量，但旨在提高文本处理效率，这是影响所有 API 用户的核心技术变更。 新的自适应思考模式取代了之前的 `budget_tokens` 配置，通过 `thinking.type: "adaptive"` 和一个 `effort` 参数来控制。更新后的分词器使相同输入的 token 数量大约增加 1.0 到 1.35 倍，具体取决于内容类型，这可能会影响 API 定价和上下文窗口的使用。

hackernews · meetpateltech · Apr 16, 14:23

**背景**: Claude 是由 Anthropic 开发的大型语言模型。“思考”或“思维链”能力允许模型在生成最终答案前进行内部的、逐步的推理，这对于解决复杂问题至关重要。分词器是 LLM 的核心组件，它将文本分解成更小的单元进行处理；其效率直接影响模型的性能和成本。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://platform.claude.com/docs/en/build-with-claude/adaptive-thinking">Adaptive thinking - Claude API Docs</a></li>
<li><a href="https://seantrott.substack.com/p/tokenization-in-large-language-models">Tokenization in large language models, explained</a></li>
<li><a href="https://www.anthropic.com/news/claude-opus-4-7">Introducing Claude Opus 4.7 \ Anthropic</a></li>

</ul>
</details>

**社区讨论**: 开发者情绪复杂，一些人对 API 变更表示困惑，并报告了诸如模型拒绝执行其自身文档中的任务等问题。其他人则指出与上一版本相比的性能不一致性，并强调了分词器变更对成本的实际影响。还有人提到了在潜在调整之前存在一个短暂的“未削弱”智能体编码窗口期。

**标签**: `#llm`, `#anthropic`, `#api`, `#ai-models`, `#developer-tools`

---

<a id="item-4"></a>
## [通义千问发布开源权重 35B 代码模型 Qwen3.6-35B-A3B，专为智能体应用设计](https://qwen.ai/blog?id=qwen3.6-35b-a3b) ⭐️ 8.0/10

阿里巴巴的通义千问团队公开发布了 Qwen3.6-35B-A3B，这是一个拥有 350 亿参数的开源权重代码模型，专门为智能体应用设计。该模型现已可供公众下载和使用。 此次发布为构建自主 AI 编程智能体的开发者提供了一个强大的专用工具，对于银行和医疗等因数据隐私限制而无法使用公共云模型的行业尤其有价值。这代表了通义千问团队在面临近期组织挑战后，对开源权重 AI 的持续承诺。 该模型采用混合注意力架构，支持 256K 上下文窗口，并以 GGUF 等量化格式提供，便于本地部署。它是更大的 Qwen3.6 模型家族的一部分，该家族模型原生支持多模态，并支持超过 200 种语言。

hackernews · cmitsakis · Apr 16, 13:36

**背景**: 通义千问是阿里巴巴开发的一系列 AI 模型。'开源权重'模型向公众提供训练好的模型参数（权重）供使用，但可能不包含完整的训练代码、数据或实现完全可复现性所需的规范，这与'开源'模型不同。智能体编码指的是一种 AI 范式，即大型语言模型通过与编译器和调试器等工具交互，自主规划和执行多步骤的软件开发任务。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://unsloth.ai/docs/models/qwen3.6">Run the new Qwen 3 . 6 - 35 - A 3 B model locally! | Unsloth Documentation</a></li>
<li><a href="https://hellofuture.orange.com/en/a-typology-of-artificial-intelligence-models/">AI models explained: open source vs. open weight vs. closed</a></li>
<li><a href="https://arxiv.org/html/2508.11126v1">AI Agentic Programming: A Survey of Techniques, Challenges, and Opportunities</a></li>

</ul>
</details>

**社区讨论**: 社区情绪积极，强调了通过量化格式实现的实用可访问性以及该模型对受限行业的相关性。尽管面临内部挑战，社区对通义千问持续发布开源权重模型表示赞赏，同时也对为何选择此变体而非公开投票中更受欢迎的变体感到好奇。

**标签**: `#open-source-ai`, `#coding-agents`, `#llm`, `#model-release`, `#qwen`

---

<a id="item-5"></a>
## [谷歌发布采用 Swift 原生开发的 macOS 版 Gemini 应用，支持快捷键并宣布与苹果达成多年合作](https://9to5mac.com/2026/04/15/google-launches-gemini-mac-app-heres-what-it-offers/) ⭐️ 8.0/10

谷歌于 4 月 15 日正式推出了其 Gemini AI 助手的原生 macOS 应用程序，该应用使用苹果的 Swift 编程语言开发，并支持通过 Option + Space 快捷键快速呼出。此外，谷歌与苹果宣布达成一项多年期合作伙伴关系，Gemini 将为即将推出的 iOS 27 和 macOS 27 提供 AI 功能支持，更多合作细节将于 2026 年 6 月 8 日的 WWDC 上公布。 这标志着谷歌通过原生开发将其 AI 助手深度集成到苹果生态系统的重大战略举措，有望在 macOS 上提供更优的用户体验。宣布的合作关系标志着竞争格局的重大转变，两大科技巨头联手，用谷歌的 Gemini 技术增强苹果的 AI 能力（如 Siri 和 Apple Intelligence），这可能会重塑苹果设备上 AI 助手的未来。 这款原生 Swift 应用支持 Gemini 的核心功能，如快速问答、内容草拟、信息摘要、代码编写和图像分析，并允许屏幕共享以为查询提供更丰富的上下文。该合作关系的具体目标是为下一代主要操作系统版本中的升级版 Siri 和 Apple Intelligence 功能提供动力，这表明其技术集成深度远超简单的 API 调用。

telegram · zaihuapd · Apr 16, 00:33

**背景**: Gemini 是谷歌旗舰的多模态大语言模型（LLM）和 AI 助手系列，与 OpenAI 的 ChatGPT 等产品竞争。原生应用开发使用平台首选语言（如针对 macOS 的 Swift），与跨平台框架相比，通常能提供更好的性能、与系统功能更顺畅的集成以及更灵敏的用户界面。Apple Intelligence 是苹果于 2024 年宣布的自有生成式 AI 系统，旨在通过设备端和云端混合处理的方式在其设备上运行。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://learningswift.brightdigit.com/articles/native-app-development-advantages/">Native App Development and Its Advantages | BrightDigit</a></li>
<li><a href="https://en.wikipedia.org/wiki/Apple_Intelligence">Apple Intelligence - Wikipedia</a></li>

</ul>
</details>

**标签**: `#AI-Assistants`, `#macOS`, `#Google-Gemini`, `#Apple-Google-Partnership`, `#Native-Development`

---

<a id="item-6"></a>
## [OpenAI、Anthropic 和 Google 罕见联手，遏制中国竞争对手的对抗性蒸馏行为。](https://t.me/zaihuapd/40889) ⭐️ 8.0/10

OpenAI、Anthropic 和 Alphabet 旗下的 Google 已通过 Frontier Model Forum 启动了一项罕见的协作，旨在共享有关“对抗性蒸馏”的信息。此举是为了遏制中国竞争对手未经授权提取美国前沿 AI 模型的输出并复制其能力的行为。 此次合作标志着领先的 AI 竞争对手开始联合起来，以保护其核心知识产权，并应对他们眼中兼具商业威胁和潜在国家安全风险的行为。这凸显了 AI 开发中日益加剧的地缘政治因素，模型安全正变得与模型能力同等重要。 OpenAI 已确认参与此次信息共享行动，并提到了其近期提交给美国国会的相关备忘录。此次协作是在 Frontier Model Forum 的框架内进行的，该行业组织最初专注于 AI 安全，现已将其范围扩大到包括防范模型提取攻击的安全领域。

telegram · zaihuapd · Apr 16, 04:06

**背景**: 对抗性蒸馏是一种模型提取攻击，通过使用原始专有模型（如 GPT-4 或 Claude）的输出（通常通过 API 查询获得）来训练一个次级模型以模仿前者。Frontier Model Forum 是一个行业组织，由 Anthropic、Google、Microsoft 和 OpenAI 于 2023 年 7 月创立，其最初声明的使命是确保前沿 AI 模型的安全和负责任开发。模型提取攻击针对的是训练模型中所蕴含的知识产权，是 AI 安全领域一种复杂的威胁。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.frontiermodelforum.org/issue-briefs/issue-brief-adversarial-distillation/">Adversarial Distillation - Frontier Model Forum</a></li>
<li><a href="https://www.frontiermodelforum.org/">Frontier Model Forum</a></li>
<li><a href="https://snyk.io/articles/ai-model-theft/">AI Model Theft: Understanding the Threat Landscape and ... - Snyk</a></li>

</ul>
</details>

**标签**: `#AI Safety`, `#Geopolitics`, `#Intellectual Property`, `#Industry Collaboration`, `#Model Security`

---

<a id="item-7"></a>
## [苹果据称计划授权谷歌 1.2 万亿参数 Gemini AI 模型，以全面重构 Siri。](https://t.me/zaihuapd/40891) ⭐️ 8.0/10

据报道，苹果正在敲定一项协议，授权谷歌的 1.2 万亿参数 Gemini AI 模型，为其 Siri 语音助手提供一次重大升级。该协议涉及苹果每年向谷歌支付约 10 亿美元，新版 Siri 代号为“Linwood”，计划于明年春季在 iOS 26.4 中发布。 这一潜在合作对苹果而言是一次重大的战略转变，该公司历来都自主研发 AI 技术，此举可能极大地重塑 AI 助手领域的竞争格局。如此大规模的协议，将谷歌尖端的大语言模型整合进苹果的生态系统，将是一次前所未有的跨公司合作，对用户体验和市场动态产生重大影响。 据报道，这款 1.2 万亿参数的 Gemini 模型将远超苹果目前使用的云端 AI 模型，后者据称仅有 15 亿参数。新版 Siri 预计将利用谷歌的模型来处理摘要和规划等任务，查询将通过苹果的 Private Cloud Compute 基础设施进行处理。

telegram · zaihuapd · Apr 16, 05:18

**背景**: 像 Gemini 这样的大语言模型（LLM）是经过海量文本和多模态数据训练的 AI 系统，用于理解和生成类人语言。模型的参数数量是其规模和潜在能力的关键指标，参数越多通常意味着更复杂的性能。谷歌的 Gemini 模型家族，包括 Gemini 1.5 等版本，采用了如混合专家（Mixture of Experts, MoE）等先进架构来提高效率和能力。Siri 是苹果长期以来的语音激活虚拟助手，集成在其设备中。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://udit.co/blog/apple-siri-google-gemini-trillion-parameter-ai-overhaul">Apple Redesigns Siri with Google's Trillion - Parameter Gemin</a></li>
<li><a href="https://biggo.com/news/202511052052_Apple_Siri_Google_Gemini_AI_Model">Apple's Siri Revamp to Run on Google's 1 . 2 Trillion - Parameter AI ...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Gemini_(language_model)">Gemini (language model) - Wikipedia</a></li>

</ul>
</details>

**标签**: `#artificial-intelligence`, `#voice-assistants`, `#tech-industry`, `#large-language-models`, `#mobile-operating-systems`

---

<a id="item-8"></a>
## [阿里腾讯同日发布 3D 内容生成 AI 模型](https://www.bloomberg.com/news/articles/2026-04-16/alibaba-releases-new-ai-model-for-gaming-development) ⭐️ 8.0/10

2026 年 4 月 16 日，阿里巴巴发布了名为“Happy Oyster”的 AI 模型，该模型可生成用于游戏开发和影视制作的三维、可交互视频内容。同日，腾讯开源了其混元 3D 世界模型 2.0，该模型支持根据文字、图片或视频生成、重建和模拟 3D 世界，并能导出 Mesh、3D 高斯泼溅（3DGS）等资产，以便接入现有游戏工作流。 这标志着中国科技巨头在先进多模态 AI 和世界建模能力竞赛上的重大升级，直接瞄准了高价值的游戏和数字孪生产业。两家公司同日发布模型，显示出其战略意图是普及和加速 3D 内容创作，有望降低游戏开发者、电影制作人和数字孪生创作者的制作门槛并重塑其工作流程。 腾讯的模型特别支持将生成内容导出到 Unity、Unreal Engine 等行业标准引擎进行二次编辑，并能根据真实空间视频或多视角图片构建数字孪生场景。阿里巴巴的 Happy Oyster 则侧重于生成可交互的 3D 视频，这表明两者在广阔的 3D 内容生成领域内有着略有不同的应用侧重点。

telegram · zaihuapd · Apr 16, 07:58

**背景**: 3D 高斯泼溅（3DGS）是一种用于实时辐射场渲染的技术，于 2023 年开始受到广泛关注，它能够从视频中重建高质量的 3D 场景。AI 世界模型是一种能理解真实世界动态（包括物理和空间属性）的神经网络，可以根据文本或视频等多种输入生成逼真的物理环境模拟。这些技术代表了 AI 从 2D 图像生成向理解和创建复杂、交互式 3D 空间迈进的前沿。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Gaussian_splatting">Gaussian splatting - Wikipedia</a></li>
<li><a href="https://www.nvidia.com/en-us/glossary/world-models/">What Is a World Model? | NVIDIA Glossary</a></li>

</ul>
</details>

**标签**: `#3D Generation`, `#AI Models`, `#Game Development`, `#Multimodal AI`, `#Digital Twins`

---

<a id="item-9"></a>
## [Qwen3.6-35B-A3B 开源发布：一款仅激活 3B 参数的稀疏 MoE 代理式编程模型](https://qwenlm.github.io/blog/qwen3.6-35b-a3b/) ⭐️ 8.0/10

Qwen 团队开源了 Qwen3.6-35B-A3B，这是一款稀疏混合专家模型，拥有 350 亿总参数，但在推理时仅激活 30 亿参数。官方宣称其在 SWE-bench、MCPMark 等编码与工具使用基准测试中显著优于前代模型，并能与部分更大规模的稠密模型竞争，同时保留了多模态理解与推理能力。 此次发布标志着面向软件工程的高效、强大 AI 智能体发展迈出了重要一步。该模型能以远低于典型稠密模型的计算成本，在复杂的现实世界编码任务上实现强劲性能，这使得强大的代理式编程能力对开发者和研究人员而言更加触手可及，有望加速 AI 与软件开发工作流的融合。 该模型专为“代理式编程”设计，在测试现实世界软件问题解决能力的 SWE-bench 和测试综合智能体能力的 MCPMark 等基准上表现出色。官方提供了开放的模型权重、支持自托管部署，并提供了兼容 OpenAI/Anthropic 风格的 API 接口，便于集成到 OpenClaw、Qwen Code 等现有的开发者工具链中。

telegram · zaihuapd · Apr 16, 13:59

**背景**: 稀疏混合专家模型是一种通过增加模型总参数量（容量）但不成比例增加每次输入计算成本的架构。与每次计算都使用全部参数的稠密模型不同，MoE 模型通过一个路由网络仅为每个输入激活一小部分“专家”，从而实现更快速、更高效的推理。SWE-bench 等基准测试用于评估模型解决来自 GitHub 的真实世界软件工程问题的能力，而 MCPMark 是一个较新的综合性基准，旨在通过多样化的现实任务对模型和智能体的能力进行压力测试。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arxiv.org/abs/2308.00951">[2308.00951] From Sparse to Soft Mixtures of Experts</a></li>
<li><a href="https://www.swebench.com/">SWE - bench Leaderboards</a></li>
<li><a href="https://mcpmark.ai/">MCPMark - Stress-Testing Comprehensive MCP Benchmark</a></li>

</ul>
</details>

**标签**: `#AI`, `#Large Language Models`, `#Open Source`, `#Mixture of Experts`, `#Code Generation`

---

<a id="item-10"></a>
## [Anthropic 发布 Claude Opus 4.6，支持 200K 上下文窗口和自适应思考模式。](https://t.me/zaihuapd/40903) ⭐️ 8.0/10

Anthropic 发布了新一代 Claude Opus 4.6 模型，将上下文窗口提升至 200K token（测试版提供 100 万 token），并将最大输出 token 数翻倍至 128K。该模型引入了自适应思考模式，可根据问题复杂度动态调整思考深度，并新增了最高级别的 'max effort' 参数。 此次更新显著增强了 Claude 处理长篇复杂文档和长时间对话的能力，使其在与 GPT 等其他领先模型的竞争中更具优势。自适应思考功能代表了 AI 推理向更自主、更高效方向的转变，有望减少开发者的猜测工作，并提升模型在复杂任务上的表现。 该模型还推出了上下文压缩功能，当对话接近窗口限制时会自动总结早期内容，从而实现近乎无限长度的对话。100 万 token 的上下文窗口目前处于测试阶段，这表明它是一项实验性功能，可能存在潜在限制。

telegram · zaihuapd · Apr 16, 14:28

**背景**: 大型语言模型（LLM）的上下文窗口是指模型在单次交互中能够处理和记忆的文本量，以 token 为单位计量，类似于人类的短期记忆。自适应思考是 AI 推理能力的一项演进，它让模型能够根据请求的复杂度，自行决定何时以及进行多长时间的深度、扩展性思考，从而改变了以往需要开发者手动设置固定思考预算的模式。上下文压缩是一种工程化技术，用于管理 AI 智能体中不断膨胀的对话历史，通过总结或修剪信息来保持在模型限制之内。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.mckinsey.com/featured-insights/mckinsey-explainers/what-is-a-context-window">What is a context window for Large Language Models? | McKinsey</a></li>
<li><a href="https://platform.claude.com/docs/en/build-with-claude/adaptive-thinking">Adaptive thinking - Claude API Docs</a></li>
<li><a href="https://medium.com/the-ai-forum/automatic-context-compression-in-llm-agents-why-agents-need-to-forget-and-how-to-help-them-do-it-43bff14c341d">Automatic Context Compression in LLM Agents: Why ... - Medium</a></li>

</ul>
</details>

**标签**: `#AI`, `#LLM`, `#Anthropic`, `#Claude`, `#Natural Language Processing`

---

<a id="item-11"></a>
## [谷歌发布 Gemini 3.1 Flash TTS，支持场景化提示控制](https://simonwillison.net/2026/Apr/15/gemini-31-flash-tts/#atom-everything) ⭐️ 7.0/10

谷歌发布了 Gemini 3.1 Flash TTS，这是一款新的文本转语音模型，可通过 Gemini API 使用模型 ID `gemini-3.1-flash-tts-preview` 进行访问。该模型的关键创新在于，它可以通过详细的场景设定提示来控制，这些提示描述了说话者的环境、声音风格、口音和情绪状态，如其官方提示指南所示。 这代表了 AI 语音合成领域的一个重要转变，从简单的语音选择转向可定向的、具有上下文感知的音频生成。它使创作者、开发者和媒体制作人能够为有声读物、游戏对话和动态媒体内容等应用生成高度细致和特定的语音表演，而无需手动进行音频编辑。 该模型目前仅输出音频文件，并且处于预览状态。根据谷歌的文档，Gemini 3.1 Flash TTS 支持 70 多种语言，并使用 SynthID 水印技术来识别 AI 生成的音频，以解决关于音频真实性和滥用的担忧。

rss · Simon Willison · Apr 15, 17:13

**背景**: 文本转语音（TTS）技术将书面文本转换为语音音频。传统的 TTS 模型通常提供有限的控制，例如从预定义的声音中选择或调整速度和音调等基本参数。Gemini API 是谷歌用于访问其大型语言和多模态模型系列的平台，现在包含了这个专门的 TTS 模型。使用详细的描述性提示进行生成的概念，灵感来源于 AI 图像和视频生成中使用的技术。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://ai.google.dev/gemini-api/docs/speech-generation">Text-to-speech generation (TTS) | Gemini API | Google AI for ...</a></li>
<li><a href="https://blog.google/innovation-and-ai/models-and-research/gemini-models/gemini-3-1-flash-tts/">Gemini 3.1 Flash TTS: New text-to-speech AI model - The Keyword</a></li>

</ul>
</details>

**标签**: `#AI`, `#text-to-speech`, `#Google`, `#Gemini`, `#speech-synthesis`

---

<a id="item-12"></a>
## [俄罗斯多款流行安卓应用被曝检测 VPN 状态并扫描外国应用，或响应政府限制指令](https://files.rks.global/russian_apps_search_for_vpn_en.pdf) ⭐️ 7.0/10

RKS Global 的一项研究发现，俄罗斯 30 款最流行的安卓应用中有 22 款具备 VPN 检测功能，其中 19 款会将 VPN 状态数据发送至服务器。此外，Avito 应用还被发现会扫描设备上是否安装了超过 200 种外国应用，包括银行、加密货币钱包和即时通讯工具。 这种由流行应用实施的系统性大规模监控，直接支持了政府限制 VPN 用户服务的指令，严重侵蚀了数百万俄罗斯公民的数字隐私。这是俄罗斯推行“数字主权”学说的具体步骤，旨在有效隔离用户与全球互联网，并实现国家对在线访问的控制。 此次检测和数据收集行为与俄罗斯数字发展部的要求相关，该部门已指示大型企业从 2026 年 4 月 15 日起，限制对启用 VPN 的用户提供服务。Avito 应用的扫描行为特别针对种类繁多的外国金融和通讯工具，这些工具常被用于绕过国内限制。

telegram · zaihuapd · Apr 16, 04:38

**背景**: 虚拟专用网络（VPN）通过加密用户流量并将其路由至其他位置的服务器，以隐藏用户的真实 IP 地址。VPN 通常用于增强隐私、访问受地域限制的内容或绕过网络审查。近年来，俄罗斯政府推行“数字主权”政策，寻求对境内互联网的更大控制，这包括限制 VPN 等可以绕过国家封锁的工具。安卓应用可以通过系统 API（例如通过 ConnectivityManager 检查活动网络的能力）来检测 VPN 的使用状态。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://rks.global/en/research/">RKS Global Researches</a></li>
<li><a href="https://blog.tarkalabs.com/the-ultimate-vpn-detection-guide-for-ios-and-android-313b521186cb">How to detect VPN usage on iOS and Android | Tarka Labs Blogs GitHub - s1mb1o/vpn-detector-android: Android app that ... Implementing VPN Detection in Mobile Applications: Client vs ... How to Detect VPNs Used With Android & iOS Apps Using AI How I Bypassed VPN Detection, Broke Client-Side ... - Medium VPNDroid: Malicious Android VPN Detection Using a CNN-RF ...</a></li>

</ul>
</details>

**标签**: `#privacy`, `#surveillance`, `#android-security`, `#vpn`, `#digital-rights`

---