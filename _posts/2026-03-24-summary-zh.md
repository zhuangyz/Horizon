---
layout: default
title: "Horizon Summary: 2026-03-24 (ZH)"
date: 2026-03-24
lang: zh
---

> From 24 items, 4 important content pieces were selected

---

1. [iPhone 17 Pro 演示运行 4000 亿参数大语言模型](#item-1) ⭐️ 8.0/10
2. [Autoresearch：一个利用 LLM 实现自动化代码改进与实验的系统](#item-2) ⭐️ 7.0/10
3. [科技企业将绩效考核与员工消耗的 LLM token 数量挂钩](#item-3) ⭐️ 7.0/10
4. [OpenAI 建议英国将 AI 聊天机器人纳入 Google 搜索选择页](#item-4) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [iPhone 17 Pro 演示运行 4000 亿参数大语言模型](https://twitter.com/anemll/status/2035901335984611412) ⭐️ 8.0/10

一则演示显示，一个拥有 4000 亿参数的大语言模型在 iPhone 17 Pro 上运行。社区讨论澄清，该模型采用了混合专家架构，并涉及量化技术才得以实现。 这一演示代表了设备端人工智能的重大进展，突破了移动硬件能力的边界。它预示着一个未来：强大的 AI 助手可以完全在本地运行，从而增强隐私性、降低延迟，并在无需持续云端连接的情况下启用新的应用。 该模型是一个混合专家模型，这意味着其 4000 亿的参数是稀疏的；每次推理时只有一小部分参数被激活，从而提高了效率。演示还依赖于量化技术，这是一种通过降低模型权重的数值精度来减少其内存占用和计算需求的压缩方法。

hackernews · anemll · Mar 23, 14:30

**背景**: 大语言模型是在海量文本数据上训练的 AI 系统，其能力通常随参数数量增加而提升。在内存和处理能力有限的移动设备上运行此类模型具有挑战性。混合专家架构是一种模型设计，其中模型由许多子网络（'专家'）组成，一个路由网络为每个输入选择少数几个相关的专家，从而实现巨大的总参数量，同时每个词元的计算成本可控。量化是一种通过使用更少的比特（例如，用 4 位整数代替 16 位浮点数）来表示神经网络权重，从而压缩模型的技术，它能显著减小模型大小并加速推理，通常精度损失很小。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arxiv.org/abs/2507.11181">[2507.11181] Mixture of Experts in Large Language Models</a></li>
<li><a href="https://huggingface.co/blog/moe">Mixture of Experts Explained - Hugging Face</a></li>
<li><a href="https://blog.premai.io/llm-quantization-guide-gguf-vs-awq-vs-gptq-vs-bitsandbytes-compared-2026/">LLM Quantization Guide: GGUF vs AWQ vs GPTQ vs bitsandbytes ...</a></li>

</ul>
</details>

**社区讨论**: 社区情绪复杂，既有技术上的审视，也有更广泛的担忧。从技术角度看，评论者指出，标题具有误导性，因为它没有提及对在手机上运行 4000 亿参数模型至关重要的混合专家架构和量化技术；一位用户指出，这样的模型其行为可能更像一个参数少得多的稠密模型。其他评论则对持续推理导致的设备过热以及更广泛的社会影响（如加剧手机成瘾）表示担忧。

**标签**: `#on-device-ai`, `#llm`, `#mobile-computing`, `#quantization`, `#apple`

---

<a id="item-2"></a>
## [Autoresearch：一个利用 LLM 实现自动化代码改进与实验的系统](https://ykumar.me/blog/eclip-autoresearch/) ⭐️ 7.0/10

一篇博客文章详细介绍了一个自动化研究系统，该系统利用大语言模型（LLM）以循环方式迭代改进代码、运行实验并评估结果。该系统的核心是一个单一的系统提示（program.md），它指示智能体反复改进训练脚本、执行训练、运行评估并记录结果。 这展示了 LLM 智能体在自动化和加速研发周期（尤其是在机器学习领域）的实际应用。它可以显著减少代码优化和超参数探索等任务所需的人工投入，有可能更快地发现最优解决方案。 该系统被描述为像一个内置了基本推理能力的超参数优化算法，在其迭代循环中倾向于简单性。社区的一个关键见解是，在不同迭代中使用不同的 LLM 模型可能是有益的，类似于为问题获得一个新的视角。

hackernews · ykumards · Mar 23, 18:40

**背景**: LLM 智能体是一种人工智能系统，它使用大语言模型作为核心推理引擎，来规划和执行一系列以实现目标（如进行研究或编写代码）为导向的行动。自动化研究框架旨在覆盖从构思、实验到分析等主要研究阶段。超参数优化是为机器学习模型寻找最佳配置参数的过程，这通常是一项耗时的手动任务。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://agentlaboratory.github.io/">Agent Laboratory: Using LLMs as Research Assistants</a></li>
<li><a href="https://deepwiki.com/karpathy/autoresearch">karpathy/autoresearch | DeepWiki</a></li>
<li><a href="https://arxiv.org/html/2312.04528v2">Using Large Language Models for Hyperparameter Optimization</a></li>

</ul>
</details>

**社区讨论**: 社区讨论强调了实际应用，并对效率提出了疑问。一些用户将该系统与成熟的超参数优化技术进行比较，并质疑其新颖性，而另一些用户则分享了他们自己使用 LLM 进行现有技术探索或迭代代码调试的经验。一个反复出现的主题是自动化探索的潜力与让智能体尝试所有 LLM 建议的想法所带来的成本（计算和财务）之间的平衡。

**标签**: `#LLM-agents`, `#automated-research`, `#machine-learning`, `#code-generation`, `#hyperparameter-optimization`

---

<a id="item-3"></a>
## [科技企业将绩效考核与员工消耗的 LLM token 数量挂钩](https://gizmodo.com/tech-employees-are-reportedly-being-evaluated-by-how-fast-they-burn-through-llm-tokens-2000736627) ⭐️ 7.0/10

据《纽约时报》专栏报道，Meta、OpenAI 等科技公司据称正在创建内部排行榜，以比较员工消耗的 LLM token 数量，其中 Meta 和 Shopify 明确将 AI 使用量指标纳入绩效考核。报道还称，一名 OpenAI 工程师累计消耗了 2100 亿个 token，而 OpenAI 总裁 Greg Brockman 表示，GPT-5.4 上线仅一周后，其日处理量已达到 5 万亿 token。 这种做法标志着职场绩效评估标准的一次重大转变，将 AI 工具采用情况与个人评估直接挂钩，这可能会加速企业 AI 集成，但也存在鼓励浪费性使用而非有意义的生产力的风险。它反映了科技公司在证明和量化 AI 投资回报方面日益增长的压力，并可能为 AI 时代衡量员工贡献设定新的行业标准。 报道中提到的指标侧重于原始的 token 消耗量，这是衡量 LLM 输入/输出大小的指标，但不一定代表输出质量或任务效率。所提及的规模是巨大的，个别工程师消耗了数千亿 token，而像 GPT-5.4 这样的旗舰模型日处理量达数万亿 token，凸显了现代 AI 工作流程所涉及的海量计算资源。

telegram · zaihuapd · Mar 23, 08:42

**背景**: 像 GPT-4、LLaMA 或 Gemini 这样的大型语言模型（LLM）通过将文本分解为 token 来处理文本，token 是单词或词段的数字表示。模型处理的 token 数量直接与计算成本相关，并且是 AI API 服务（例如 OpenAI 的 API）计费的基本单位。上下文窗口定义了模型一次可以考虑的最大 token 数量，这影响了其处理长文档或对话的能力。公司跟踪 token 使用量以管理成本并了解采用情况，但将其用作绩效指标是一种新颖且有争议的应用。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Large_language_model">Large language model - Wikipedia</a></li>
<li><a href="https://winder.ai/calculating-token-counts-llm-context-windows-practical-guide/">Calculating LLM Token Counts: A Practical Guide</a></li>
<li><a href="https://hackernoon.com/whos-used-one-trillion-plus-openai-tokens-salesforce-shopify-canva-hubspot-and-26-more-companies">Who's Used One Trillion Plus OpenAI Tokens? Salesforce ...</a></li>

</ul>
</details>

**标签**: `#AI Adoption`, `#Workplace Culture`, `#Performance Metrics`, `#LLM Usage`, `#Tech Industry`

---

<a id="item-4"></a>
## [OpenAI 建议英国将 AI 聊天机器人纳入 Google 搜索选择页](https://assets.publishing.service.gov.uk/media/69b970dcc06ba9576435ab5a/OpenAI.pdf) ⭐️ 7.0/10

3 月 6 日，OpenAI 正式向英国竞争与市场管理局提交建议，主张 Google 搜索选择页的资格标准应明确纳入具备搜索功能的 AI 聊天机器人。这将使 ChatGPT 等服务能够在 Android 设备和 Chrome 浏览器上被用户选为默认搜索服务。 此举是 OpenAI 的一项战略举措，旨在为其对话式 AI 产品在英国这个监管严格的数字市场中争取显著的位置和用户访问渠道。如果建议被采纳，将可能重塑搜索市场竞争格局，让 AI 优先的服务在主要平台上获得与传统搜索引擎同等的地位，从而加速向 AI 驱动信息检索的转变。 OpenAI 认为，像 ChatGPT 这样通过对话式或多模态界面进行信息发现的服务，在功能上与 Google 自家的 AI Overviews 和 AI Mode 功能相近。它还建议采用透明、动态的流行度指标来决定哪些服务出现在选择页上，并将选择页的覆盖范围扩展到语音、视觉和 AI 辅助搜索等入口点。

telegram · zaihuapd · Mar 23, 14:50

**背景**: 英国竞争与市场管理局已认定 Google 在通用搜索服务中具有战略市场地位，这赋予了监管机构实施促进竞争规则的权力。正在考虑的一项关键补救措施是推出“搜索选择页”，在 Android 和 Chrome 上提示用户从选项列表中选择默认搜索引擎。目前，该列表仅限于传统的“通用搜索服务”，CMA 正在就是否纳入更新的、生成式 AI 驱动的搜索工具进行咨询。Google 已通过 AI Overviews（摘要）和用于复杂查询的实验性 AI Mode 等功能，将 AI 直接集成到其搜索结果中。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://assets.publishing.service.gov.uk/media/68c29c52d65a1a2a5172a9ab/_Summary_of_choice_architecture_roundtable.pdf">Summary of choice architecture roundtable - GOV.UK</a></li>
<li><a href="https://www.gov.uk/cma-cases/googles-general-search-and-search-advertising-services">Google's general search and search advertising services</a></li>
<li><a href="https://en.wikipedia.org/wiki/AI_Overviews">AI Overviews - Wikipedia</a></li>

</ul>
</details>

**标签**: `#AI Regulation`, `#Search Competition`, `#OpenAI`, `#UK CMA`, `#Market Access`

---