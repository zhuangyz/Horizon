---
layout: default
title: "Horizon Summary: 2026-03-27 (EN)"
date: 2026-03-27
lang: en
---

> From 25 items, 8 important content pieces were selected

---

1. [Google Announces Post-Quantum Cryptography Integration in Android 17](#item-1) ⭐️ 9.0/10
2. [Developer publishes real-time transcript of discovering and responding to LiteLLM PyPI malware attack](#item-2) ⭐️ 8.0/10
3. [Interactive educational essay explains LLM quantization with exceptional visualizations](#item-3) ⭐️ 8.0/10
4. [Apifox Desktop Client Compromised in Supply Chain Attack via CDN Script](#item-4) ⭐️ 8.0/10
5. [Chinese Academy of Sciences Launches 'Xiangshan' Open-Source RISC-V Processor and 'Ruyi' Native OS](#item-5) ⭐️ 8.0/10
6. [58th-generation cloned mouse dies after one day, suggesting a fundamental limit to mammalian cloning.](#item-6) ⭐️ 8.0/10
7. [Google Launches Gemini 3.1 Flash Live, Speeds Up Gemini Live, and Expands Search Live to 200+ Countries](#item-7) ⭐️ 8.0/10
8. [AI-Powered Port of JSONata to Go Completed in One Day, Saving $500K Annually](#item-8) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [Google Announces Post-Quantum Cryptography Integration in Android 17](https://security.googleblog.com/2026/03/post-quantum-cryptography-in-android.html) ⭐️ 9.0/10

Google has announced plans to integrate post-quantum cryptography (PQC) standards into Android 17, specifically by adding quantum-resistant digital signatures to the bootloader and migrating the Android Keystore to a PQC-compliant system. This proactive upgrade aims to secure the device boot process and protect authentication and sensitive data transmission against future quantum computing threats. This integration represents a paradigm shift in mobile security infrastructure, as it is one of the first major implementations of PQC in a widely-used consumer operating system. It proactively addresses the 'harvest now, decrypt later' threat, where encrypted data intercepted today could be decrypted by future quantum computers, thereby safeguarding billions of Android devices and their communications for the long term. Google is implementing the NIST-standardized ML-DSA quantum-resistant signature algorithm and has set a timeline to complete this migration by 2029, ahead of NIST's suggested 2030 mandate. The upgrade focuses on two critical layers: the bootloader to maintain a secure boot chain and the Keystore to protect app-to-server authentication and data encryption.

telegram · zaihuapd · Mar 26, 07:09

**Background**: Post-quantum cryptography (PQC) refers to cryptographic algorithms designed to be secure against attacks by both classical and future quantum computers. In August 2024, NIST released its first set of finalized PQC standards, including algorithms for encryption and digital signatures, to protect electronic information. A secure bootloader verifies the integrity of software during device startup, while the Android Keystore is a system service that manages and stores cryptographic keys for apps in a secure hardware-backed container.

<details><summary>References</summary>
<ul>
<li><a href="https://www.nist.gov/news-events/news/2024/08/nist-releases-first-3-finalized-post-quantum-encryption-standards">NIST Releases First 3 Finalized Post-Quantum Encryption Standards</a></li>
<li><a href="https://bootlin.com/blog/the-nists-new-plan-for-digital-signatures-impact-on-secure-boot/">The NIST’s new plan for digital signatures : impact on secure boot ...</a></li>
<li><a href="https://winbuzzer.com/2026/03/26/google-android-17-quantum-resistant-encryption-pqc-xcxwbn/">Android 17 Gets Quantum-Safe Encryption Across Full Security ...</a></li>

</ul>
</details>

**Tags**: `#post-quantum-cryptography`, `#android-security`, `#quantum-computing`, `#mobile-security`, `#cryptography`

---

<a id="item-2"></a>
## [Developer publishes real-time transcript of discovering and responding to LiteLLM PyPI malware attack](https://futuresearch.ai/blog/litellm-attack-transcript/) ⭐️ 8.0/10

A developer named Callum has published an unedited, minute-by-minute transcript documenting his discovery and response to a supply chain attack targeting versions 1.82.7 and 1.82.8 of the LiteLLM Python package on PyPI. The transcript, created using a tool to log interactions with the Claude AI assistant, details the real-time investigation that identified a malicious `.pth` file designed to steal credentials. This incident highlights the severe risks of supply chain attacks in the AI/ML ecosystem, as LiteLLM is a widely used library for unifying API calls to over 100 large language models. The first-person account provides invaluable, real-world insight into the detection and mitigation process for a sophisticated attack that could have compromised AI pipelines and cloud credentials on a massive scale. The malware was delivered via a `.pth` file, which executes on every Python startup, not just during package import, making it a persistent and stealthy threat. The compromised versions were designed to exfiltrate environment variables, SSH keys, and cloud credentials to an attacker-controlled server, constituting a multi-stage credential stealer.

hackernews · Fibonar · Mar 26, 15:48

**Background**: LiteLLM is an open-source Python library that provides a unified interface for calling various large language model (LLM) APIs from providers like OpenAI, Anthropic, and Google. PyPI (the Python Package Index) is the primary repository for Python software, making it a critical piece of infrastructure and a frequent target for supply chain attacks, where malicious code is inserted into legitimate software packages.

<details><summary>References</summary>
<ul>
<li><a href="https://www.truesec.com/hub/blog/malicious-pypi-package-litellm-supply-chain-compromise">Malicious PyPI Package - LiteLLM Supply Chain Compromise - Truesec</a></li>
<li><a href="https://docs.litellm.ai/docs/">Getting Started - LiteLLM Docs</a></li>
<li><a href="https://blog.pypi.org/posts/2024-12-11-ultralytics-attack-analysis/">Supply-chain attack analysis: Ultralytics - The Python Package Index Blog</a></li>

</ul>
</details>

**Discussion**: The community discussion validated the attack's significance, with commenters highlighting the stealthy nature of `.pth` file execution and the need for better real-time security monitoring of package registries. There was also discussion about the responsible use of AI assistants in security investigations, cautioning against accidentally executing malicious code.

**Tags**: `#security`, `#supply-chain`, `#python`, `#malware`, `#incident-response`

---

<a id="item-3"></a>
## [Interactive educational essay explains LLM quantization with exceptional visualizations](https://simonwillison.net/2026/Mar/26/quantization-from-the-ground-up/#atom-everything) ⭐️ 8.0/10

Sam Rose published an interactive educational essay titled 'Quantization from the ground up' that explains quantization techniques for Large Language Models, featuring what Simon Willison calls 'the best visual explanation I've ever seen' of floating-point number representation using binary digits. The essay includes practical analysis showing how different quantization levels (16-bit to 8-bit and 4-bit) affect model accuracy using the Qwen 3.5 9B model and llama.cpp tools. This matters because quantization is essential for deploying large language models on resource-constrained devices like mobile phones and edge devices, and clear educational resources help more developers understand and implement these optimization techniques effectively. The exceptional visual explanations make complex concepts like floating-point representation and outlier values accessible, which can accelerate adoption of quantization in real-world applications. The essay highlights the importance of 'outlier values' or 'super weights' in quantization—rare float values that are critical to model quality, where removing even a single one can cause the model to output gibberish, requiring special handling in quantization schemes. Practical testing shows that 16-bit to 8-bit quantization carries almost no quality penalty, while 16-bit to 4-bit quantization retains approximately 90% of original quality depending on measurement method.

rss · Simon Willison · Mar 26, 16:21

**Background**: Quantization is a technique that reduces the precision of numerical values in neural networks, typically from 32-bit or 16-bit floating-point numbers to lower-bit representations like 8-bit integers or 4-bit values, which decreases model size and computational requirements. This is particularly important for Large Language Models (LLMs) which are often too large to run efficiently on consumer hardware without optimization. Floating-point representation in computers uses binary digits to store numbers with three components: sign bit, exponent, and significand (mantissa), with IEEE 754 being the standard format. Perplexity and KL divergence are metrics used to evaluate language model performance and the difference between probability distributions, respectively, which help quantify the impact of quantization on model accuracy.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/html/2411.02530v1">A Comprehensive Study on Quantization Techniques for Large ...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Floating-point_arithmetic">Floating-point arithmetic - Wikipedia</a></li>
<li><a href="https://github.com/pprp/Awesome-LLM-Quantization">Awesome-LLM-Quantization - GitHub</a></li>

</ul>
</details>

**Tags**: `#quantization`, `#llm-optimization`, `#machine-learning`, `#educational-content`, `#floating-point`

---

<a id="item-4"></a>
## [Apifox Desktop Client Compromised in Supply Chain Attack via CDN Script](https://t.me/zaihuapd/40514) ⭐️ 8.0/10

The Apifox desktop client was compromised in a supply chain attack where attackers modified a front-end analytics script hosted on its official CDN. The injected malicious code, active since March 4, steals SSH keys, Git credentials, shell history, and process lists from affected Windows, macOS, and Linux systems. This attack is significant because Apifox is a widely-used API development tool, and a compromise of its desktop client directly targets developers who often possess high-value credentials for accessing source code and infrastructure. Such supply chain attacks can lead to massive data breaches and lateral movement within corporate networks, posing a severe risk to organizations' intellectual property and operational security. Security researcher phith0n independently analyzed and published details of the malicious payload. The attack vector involved tampering with a trusted, externally hosted script (a common CDN risk), demonstrating how attackers can compromise tools that teams already trust and are actively using.

telegram · zaihuapd · Mar 26, 04:19

**Background**: Apifox is an integrated platform for API documentation, debugging, mocking, and testing, often compared to tools like Postman and Swagger. A supply chain attack occurs when an attacker compromises a component or service (like a CDN-hosted script) that is trusted and used by many downstream applications or users. SSH keys and Git credentials are critical access tokens; stealing them can grant attackers unauthorized access to private source code repositories and secure servers.

<details><summary>References</summary>
<ul>
<li><a href="https://www.binance.com/en/square/post/03-26-2026-apifox-desktop-client-faces-supply-chain-attack-with-malicious-code-injection-305605946597617">Apifox Desktop Client Faces... | Binance News on Binance Square</a></li>
<li><a href="https://developer.mozilla.org/en-US/docs/Web/Security/Attacks/Supply_chain_attacks">Supply chain attacks - Security | MDN</a></li>
<li><a href="https://www.kodemsecurity.com/resources/when-the-scanner-becomes-the-threat-inside-the-trivy-supply-chain-attack">When the Scanner Becomes the Threat: Inside the Trivy Supply ...</a></li>

</ul>
</details>

**Tags**: `#security`, `#supply-chain-attack`, `#developer-tools`, `#credential-theft`, `#malware`

---

<a id="item-5"></a>
## [Chinese Academy of Sciences Launches 'Xiangshan' Open-Source RISC-V Processor and 'Ruyi' Native OS](https://h.xinhuaxmt.com/vh512/share/13024070?docid=13024070) ⭐️ 8.0/10

On March 26, at the RISC-V Ecosystem Technology Forum of the Zhongguancun Forum Annual Conference, the Chinese Academy of Sciences (CAS) officially launched the open-source 'Xiangshan' high-performance RISC-V processor and the 'Ruyi' native operating system. The event also marked the kickoff of a joint development initiative for the next-generation 'Kunming Lake' architecture and the 'Ruyi' OS, involving dozens of major companies including China Mobile, China Telecom, ZTE, Alibaba, Tencent, and ByteDance. This launch represents a significant milestone in China's push for open-source hardware and software ecosystems, reducing reliance on proprietary architectures. The involvement of major tech firms and telecom operators signals strong industry commitment and accelerates the path towards commercial adoption and a robust domestic RISC-V ecosystem. The 'Xiangshan' processor is claimed to achieve internationally advanced performance levels and introduced the world's first open-source on-chip interconnect network IP. Commercial chips based on 'Xiangshan' are already in production by companies like InDie, Blue Core Computing, InnoSilicon, and ESWIN. The 'Ruyi' OS is noted for its comprehensive support of international standards.

telegram · zaihuapd · Mar 26, 10:08

**Background**: RISC-V is a free and open standard Instruction Set Architecture (ISA) based on reduced instruction set computer principles, enabling anyone to design, manufacture, and sell RISC-V chips and software without royalties. An on-chip interconnect network (OCIN or NoC) is a critical component within a chip multiprocessor that connects cores, memory, and other modules, determining overall system performance and scalability. A native operating system is software built to run directly on a specific processor's instruction set without translation layers, typically offering higher performance and efficiency compared to general-purpose OSes that run on various architectures through abstraction.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/RISC-V">RISC - V - Wikipedia</a></li>
<li><a href="https://www.academia.edu/4851977/On_Chip_Interconnection_Networks_Why_They_are_Different_and_How_to_Compare_Them">(PDF) On - Chip Interconnection Networks : Why They are Different...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Native_(computing)">Native (computing) - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#RISC-V`, `#Open-Source Hardware`, `#Operating Systems`, `#Computer Architecture`, `#China Tech`

---

<a id="item-6"></a>
## [58th-generation cloned mouse dies after one day, suggesting a fundamental limit to mammalian cloning.](https://www.nature.com/articles/s41467-026-69765-7) ⭐️ 8.0/10

A Japanese research team, after a 20-year study, has successfully created 58 generations of cloned mice from a single female, producing over 1200 individuals. The 58th generation of cloned mice all died the day after birth, and the survival rate had already dropped below 1% by the 57th generation. This research provides the first long-term experimental evidence that serial cloning in mammals has a fundamental biological limit, as genetic errors accumulate over generations, leading to reproductive failure. It challenges the theoretical possibility of maintaining a species indefinitely through cloning and has implications for understanding genetic stability, reproductive technologies, and conservation biology. The study found that de novo mutations accumulated at a rate about three times higher than in naturally bred offspring, and significant chromosomal abnormalities, such as the loss of an entire X chromosome, became prominent after the 25th generation. While the first 25 generations were relatively healthy, reproductive decline, reduced litter sizes, and enlarged placentas were observed from the 27th generation onward.

telegram · zaihuapd · Mar 26, 16:46

**Background**: Cloning, specifically somatic cell nuclear transfer (SCNT), involves taking the nucleus from a somatic (body) cell of an adult animal and transferring it into an egg cell that has had its own nucleus removed. This technique, famously used to create Dolly the sheep, can produce genetically identical copies of an individual. Serial cloning refers to the process of repeatedly using cells from one clone to create the next generation of clones, a method used to test the long-term viability and genetic stability of this form of reproduction.

<details><summary>References</summary>
<ul>
<li><a href="https://www.nature.com/articles/s41467-026-69765-7">Limitations of serial cloning in mammals - Nature</a></li>
<li><a href="https://www.sciencealert.com/dead-end-radical-20-year-study-reveals-genetic-cloning-hits-a-limit">'Dead End': Radical 20-Year Study Reveals Genetic Cloning Hits a Limit</a></li>

</ul>
</details>

**Tags**: `#cloning`, `#genetics`, `#reproductive-biology`, `#longitudinal-study`, `#mammalian-research`

---

<a id="item-7"></a>
## [Google Launches Gemini 3.1 Flash Live, Speeds Up Gemini Live, and Expands Search Live to 200+ Countries](https://blog.google/innovation-and-ai/models-and-research/gemini-models/gemini-3-1-flash-live/) ⭐️ 8.0/10

Google has released Gemini 3.1 Flash Live, a real-time audio and voice model, and integrated it into Gemini Live, Search Live, Gemini Enterprise for Customer Experience, and a preview version of the Gemini Live API in Google AI Studio. The model supports real-time multimodal conversations in over 90 languages, with improved instruction following, tool use, acoustic detail recognition, and noise handling. This release significantly advances the capabilities of real-time, conversational AI by making interactions faster, more natural, and globally accessible. It enables more fluid and extended conversations with AI assistants and expands the reach of multimodal search to a vast global audience, potentially setting a new standard for voice and audio AI applications. In Gemini Live on Android and iOS, the new model delivers faster responses with fewer pauses and doubles the context retention for continuous conversations. The Gemini Live API is designed for production environments and is available starting today via the Gemini API and Google AI Studio.

telegram · zaihuapd · Mar 26, 17:01

**Background**: Multimodal dialogue systems are AI models that can process and understand information from multiple sources, such as text, images, audio, and video, to conduct more natural and context-aware conversations. Real-time voice AI models process speech input and output simultaneously to minimize delays, enabling smoother, more human-like interactions. Google's Gemini family of models represents its flagship suite of multimodal AI systems designed to compete in the rapidly evolving generative AI landscape.

<details><summary>References</summary>
<ul>
<li><a href="https://deepmind.google/models/model-cards/gemini-3-1-flash-live/">Gemini 3.1 Flash Live - Model Card — Google DeepMind</a></li>
<li><a href="https://blog.google/innovation-and-ai/models-and-research/gemini-models/gemini-3-1-flash-live/">Gemini 3.1 Flash Live: Making audio AI more natural and reliable</a></li>
<li><a href="https://braintitan.medium.com/mini-omni-real-time-voice-ai-model-supports-thinking-while-talking-28d554cbb9f8">Mini-Omni: Real - Time Voice AI Model Supports ‘Thinking... | Medium</a></li>

</ul>
</details>

**Tags**: `#AI`, `#Google`, `#Multimodal AI`, `#Voice AI`, `#Real-time Systems`

---

<a id="item-8"></a>
## [AI-Powered Port of JSONata to Go Completed in One Day, Saving $500K Annually](https://simonwillison.net/2026/Mar/27/vine-porting-jsonata/#atom-everything) ⭐️ 7.0/10

The Reco team used AI-assisted development to port the JSONata JSON query language from its original JavaScript implementation to Go in just 7 hours, spending approximately $400 on AI tokens. They validated the new implementation through a week-long shadow deployment, running both versions in parallel to ensure behavioral equivalence. This case study demonstrates the practical and economic impact of 'vibe-porting'—using AI to rapidly rewrite codebases with existing test suites. It shows how AI can accelerate infrastructure modernization, leading to significant performance gains and operational cost reductions, potentially influencing how teams approach legacy system migrations. The porting effort relied heavily on JSONata's comprehensive existing test suite to guide the AI and verify correctness. The resulting Go implementation is expected to deliver substantial performance improvements over the JavaScript version, which directly translates to the projected $500,000 annual cost savings.

rss · Simon Willison · Mar 27, 00:35

**Background**: JSONata is a lightweight query and transformation language specifically designed for JSON data, similar to jq but with a syntax inspired by XPath. It is commonly used within platforms like Node-RED for data manipulation. 'Vibe-porting' or 'vibe-coding' is an emerging AI-assisted development pattern where developers use detailed prompts and existing test suites to guide LLMs in porting or rewriting software components. Shadow deployment is a testing strategy where a new version of an application runs alongside the production version, processing a copy of real traffic without affecting users, to validate correctness and performance under real-world conditions.

<details><summary>References</summary>
<ul>
<li><a href="https://jsonata.org/">JSONata</a></li>
<li><a href="https://tsjohnnychan.medium.com/vibe-coding-series-you-do-not-have-to-start-from-scratch-77c13a48853a">Vibe Coding Series — You Do Not Have To Start From Scratch</a></li>
<li><a href="https://www.devopstraininginstitute.com/blog/what-is-shadow-deployment-and-how-is-it-used-for-risk-free-testing">What Is Shadow Deployment and How Is It Used for Risk-Free ...</a></li>

</ul>
</details>

**Tags**: `#ai-assisted-development`, `#code-porting`, `#go`, `#jsonata`, `#cost-optimization`

---