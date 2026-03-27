---
layout: default
title: "Horizon Summary: 2026-03-27 (ZH)"
date: 2026-03-27
lang: zh
---

> From 25 items, 8 important content pieces were selected

---

1. [谷歌宣布在 Android 17 中引入后量子加密](#item-1) ⭐️ 9.0/10
2. [开发者发布实时记录，详述发现并应对 LiteLLM PyPI 恶意软件攻击的过程](#item-2) ⭐️ 8.0/10
3. [交互式教育文章通过卓越的可视化解释大语言模型量化技术](#item-3) ⭐️ 8.0/10
4. [Apifox 桌面端遭供应链投毒攻击，CDN 脚本被篡改](#item-4) ⭐️ 8.0/10
5. [中科院发布“香山”开源 RISC-V 处理器和“如意”原生操作系统](#item-5) ⭐️ 8.0/10
6. [日本团队第 58 代克隆小鼠出生次日死亡，或证明哺乳动物克隆存在极限。](#item-6) ⭐️ 8.0/10
7. [Google 发布 Gemini 3.1 Flash Live，Gemini Live 提速，Search Live 扩至 200 多个国家和地区](#item-7) ⭐️ 8.0/10
8. [团队用 AI 一天内将 JSONata 移植到 Go，实现每年 50 万美元成本节约](#item-8) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [谷歌宣布在 Android 17 中引入后量子加密](https://security.googleblog.com/2026/03/post-quantum-cryptography-in-android.html) ⭐️ 9.0/10

谷歌宣布计划在 Android 17 中引入后量子加密（PQC）标准，具体措施包括在引导加载程序（Bootloader）中加入具备量子抗性的数字签名，并将 Android 密钥库（Keystore）迁移至符合 PQC 标准的体系。这一前瞻性升级旨在保护设备启动过程，并防范未来量子计算对身份验证和敏感信息传输的威胁。 此次集成代表了移动安全基础设施的一次范式转变，因为这是后量子加密在广泛使用的消费级操作系统中的首批重大实施之一。它主动应对了“现在收集，以后解密”的威胁（即今日被截获的加密数据未来可能被量子计算机解密），从而为数十亿 Android 设备及其通信提供了长期安全保障。 谷歌正在实施 NIST 标准化的 ML-DSA 量子抗性签名算法，并设定了在 2029 年前完成此次迁移的时间表，早于 NIST 建议的 2030 年最后期限。此次升级聚焦于两个关键层面：引导加载程序（以维持安全的启动链）和密钥库（以保护应用与服务器之间的身份验证和数据加密）。

telegram · zaihuapd · Mar 26, 07:09

**背景**: 后量子加密（PQC）指的是设计用于抵御经典计算机和未来量子计算机攻击的加密算法。2024 年 8 月，美国国家标准与技术研究院（NIST）发布了其首套最终版 PQC 标准，包括用于加密和数字签名的算法，以保护电子信息。安全的引导加载程序在设备启动期间验证软件的完整性，而 Android 密钥库是一项系统服务，用于在安全的硬件支持容器中管理和存储应用程序的加密密钥。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.nist.gov/news-events/news/2024/08/nist-releases-first-3-finalized-post-quantum-encryption-standards">NIST Releases First 3 Finalized Post-Quantum Encryption Standards</a></li>
<li><a href="https://bootlin.com/blog/the-nists-new-plan-for-digital-signatures-impact-on-secure-boot/">The NIST’s new plan for digital signatures : impact on secure boot ...</a></li>
<li><a href="https://winbuzzer.com/2026/03/26/google-android-17-quantum-resistant-encryption-pqc-xcxwbn/">Android 17 Gets Quantum-Safe Encryption Across Full Security ...</a></li>

</ul>
</details>

**标签**: `#post-quantum-cryptography`, `#android-security`, `#quantum-computing`, `#mobile-security`, `#cryptography`

---

<a id="item-2"></a>
## [开发者发布实时记录，详述发现并应对 LiteLLM PyPI 恶意软件攻击的过程](https://futuresearch.ai/blog/litellm-attack-transcript/) ⭐️ 8.0/10

一位名叫 Callum 的开发者发布了一份未经编辑的、按分钟记录的实时文字稿，详细记录了他发现并应对针对 PyPI 上 LiteLLM Python 包 1.82.7 和 1.82.8 版本的供应链攻击的过程。这份文字稿使用了一个记录与 Claude AI 助手交互的工具创建，详细描述了识别出一个旨在窃取凭证的恶意 `.pth` 文件的实时调查过程。 这一事件凸显了 AI/ML 生态系统中供应链攻击的严重风险，因为 LiteLLM 是一个广泛使用的、用于统一调用超过 100 个大语言模型 API 的库。这份第一人称的叙述为一次复杂的攻击的检测和缓解过程提供了宝贵的、真实的见解，该攻击本可能大规模地危害 AI 流水线和云凭证。 恶意软件是通过一个 `.pth` 文件传递的，该文件在每次 Python 启动时都会执行，而不仅仅是在包导入时，这使其成为一种持久且隐蔽的威胁。受感染的版本旨在将环境变量、SSH 密钥和云凭证外泄到攻击者控制的服务器，构成了一个多阶段的凭证窃取程序。

hackernews · Fibonar · Mar 26, 15:48

**背景**: LiteLLM 是一个开源的 Python 库，它为调用来自 OpenAI、Anthropic 和 Google 等提供商的各种大语言模型 (LLM) API 提供了一个统一的接口。PyPI (Python 包索引) 是 Python 软件的主要仓库，这使其成为关键的基础设施，也是供应链攻击的常见目标，即恶意代码被插入到合法的软件包中。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.truesec.com/hub/blog/malicious-pypi-package-litellm-supply-chain-compromise">Malicious PyPI Package - LiteLLM Supply Chain Compromise - Truesec</a></li>
<li><a href="https://docs.litellm.ai/docs/">Getting Started - LiteLLM Docs</a></li>
<li><a href="https://blog.pypi.org/posts/2024-12-11-ultralytics-attack-analysis/">Supply-chain attack analysis: Ultralytics - The Python Package Index Blog</a></li>

</ul>
</details>

**社区讨论**: 社区讨论证实了此次攻击的重要性，评论者强调了 `.pth` 文件执行的隐蔽性，以及对软件包注册表进行更好的实时安全监控的必要性。此外，还讨论了在安全调查中负责任地使用 AI 助手，并警告要避免意外执行恶意代码。

**标签**: `#security`, `#supply-chain`, `#python`, `#malware`, `#incident-response`

---

<a id="item-3"></a>
## [交互式教育文章通过卓越的可视化解释大语言模型量化技术](https://simonwillison.net/2026/Mar/26/quantization-from-the-ground-up/#atom-everything) ⭐️ 8.0/10

Sam Rose 发表了一篇名为《Quantization from the ground up》的交互式教育文章，解释了大语言模型的量化技术，其中包含被 Simon Willison 称为“我所见过的最佳视觉解释”的浮点数二进制表示法可视化。文章还通过使用 Qwen 3.5 9B 模型和 llama.cpp 工具进行了实际分析，展示了不同量化级别（从 16 位到 8 位和 4 位）如何影响模型精度。 这很重要，因为量化对于在手机和边缘设备等资源受限的设备上部署大语言模型至关重要，而清晰的教育资源有助于更多开发者有效理解和实施这些优化技术。卓越的可视化解释使浮点数表示和异常值等复杂概念变得易于理解，可以加速量化技术在实际应用中的采用。 文章强调了量化中“异常值”或“超级权重”的重要性——这些罕见的浮点数值对模型质量至关重要，移除单个此类值就可能导致模型输出乱码，因此在量化方案中需要特殊处理。实际测试表明，从 16 位量化到 8 位几乎不会造成质量损失，而从 16 位量化到 4 位则能保留大约 90% 的原始质量，具体取决于测量方法。

rss · Simon Willison · Mar 26, 16:21

**背景**: 量化是一种降低神经网络中数值精度的技术，通常将 32 位或 16 位浮点数转换为 8 位整数或 4 位值等低位表示，从而减少模型大小和计算需求。这对于大语言模型尤为重要，因为未经优化，这些模型通常太大而无法在消费级硬件上高效运行。计算机中的浮点数表示使用二进制位来存储数字，包含三个部分：符号位、指数和有效数（尾数），IEEE 754 是标准格式。困惑度和 KL 散度分别是用于评估语言模型性能和概率分布之间差异的指标，有助于量化量化对模型精度的影响。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arxiv.org/html/2411.02530v1">A Comprehensive Study on Quantization Techniques for Large ...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Floating-point_arithmetic">Floating-point arithmetic - Wikipedia</a></li>
<li><a href="https://github.com/pprp/Awesome-LLM-Quantization">Awesome-LLM-Quantization - GitHub</a></li>

</ul>
</details>

**标签**: `#quantization`, `#llm-optimization`, `#machine-learning`, `#educational-content`, `#floating-point`

---

<a id="item-4"></a>
## [Apifox 桌面端遭供应链投毒攻击，CDN 脚本被篡改](https://t.me/zaihuapd/40514) ⭐️ 8.0/10

Apifox 桌面端遭到供应链投毒攻击，攻击者篡改了其官方 CDN 上托管的一个前端事件统计脚本。自 3 月 4 日起活跃的注入恶意代码会窃取受影响 Windows、macOS 和 Linux 系统中的 SSH 密钥、Git 凭证、Shell 历史记录和进程列表。 此次攻击影响重大，因为 Apifox 是一款广泛使用的 API 开发工具，其桌面客户端被入侵直接针对了通常持有访问源代码和基础设施的高价值凭证的开发者。此类供应链攻击可能导致大规模数据泄露和在企业内部网络中的横向移动，对组织的知识产权和运营安全构成严重威胁。 安全研究员 phith0n 已独立分析并公开了恶意载荷的细节。攻击向量涉及篡改受信任的外部托管脚本（一种常见的 CDN 风险），展示了攻击者如何能够入侵团队已经信任并正在积极使用的工具。

telegram · zaihuapd · Mar 26, 04:19

**背景**: Apifox 是一个集 API 文档、调试、Mock 和测试于一体的平台，常被比作 Postman 和 Swagger 等工具。供应链攻击是指攻击者入侵一个被许多下游应用或用户信任和使用的组件或服务（如 CDN 托管的脚本）。SSH 密钥和 Git 凭证是关键访问令牌；窃取它们可使攻击者获得对私有源代码仓库和安全服务器的未授权访问。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.binance.com/en/square/post/03-26-2026-apifox-desktop-client-faces-supply-chain-attack-with-malicious-code-injection-305605946597617">Apifox Desktop Client Faces... | Binance News on Binance Square</a></li>
<li><a href="https://developer.mozilla.org/en-US/docs/Web/Security/Attacks/Supply_chain_attacks">Supply chain attacks - Security | MDN</a></li>
<li><a href="https://www.kodemsecurity.com/resources/when-the-scanner-becomes-the-threat-inside-the-trivy-supply-chain-attack">When the Scanner Becomes the Threat: Inside the Trivy Supply ...</a></li>

</ul>
</details>

**标签**: `#security`, `#supply-chain-attack`, `#developer-tools`, `#credential-theft`, `#malware`

---

<a id="item-5"></a>
## [中科院发布“香山”开源 RISC-V 处理器和“如意”原生操作系统](https://h.xinhuaxmt.com/vh512/share/13024070?docid=13024070) ⭐️ 8.0/10

3 月 26 日，在中关村论坛年会的 RISC-V 生态科技论坛上，中国科学院正式发布了“香山”开源高性能 RISC-V 处理器和“如意”原生操作系统。同时，论坛启动了下一代“昆明湖”架构与“如意”操作系统的联合开发，中国移动、中国电信、中兴、阿里、腾讯、字节跳动等数十家单位将参与协同攻关。 此次发布是中国推动开源硬件和软件生态发展的一个重要里程碑，有助于减少对专有架构的依赖。众多头部科技公司和电信运营商的参与，表明了强大的产业投入决心，将加速其商业化进程并推动构建一个健壮的国内 RISC-V 生态。 “香山”处理器据称达到了国际先进性能水平，并同步推出了全球首个开源片上互连网络 IP。基于“香山”的高性能开源芯片已实现规模化产业落地，进迭时空、蓝芯算力、芯动科技、奕斯伟计算等企业已推出商用芯片。“如意”操作系统的特点是率先全面支持国际标准。

telegram · zaihuapd · Mar 26, 10:08

**背景**: RISC-V 是一个基于精简指令集计算机原则的免费开放标准指令集架构，允许任何人在无需支付授权费的情况下设计、制造和销售 RISC-V 芯片及软件。片上互连网络是芯片多处理器内部连接核心、内存及其他模块的关键组件，决定了系统的整体性能和可扩展性。原生操作系统是指为直接在特定处理器的指令集上运行而构建的软件，无需通过翻译层，与通过抽象层在多种架构上运行的通用操作系统相比，通常能提供更高的性能和效率。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/RISC-V">RISC - V - Wikipedia</a></li>
<li><a href="https://www.academia.edu/4851977/On_Chip_Interconnection_Networks_Why_They_are_Different_and_How_to_Compare_Them">(PDF) On - Chip Interconnection Networks : Why They are Different...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Native_(computing)">Native (computing) - Wikipedia</a></li>

</ul>
</details>

**标签**: `#RISC-V`, `#Open-Source Hardware`, `#Operating Systems`, `#Computer Architecture`, `#China Tech`

---

<a id="item-6"></a>
## [日本团队第 58 代克隆小鼠出生次日死亡，或证明哺乳动物克隆存在极限。](https://www.nature.com/articles/s41467-026-69765-7) ⭐️ 8.0/10

日本研究团队历时 20 年，从一只雌性小鼠出发，成功克隆了 58 代、超过 1200 只克隆鼠。第 58 代克隆鼠全部在出生后第二天死亡，而到第 57 代时，小鼠的存活率已不足 1%。 这项研究首次提供了长期实验证据，表明哺乳动物的连续克隆存在根本性的生物学极限，因为遗传错误会代代累积，最终导致繁殖失败。它挑战了通过克隆无限期维持一个物种的理论可能性，并对理解遗传稳定性、生殖技术和保护生物学具有重要意义。 研究发现，克隆过程中新生突变的发生率约为自然繁殖后代的 3 倍，并且从第 25 代之后开始出现显著的染色体异常，例如整条 X 染色体的丢失。虽然前 25 代克隆鼠相对健康，但从第 27 代起，观察到繁殖力下降、产仔数减少和胎盘增大等现象。

telegram · zaihuapd · Mar 26, 16:46

**背景**: 克隆，特指体细胞核移植技术，涉及将成年动物的体细胞核取出，移植到已去除细胞核的卵细胞中。这项因克隆羊多莉而闻名的技术，可以产生遗传上完全相同的个体。连续克隆是指反复使用一个克隆体的细胞来创造下一代克隆体的过程，这种方法用于测试这种繁殖方式的长期生存能力和遗传稳定性。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.nature.com/articles/s41467-026-69765-7">Limitations of serial cloning in mammals - Nature</a></li>
<li><a href="https://www.sciencealert.com/dead-end-radical-20-year-study-reveals-genetic-cloning-hits-a-limit">'Dead End': Radical 20-Year Study Reveals Genetic Cloning Hits a Limit</a></li>

</ul>
</details>

**标签**: `#cloning`, `#genetics`, `#reproductive-biology`, `#longitudinal-study`, `#mammalian-research`

---

<a id="item-7"></a>
## [Google 发布 Gemini 3.1 Flash Live，Gemini Live 提速，Search Live 扩至 200 多个国家和地区](https://blog.google/innovation-and-ai/models-and-research/gemini-models/gemini-3-1-flash-live/) ⭐️ 8.0/10

Google 发布了实时音频与语音模型 Gemini 3.1 Flash Live，并将其接入 Gemini Live、Search Live、Gemini Enterprise for Customer Experience，以及在 Google AI Studio 中以预览版开放的 Gemini Live API。该模型支持 90 多种语言的实时多模态对话，并强化了复杂指令遵循、外部工具调用、声学细节识别以及在嘈杂环境中的语音处理能力。 此次发布通过使交互更快、更自然且全球可访问，显著提升了实时对话式 AI 的能力。它使得与 AI 助手的对话更加流畅持久，并将多模态搜索的覆盖范围扩展至全球广大用户，可能为语音和音频 AI 应用设定新的标准。 在 Android 和 iOS 的 Gemini Live 中，新模型带来了更快的响应、更少的停顿，并将连续对话的上下文保持时间提升至此前的两倍。Gemini Live API 专为生产环境设计，已于今日起通过 Gemini API 和 Google AI Studio 提供。

telegram · zaihuapd · Mar 26, 17:01

**背景**: 多模态对话系统是一种能够处理和理解来自文本、图像、音频和视频等多种信息源的 AI 模型，以进行更自然、更具上下文感知的对话。实时语音 AI 模型同时处理语音输入和输出，以最小化延迟，实现更流畅、更接近人类的交互。Google 的 Gemini 模型系列是其旗舰多模态 AI 系统套件，旨在快速发展的生成式 AI 领域参与竞争。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://deepmind.google/models/model-cards/gemini-3-1-flash-live/">Gemini 3.1 Flash Live - Model Card — Google DeepMind</a></li>
<li><a href="https://blog.google/innovation-and-ai/models-and-research/gemini-models/gemini-3-1-flash-live/">Gemini 3.1 Flash Live: Making audio AI more natural and reliable</a></li>
<li><a href="https://braintitan.medium.com/mini-omni-real-time-voice-ai-model-supports-thinking-while-talking-28d554cbb9f8">Mini-Omni: Real - Time Voice AI Model Supports ‘Thinking... | Medium</a></li>

</ul>
</details>

**标签**: `#AI`, `#Google`, `#Multimodal AI`, `#Voice AI`, `#Real-time Systems`

---

<a id="item-8"></a>
## [团队用 AI 一天内将 JSONata 移植到 Go，实现每年 50 万美元成本节约](https://simonwillison.net/2026/Mar/27/vine-porting-jsonata/#atom-everything) ⭐️ 7.0/10

Reco 团队利用 AI 辅助开发，在 7 小时内将 JSONata JSON 查询语言从其原始的 JavaScript 实现移植到 Go，花费了约 400 美元的 AI 代币。他们通过为期一周的影子部署验证了新实现，并行运行两个版本以确保行为一致。 这个案例研究展示了'氛围移植'（vibe-porting）——利用 AI 和现有测试套件快速重写代码库——的实际和经济影响。它表明 AI 可以加速基础设施现代化，带来显著的性能提升和运营成本降低，可能影响团队处理遗留系统迁移的方式。 移植工作严重依赖 JSONata 现有的全面测试套件来指导 AI 并验证正确性。最终生成的 Go 实现预计比 JavaScript 版本带来显著的性能提升，这直接转化为预计的每年 50 万美元的成本节约。

rss · Simon Willison · Mar 27, 00:35

**背景**: JSONata 是一种专为 JSON 数据设计的轻量级查询和转换语言，类似于 jq，但其语法灵感来源于 XPath。它通常用于 Node-RED 等平台中进行数据操作。'氛围移植'或'氛围编码'是一种新兴的 AI 辅助开发模式，开发者使用详细的提示词和现有的测试套件来指导大语言模型移植或重写软件组件。影子部署是一种测试策略，新版本的应用程序与生产版本并行运行，处理真实流量的副本而不影响用户，以在真实条件下验证正确性和性能。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://jsonata.org/">JSONata</a></li>
<li><a href="https://tsjohnnychan.medium.com/vibe-coding-series-you-do-not-have-to-start-from-scratch-77c13a48853a">Vibe Coding Series — You Do Not Have To Start From Scratch</a></li>
<li><a href="https://www.devopstraininginstitute.com/blog/what-is-shadow-deployment-and-how-is-it-used-for-risk-free-testing">What Is Shadow Deployment and How Is It Used for Risk-Free ...</a></li>

</ul>
</details>

**标签**: `#ai-assisted-development`, `#code-porting`, `#go`, `#jsonata`, `#cost-optimization`

---