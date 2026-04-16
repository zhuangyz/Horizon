---
layout: default
title: "Horizon Summary: 2026-04-16 (EN)"
date: 2026-04-16
lang: en
---

> From 24 items, 12 important content pieces were selected

---

1. [IETF Publishes IPv8 Draft Protocol with 64-bit Addressing and Full IPv4 Backward Compatibility](#item-1) ⭐️ 9.0/10
2. [DeepSeek releases major DeepGEMM update with Mega MoE fused operators and FP4 precision support](#item-2) ⭐️ 9.0/10
3. [Anthropic releases Claude Opus 4.7 with adaptive thinking and updated tokenizer.](#item-3) ⭐️ 8.0/10
4. [Qwen releases open-weight 35B coding model Qwen3.6-35B-A3B for agentic applications](#item-4) ⭐️ 8.0/10
5. [Google launches native Swift macOS Gemini app with hotkey support and announces multi-year Apple partnership](#item-5) ⭐️ 8.0/10
6. [OpenAI, Anthropic, and Google collaborate to counter adversarial distillation by Chinese competitors.](#item-6) ⭐️ 8.0/10
7. [Apple reportedly plans to license Google's 1.2 trillion parameter Gemini AI model to overhaul Siri.](#item-7) ⭐️ 8.0/10
8. [Alibaba and Tencent Simultaneously Release New 3D Content Generation AI Models](#item-8) ⭐️ 8.0/10
9. [Qwen3.6-35B-A3B Released: A Sparse MoE Model with 3B Active Parameters for Agentic Programming](#item-9) ⭐️ 8.0/10
10. [Anthropic releases Claude Opus 4.6 with 200K context window and adaptive thinking mode.](#item-10) ⭐️ 8.0/10
11. [Google Releases Gemini 3.1 Flash TTS with Scene-Setting Prompt Control](#item-11) ⭐️ 7.0/10
12. [Popular Russian Android apps detect VPN usage and scan for foreign apps, aligning with government restrictions](#item-12) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [IETF Publishes IPv8 Draft Protocol with 64-bit Addressing and Full IPv4 Backward Compatibility](https://www.ietf.org/archive/id/draft-thain-ipv8-00.html) ⭐️ 9.0/10

The Internet Engineering Task Force (IETF) has published the initial draft for Internet Protocol Version 8 (IPv8), which introduces a 64-bit address space and treats IPv4 as a proper subset, achieving 100% backward compatibility. The draft proposes integrating services like DHCP, DNS, and authentication into a unified 'Zone Server' architecture and introduces new mechanisms for security and routing efficiency. This proposal represents a potential paradigm shift by directly addressing the long-standing address exhaustion problem of IPv4 while avoiding the complex dual-stack deployment challenges of IPv6. If adopted, it could simplify internet infrastructure management, enhance routing security, and enable a smoother transition from legacy IPv4 networks. The draft specifies that each Autonomous System Number (ASN) would be allocated over 4.2 billion host addresses, and it proposes mandatory OAuth2-based authorization and a 'Cost Factor' algorithm for optimal path selection. It also includes mechanisms like 8to4 tunneling for interoperability during migration and rules like a /16 minimum injection prefix to prevent BGP hijacking and global routing table bloat.

telegram · zaihuapd · Apr 16, 08:43

**Background**: The current Internet primarily runs on two protocols: IPv4, which uses 32-bit addresses and has exhausted its available space, and IPv6, which uses 128-bit addresses to provide vast capacity but requires a dual-stack approach for compatibility, complicating deployment. The IETF is the standards body responsible for defining core internet protocols, and its drafts represent early-stage proposals for community review and discussion. Transition mechanisms like 6to4 have been used to bridge IPv4 and IPv6 networks.

<details><summary>References</summary>
<ul>
<li><a href="https://www.ietf.org/archive/id/draft-thain-ipv8-00.html">Internet Protocol Version 8 (IPv8)</a></li>
<li><a href="https://cybernews.com/tech/ipv8-proposal-slammed-by-tech-professionals/">Tech pros slam new IPv8 proposal as AI slop | Cybernews</a></li>
<li><a href="https://lowendtalk.com/discussion/216334/internet-protocol-version-8-ipv8-proposal">Internet Protocol Version 8 (IPv8) proposal — LowEndTalk</a></li>

</ul>
</details>

**Discussion**: The proposal has sparked significant controversy and criticism from technical professionals shortly after its publication. Many in the community are skeptical, labeling the draft as impractical 'AI slop' and questioning the need for a new protocol given the ongoing, albeit slow, deployment of IPv6.

**Tags**: `#networking`, `#protocols`, `#ietf`, `#ipv8`, `#internet-infrastructure`

---

<a id="item-2"></a>
## [DeepSeek releases major DeepGEMM update with Mega MoE fused operators and FP4 precision support](https://github.com/deepseek-ai/DeepGEMM/tree/public-release-260416) ⭐️ 9.0/10

On April 16, 2026, DeepSeek released a major update to its DeepGEMM high-performance operator library, introducing the Mega MoE fused operator that overlaps dispatch, SwiGLU computation, and NVLink communication. The update also adds FP8xFP4 GEMM operators, FP4 Indexer, Programmatic Dependency Launch (PDL) support, and significantly improves JIT compilation speed. This update addresses critical bottlenecks in training and inference for large mixture-of-experts (MoE) models by optimizing both computation and communication patterns. The introduction of FP4 precision support enables more memory-efficient model deployment, potentially allowing larger models to run on existing hardware or reducing infrastructure costs for AI companies. The DeepGEMM library is designed for modern large models and supports NVIDIA SM90 and SM100 architectures, featuring lightweight design and runtime just-in-time compilation without complex installation builds. The Mega MoE operator specifically uses symmetric memory technology to optimize performance for multi-expert models during both inference and training.

telegram · zaihuapd · Apr 16, 09:57

**Background**: Mixture-of-Experts (MoE) models are a type of neural network architecture where different specialized sub-networks (experts) handle different inputs, allowing for larger model capacity without proportional increases in computation. Fused operators combine multiple computational steps into a single GPU kernel to reduce memory transfers and improve efficiency. NVLink is NVIDIA's high-speed GPU interconnect technology that enables faster data transfer between GPUs compared to traditional PCIe connections. FP4 (4-bit floating point) quantization reduces the numerical precision of model weights to save memory, though it can impact model accuracy if not implemented carefully.

<details><summary>References</summary>
<ul>
<li><a href="https://medium.com/@datenlord/from-loops-to-fusion-understanding-the-principles-of-the-fused-moe-operato-part2-1ff65a17cd56">From Loops to Fusion: Understanding the Principles of the Fused MoE ...</a></li>
<li><a href="https://stevenfoerster.com/tutorials/efficient-fine-tuning-with-lora-and-quantization/">Efficient Fine-Tuning with LoRA and Quantization · Steven Foerster</a></li>
<li><a href="https://uvation.com/articles/unlocking-ultra-fast-gpu-communication-with-nvidia-nvlink-nvlink-switch">NVIDIA NVLink and NVLink Switch: Redefining GPU Interconnects</a></li>

</ul>
</details>

**Tags**: `#AI-Infrastructure`, `#High-Performance-Computing`, `#CUDA-Optimization`, `#Mixture-of-Experts`, `#Quantization`

---

<a id="item-3"></a>
## [Anthropic releases Claude Opus 4.7 with adaptive thinking and updated tokenizer.](https://www.anthropic.com/news/claude-opus-4-7) ⭐️ 8.0/10

Anthropic has released Claude Opus 4.7, which introduces a new 'adaptive thinking' capability and an updated tokenizer. The release also deprecates the previous manual thinking budget mode and changes the default output to no longer include a human-readable reasoning summary. This is a major update to a leading AI model that fundamentally changes how developers interact with its reasoning capabilities, potentially improving performance on complex tasks. The tokenizer update, while increasing token counts for the same input, aims to improve text processing efficiency, which is a core technical change affecting all API users. The new adaptive thinking mode replaces the previous `budget_tokens` configuration and is controlled via `thinking.type: "adaptive"` with an `effort` parameter. The updated tokenizer increases token counts for the same input by roughly 1.0 to 1.35 times, depending on content type, which can impact API pricing and context window usage.

hackernews · meetpateltech · Apr 16, 14:23

**Background**: Claude is a large language model (LLM) developed by Anthropic. 'Thinking' or 'chain-of-thought' capabilities allow the model to perform internal, step-by-step reasoning before producing a final answer, which is crucial for complex problem-solving. A tokenizer is a core component of an LLM that breaks down text into smaller units (tokens) for processing; its efficiency directly impacts the model's performance and cost.

<details><summary>References</summary>
<ul>
<li><a href="https://platform.claude.com/docs/en/build-with-claude/adaptive-thinking">Adaptive thinking - Claude API Docs</a></li>
<li><a href="https://seantrott.substack.com/p/tokenization-in-large-language-models">Tokenization in large language models, explained</a></li>
<li><a href="https://www.anthropic.com/news/claude-opus-4-7">Introducing Claude Opus 4.7 \ Anthropic</a></li>

</ul>
</details>

**Discussion**: Developer sentiment is mixed, with some expressing confusion over the API changes and reporting issues like the model refusing tasks from its own documentation. Others note performance inconsistencies compared to the previous version and highlight the practical impact of the tokenizer change on costs. There is also a mention of a brief window for 'un-nerfed' agentic coding before potential adjustments.

**Tags**: `#llm`, `#anthropic`, `#api`, `#ai-models`, `#developer-tools`

---

<a id="item-4"></a>
## [Qwen releases open-weight 35B coding model Qwen3.6-35B-A3B for agentic applications](https://qwen.ai/blog?id=qwen3.6-35b-a3b) ⭐️ 8.0/10

The Qwen team from Alibaba has publicly released Qwen3.6-35B-A3B, a 35-billion-parameter open-weight coding model specifically designed for agentic applications. The model is now available for download and use by the public. This release provides a powerful, specialized tool for developers building autonomous AI coding agents, particularly valuable for industries like banking and healthcare that have data privacy restrictions and cannot use public cloud models. It represents a continued commitment to open-weight AI from the Qwen team despite recent organizational challenges. The model features a hybrid attention architecture, supports a 256K context window, and is available in quantized formats like GGUF for easier local deployment. It is part of the larger Qwen3.6 family of models, which are natively multimodal and support over 200 languages.

hackernews · cmitsakis · Apr 16, 13:36

**Background**: Qwen is a family of AI models developed by Alibaba. 'Open-weight' models provide the trained model parameters (weights) for public use but may not include the full training code, data, or specifications required for complete reproducibility, unlike 'open-source' models. Agentic coding refers to an AI paradigm where large language models autonomously plan and execute multi-step software development tasks by interacting with tools like compilers and debuggers.

<details><summary>References</summary>
<ul>
<li><a href="https://unsloth.ai/docs/models/qwen3.6">Run the new Qwen 3 . 6 - 35 - A 3 B model locally! | Unsloth Documentation</a></li>
<li><a href="https://hellofuture.orange.com/en/a-typology-of-artificial-intelligence-models/">AI models explained: open source vs. open weight vs. closed</a></li>
<li><a href="https://arxiv.org/html/2508.11126v1">AI Agentic Programming: A Survey of Techniques, Challenges, and Opportunities</a></li>

</ul>
</details>

**Discussion**: Community sentiment is positive, highlighting practical accessibility through quantized formats and the model's relevance for restricted sectors. There is also appreciation for Qwen's continued open-weight releases despite internal challenges, alongside some curiosity about why a different model variant was chosen over a more popular one indicated by a public poll.

**Tags**: `#open-source-ai`, `#coding-agents`, `#llm`, `#model-release`, `#qwen`

---

<a id="item-5"></a>
## [Google launches native Swift macOS Gemini app with hotkey support and announces multi-year Apple partnership](https://9to5mac.com/2026/04/15/google-launches-gemini-mac-app-heres-what-it-offers/) ⭐️ 8.0/10

On April 15, Google officially launched a native macOS application for its Gemini AI assistant, built using Apple's Swift programming language and featuring a hotkey (Option + Space) for quick summoning. Furthermore, Google and Apple announced a multi-year partnership where Gemini will power AI features in the upcoming iOS 27 and macOS 27, with more details to be revealed at WWDC on June 8, 2026. This marks a significant strategic move by Google to deeply integrate its AI assistant into the Apple ecosystem through native development, potentially offering a superior user experience on macOS. The announced partnership signals a major shift in the competitive landscape, where two tech giants are collaborating to enhance Apple's AI capabilities (like Siri and Apple Intelligence) with Google's Gemini technology, which could reshape the future of AI assistants on Apple devices. The native Swift app supports core Gemini functionalities like quick Q&A, content drafting, summarization, code writing, and image analysis, and it also allows screen sharing to provide richer context for queries. The partnership specifically aims to power an upgraded Siri and Apple Intelligence features in the next major OS versions, indicating a deep technical integration beyond a simple API call.

telegram · zaihuapd · Apr 16, 00:33

**Background**: Gemini is Google's flagship family of multimodal large language models (LLMs) and AI assistants, competing with offerings like OpenAI's ChatGPT. Native app development, using a platform's preferred language like Swift for macOS, typically offers better performance, smoother integration with system features, and a more responsive user interface compared to cross-platform frameworks. Apple Intelligence is Apple's own generative AI system announced in 2024, designed to work across its devices with a mix of on-device and cloud processing.

<details><summary>References</summary>
<ul>
<li><a href="https://learningswift.brightdigit.com/articles/native-app-development-advantages/">Native App Development and Its Advantages | BrightDigit</a></li>
<li><a href="https://en.wikipedia.org/wiki/Apple_Intelligence">Apple Intelligence - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#AI-Assistants`, `#macOS`, `#Google-Gemini`, `#Apple-Google-Partnership`, `#Native-Development`

---

<a id="item-6"></a>
## [OpenAI, Anthropic, and Google collaborate to counter adversarial distillation by Chinese competitors.](https://t.me/zaihuapd/40889) ⭐️ 8.0/10

OpenAI, Anthropic, and Google (via Alphabet) have initiated a rare collaboration through the Frontier Model Forum to share information specifically about "adversarial distillation" attempts. Their goal is to counter unauthorized efforts, primarily attributed to Chinese competitors, to extract outputs from and replicate the capabilities of leading U.S. AI models. This collaboration signifies a major shift where leading AI competitors are aligning to protect their core intellectual property and address what they perceive as both a commercial threat and a potential national security risk. It highlights the intensifying geopolitical dimension of AI development, where model security is becoming as critical as model capability. OpenAI has confirmed its participation and referenced a recent memo submitted to the U.S. Congress on this issue. The collaboration is framed within the Frontier Model Forum, an industry body originally focused on AI safety, now expanding its scope to include security against model extraction.

telegram · zaihuapd · Apr 16, 04:06

**Background**: Adversarial distillation is a type of model extraction attack where a secondary model is trained to mimic a proprietary, originator model (like GPT-4 or Claude) by using its outputs, often obtained through API queries. The Frontier Model Forum is an industry body founded in July 2023 by Anthropic, Google, Microsoft, and OpenAI with the initial stated mission of ensuring the safe and responsible development of frontier AI models. Model extraction attacks target the intellectual property embedded within trained models, representing a sophisticated threat in AI security.

<details><summary>References</summary>
<ul>
<li><a href="https://www.frontiermodelforum.org/issue-briefs/issue-brief-adversarial-distillation/">Adversarial Distillation - Frontier Model Forum</a></li>
<li><a href="https://www.frontiermodelforum.org/">Frontier Model Forum</a></li>
<li><a href="https://snyk.io/articles/ai-model-theft/">AI Model Theft: Understanding the Threat Landscape and ... - Snyk</a></li>

</ul>
</details>

**Tags**: `#AI Safety`, `#Geopolitics`, `#Intellectual Property`, `#Industry Collaboration`, `#Model Security`

---

<a id="item-7"></a>
## [Apple reportedly plans to license Google's 1.2 trillion parameter Gemini AI model to overhaul Siri.](https://t.me/zaihuapd/40891) ⭐️ 8.0/10

According to reports, Apple is finalizing a deal to license Google's 1.2 trillion parameter Gemini AI model to power a major upgrade for its Siri voice assistant. The agreement involves an annual payment of approximately $1 billion from Apple to Google, with the new Siri, codenamed 'Linwood,' planned for release in iOS 26.4 next spring. This potential partnership represents a significant strategic shift for Apple, which has historically developed its own AI technology, and could dramatically reshape the competitive landscape for AI assistants. A deal of this scale, integrating Google's cutting-edge large language model into Apple's ecosystem, would be an unprecedented cross-company collaboration with major implications for user experience and market dynamics. The reported 1.2 trillion parameter Gemini model would be a massive leap from Apple's current cloud-based AI model, which reportedly uses only 1.5 billion parameters. The new Siri is expected to leverage Google's model for tasks like summarization and planning, and queries will be processed through Apple's Private Cloud Compute infrastructure.

telegram · zaihuapd · Apr 16, 05:18

**Background**: Large Language Models (LLMs) like Gemini are AI systems trained on vast amounts of text and multimodal data to understand and generate human-like language. The number of parameters in a model is a key indicator of its scale and potential capability, with higher counts generally associated with more sophisticated performance. Google's Gemini family of models, including versions like Gemini 1.5, utilizes advanced architectures such as the Mixture of Experts (MoE) to improve efficiency and capability. Siri is Apple's long-standing voice-activated virtual assistant integrated into its devices.

<details><summary>References</summary>
<ul>
<li><a href="https://udit.co/blog/apple-siri-google-gemini-trillion-parameter-ai-overhaul">Apple Redesigns Siri with Google's Trillion - Parameter Gemin</a></li>
<li><a href="https://biggo.com/news/202511052052_Apple_Siri_Google_Gemini_AI_Model">Apple's Siri Revamp to Run on Google's 1 . 2 Trillion - Parameter AI ...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Gemini_(language_model)">Gemini (language model) - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#artificial-intelligence`, `#voice-assistants`, `#tech-industry`, `#large-language-models`, `#mobile-operating-systems`

---

<a id="item-8"></a>
## [Alibaba and Tencent Simultaneously Release New 3D Content Generation AI Models](https://www.bloomberg.com/news/articles/2026-04-16/alibaba-releases-new-ai-model-for-gaming-development) ⭐️ 8.0/10

On April 16, 2026, Alibaba released its 'Happy Oyster' AI model capable of generating interactive 3D video content for game development and film production. Simultaneously, Tencent open-sourced its Hunyuan 3D World Model 2.0, which can generate, reconstruct, and simulate 3D worlds from text, images, or videos, and export assets like Mesh and 3D Gaussian Splatting (3DGS) for integration into existing game workflows. This marks a significant escalation in the race for advanced multimodal AI and world modeling capabilities between China's tech giants, directly targeting the high-value gaming and digital twin industries. The simultaneous release signals a strategic push to democratize and accelerate 3D content creation, potentially lowering production barriers and reshaping workflows for game developers, filmmakers, and digital twin creators. Tencent's model specifically supports exporting content to industry-standard engines like Unity and Unreal Engine for further editing and can build digital twin scenes from real spatial videos or multi-view images. Alibaba's Happy Oyster focuses on generating interactive 3D video, indicating a slightly different application emphasis within the broader 3D content generation domain.

telegram · zaihuapd · Apr 16, 07:58

**Background**: 3D Gaussian Splatting (3DGS) is a technique for real-time radiance field rendering that gained prominence in 2023, enabling high-quality 3D scene reconstruction from videos. AI world models are neural networks that understand real-world dynamics, including physics and spatial properties, and can generate realistic simulations of physical environments from various inputs like text or video. These technologies represent the frontier of AI's move from 2D image generation to understanding and creating complex, interactive 3D spaces.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Gaussian_splatting">Gaussian splatting - Wikipedia</a></li>
<li><a href="https://www.nvidia.com/en-us/glossary/world-models/">What Is a World Model? | NVIDIA Glossary</a></li>

</ul>
</details>

**Tags**: `#3D Generation`, `#AI Models`, `#Game Development`, `#Multimodal AI`, `#Digital Twins`

---

<a id="item-9"></a>
## [Qwen3.6-35B-A3B Released: A Sparse MoE Model with 3B Active Parameters for Agentic Programming](https://qwenlm.github.io/blog/qwen3.6-35b-a3b/) ⭐️ 8.0/10

The Qwen team has open-sourced Qwen3.6-35B-A3B, a sparse Mixture-of-Experts (MoE) model with 35 billion total parameters but only 3 billion active parameters during inference. It claims to outperform its predecessors and compete with some larger dense models on coding and tool-use benchmarks like SWE-bench and MCPMark, while retaining multimodal reasoning capabilities. This release represents a significant step towards more efficient and capable AI agents for software engineering. By achieving strong performance on complex, real-world coding tasks with a fraction of the typical computational cost, it makes powerful agentic programming more accessible to developers and researchers, potentially accelerating the integration of AI into software development workflows. The model is specifically designed for 'agentic programming,' excelling at benchmarks that test real-world software issue resolution (SWE-bench) and comprehensive agent capabilities (MCPMark). It is released with open weights, supports self-hosting, and provides API compatibility with OpenAI/Anthropic-style interfaces for easy integration into existing developer tools like OpenClaw or Qwen Code.

telegram · zaihuapd · Apr 16, 13:59

**Background**: A sparse Mixture-of-Experts (MoE) model is an architecture that increases a model's total parameter count (capacity) without proportionally increasing the computational cost for each input. Instead of using all parameters for every computation, a routing network selects only a small subset of 'experts' to be active, leading to faster and more efficient inference. Benchmarks like SWE-bench evaluate a model's ability to solve real-world software engineering issues from GitHub, while MCPMark is a newer, comprehensive benchmark designed to stress-test model and agent capabilities across diverse, realistic tasks.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/abs/2308.00951">[2308.00951] From Sparse to Soft Mixtures of Experts</a></li>
<li><a href="https://www.swebench.com/">SWE - bench Leaderboards</a></li>
<li><a href="https://mcpmark.ai/">MCPMark - Stress-Testing Comprehensive MCP Benchmark</a></li>

</ul>
</details>

**Tags**: `#AI`, `#Large Language Models`, `#Open Source`, `#Mixture of Experts`, `#Code Generation`

---

<a id="item-10"></a>
## [Anthropic releases Claude Opus 4.6 with 200K context window and adaptive thinking mode.](https://t.me/zaihuapd/40903) ⭐️ 8.0/10

Anthropic has released the Claude Opus 4.6 model, which doubles the context window to 200K tokens (with a 1M token beta) and doubles the maximum output tokens to 128K. The model introduces an adaptive thinking mode that dynamically adjusts reasoning depth based on problem complexity and adds a new 'max effort' parameter. This update significantly enhances Claude's ability to handle long, complex documents and extended conversations, making it more competitive against other leading models like GPT. The adaptive thinking feature represents a shift towards more autonomous and efficient AI reasoning, potentially reducing developer guesswork and improving performance on nuanced tasks. The model also includes a context compression feature that automatically summarizes early parts of a conversation as it approaches the window limit, enabling near-infinite length dialogues. The 1M token context window is currently in beta, indicating it's an experimental feature with potential limitations.

telegram · zaihuapd · Apr 16, 14:28

**Background**: A context window in a large language model (LLM) is the amount of text, measured in tokens, that the model can process and remember in a single interaction, analogous to a human's short-term memory. Adaptive thinking is an evolution in AI reasoning where the model itself decides when and how much to engage in deeper, extended reasoning based on the complexity of the request, moving away from developers manually setting a fixed thinking budget. Context compression is an engineering technique used to manage ballooning conversation histories in AI agents by summarizing or trimming information to stay within model limits.

<details><summary>References</summary>
<ul>
<li><a href="https://www.mckinsey.com/featured-insights/mckinsey-explainers/what-is-a-context-window">What is a context window for Large Language Models? | McKinsey</a></li>
<li><a href="https://platform.claude.com/docs/en/build-with-claude/adaptive-thinking">Adaptive thinking - Claude API Docs</a></li>
<li><a href="https://medium.com/the-ai-forum/automatic-context-compression-in-llm-agents-why-agents-need-to-forget-and-how-to-help-them-do-it-43bff14c341d">Automatic Context Compression in LLM Agents: Why ... - Medium</a></li>

</ul>
</details>

**Tags**: `#AI`, `#LLM`, `#Anthropic`, `#Claude`, `#Natural Language Processing`

---

<a id="item-11"></a>
## [Google Releases Gemini 3.1 Flash TTS with Scene-Setting Prompt Control](https://simonwillison.net/2026/Apr/15/gemini-31-flash-tts/#atom-everything) ⭐️ 7.0/10

Google released Gemini 3.1 Flash TTS, a new text-to-speech model accessible via the Gemini API under the model ID `gemini-3.1-flash-tts-preview`. The model's key innovation is that it can be directed using detailed, scene-setting prompts that describe the speaker's environment, vocal style, accent, and emotional state, as demonstrated in its official prompting guide. This represents a significant shift in AI speech synthesis, moving from simple voice selection to directable, context-aware audio generation. It enables creators, developers, and media producers to generate highly nuanced and specific vocal performances for applications like audiobooks, game dialogue, and dynamic media content without requiring manual audio editing. The model currently only outputs audio files and is in a preview state. According to Google's documentation, Gemini 3.1 Flash TTS supports over 70 languages and uses SynthID watermarking to identify AI-generated audio, addressing concerns about audio authenticity and misuse.

rss · Simon Willison · Apr 15, 17:13

**Background**: Text-to-speech (TTS) technology converts written text into spoken audio. Traditional TTS models often offer limited control, such as selecting from predefined voices or adjusting basic parameters like speed and pitch. The Gemini API is Google's platform for accessing its family of large language and multimodal models, which now includes this specialized TTS model. The concept of using detailed, descriptive prompts for generation is inspired by techniques used in AI image and video generation.

<details><summary>References</summary>
<ul>
<li><a href="https://ai.google.dev/gemini-api/docs/speech-generation">Text-to-speech generation (TTS) | Gemini API | Google AI for ...</a></li>
<li><a href="https://blog.google/innovation-and-ai/models-and-research/gemini-models/gemini-3-1-flash-tts/">Gemini 3.1 Flash TTS: New text-to-speech AI model - The Keyword</a></li>

</ul>
</details>

**Tags**: `#AI`, `#text-to-speech`, `#Google`, `#Gemini`, `#speech-synthesis`

---

<a id="item-12"></a>
## [Popular Russian Android apps detect VPN usage and scan for foreign apps, aligning with government restrictions](https://files.rks.global/russian_apps_search_for_vpn_en.pdf) ⭐️ 7.0/10

A study by RKS Global found that 22 out of Russia's 30 most popular Android apps can detect VPN usage, with 19 sending this data to their servers. Furthermore, the Avito app was found to scan devices for the presence of over 200 foreign applications, including banking, cryptocurrency wallets, and messaging tools. This systematic, large-scale surveillance by popular apps directly supports government directives to restrict services for VPN users, significantly eroding digital privacy for millions of Russian citizens. It represents a concrete step towards enforcing Russia's 'digital sovereignty' doctrine, effectively isolating users from the global internet and enabling state control over online access. The detection and data collection are linked to a mandate from Russia's Ministry of Digital Development, which has instructed major companies to restrict service access for users with active VPNs starting April 15, 2026. The Avito app's scan specifically targets a wide range of foreign financial and communication tools, which are often used to bypass domestic restrictions.

telegram · zaihuapd · Apr 16, 04:38

**Background**: A Virtual Private Network (VPN) encrypts a user's internet traffic and routes it through a server in another location, masking their real IP address. This is commonly used to enhance privacy, access geo-blocked content, or bypass censorship. In recent years, the Russian government has pursued a 'digital sovereignty' policy, seeking greater control over the internet within its borders, which includes restricting tools like VPNs that can circumvent state-imposed blocks. Android apps can detect VPN usage through system APIs, such as checking the active network's capabilities via the ConnectivityManager.

<details><summary>References</summary>
<ul>
<li><a href="https://rks.global/en/research/">RKS Global Researches</a></li>
<li><a href="https://blog.tarkalabs.com/the-ultimate-vpn-detection-guide-for-ios-and-android-313b521186cb">How to detect VPN usage on iOS and Android | Tarka Labs Blogs GitHub - s1mb1o/vpn-detector-android: Android app that ... Implementing VPN Detection in Mobile Applications: Client vs ... How to Detect VPNs Used With Android & iOS Apps Using AI How I Bypassed VPN Detection, Broke Client-Side ... - Medium VPNDroid: Malicious Android VPN Detection Using a CNN-RF ...</a></li>

</ul>
</details>

**Tags**: `#privacy`, `#surveillance`, `#android-security`, `#vpn`, `#digital-rights`

---