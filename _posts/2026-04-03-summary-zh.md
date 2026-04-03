---
layout: default
title: "Horizon Summary: 2026-04-03 (ZH)"
date: 2026-04-03
lang: zh
---

> From 26 items, 13 important content pieces were selected

---

1. [谷歌发布 Gemma 4 开源模型，具备推理、多模态和工具调用能力。](#item-1) ⭐️ 9.0/10
2. [Google DeepMind 发布 Gemma 4，一个包含四款具备视觉和音频能力的高效开源模型家族。](#item-2) ⭐️ 9.0/10
3. [Google 发布 Gemma 4 开放模型家族，四款规格覆盖手机到工作站](#item-3) ⭐️ 9.0/10
4. [前 Azure 核心工程师详述侵蚀微软云平台信任的内部决策](#item-4) ⭐️ 8.0/10
5. [阿里通义千问发布 Qwen3.6-Plus，这是一款专注于现实世界智能体能力的托管式 AI 模型。](#item-5) ⭐️ 8.0/10
6. [智谱 AI 发布首款多模态编程基础模型 GLM-5V-Turbo，支持原生视觉编码与 Agent 协同。](#item-6) ⭐️ 8.0/10
7. [阿里巴巴发布新一代大语言模型 Qwen3.6-Plus，编程与多模态能力显著增强](#item-7) ⭐️ 8.0/10
8. [英伟达在中国 AI 芯片市场份额降至 55%，本土厂商合计占比 41%](#item-8) ⭐️ 8.0/10
9. [微软发布三款自研 AI 模型，覆盖转写、语音和图像生成。](#item-9) ⭐️ 8.0/10
10. [Nekogram 12.5.2 被曝存在后门，静默窃取用户手机号](#item-10) ⭐️ 8.0/10
11. [Cursor IDE 发布第 3 版，搭载 Composer 2 模型与智能体集群能力](#item-11) ⭐️ 7.0/10
12. [AMD 推出 Lemonade，一款适用于 GPU 和 NPU 的开源本地 LLM 服务器](#item-12) ⭐️ 7.0/10
13. [Simon Willison 在 Lenny 播客中探讨 AI 拐点与智能体工程](#item-13) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [谷歌发布 Gemma 4 开源模型，具备推理、多模态和工具调用能力。](https://deepmind.google/models/gemma/gemma-4/) ⭐️ 9.0/10

谷歌发布了 Gemma 4 系列开源模型，该系列模型具备思维/推理能力、多模态支持（视觉和音频）以及工具调用功能。模型提供四种规模：Effective 2B (E2B)、Effective 4B (E4B)、一个 260 亿参数的混合专家模型和一个 310 亿参数的密集模型。 此次发布代表了开源 AI 领域的重大进展，将前沿的多模态推理和智能体能力（通过工具调用）带到了可在消费级硬件上运行的模型中。这加剧了开源模型领域的竞争，特别是针对 Qwen 等其他领先模型，并为开发者提供了功能强大、可本地部署的 AI 工具。 关键的技术创新包括共享 KV 缓存以减少内存开销、保留图像原始宽高比的视觉编码器，以及在较小模型中采用的 Per-Layer Embeddings (PLE)以提高效率。早期的社区基准测试显示，310 亿参数模型取得了强劲的分数（例如在 MMLU 上达到 88.4%），不过有用户报告特定模型变体存在问题，例如在某些设置下 310 亿参数模型会输出重复文本。

hackernews · jeffmcjunkin · Apr 2, 16:10

**背景**: Gemma 是谷歌推出的轻量级开源语言模型系列，旨在高效且易于获取。'开源模型'指的是权重公开发布的 AI 模型，允许修改和本地部署。'工具调用'是一种让 AI 模型能够与外部工具和 API 交互以执行超越文本生成任务的能力，这对于构建自主 AI 智能体至关重要。参数规模（例如 20 亿、310 亿）指的是模型中可训练变量的数量，通常与其能力和计算需求相关。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://deepmind.google/models/gemma/gemma-4/">Gemma 4 — Google DeepMind</a></li>
<li><a href="https://blog.google/innovation-and-ai/technology/developers-tools/gemma-4/">Gemma 4: Byte for byte, the most capable open models</a></li>
<li><a href="https://huggingface.co/blog/gemma4">Welcome Gemma 4: Frontier multimodal intelligence on device</a></li>

</ul>
</details>

**社区讨论**: 社区正在积极测试这些模型，分享量化版本以便于本地使用，并提供具体的配置建议（例如 temperature=1.0）。用户们分享了与 Qwen 3.5 等模型的基准测试对比，并报告了在图像生成方面的不同体验，有人称赞 260 亿参数模型在笔记本电脑上的输出质量，也有人指出 310 亿参数模型在本地运行中存在缺陷。讨论重点集中在实际应用和即时性能验证上。

**标签**: `#open-source-ai`, `#llm`, `#multimodal-ai`, `#reasoning-models`, `#model-benchmarks`

---

<a id="item-2"></a>
## [Google DeepMind 发布 Gemma 4，一个包含四款具备视觉和音频能力的高效开源模型家族。](https://simonwillison.net/2026/Apr/2/gemma-4/#atom-everything) ⭐️ 9.0/10

Google DeepMind 发布了 Gemma 4，这是一个在 Apache 2.0 许可证下发布的包含四款新模型的开源家族，模型规模包括 2B、4B、31B 以及一个 26B-A4B 的混合专家模型变体。这些模型具备视觉能力，其中两款较小的模型（E2B 和 E4B）采用了逐层嵌入技术以提高参数效率，并具备原生音频输入功能，可用于语音识别。 此次发布代表了在创建用于设备端部署的小型高性能模型方面取得了重大进展，推动了参数效率智能的前沿。Apache 2.0 许可证和多模态能力（视觉、音频）使这些模型对于需要本地、高效 AI 的应用开发者来说极具可访问性和实用性。 较小的 E2B 和 E4B 模型使用了逐层嵌入技术，其中每个解码器层为每个令牌都有自己的小型嵌入表，这使得其'有效'参数数量远少于总参数。虽然在 LM Studio 等本地测试工具中，2B、4B 和 26B-A4B 模型运行正常，但据报道 31B 模型存在问题，会输出重复的错误字符串。

rss · Simon Willison · Apr 2, 18:28

**背景**: 逐层嵌入是一种旨在提高小型模型参数效率的技术，尤其适用于设备端部署。与所有层共享一个大型嵌入表不同，PLE 为每个 Transformer 解码器层提供其自身的小型嵌入表，从而减少了推理过程中的活跃或'有效'参数。混合专家模型是一种使用多个专用子网络来处理输入不同部分的架构，它允许模型拥有更大的容量，而无需为每个输入按比例增加计算量。追求高性能的小型语言模型是一个主要的研究领域，旨在提供能够在消费级硬件上运行的强大 AI。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://huggingface.co/blog/rishiraj/matformer-in-gemma-3n">Understanding Gemma 3n: How MatFormer Gives You Many Models ...</a></li>
<li><a href="https://medium.com/@tahirbalarabe2/what-is-mixture-of-experts-moe-architecture-models-and-applications-ca86f8beb58c">What is Mixture of Experts ( MOE ): Architecture , Models... | Medium</a></li>
<li><a href="https://arxiv.org/html/2501.05465v1">Small Language Models (SLMs) Can Still Pack a Punch: A survey</a></li>

</ul>
</details>

**标签**: `#llm`, `#open-source`, `#model-efficiency`, `#computer-vision`, `#google-deepmind`

---

<a id="item-3"></a>
## [Google 发布 Gemma 4 开放模型家族，四款规格覆盖手机到工作站](https://blog.google/innovation-and-ai/technology/developers-tools/gemma-4/) ⭐️ 9.0/10

Google 发布了 Gemma 4 开放模型家族，提供 E2B、E4B、26B MoE 和 31B Dense 四款规格，均采用 Apache 2.0 许可证。该系列针对从 Android 设备、笔记本 GPU 到开发工作站和加速器等不同硬件进行了优化，主打高级推理、Agent 工作流和多模态能力。 此次发布通过提供一套能在从手机到工作站等消费级硬件上高效运行的顶级开放模型，显著推进了高性能、易获取 AI 的发展。转向标准的 Apache 2.0 许可证消除了先前的许可障碍，使开发者和企业更容易采用并基于这些模型进行构建，有望加速边缘 AI 和本地部署领域的创新。 较小的 E2B 和 E4B 模型专为设备端离线运行设计，支持 128K 上下文窗口，而较大的模型最高支持 256K 上下文。31B Dense 模型在 Arena AI 文本榜单的开放模型中排名第 3，26B MoE 模型排名第 6，展现了强大的基准测试性能。这些模型支持函数调用、结构化 JSON 输出、代码生成以及图像/视频处理，其中 E2B/E4B 还支持原生音频输入。

telegram · zaihuapd · Apr 2, 16:12

**背景**: Gemma 是 Google 的开放、轻量级大语言模型（LLM）家族。26B 变体采用的混合专家（MoE）架构是一种通过针对每个输入仅激活一部分‘专家’神经网络，从而在保持单次推理计算成本相对较低的同时大幅增加模型总参数量的设计。Apache 2.0 许可证是一种宽松的开源许可证，允许在最小限制下广泛使用、修改和分发。Arena AI 是一个流行的社区驱动平台，基于真实用户评估对 AI 模型进行基准测试和排名。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arxiv.org/abs/2507.11181">[2507.11181] Mixture of Experts in Large Language Models - arXiv</a></li>
<li><a href="https://venturebeat.com/technology/google-releases-gemma-4-under-apache-2-0-and-that-license-change-may-matter">Google releases Gemma 4 under Apache 2.0 — and that license ...</a></li>
<li><a href="https://arena.ai/">Arena AI: The Official AI Ranking & LLM Leaderboard</a></li>

</ul>
</details>

**标签**: `#open-source-ai`, `#large-language-models`, `#google-research`, `#edge-ai`, `#model-optimization`

---

<a id="item-4"></a>
## [前 Azure 核心工程师详述侵蚀微软云平台信任的内部决策](https://isolveproblems.substack.com/p/how-microsoft-vaporized-a-trillion) ⭐️ 8.0/10

一位前 Azure 核心工程师发表了一份详细报告，阐述了据其称导致 Azure 平台产生重大技术债务、用户体验不佳并侵蚀客户信任的微软内部决策和文化问题。该工程师声称已于 2025 年初将相关问题上报给 CEO 萨提亚·纳德拉和董事会，但未得到回应。 这一内部视角罕见地揭示了全球最大云平台之一所面临的操作和技术挑战，可能影响企业的采购决策和开发者的平台偏好。如果指控属实，则表明 Azure 在开发和管理方面存在系统性问题，可能影响其与 AWS 和 Google Cloud 的竞争力。 作者特别批评了 Azure 的用户界面是'勉强拼凑的混乱系统'，其文档由 AI 生成且经常出错，以及其服务产品过于复杂令人难以选择。文章还将微软 2025 年的大规模裁员（约 15,000 个岗位）与据称与 CoreWeave 交易后带来的财务压力联系起来。

hackernews · axelriet · Apr 2, 16:00

**背景**: Microsoft Azure 是公司的云计算平台，提供虚拟机、网站和 AI 工具等服务。Azure 核心工程团队历史上属于云和企业部门，后来经过扩展，负责该平台的核心应用程序和基础设施。技术债务指的是现在选择简单、有限的解决方案而非需要更长时间但更好的方法所导致的未来返工的隐含成本，这在云平台等大型、快速发展的软件项目中容易累积。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Microsoft_engineering_groups">Microsoft engineering groups - Wikipedia</a></li>
<li><a href="https://aws.amazon.com/blogs/mt/reversing-technical-debt-with-cloud/">Reversing Technical Debt with Cloud | AWS Cloud Operations Blog</a></li>
<li><a href="https://www.clouddatainsights.com/how-to-eradicate-technical-debt-in-the-cloud-lessons-from-devops/">How to Eradicate Technical Debt in the Cloud: Lessons from DevOps - CDInsights</a></li>

</ul>
</details>

**社区讨论**: 社区情绪很大程度上验证了文章的说法，许多用户分享了他们使用 Azure 界面、文档和服务可靠性时的挫败经历。一些评论者认为该工程师的描述可信且符合他们的专业观察，而另一些人则质疑作者的动机，但也承认所描述的问题具有合理性。讨论还延伸至对企业裁员与战略性财务操作相关的担忧。

**标签**: `#cloud-computing`, `#microsoft`, `#software-engineering`, `#devops`, `#corporate-culture`

---

<a id="item-5"></a>
## [阿里通义千问发布 Qwen3.6-Plus，这是一款专注于现实世界智能体能力的托管式 AI 模型。](https://qwen.ai/blog?id=qwen3.6) ⭐️ 8.0/10

阿里通义千问团队发布了新的旗舰大语言模型 Qwen3.6-Plus，该模型仅通过 API 作为托管服务提供。该模型特别定位为具备增强的“智能体”能力，旨在规划和执行现实世界中的多步骤任务，并默认具备 100 万 token 的上下文长度。 此次发布标志着以开源模型闻名的通义千问团队一次重大的战略转变，开始直接与 Anthropic 的 Claude 和 OpenAI 的 ChatGPT 等领先的商业托管式模型竞争。其专注于现实世界智能体能力，瞄准了 AI 行业向能够自主执行复杂、实际任务发展的关键趋势，可能影响编程、客户支持和流程自动化等领域。 与之前大多数通义千问模型不同，Qwen3.6-Plus 并非开源权重模型，其参数数量也未公开。其初步的基准测试比较因针对的是竞争对手的旧版本（例如 Claude 3.5 Opus 而非更新的 Claude 3.6）而引发了社区审视。

hackernews · pretext · Apr 2, 14:28

**背景**: 通义千问（Qwen）是阿里云开发的一系列大语言模型。历史上，其许多模型都以“开源权重”形式发布，意味着其模型权重可供公开下载和本地部署。“AI 智能体”指的是能够自主感知环境、做出决策并采取行动以实现目标的 AI 系统，通常通过使用工具和分解复杂任务来实现。“仅托管”或“闭源”模型是指只能通过开发者提供的云 API 访问的模型，这与用户可以自行在基础设施上运行的开源权重模型形成对比。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://medium.com/@mehulgupta_7991/qwen3-6-plus-the-first-real-agentic-llm-c0d564450adc">Qwen3.6-Plus: The First Real “Agentic” LLM? | by Mehul Gupta</a></li>
<li><a href="https://www.constellationr.com/insights/news/alibabas-qwen-launches-new-flagship-llm-qwen-36-plus">Alibaba's Qwen launches new flagship LLM with Qwen 3.6-Plus</a></li>
<li><a href="https://www.ibm.com/think/topics/ai-agents">What Are AI Agents? | IBM</a></li>

</ul>
</details>

**社区讨论**: 社区反应不一，显著的批评集中在通义千问从开源权重提供者转向仅托管服务的战略转变上，一些用户认为这是在利用开源模型获得知名度后的“诱饵调包”策略。此外，对于其基准测试与稍显过时的竞争对手模型进行比较的公平性也存在争论。不过，也有评论者为这些比较辩护，指出 AI 领域的发布周期非常快。

**标签**: `#artificial-intelligence`, `#llm`, `#qwen`, `#ai-agents`, `#machine-learning`

---

<a id="item-6"></a>
## [智谱 AI 发布首款多模态编程基础模型 GLM-5V-Turbo，支持原生视觉编码与 Agent 协同。](https://docs.bigmodel.cn/cn/update/new-releases) ⭐️ 8.0/10

智谱 AI 发布了其首款多模态编程基础模型 GLM-5V-Turbo，该模型原生支持图像、视频、文本等多模态输入，并针对 Agent 协同进行了深度优化。该模型旨在完成“理解环境—规划动作—执行任务”的完整 Agent 闭环，并针对 Claude Code、OpenClaw 等 Agent 进行了优化。 此次发布标志着面向复杂软件工程任务（如 GUI 自主探索和代码调试）的、更自主、更强大的 AI 系统迈出了重要一步。通过将原生多模态理解与 Agent 协同相结合，该模型有望加速开发能够直接与数字环境交互和操作的 AI 驱动工具。 该模型是更广泛模型家族升级的一部分，同期升级的还包括 GLM-4-Air/Flash 基座模型、GLM-Z1 系列推理模型以及支持多引擎切换的 AI 搜索工具。它扩展了多模态工具链，具备画框、截图、读网页（含图片识别）等能力。

telegram · zaihuapd · Apr 2, 01:48

**背景**: 多模态基础模型是经过训练以理解和生成跨不同数据类型（如文本、图像和代码）内容的 AI 系统。“原生视觉编码”指的是一种模型架构设计，即模型从底层就被设计为将视觉输入作为主要数据进行处理，而非依赖于分离的、预处理的视觉特征。AI Agent 是能够通过推理、规划和行动来自主执行任务的系统，其协同工作是处理编码等复杂应用的一个日益增长的模式。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://docs.z.ai/guides/vlm/glm-5v-turbo">GLM-5V-Turbo - Overview - Z.AI DEVELOPER DOCUMENT</a></li>
<li><a href="https://research.google/blog/towards-a-science-of-scaling-agent-systems-when-and-why-agent-systems-work/">Towards a science of scaling agent systems - Google Research</a></li>

</ul>
</details>

**标签**: `#Multimodal AI`, `#Foundation Models`, `#AI Programming`, `#Visual Encoding`, `#AI Agents`

---

<a id="item-7"></a>
## [阿里巴巴发布新一代大语言模型 Qwen3.6-Plus，编程与多模态能力显著增强](https://t.me/zaihuapd/40658) ⭐️ 8.0/10

阿里巴巴发布了新一代千问大语言模型 Qwen3.6-Plus。该模型具备原生多模态理解和推理能力，在 SWE-bench、Claw-Eval 等权威评测中，其编程表现已接近全球顶尖的 Claude 系列模型，并能通过自主任务拆解与规划，实现“氛围编程”，即用一句话驱动 AI 完成复杂代码编写。 此次发布标志着阿里巴巴 AI 能力的一次重大飞跃，使千问模型在编程和智能体任务这一关键领域成为全球领先模型的有力竞争者。其增强的自主编码和多模态推理能力有望加速软件开发流程，并拓展 AI 智能体在真实世界环境中的实际应用。 该模型的性能在 SWE-bench（测试解决真实 GitHub 问题的能力）和 Claw-Eval（评估 LLM 在实时操作环境中的智能体表现）等基准测试中得到突出体现。其宣称的“氛围编程”能力使模型能够针对前端网页开发、仓库级复杂任务等场景，自主进行任务拆解、路径规划、测试修改直至完成。

telegram · zaihuapd · Apr 2, 05:02

**背景**: SWE-bench 是一个基准测试，用于评估大语言模型解决来自 GitHub 的真实世界软件工程问题的能力。Claw-Eval 是一个较新的基准，旨在评估 LLM 作为智能体的表现，重点关注其在实时操作环境中的性能，而非单纯的知识回忆。'氛围编程'似乎是阿里巴巴使用的一个术语，用于描述由先进 AI 智能体实现的、高度自主的、由自然语言驱动的编码工作流程。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.swebench.com/">SWE-bench</a></li>
<li><a href="https://github.com/swe-bench/SWE-bench">SWE-bench: Can Language Models Resolve Real-world Github Issues?</a></li>
<li><a href="https://github.com/claw-eval/claw-eval">GitHub - claw - eval / claw - eval : Claw - Eval is an evaluation harness for...</a></li>

</ul>
</details>

**标签**: `#AI`, `#Large Language Models`, `#Programming`, `#Multimodal AI`, `#Alibaba`

---

<a id="item-8"></a>
## [英伟达在中国 AI 芯片市场份额降至 55%，本土厂商合计占比 41%](https://www.tomshardware.com/tech-industry/nvidia-market-share-in-china-falls-to-less-than-60-percent-chinese-chip-makers-deliver-1-65-million-ai-gpus-as-the-government-pushes-data-centers-to-use-domestic-chips) ⭐️ 8.0/10

2025 年，英伟达在中国 AI 芯片市场的份额已从制裁前的 95%大幅降至 55%，全年出货约 220 万块；中国本土芯片厂商合计拿下 41%的市场份额，共交付 165 万块 AI GPU。其中华为表现最为突出，出货约 81.2 万块，占比近 20%，并于上周发布了性能号称接近英伟达 H20 三倍的 Atlas 350 加速器。 这一变化标志着在地缘政治紧张和国家政策驱动下，全球 AI 硬件供应链发生重大重组，降低了中国对外国技术的依赖。以华为昇腾系列为代表的国产替代品快速增长，可能加速形成一个以中国为中心的平行 AI 生态系统，对全球科技竞争格局产生深远影响。 阿里旗下平头哥以 25.6 万块的出货量位居本土厂商第三，AMD、百度昆仑芯和寒武纪紧随其后。作为对比基准的英伟达 H20 GPU 属于 Hopper 架构，是一款仅支持 PCIe 的 GPU，专为推理和小规模工作负载设计。

telegram · zaihuapd · Apr 2, 06:08

**背景**: AI GPU（如图形处理器）是专门用于训练和运行大型人工智能模型的处理器，英伟达在此领域曾占据主导地位。近年来，美国的出口限制措施制约了先进 AI 芯片对华销售，创造了市场空白。与此同时，中国政府推行了鼓励数据中心采用国产芯片的政策导向，以培育本土半导体企业的发展。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://awesomeagents.ai/hardware/huawei-atlas-350/">Huawei Atlas 350 - China's FP4 Inference Accelerator</a></li>
<li><a href="https://getdeploying.com/gpus/nvidia-h20">Nvidia H20 - GetDeploying</a></li>
<li><a href="https://www.t-head.cn/">平头哥半导体</a></li>

</ul>
</details>

**标签**: `#AI Chips`, `#Semiconductor Industry`, `#Geopolitics`, `#Market Analysis`, `#Hardware`

---

<a id="item-9"></a>
## [微软发布三款自研 AI 模型，覆盖转写、语音和图像生成。](https://venturebeat.com/technology/microsoft-launches-3-new-ai-models-in-direct-shot-at-openai-and-google) ⭐️ 8.0/10

微软于 4 月 2 日发布了三款完全自研的基础 AI 模型：语音转写模型 MAI-Transcribe-1、语音生成模型 MAI-Voice-1 和图像生成模型 MAI-Image-2。这些模型已通过 Microsoft Foundry 平台和新的 MAI Playground 上线。 此次发布是微软在核心且具有高商业价值的企业 AI 应用领域，直接与 OpenAI 和谷歌等领先 AI 提供商竞争的重要战略举措。通过提供高性能的自研转录、语音合成和图像生成模型，微软增强了其全栈 AI 产品能力，并减少了对关键技术的对外部合作伙伴的依赖。 微软声称，MAI-Transcribe-1 在 FLEURS 基准测试覆盖的 25 种主要语言上平均词错误率为 3.8%，全面领先于 OpenAI 的 Whisper-large-v3。MAI-Voice-1 可在单个 GPU 上 1 秒内生成 60 秒语音，并支持用数秒音频定制声音。MAI-Image-2 在 Foundry 和 Copilot 中的生成速度较前代至少提升 2 倍，并已开始向 Bing 和 PowerPoint 推出。

telegram · zaihuapd · Apr 2, 11:31

**背景**: Microsoft Foundry（前身为 Azure AI Studio）是一个用于构建、定制和扩展生成式 AI 应用程序的统一平台。FLEURS（Few-shot Learning Evaluation of Universal Representations of Speech）基准测试是一个多语言语音数据集，用于评估跨多种语言的语音识别模型。OpenAI 的 Whisper 是一个广泛使用的开源语音识别模型，Whisper-large-v3 是其近期发布的高性能版本。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://microsoft.ai/news/today-were-announcing-3-new-world-class-mai-models-available-in-foundry/">Today we're announcing 3 new world class MAI models... | Microsoft AI</a></li>
<li><a href="https://research.google/pubs/fleurs-few-shot-learning-evaluation-of-universal-representations-of-speech/">FLEURS: Few-shot Learning Evaluation of Universal ...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Whisper_(speech_recognition_system)">Whisper (speech recognition system) - Wikipedia</a></li>

</ul>
</details>

**标签**: `#AI Models`, `#Microsoft`, `#Speech Recognition`, `#Image Generation`, `#Enterprise AI`

---

<a id="item-10"></a>
## [Nekogram 12.5.2 被曝存在后门，静默窃取用户手机号](https://thebadinteger.github.io/nekogram-phone-exfiltration/) ⭐️ 8.0/10

安全研究人员发现，第三方 Telegram 客户端 Nekogram 12.5.2（Google Play 版）内置后门代码，会在用户不知情的情况下收集所有已登录账号的手机号，并通过 Inline Query 外传至开发者控制的 Bot（@nekonotificationbot）。该后门仅存在于编译发布的 APK 中，GitHub 公开源码中的对应文件为无害占位。 这一事件对一款流行开源应用的用户构成了严重的信任与隐私侵犯，它展示了恶意代码如何能在源代码看似干净的情况下被植入分发的二进制文件中。这凸显了使用第三方客户端访问敏感通信平台的风险，并强调了将编译后的应用与其源代码进行完整性验证的重要性。 后门代码位于 Extra.java（混淆后为 uo5）中，其核心逻辑是遍历 8 个账号槽位，提取用户 ID 与手机号，拼接密钥后以 Inline Query 发送，所有关键字符串均经过自定义加密混淆。开发者回应称 Bot 仅用于“解析用户名”，但代码中明确提取了 phone 字段并使用无痕传输方式，与其说辞不符。

telegram · zaihuapd · Apr 2, 12:58

**背景**: Nekogram 是一款开源的第三方 Telegram 客户端，以其提供官方应用所没有的实用修改而闻名。Telegram 机器人可以运行在“inline”模式下，允许用户在任何聊天的文本输入框中直接输入机器人的用户名和查询来与之交互；该功能在此次事件中被用于隐秘地外传数据。APK 反编译是一种从 Android 应用的编译包（.apk 文件）中恢复其源代码的逆向工程过程，研究人员正是通过此方法验证了公开源代码与分发二进制文件之间的差异。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/Nekogram/Nekogram">GitHub - Nekogram/Nekogram: Open-source third-party Telegram ...</a></li>
<li><a href="https://core.telegram.org/bots/inline">Inline Bots</a></li>
<li><a href="https://hackernoon.com/apk-decompilation-a-beginners-guide-for-reverse-engineers">APK Decompilation : A Beginner's Guide for Reverse... | HackerNoon</a></li>

</ul>
</details>

**标签**: `#security`, `#privacy`, `#telegram`, `#malware`, `#mobile-security`

---

<a id="item-11"></a>
## [Cursor IDE 发布第 3 版，搭载 Composer 2 模型与智能体集群能力](https://cursor.com/blog/cursor-3) ⭐️ 7.0/10

Cursor 宣布了其 AI 驱动的集成开发环境（IDE）的第 3 版，引入了新的 Composer 2 模型和多智能体“集群”协作功能。此次更新标志着开发环境向更具自主性和协作性的方向迈出了重要一步。 此次发布之所以重要，是因为它将 AI 辅助开发的前沿从简单的代码补全，推向了由协调的 AI 智能体进行复杂、多步骤问题解决的新阶段。它可能通过自动化软件开发生命周期中更大部分的工作，从根本上改变开发者的工作流程，从而潜在地提高处理复杂项目的团队和个人的生产力。 Composer 2 模型专为“智能体软件工程”设计，强调长期规划和编码智能。新的“智能体集群”功能允许多个 AI 智能体在共享工作区内同时处理一个功能的不同方面，并协调彼此的工作。

hackernews · adamfeldman · Apr 2, 18:13

**背景**: Cursor 是一个 AI 优先的集成开发环境（IDE），它将代码生成、解释和重构等 AI 能力深度集成到编码工作流中。在此语境下，“AI 智能体”是一种能够理解开发者意图、规划任务并执行代码更改的自主程序。“智能体式”IDE 代表了一类新工具，其中 AI 扮演着更主动、基于规划的角色，而不仅仅是对提示做出反应。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://cursor.com/resources/Composer2.pdf">Composer 2 Technical Report</a></li>
<li><a href="https://www.programming-helper.com/tech/cursor-2026-ai-first-ide-composer-agents-python">Cursor 2026: How the AI-First IDE Redefined Developer ...</a></li>
<li><a href="https://www.builder.io/blog/agentic-ide">The best agentic IDEs heading into 2026</a></li>

</ul>
</details>

**社区讨论**: 社区讨论显示出复杂的反应。一些高级用户赞扬 Composer 2 的直观性和效率，即使它不如 OpenAI 或 Anthropic 的旗舰模型那么“智能”。然而，用户也提出了重大关切，包括企业版计划的高昂成本、对 IDE 设计方向从“代码优先”转向“聊天优先”的担忧，以及对“智能体集群”相较于更简单的单智能体工作流之实用价值的怀疑。

**标签**: `#AI-assisted-development`, `#IDE`, `#developer-tools`, `#code-generation`, `#product-announcement`

---

<a id="item-12"></a>
## [AMD 推出 Lemonade，一款适用于 GPU 和 NPU 的开源本地 LLM 服务器](https://lemonade-server.ai/) ⭐️ 7.0/10

AMD 正式发布了一款名为 Lemonade 的开源本地 LLM 服务器，它支持在 AMD 硬件上使用 GPU（通过 ROCm 或 Vulkan）和 NPU 运行大语言模型，并能处理文本、图像和音频生成任务。该项目旨在简化在 AMD 系统上进行本地 AI 推理通常复杂的设置过程。 这具有重要意义，因为它代表了 AMD 官方对一个统一的本地 AI 开源解决方案的支持，这可能会极大地改善 AMD 硬件上的开发者和用户体验，尤其是考虑到 ROCm 部署的历史性挑战。通过提供一个能协调多种 AI 模态（文本、图像、音频）的单一服务器，它解决了碎片化的本地 AI 工具生态中的一个关键痛点。 该服务器支持多种后端（ROCm、Vulkan、CPU）和硬件目标（GPU、NPU），但一个值得注意的细节是，它使用的 NPU 模型和内核是专有的，并非开源。社区反馈表明，虽然该工具前景看好，但就推理而言，Ryzen AI NPU 的实际性能和吞吐量目前可能仍比使用独立显卡（dGPU）有限。

hackernews · AbuAssar · Apr 2, 11:04

**背景**: 在个人电脑上本地运行 AI 模型已变得越来越流行，Ollama 和 LM Studio 等工具允许用户运行语言模型而无需依赖云端。本地 LLM 服务器充当托管和提供这些模型的后端。对于 AI 推理，会使用 GPU（图形处理器）和 NPU（神经网络处理器）等硬件加速器；GPU 是功能强大的通用并行处理器，而 NPU 专为神经网络任务设计，对于某些工作负载可能更节能。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://dev.to/primghostdev/run-your-own-ai-model-locally-a-practical-ollama-setup-guide-2026-2kk9">Run Your Own AI Model Locally: A Practical Ollama Setup Guide ...</a></li>
<li><a href="https://contabo.com/blog/npu-vs-gpu/">NPU vs GPU : Differences in AI Processing | Contabo Blog</a></li>

</ul>
</details>

**社区讨论**: 社区反应总体上是积极的，用户验证了该工具在简化 AMD 硬件上 ROCm 体验方面的实用性。关键的讨论点包括与 Ollama 和 LM Studio 等替代方案的实用性比较，Lemonade 被视为一个更统一的“运行时”。关于 NPU 与独立显卡在实际应用中的性能存在积极辩论，一些用户发现 NPU 是瓶颈，并有人指出 NPU 组件并非开源。

**标签**: `#llm-inference`, `#amd-hardware`, `#open-source`, `#local-ai`, `#model-serving`

---

<a id="item-13"></a>
## [Simon Willison 在 Lenny 播客中探讨 AI 拐点与智能体工程](https://simonwillison.net/2026/Apr/2/lennys-podcast/#atom-everything) ⭐️ 7.0/10

Simon Willison 发布了他近期在 Lenny Rachitsky 播客中亮相的要点总结，他们讨论了以 GPT-5.1 和 Claude Opus 4.5 为标志的 2025 年 11 月 AI 拐点、'暗工厂'概念，以及软件开发中不断演进的智能体工程实践。 这次讨论之所以重要，是因为它捕捉到了一个关键转折点：AI 编程智能体从不可靠的助手转变为持续高效的工具，这标志着软件开发方式的根本性转变，并预示着自动化将对更广泛的信息工作产生深远影响。 Willison 指出，2025 年 11 月的拐点特征是，AI 生成的代码从'大部分能用但需要仔细检查'转变为'几乎总是能完成你的指令'。他还强调，开发中的主要瓶颈现已从编写代码转移到了测试和评估环节。

rss · Simon Willison · Apr 2, 20:40

**背景**: 智能体工程指的是在 AI 编程智能体的辅助下进行软件开发，并将其集成到现有工作流程中的实践。'暗工厂'是指无需现场人工干预即可运行的全自动化制造工厂，这一概念现在被类比应用于软件开发。讨论中提到的'拐点'源于 2025 年 11 月同时发布的、性能显著提升的 AI 模型（GPT-5.1 和 Claude Opus 4.5），这些模型极大地提高了代码生成的可靠性。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://simonwillison.net/guides/agentic-engineering-patterns/what-is-agentic-engineering/">What is agentic engineering? - Simon Willison's Weblog</a></li>
<li><a href="https://spikestory.com/en/dark-factories-ai-powered-manufacturing/">Dark Factories : The Future of Smart Manufacturing with... - Spike Story</a></li>
<li><a href="https://simonwillison.net/2026/Jan/4/inflection/">The November 2025 inflection point - Simon Willison's Weblog</a></li>

</ul>
</details>

**标签**: `#AI`, `#Agentic Engineering`, `#Software Engineering`, `#Automation`, `#Podcast`

---