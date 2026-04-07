---
layout: default
title: "Horizon Summary: 2026-04-07 (EN)"
date: 2026-04-07
lang: en
---

> From 21 items, 9 important content pieces were selected

---

1. [New Yorker investigation questions Sam Altman's leadership and OpenAI's governance](#item-1) ⭐️ 8.0/10
2. [Cryptography engineer argues for urgent post-quantum standards adoption amid accelerated quantum computing timelines.](#item-2) ⭐️ 8.0/10
3. [Claude Code's February updates cause severe regression for complex engineering tasks](#item-3) ⭐️ 8.0/10
4. [OpenAI Proposes Automation Tax and Sovereign Wealth Fund for the Superintelligence Era](#item-4) ⭐️ 8.0/10
5. [Scientists engineer tobacco plants to produce five natural psychedelics with up to 40x yield boost](#item-5) ⭐️ 8.0/10
6. [Chinese researchers develop self-protecting electrolyte that completely blocks thermal runaway in Ah-scale sodium-ion batteries.](#item-6) ⭐️ 8.0/10
7. [SGLang v0.5.10 enhances MoE fault tolerance, GPU throughput, and sparse attention.](#item-7) ⭐️ 7.0/10
8. [Google releases official AI Edge Gallery app for running Gemma 4 models on iPhone](#item-8) ⭐️ 7.0/10
9. [Apple Blocks Updates for AI-Powered Code Generation Apps Like Replit and Vibecode on App Store](#item-9) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [New Yorker investigation questions Sam Altman's leadership and OpenAI's governance](https://www.newyorker.com/magazine/2026/04/13/sam-altman-may-control-our-future-can-he-be-trusted) ⭐️ 8.0/10

An 18-month New Yorker investigation, reported by Ronan Farrow and Andrew Marantz, reveals internal dynamics at OpenAI, including co-founder Greg Brockman's documented ambitions for "money and power" and his dismissal of early safety proposals. The article examines Sam Altman's leadership and raises fundamental questions about trust and governance in the development of powerful AI. This matters because OpenAI is a leading force shaping the future of artificial intelligence, and its internal governance and leadership priorities directly influence how safe, ethical, and beneficial this transformative technology will be. The investigation highlights the tension between mission-driven ideals and commercial pressures, a critical issue for the entire AI industry as it seeks public trust. The report cites specific internal documents, such as Brockman's diary entries showing conflicting desires between altruism and personal wealth accumulation. It also details an early safety proposal from a policy adviser, which suggested forming an international coalition akin to NATO to prevent an AI arms race, an idea reportedly dismissed by Brockman.

hackernews · adrianhon · Apr 6, 10:36

**Background**: OpenAI was founded as a non-profit with a mission to ensure artificial general intelligence (AGI) benefits all of humanity. To fund its massive compute needs, it created a unique "capped-profit" hybrid structure, where a for-profit subsidiary (OpenAI LP, later Group) could raise capital and generate returns for investors, but ultimate control remained with the non-profit board to safeguard the mission. This structure, designed to balance funding and ethics, has been a subject of intense scrutiny, especially following leadership upheavals in late 2023.

<details><summary>References</summary>
<ul>
<li><a href="https://openai.com/our-structure/">Our structure - OpenAI</a></li>
<li><a href="https://www.revenuememo.com/p/who-owns-openai">Who owns OpenAI? Ownership structure explained (2026)</a></li>
<li><a href="https://www.techrepublic.com/article/news-openai-structure-explained/">How OpenAI’s Corporate Structure Works and Why Changing It ...</a></li>

</ul>
</details>

**Discussion**: The community discussion reflects deep engagement with the investigative findings. Commenters express alarm at the specific revelations about Greg Brockman's motivations and his handling of safety proposals, describing them as "terrifying." There is widespread appreciation for the depth and quality of the journalism, seen as essential for holding powerful tech leaders accountable. Some minor critiques include discomfort with pop culture analogies used in the article.

**Tags**: `#AI Governance`, `#OpenAI`, `#Tech Ethics`, `#Investigative Journalism`, `#Leadership`

---

<a id="item-2"></a>
## [Cryptography engineer argues for urgent post-quantum standards adoption amid accelerated quantum computing timelines.](https://words.filippo.io/crqc-timeline/) ⭐️ 8.0/10

A cryptography engineer published an analysis reassessing quantum computing development timelines, concluding that the window for secure migration to post-quantum cryptographic (PQC) standards is shorter than commonly assumed. The analysis specifically calls for prioritizing the deployment of standards like FIPS 203 (ML-KEM) to replace vulnerable key-exchange algorithms in protocols like TLS and SSH. This matters because widely used public-key cryptography (like RSA and ECC) is vulnerable to attacks from sufficiently powerful quantum computers, which could decrypt past and future intercepted communications. A delayed transition to quantum-resistant algorithms poses a significant 'harvest now, decrypt later' risk to global data security, affecting everything from internet traffic to financial systems. The engineer highlights that standards body processes, like the IETF's nearly two-year deliberation on selecting a stable label for the X-Wing/ML-KEM hybrid scheme, are a major bottleneck to timely deployment. The argument is notable for being non-linear, contrasting with the incremental progress seen in classical cryptanalysis, where capabilities scaled predictably with problem size.

hackernews · thadt · Apr 6, 15:31

**Background**: Post-quantum cryptography (PQC) refers to cryptographic algorithms designed to be secure against attacks by both classical and quantum computers. In August 2024, NIST released its first three finalized PQC standards, including FIPS 203 for ML-KEM (Module-Lattice-Based Key-Encapsulation Mechanism), which is intended to replace Diffie-Hellman key exchange. Quantum computing leverages quantum mechanical phenomena like superposition and entanglement to perform certain calculations, such as integer factorization, exponentially faster than classical computers, threatening current public-key infrastructure.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Post-quantum_cryptography">Post-quantum cryptography - Wikipedia</a></li>
<li><a href="https://www.nist.gov/news-events/news/2024/08/nist-releases-first-3-finalized-post-quantum-encryption-standards">NIST Releases First 3 Finalized Post-Quantum Encryption Standards</a></li>
<li><a href="https://en.wikipedia.org/wiki/Quantum_computing">Quantum computing - Wikipedia</a></li>

</ul>
</details>

**Discussion**: The discussion shows high engagement, with commenters agreeing on the urgency of deploying FIPS 203/ML-KEM and criticizing slow standards processes. Some skeptics reported that the analysis helped them re-evaluate their risk assessment, moving away from a 'QC is irrelevant' stance. Others noted the non-linear nature of quantum computing progress compared to classical cryptanalysis.

**Tags**: `#cryptography`, `#quantum-computing`, `#security`, `#post-quantum-cryptography`, `#standards`

---

<a id="item-3"></a>
## [Claude Code's February updates cause severe regression for complex engineering tasks](https://github.com/anthropics/claude-code/issues/42796) ⭐️ 8.0/10

Following February 2024 updates, users report Claude Code has become unusable for complex engineering tasks, with detailed analysis showing degraded reasoning capabilities and problematic patterns like 'simplest fix' responses. The issue has generated 452 comments on GitHub, including responses from the Claude Code team acknowledging the problem. This regression significantly impacts developers who rely on Claude Code for complex software engineering workflows, potentially slowing development velocity and reducing trust in AI coding assistants. The widespread discussion indicates this isn't an isolated issue but represents a broader concern about model stability and quality control in rapidly evolving AI tools. The regression analysis was partially conducted by Claude Opus 4.6 analyzing its own session logs, revealing patterns like reduced read-to-edit ratios and thinking character shifts. A key technical detail is the 'redact-thinking-2026-02-12' beta header that hides thinking from the UI but reportedly doesn't impact model reasoning capabilities.

hackernews · StanAngeloff · Apr 6, 13:50

**Background**: Claude Code is an agentic coding tool from Anthropic that lives in the terminal, understands codebases, and helps developers code faster by executing routine tasks and explaining complex code. AI regression refers to when a model improves in one technical area but degrades in overall intellectual capability, similar to how a chatbot might gain speed but lose conversational nuance. The 'simplest fix' pattern represents a problematic response where AI assistants prioritize minimal changes over correct solutions.

<details><summary>References</summary>
<ul>
<li><a href="https://intellirate.ai/blog/ai-regressions-and-prevention">The Hidden Cost of AI Regressions — and How to Prevent... | Intellirate</a></li>
<li><a href="https://lexler.github.io/augmented-coding-patterns/">Augmented Coding Patterns - lexler.github.io</a></li>
<li><a href="https://code.claude.com/docs/en/changelog">Changelog - Claude Code Docs</a></li>

</ul>
</details>

**Discussion**: Community sentiment shows frustration with the regression, with users reporting similar issues across Claude Opus 4.6 models in other interfaces like Copilot. The discussion includes technical analysis from the issue author showing indicators of shallow thinking, while some commenters note the irony of using Claude to analyze its own performance degradation. The Claude Code team has engaged directly, with Boris from the team acknowledging the detailed analysis and attempting to address concerns.

**Tags**: `#AI-Coding-Assistants`, `#Claude`, `#Software-Engineering`, `#Model-Regression`, `#Developer-Tools`

---

<a id="item-4"></a>
## [OpenAI Proposes Automation Tax and Sovereign Wealth Fund for the Superintelligence Era](https://openai.com/index/industrial-policy-for-the-intelligence-age) ⭐️ 8.0/10

OpenAI has published a policy proposal titled 'Industrial Policy for the Intelligence Age,' which recommends restructuring the tax system to levy higher taxes on companies profiting from automation and establishing a public investment fund to distribute universal dividends. The company also announced plans to open a new office in Washington, D.C., in May and offer up to $1 million in API credits and $100,000 in cash grants to kickstart cross-disciplinary discussions on AI policy. This proposal is significant because it represents a major AI company proactively outlining a concrete policy framework to address the profound societal and economic disruptions anticipated from the advent of superintelligence. It moves the conversation beyond theoretical risks to practical governance, potentially influencing future legislation on taxation, social safety nets, and labor policies in an increasingly automated world. Beyond the automation tax and sovereign wealth fund, the proposal includes support for 'portable benefits' that are not tied to a specific employer, shorter working hours, and strengthening the power grid to support AI competition. OpenAI also advocates for granting governments greater authority to evaluate and contain dangerous AI systems, attempting to balance pro-innovation and pro-safety stances.

telegram · zaihuapd · Apr 6, 09:41

**Background**: Superintelligence refers to a hypothetical AI system that vastly exceeds human cognitive performance in virtually all domains. A sovereign wealth fund is a state-owned investment fund that manages national savings for long-term economic benefit, with the Alaska Permanent Fund being a prominent example that pays annual dividends to state residents. Portable benefits are work-related benefits, such as health insurance or retirement savings, that are attached to the individual worker rather than a specific job or employer, providing flexibility in a changing labor market.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Superintelligence">Superintelligence - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Alaska_Permanent_Fund">Alaska Permanent Fund - Wikipedia</a></li>
<li><a href="https://www.aspeninstitute.org/publications/designing-portable-benefits/">Designing Portable Benefits : A Resource Guide for... - Aspen Institute</a></li>

</ul>
</details>

**Tags**: `#AI Policy`, `#Automation`, `#Universal Basic Income`, `#OpenAI`, `#Future of Work`

---

<a id="item-5"></a>
## [Scientists engineer tobacco plants to produce five natural psychedelics with up to 40x yield boost](https://www.science.org/doi/10.1126/sciadv.aeb3034) ⭐️ 8.0/10

Researchers from the Weizmann Institute of Science and other institutions have genetically engineered Nicotiana benthamiana tobacco plants to produce five natural psychedelic compounds, including DMT, psilocybin, and 5-MeO-DMT. Using AlphaFold3-guided protein engineering, they achieved a 40-fold increase in the production yield of 5-MeO-DMT. This breakthrough creates a sustainable, scalable, and 'cruelty-free' production platform for psychedelic compounds, which are being investigated as potential treatments for mental health conditions like depression, anxiety, and PTSD. It addresses ecological and ethical concerns associated with traditional extraction methods from endangered plants, fungi, or animals. The engineered system repurposes the plant's endogenous tryptophan as a starting material to reconstruct biosynthetic pathways across plant, fungal, and animal kingdoms. It can also produce non-natural halogenated derivatives, showcasing the platform's versatility for generating novel compounds.

telegram · zaihuapd · Apr 6, 12:05

**Background**: Psychedelic compounds like DMT, psilocybin, and 5-MeO-DMT are naturally produced by various plants, fungi, and animals and are under clinical investigation for psychiatric therapies. Nicotiana benthamiana is a close relative of tobacco widely used in laboratories as a platform for recombinant protein production and transient gene expression due to its ease of genetic manipulation. AlphaFold3 is an AI program developed by DeepMind that predicts the 3D structure of proteins and their interactions with other molecules, revolutionizing protein engineering by enabling precise design of enzymes with desired functions.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/AlphaFold">AlphaFold - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Nicotiana_benthamiana">Nicotiana benthamiana - Wikipedia</a></li>
<li><a href="https://www.science.org/doi/10.1126/sciadv.aeb3034">Complete biosynthesis of psychedelic tryptamines from three kingdoms in plants | Science Advances</a></li>

</ul>
</details>

**Tags**: `#synthetic-biology`, `#protein-engineering`, `#drug-discovery`, `#AlphaFold3`, `#biotechnology`

---

<a id="item-6"></a>
## [Chinese researchers develop self-protecting electrolyte that completely blocks thermal runaway in Ah-scale sodium-ion batteries.](https://api3.cls.cn/share/article/2335878?os=android&amp;sv=8.7.5&amp;app=cailianpress) ⭐️ 8.0/10

On April 6, a team led by Hu Yongsheng from the Institute of Physics, Chinese Academy of Sciences, published a breakthrough in Nature Energy, announcing the development of a polymerizable non-flammable electrolyte (PNE) with self-protecting capabilities. This marks the first time globally that thermal runaway has been completely blocked in Ah-scale sodium-ion batteries. This breakthrough fundamentally challenges the conventional safety paradigm that 'flame-retardant electrolyte equals safety' and establishes a comprehensive 'thermal stability-interface stability-physical isolation' protection system. It paves a solid technical path for the safe commercialization of sodium-ion batteries in high-risk applications like electric vehicles and large-scale energy storage, potentially accelerating their adoption. The PNE electrolyte automatically solidifies from a liquid into a dense barrier when the battery temperature abnormally rises above 150°C, acting as an 'intelligent firewall' to cut off the propagation path of thermal runaway. Crucially, this safety enhancement is achieved without sacrificing the battery's high performance, which includes excellent wide-temperature performance and high-voltage stability.

telegram · zaihuapd · Apr 6, 14:10

**Background**: Sodium-ion batteries are an emerging energy storage technology that uses abundant and low-cost sodium instead of lithium. Thermal runaway is a critical safety hazard where a battery's internal heat generation exceeds its dissipation, leading to a rapid, uncontrollable temperature increase that can cause fire or explosion. Ah-scale refers to battery cells with capacities measured in ampere-hours (Ah), representing a practical size relevant for commercial applications like EVs and grid storage.

<details><summary>References</summary>
<ul>
<li><a href="https://www.ossila.com/pages/thermal-runaway">What is Thermal Runaway in Batteries ? Causes | Ossila</a></li>
<li><a href="https://en.wikipedia.org/wiki/Sodium-ion_battery">Sodium-ion battery - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#battery-technology`, `#sodium-ion`, `#energy-storage`, `#materials-science`, `#electrochemistry`

---

<a id="item-7"></a>
## [SGLang v0.5.10 enhances MoE fault tolerance, GPU throughput, and sparse attention.](https://github.com/sgl-project/sglang/releases/tag/v0.5.10) ⭐️ 7.0/10

SGLang v0.5.10 was released, introducing elastic partial failure tolerance for Mixture-of-Experts (MoE) models, GPU staging buffers that improve throughput by up to 5x, piecewise CUDA graph capture as the default, and integration of the HiSparse sparse attention backend. The release also includes major upgrades like FlashInfer MXFP8 kernel support, an update to Transformers 5.3.0, and optimizations for models like DeepSeek V3.2 and Qwen3.5. This release significantly improves the reliability and performance of large language model serving in production, especially for large-scale MoE models like DeepSeek. The partial failure tolerance feature prevents a single GPU failure from halting the entire service, while the performance optimizations directly reduce inference costs and latency, making advanced LLM deployment more robust and economical. The elastic partial failure tolerance, based on Elastic NIXL-EP, redistributes expert weights when a GPU fails, allowing service to continue without a full restart. The GPU staging buffer achieves a ~5x throughput improvement by gathering scattered head slices for bulk RDMA transfers, reducing request counts by ~1000x for GQA models. Piecewise CUDA graph is now the default to handle variable token counts in prefill/extend phases.

github · Fridge003 · Apr 6, 04:42

**Background**: SGLang is a high-performance language model serving system designed for efficient inference. Mixture-of-Experts (MoE) models are large language models where different parts of the network (experts) are activated for different inputs, improving efficiency but complicating distributed serving. Piecewise CUDA Graph is a technique that splits the model's computation graph into pieces to handle variable-length inputs more efficiently than a single, static CUDA graph. Sparse attention is an optimization that reduces the computational cost of the attention mechanism by focusing only on a subset of token interactions, which is crucial for long-context inference.

<details><summary>References</summary>
<ul>
<li><a href="https://www.lmsys.org/blog/2026-03-25-eep-partial-failure-tolerance/">Elastic EP in SGLang: Achieving Partial Failure Tolerance for DeepSeek MoE Deployments - LMSYS Blog | LMSYS Org</a></li>
<li><a href="https://docs.sglang.io/advanced_features/piecewise_cuda_graph.html">Piecewise CUDA Graph — SGLang</a></li>
<li><a href="https://nvidia.github.io/TensorRT-LLM/blogs/tech_blog/blog17_Sparse_Attention_in_TensorRT-LLM.html">Sparse Attention in TensorRT LLM — TensorRT LLM</a></li>

</ul>
</details>

**Tags**: `#llm-serving`, `#gpu-optimization`, `#model-inference`, `#distributed-systems`, `#sparse-attention`

---

<a id="item-8"></a>
## [Google releases official AI Edge Gallery app for running Gemma 4 models on iPhone](https://simonwillison.net/2026/Apr/6/google-ai-edge-gallery/#atom-everything) ⭐️ 7.0/10

Google has released an official iOS app called AI Edge Gallery that enables users to run Gemma 4 models (specifically the E2B and E4B sizes) directly on iPhones. The app provides practical features including image analysis, audio transcription up to 30 seconds, and a demonstration of tool calling through eight interactive widgets. This represents a significant step in edge AI deployment, as it's the first time a major model vendor has released an official app for local model testing on iPhones. It demonstrates the practical viability of on-device AI for mobile users, reducing reliance on cloud services while maintaining useful functionality. The Gemma 4 E2B model requires a 2.54GB download and reportedly performs well with fast response times. However, the app currently lacks conversation logging (making chats ephemeral), and the interactive skills demo reportedly froze when attempting follow-up prompts during testing.

rss · Simon Willison · Apr 6, 05:18

**Background**: Gemma 4 is Google's family of open language models that come in four sizes, with the E2B and E4B variants specifically designed for mobile and edge device deployment. Edge AI refers to running artificial intelligence models directly on local devices rather than in the cloud, offering benefits like reduced latency, improved privacy, and offline functionality. Tool calling is a capability that allows AI models to interact with external systems and APIs, enabling them to perform actions beyond text generation.

<details><summary>References</summary>
<ul>
<li><a href="https://ai.google.dev/gemma/docs/core/model_card_4">Gemma 4 model card | Google AI for Developers</a></li>
<li><a href="https://arxiv.org/abs/2503.06027">[2503.06027] Empowering Edge Intelligence: A Comprehensive ...</a></li>
<li><a href="https://machinelearningmastery.com/mastering-llm-tool-calling-the-complete-framework-for-connecting-models-to-the-real-world/">Mastering LLM Tool Calling: The Complete Framework for ...</a></li>

</ul>
</details>

**Tags**: `#edge-ai`, `#mobile-ai`, `#gemma`, `#on-device-inference`, `#google-ai`

---

<a id="item-9"></a>
## [Apple Blocks Updates for AI-Powered Code Generation Apps Like Replit and Vibecode on App Store](https://t.me/zaihuapd/40710) ⭐️ 7.0/10

Apple has recently blocked updates to AI programming applications, including Replit and Vibecode, on the App Store. These apps allow users to generate and run code or web applications directly within the app using natural language prompts. This action represents a significant enforcement of App Store policies against a new class of AI-assisted development tools that could bypass traditional app review. It highlights the tension between platform governance and the rapid evolution of low-code/no-code and AI-powered software creation, potentially impacting developers and startups relying on these platforms for iOS distribution. Apple's primary concern is that these 'vibe coding' apps could allow the instant generation and distribution of unvetted third-party software directly on iOS devices, effectively circumventing the official App Store review process. The block currently applies to app updates, not necessarily the existing versions available for download.

telegram · zaihuapd · Apr 6, 03:46

**Background**: Vibe coding is an AI-assisted software development practice where a developer describes a task in a prompt to a large language model (LLM), which then generates source code automatically. The term was coined by Andrej Karpathy in early 2025. Replit is an online coding platform that evolved into an AI-powered software creation ecosystem where users can build applications by describing them in natural language. Apple's App Review Guidelines are designed to ensure the security, performance, and content compliance of all apps on its store, and the company has historically acted against technologies that allow dynamic code changes post-review to bypass this process.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Vibe_coding">Vibe coding</a></li>
<li><a href="https://en.wikipedia.org/wiki/Replit">Replit - Wikipedia</a></li>
<li><a href="https://developer.apple.com/app-store/review/guidelines/">App Review Guidelines - Apple Developer</a></li>

</ul>
</details>

**Tags**: `#App Store Policy`, `#AI Programming`, `#Low-Code Development`, `#Platform Governance`, `#Replit`

---