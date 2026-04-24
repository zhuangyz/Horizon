---
layout: default
title: "Horizon Summary: 2026-04-24 (EN)"
date: 2026-04-24
lang: en
---

> From 29 items, 22 important content pieces were selected

---

1. [OpenAI Launches GPT-5.5, a New Frontier Coding Model](#item-1) ⭐️ 9.0/10
2. [Bitwarden CLI compromised in supply chain attack](#item-2) ⭐️ 9.0/10
3. [vLLM v0.20.0: CUDA 13, PyTorch 2.11, FA4, TurboQuant](#item-3) ⭐️ 8.0/10
4. [Anthropic Discloses Bug That Made Claude Forgetful](#item-4) ⭐️ 8.0/10
5. [Tailscale Cofounder Proposes a Simpler Cloud](#item-5) ⭐️ 8.0/10
6. [Palantir employees question their moral role](#item-6) ⭐️ 8.0/10
7. [GPT-5.5 accessed via Codex backdoor API](#item-7) ⭐️ 8.0/10
8. [Hairdryer Used to Manipulate Paris Weather Sensors for Polymarket Profit](#item-8) ⭐️ 8.0/10
9. [Google Cloud default flaw leads to $18,000 bill for user](#item-9) ⭐️ 8.0/10
10. [DeepSeek Open-Sources TileKernels GPU Operator Library for NVIDIA Blackwell](#item-10) ⭐️ 8.0/10
11. [Tencent Open-Sources Hy3 Preview MoE Model](#item-11) ⭐️ 8.0/10
12. [TSMC Delays High-NA EUV Adoption Until 2029 Due to Cost](#item-12) ⭐️ 8.0/10
13. [China's Three Major ISPs Hit by Widespread International Network Outage](#item-13) ⭐️ 8.0/10
14. [Apple CEO Tim Cook to Step Down, John Ternus to Take Over in 2026](#item-14) ⭐️ 8.0/10
15. [EU Pressures Google to Open Android to Rival AI Assistants](#item-15) ⭐️ 8.0/10
16. [MIT Builds Math Bridge Between Classical and Quantum Physics](#item-16) ⭐️ 8.0/10
17. [Intel Q2 Outlook Beats Estimates, Stock Surges 20%](#item-17) ⭐️ 8.0/10
18. [LiteParse PDF Text Extraction Runs in Browser](#item-18) ⭐️ 7.0/10
19. [ByteDance Releases Seed3D 2.0 for Production-Ready 3D Generation](#item-19) ⭐️ 7.0/10
20. [SFC and PwC Reach HK$1 Billion Settlement for Evergrande Fraud](#item-20) ⭐️ 7.0/10
21. [UK NCSC Officially Endorses Passkeys as Top Authentication Method](#item-21) ⭐️ 7.0/10
22. [UK Biobank Tightens Access After Data Illegally Listed for Sale](#item-22) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [OpenAI Launches GPT-5.5, a New Frontier Coding Model](https://openai.com/index/introducing-gpt-5-5/) ⭐️ 9.0/10

OpenAI has announced GPT-5.5, a new frontier coding model, with a gradual rollout starting with Pro and Enterprise accounts before reaching Plus users. The model is available through ChatGPT and Codex, but API access is not yet provided. GPT-5.5 represents a major advancement in AI-assisted coding, scoring 82% on CyberGym benchmarks, which positions it as a highly capable tool for both offensive and defensive cybersecurity tasks. Its release has sparked significant community discussion about developer dependency on such models, highlighting the growing reliance on AI for coding. The rollout is gradual over many hours to ensure service stability, and the model is not yet accessible via API, though some users have reported using a backdoor through the Codex API. One engineer at NVIDIA described losing access to GPT-5.5 as feeling like having a limb amputated, underscoring the model's perceived indispensability.

hackernews · rd · Apr 23, 18:01

**Background**: GPT-5.5 is a frontier AI model specialized for coding tasks, building on OpenAI's previous GPT series. Frontier models are the most advanced AI systems available, often used for complex problem-solving in fields like software development and cybersecurity. The gradual rollout strategy is common for major releases to manage server load and ensure reliability.

**Discussion**: Community comments reveal a mix of excitement and concern: some users praise GPT-5.5's performance and openness compared to competitors like Anthropic's Mythos, while others express unease about developers becoming overly dependent on such tools. There is also discussion about the lack of official API access and the use of unofficial backdoors.

**Tags**: `#AI`, `#OpenAI`, `#GPT-5.5`, `#machine learning`, `#coding tools`

---

<a id="item-2"></a>
## [Bitwarden CLI compromised in supply chain attack](https://socket.dev/blog/bitwarden-cli-compromised) ⭐️ 9.0/10

Bitwarden CLI version 2026.4.0 was compromised as part of an ongoing Checkmarx supply chain campaign, with a malicious npm package published that steals crypto wallet data and developer credentials. This incident highlights critical risks in the npm ecosystem, as a widely-used password manager CLI tool was hijacked to exfiltrate sensitive data, potentially affecting thousands of developers and organizations. The attack exploited a compromised GitHub Action in the Bitwarden build pipeline, and the malicious package @bitwarden/cli@2026.4.0 was published on npm with a self-propagating worm that exfiltrates credentials to public GitHub repositories.

hackernews · tosh · Apr 23, 14:17

**Background**: Supply chain attacks target the software development pipeline by compromising trusted tools or dependencies. In this case, attackers poisoned the Bitwarden CLI npm package, which is used by developers to manage passwords programmatically, and the malicious code was distributed to users who updated or installed the affected version.

<details><summary>References</summary>
<ul>
<li><a href="https://thehackernews.com/2026/04/bitwarden-cli-compromised-in-ongoing.html">Bitwarden CLI Compromised in Ongoing Checkmarx Supply Chain ...</a></li>
<li><a href="https://tech.yahoo.com/cybersecurity/articles/bitwarden-cli-supply-chain-attack-142710104.html">Bitwarden CLI Supply Chain Attack Puts Crypto Wallet Keys at Risk</a></li>
<li><a href="https://www.ox.security/blog/shai-hulud-bitwarden-cli-supply-chain-attack/">Bitwarden CLI Compromised: Inside the Shai-Hulud Supply Chain Attack</a></li>

</ul>
</details>

**Discussion**: Community members discussed mitigation strategies such as setting min-release-age in npm (e.g., 7 days) and pinning dependencies, with some noting that a Rust alternative (rbw) reduces the dependency tree size. Others shared concerns about the CLI exposing sensitive data in terminal multiplexers like tmux.

**Tags**: `#supply chain security`, `#npm`, `#Bitwarden`, `#supply chain attack`, `#dependency management`

---

<a id="item-3"></a>
## [vLLM v0.20.0: CUDA 13, PyTorch 2.11, FA4, TurboQuant](https://github.com/vllm-project/vllm/releases/tag/v0.20.0) ⭐️ 8.0/10

vLLM v0.20.0, released with 546 commits from 257 contributors, upgrades the default CUDA wheel to CUDA 13.0, ships on PyTorch 2.11, and adds compatibility with HuggingFace Transformers v5. It also enables FlashAttention 4 as the default MLA prefill backend and introduces a TurboQuant 2-bit KV cache compression backend for 4× capacity. This release significantly boosts inference performance and memory efficiency for large language models, especially on modern Hopper and Blackwell GPUs. The TurboQuant 2-bit KV cache compression can reduce memory usage by 4×, enabling larger context windows or lower hardware requirements for production deployments. FlashAttention 4 is re-enabled as the default MLA prefill backend with head-dim 512 and paged-KV support on SM90+ GPUs. TurboQuant is a new attention backend that compresses KV cache to 2 bits, and the release also includes an online quantization frontend and the initial skeleton of the vLLM IR for future kernel development.

github · khluu · Apr 23, 21:02

**Background**: vLLM is a high-throughput, memory-efficient open-source inference engine for large language models, widely used in production. Multi-head Latent Attention (MLA), used by models like DeepSeek V3, reduces KV cache memory by 4–8× compared to standard MHA. FlashAttention is a series of fast and memory-efficient attention algorithms, and TurboQuant is a compression method from Google that achieves extreme reduction in model size with minimal accuracy loss.

<details><summary>References</summary>
<ul>
<li><a href="https://langcopilot.com/posts/2025-09-13-multi-head-latent-attention-mla-explained">MLA Attention : 4 -8x Less Memory Than MHA (DeepSeek...)</a></li>
<li><a href="https://research.google/blog/turboquant-redefining-ai-efficiency-with-extreme-compression/">TurboQuant: Redefining AI efficiency with extreme compression</a></li>

</ul>
</details>

**Tags**: `#vLLM`, `#LLM inference`, `#CUDA`, `#FlashAttention`, `#KV cache`

---

<a id="item-4"></a>
## [Anthropic Discloses Bug That Made Claude Forgetful](https://www.anthropic.com/engineering/april-23-postmortem) ⭐️ 8.0/10

Anthropic disclosed a bug in Claude Code that caused Claude to appear forgetful and repetitive by clearing thinking context every turn instead of only once after idle sessions, affecting Sonnet 4.6 and Opus 4.6 users from March 26 to April 10. This bug directly degraded user experience for two weeks, highlighting the fragility of AI systems and the importance of transparency in AI operations. The incident also fuels community debate about reliability and competition with OpenAI. The bug was introduced on March 26 when Anthropic shipped a change to clear older thinking from sessions idle for over an hour to reduce latency, but a coding error caused the clearing to happen every turn instead of once. The fix was deployed on April 10, and the issue affected both Sonnet 4.6 and Opus 4.6 models.

hackernews · mfiguiere · Apr 23, 17:48

**Background**: Claude Code is Anthropic's AI coding assistant that uses extended thinking to maintain context across long sessions. The bug occurred at the intersection of Claude Code's context management, the Anthropic API, and extended thinking, and it passed multiple human and automated reviews before deployment.

<details><summary>References</summary>
<ul>
<li><a href="https://www.anthropic.com/engineering/april-23-postmortem">An update on recent Claude Code quality reports \ Anthropic</a></li>
<li><a href="https://github.com/anthropics/claude-code/issues/8677">[BUG] /context fails on first try with thinking anabled ...</a></li>
<li><a href="https://dev.to/letanure/claude-code-part-10-common-issues-and-quick-fixes-186g">Claude Code: Part 10 - Common Issues and Quick Fixes</a></li>

</ul>
</details>

**Discussion**: Community reactions were mixed: some users appreciated Anthropic's transparent postmortem, while others expressed frustration over the two-week delay in fixing the bug. Several commenters also noted that this incident highlights the need for better transparency and testing in AI systems, and some compared Claude's performance unfavorably to OpenAI's offerings.

**Tags**: `#AI`, `#Claude`, `#bug`, `#transparency`, `#Anthropic`

---

<a id="item-5"></a>
## [Tailscale Cofounder Proposes a Simpler Cloud](https://crawshaw.io/blog/building-a-cloud) ⭐️ 8.0/10

David Crawshaw, a cofounder of Tailscale, published a blog post outlining his vision for a new cloud platform that prioritizes simplicity and performance over the complexity of existing clouds and Kubernetes. This critique from a respected infrastructure leader challenges the status quo of cloud complexity, potentially influencing how developers and companies think about deploying applications. The strong community response (983 points, 486 comments) shows widespread frustration with current tools like Kubernetes. Crawshaw argues that making Kubernetes good is inherently impossible, calling it 'lipstick on a pig,' and criticizes traditional clouds for defaults like 3000 IOPS per VM when a laptop offers 500k. His proposed platform, exe.dev, uses an HTTP proxy for inbound connections and lacks public IPv4, which some commenters find obscure.

hackernews · bumbledraven · Apr 23, 04:44

**Background**: Kubernetes is a popular container orchestration system known for its powerful features but also its steep learning curve and operational complexity. Tailscale is a company that provides a simple, zero-config VPN service, and its cofounder's perspective carries weight in the infrastructure community. The blog post reflects a growing sentiment that many cloud tools have become too complex for their own good.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Tailscale">Tailscale - Wikipedia</a></li>
<li><a href="https://encore.cloud/resources/kubernetes-complexity">Why Kubernetes Is So Complicated (And What to Use Instead)</a></li>
<li><a href="https://dev.to/rocktimmanta/why-does-kubernetes-feel-so-complicated-1l14">Why Does Kubernetes Feel So Complicated? - DEV Community</a></li>

</ul>
</details>

**Discussion**: Commenters largely agree with the critique of Kubernetes complexity, with one calling it 'so well put' and another noting that incidents are often caused by Kubernetes itself. However, some express skepticism about Crawshaw's own platform, exe.dev, pointing out its own obscure abstractions and limitations like no public IPv4.

**Tags**: `#cloud computing`, `#kubernetes`, `#PaaS`, `#infrastructure`, `#tailscale`

---

<a id="item-6"></a>
## [Palantir employees question their moral role](https://www.wired.com/story/palantir-employees-are-starting-to-wonder-if-theyre-the-bad-guys/) ⭐️ 8.0/10

A Wired article reports that Palantir employees are increasingly grappling with moral questions about their work for a U.S. defense contractor, amid political controversy and internal dissent. This debate highlights the growing ethical tensions within the tech industry over defense contracting and surveillance, potentially influencing employee retention, recruitment, and public perception of companies like Palantir. The article includes internal messages where employees expressed frustration that public posts about ethics hurt sales outside the U.S., while others argued that the issue affects everyone personally.

hackernews · pavel_lishin · Apr 23, 17:30

**Background**: Palantir is a U.S. software company known for its data analytics platforms used by government agencies, including defense and intelligence. Its work often involves surveillance and counterterrorism, raising ethical concerns about privacy and human rights.

**Discussion**: Commenters noted that Palantir employees should recognize they work for a defense contractor, and some referenced a former employee's interview about the company's evolution. One commenter recommended reading "Careless People" to understand how tech workers rationalize their roles.

**Tags**: `#ethics`, `#defense-contracting`, `#palantir`, `#tech-culture`, `#surveillance`

---

<a id="item-7"></a>
## [GPT-5.5 accessed via Codex backdoor API](https://simonwillison.net/2026/Apr/23/gpt-5-5/#atom-everything) ⭐️ 8.0/10

OpenAI released GPT-5.5, available in Codex and rolling out to paid ChatGPT subscribers, but not yet via the standard API. Simon Willison created a plugin called llm-openai-via-codex that uses the semi-official Codex backend API to run prompts against GPT-5.5 using an existing ChatGPT subscription. This workaround allows developers to benchmark and use GPT-5.5 via API without waiting for official API access, highlighting ongoing tensions between AI providers and third-party tools. It also demonstrates how subscription-based model access can be repurposed for programmatic use, potentially influencing future API policies. The plugin reverse-engineers authentication from OpenAI's open-source Codex CLI repository to access the /backend-api/codex/responses endpoint. Willison used this setup to run his "pelican on a bicycle" benchmark, which tests a model's ability to generate an SVG of a pelican riding a bicycle.

rss · Simon Willison · Apr 23, 19:59

**Background**: GPT-5.5 is OpenAI's latest language model, released on April 23, 2026, and is available in Codex, an AI coding agent, and to paid ChatGPT subscribers. The "pelican on a bicycle" benchmark is a popular informal test where an LLM is asked to generate an SVG of a pelican riding a bicycle, assessing its code generation and spatial reasoning abilities. The Codex API endpoint used here is semi-official, as OpenAI has publicly supported its use by third-party tools like OpenClaw and Pi, but it is not the standard API.

<details><summary>References</summary>
<ul>
<li><a href="https://simonwillison.net/2026/Apr/23/gpt-5-5/">A pelican for GPT-5.5 via the semi-official Codex backdoor API</a></li>
<li><a href="https://grokipedia.com/page/Pelican_on_a_bicycle_AI_benchmark">Pelican on a bicycle (AI benchmark)</a></li>
<li><a href="https://github.com/openai/codex/blob/main/codex-rs/responses-api-proxy/README.md">codex/codex-rs/responses-api-proxy/README.md at main - GitHub</a></li>

</ul>
</details>

**Tags**: `#GPT-5.5`, `#OpenAI`, `#API`, `#AI models`, `#benchmarking`

---

<a id="item-8"></a>
## [Hairdryer Used to Manipulate Paris Weather Sensors for Polymarket Profit](https://fibo-crypto.fr/en/blog/polymarket-weather-sensor-manipulation-paris-meteo-france-2026/) ⭐️ 8.0/10

A person used a hairdryer to artificially heat temperature sensors at Paris Charles de Gaulle Airport on April 6 and 15, 2026, causing Polymarket prediction market settlements to pay out over $34,000 based on false readings. This incident highlights a critical vulnerability in decentralized prediction markets that rely on real-world data oracles, as physical sensor manipulation can be exploited for financial gain, raising urgent questions about oracle security and market integrity. On April 6, the sensor reading jumped from near 18°C to over 21°C within minutes, and on April 15, the probability of the 22°C range surged from 0.1% to 95% in 30 minutes. Polymarket has since switched its data source to Paris Le Bourget Airport but did not reverse the settled outcomes.

telegram · zaihuapd · Apr 23, 04:36

**Background**: Polymarket is a decentralized prediction market platform where users bet on real-world outcomes, with market resolution often relying on data oracles like weather sensors. The UMA Optimistic Oracle is typically used to settle disputes, but in this case, the sensor data itself was tampered with physically. Météo-France, the French national meteorological service, filed a criminal complaint with the air transport gendarmerie after finding evidence of tampering during an on-site inspection.

<details><summary>References</summary>
<ul>
<li><a href="https://www.aol.com/articles/police-investigate-claims-hair-dryer-150607773.html">Police investigate after claims ‘ hair dryer used to manipulate weather ...</a></li>
<li><a href="https://finance.yahoo.com/markets/crypto/articles/trader-manipulates-city-weather-sensor-165804921.html">Trader manipulates city weather sensor to win $34K</a></li>
<li><a href="https://help.polymarket.com/en/articles/13364518-how-are-prediction-markets-resolved">How Are Prediction Markets Resolved? - Polymarket Help Center</a></li>

</ul>
</details>

**Discussion**: Community discussions on Telegram and crypto forums expressed shock at the simplicity of the attack, with some calling for more robust oracle designs, such as using multiple independent data sources. Others debated whether Polymarket should have voided the manipulated trades, while Vitalik Buterin reportedly offered thoughts on how prediction markets could better handle such oracle manipulation risks.

**Tags**: `#prediction markets`, `#oracle manipulation`, `#weather sensors`, `#Polymarket`, `#security`

---

<a id="item-9"></a>
## [Google Cloud default flaw leads to $18,000 bill for user](https://www.tomshardware.com/tech-industry/artificial-intelligence/google-cloud-customer-wakes-up-to-usd18-000-bill-despite-usd7-budget-thanks-to-forgotten-public-api-key-attacker-put-in-60-000-requests-and-blasted-through-usd1-400-spending-cap) ⭐️ 8.0/10

A Google Cloud user, Australian AI consultant Jesse Davies, received an $18,000 bill despite setting a $7 budget, after an attacker exploited a leaked API key stored in plaintext in a container environment variable and made 60,000 requests, bypassing spending caps. This incident highlights a systemic security risk in Google Cloud's default configurations, where budget caps can be silently overridden and credit limits automatically raised, potentially exposing many users to massive unexpected charges. The attacker accessed the API key via a public URL, and Google Cloud automatically raised the credit limit without notifying the user when the threshold was triggered, exacerbating the loss. Truffle Security noted that the Gemini API key format is uniform and security settings are disabled by default, making such attacks common.

telegram · zaihuapd · Apr 23, 05:21

**Background**: Google Cloud's budget alerts and caps are not hard limits; they are notifications that can be ignored or overridden. API keys, especially those stored in plaintext in environment variables, can be easily leaked if not properly secured. The Gemini API key format is standardized, making it easier for attackers to identify and exploit exposed keys.

<details><summary>References</summary>
<ul>
<li><a href="https://docs.cloud.google.com/billing/docs/how-to/budgets">Create, edit, or delete budgets and budget alerts | Cloud Billing | Google Cloud Documentation</a></li>
<li><a href="https://trufflesecurity.com/">Truffle Security Co.</a></li>
<li><a href="https://ai.google.dev/gemini-api/docs/api-key">Using Gemini API keys | Google AI for Developers</a></li>

</ul>
</details>

**Tags**: `#Google Cloud`, `#security`, `#API key`, `#cloud billing`, `#misconfiguration`

---

<a id="item-10"></a>
## [DeepSeek Open-Sources TileKernels GPU Operator Library for NVIDIA Blackwell](https://github.com/deepseek-ai/TileKernels) ⭐️ 8.0/10

DeepSeek has open-sourced TileKernels, a high-performance GPU operator library based on TileLang, optimized for large language model (LLM) training and inference. The library supports NVIDIA's latest SM100 (Blackwell) architecture and requires CUDA 13.1 or later. This release provides the AI community with a highly optimized, near-hardware-limit GPU operator library that can significantly accelerate LLM workloads on the latest NVIDIA Blackwell GPUs. It lowers the barrier for developers to achieve top-tier performance in training and inference, especially for advanced techniques like MoE routing and FP8/FP4 quantization. TileKernels covers MoE routing, FP8/FP4 quantization, and various fused operators, and has already been deployed in DeepSeek's internal environment. The library is designed to approach the theoretical limits of compute intensity and memory bandwidth on supported hardware.

telegram · zaihuapd · Apr 23, 09:36

**Background**: TileLang is a domain-specific language that simplifies the development of high-performance GPU and CPU kernels. NVIDIA's Blackwell architecture (SM100) is the successor to Hopper, featuring 208 billion transistors and built on a custom TSMC 4NP process, designed to power AI factories with unprecedented performance and efficiency. MoE (Mixture-of-Experts) routing and FP8/FP4 quantization are key techniques used in modern LLMs to improve model capacity and reduce memory footprint.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/tile-ai/tilelang">GitHub - tile-ai/tilelang: Domain-specific language designed to streamline the development of high-performance GPU/CPU/Accelerators kernels</a></li>
<li><a href="https://en.wikipedia.org/wiki/Blackwell_(microarchitecture)">Blackwell (microarchitecture) - Wikipedia</a></li>
<li><a href="https://resources.nvidia.com/en-us-blackwell-architecture">NVIDIA Blackwell Architecture Technical Overview</a></li>

</ul>
</details>

**Tags**: `#DeepSeek`, `#GPU算子库`, `#LLM`, `#NVIDIA Blackwell`, `#开源`

---

<a id="item-11"></a>
## [Tencent Open-Sources Hy3 Preview MoE Model](https://mp.weixin.qq.com/s/5_nUI2mDchlwoedinFUMeA) ⭐️ 8.0/10

Tencent has officially released and open-sourced the Hy3 preview language model, a Mixture-of-Experts (MoE) model with 295 billion total parameters and 21 billion activated parameters, supporting a 256K context length. The model is now available on GitHub, HuggingFace, and Tencent Cloud, and has been integrated into internal products like Yuanbao, Tencent Docs, and QQ. This release is significant because it provides the open-source community with a competitive large-scale MoE model from a major Chinese tech company, enhancing capabilities in complex reasoning and agent tasks. The deep optimization of inference performance, including a 54% reduction in first-token latency for products like CodeBuddy, makes it highly practical for real-world applications. The Hy3 preview model is the first MoE model after Tencent's architecture rebuild, with 295B total parameters but only 21B activated per inference, enabling efficient computation. Tencent Cloud also offers an API and customized Token Plan, with a personal edition priced at 28 RMB per month.

telegram · zaihuapd · Apr 23, 10:07

**Background**: Mixture-of-Experts (MoE) is a machine learning technique that uses multiple specialized sub-networks (experts) to handle different parts of the input, with a gating mechanism selecting which experts to activate. This allows models to have a very large total parameter count while keeping the computational cost per inference low, as only a subset of parameters is used. The difference between total parameters (295B) and activated parameters (21B) is a key feature of MoE models, enabling them to scale up without proportionally increasing inference cost.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Mixture_of_experts">Mixture of experts - Wikipedia</a></li>
<li><a href="https://huggingface.co/blog/moe">Mixture of Experts Explained - Hugging Face</a></li>
<li><a href="https://pandaily.com/beyond-the-model-race-how-tencent-is-building-its-global-ai-moat">Beyond the Model Race: How Tencent Is Building Its Global AI ...</a></li>

</ul>
</details>

**Tags**: `#AI/ML`, `#Large Language Model`, `#Open Source`, `#MoE`, `#Tencent`

---

<a id="item-12"></a>
## [TSMC Delays High-NA EUV Adoption Until 2029 Due to Cost](https://money.udn.com/money/story/5599/9458925?from=edn_newestlist_rank) ⭐️ 8.0/10

TSMC announced at its North America Technology Forum that it will not adopt ASML's high-NA EUV lithography machines for mass production until at least 2029, citing the high cost of over €350 million per unit. The company also revealed plans to establish CoWoS and 3D-IC packaging capacity in Arizona by 2029. This strategic decision signals that TSMC believes existing EUV tools can still deliver sufficient performance for its upcoming A13 process, potentially slowing the industry's transition to next-generation lithography. It also highlights the growing importance of advanced packaging as a cost-effective alternative to pushing lithography limits, with TSMC's US expansion addressing supply chain bottlenecks. ASML's high-NA EUV Twinscan EXE machines cost approximately €350 million each, making them prohibitively expensive for mass deployment. TSMC's first Arizona fab has already achieved yield rates close to those of its Taiwan fabs, and the second fab is scheduled to begin mass production next year.

telegram · zaihuapd · Apr 23, 11:22

**Background**: High-NA (high numerical aperture) EUV lithography is ASML's next-generation extreme ultraviolet technology, designed to produce finer chip features by using a larger numerical aperture lens. CoWoS (Chip-on-Wafer-on-Substrate) and 3D-IC are advanced packaging technologies that stack multiple chips vertically or integrate them on an interposer, improving performance and reducing power consumption without requiring the most advanced lithography.

<details><summary>References</summary>
<ul>
<li><a href="https://www.ithome.com/0/752/684.htm">ASML 高数值孔径 High NA EUV 光刻机实现“初次曝光”，助英特尔开启工艺进化 - IT之家</a></li>
<li><a href="https://www.slkormicro.com/indining-china/581256.html">ASML High-NA EUV光刻机</a></li>
<li><a href="https://en.wikipedia.org/wiki/3D_IC">3D IC</a></li>

</ul>
</details>

**Tags**: `#semiconductor`, `#TSMC`, `#ASML`, `#EUV lithography`, `#manufacturing`

---

<a id="item-13"></a>
## [China's Three Major ISPs Hit by Widespread International Network Outage](https://t.me/zaihuapd/41029) ⭐️ 8.0/10

China's three major telecom operators—China Telecom, China Unicom, and China Mobile—are experiencing widespread international network disruptions, with significant packet loss and connection interruptions affecting routes to Hong Kong, Japan, and the US. This outage impacts both consumer and business international connectivity across China's largest ISPs, potentially disrupting cross-border communications, cloud services, and global internet traffic for millions of users. Affected routes include premium lines like China Telecom's CN2 and China Unicom's 9929, as well as standard routes like 163 and 4837; China Mobile's mobile data traffic to overseas destinations also shows severe packet loss, particularly for users in Beijing.

telegram · zaihuapd · Apr 23, 12:45

**Background**: China's three major telecom operators manage distinct backbone networks for international traffic: China Telecom uses the 163 backbone and the premium CN2 (Global Internet Access) network, China Unicom operates the AS4837 backbone and the higher-performance AS9929 (CUVIP) network, and China Mobile uses the CMI backbone. These networks handle all cross-border internet traffic for consumers and businesses in China. The current disruption affects both standard and premium routes, suggesting a widespread infrastructure issue rather than a localized fault.

<details><summary>References</summary>
<ul>
<li><a href="https://www.keepnight.com/archives/1781/">cn2 gia 、cn2 gt 、163、AS9929、AS4837线路区别 - keepnight</a></li>
<li><a href="https://www.nodeseek.com/post-137012-3">有无懂哥科普线路4837、CMI、cn2、GIA、GT、cmin2、9929、cmi知识</a></li>
<li><a href="https://www.hncloud.com/news/3311.html">一文带您了解什么是AS9929线路、AS4837线路、CUVIP、CIA线路-华纳云</a></li>

</ul>
</details>

**Tags**: `#network outage`, `#China telecom`, `#internet infrastructure`, `#routing issues`, `#ISP`

---

<a id="item-14"></a>
## [Apple CEO Tim Cook to Step Down, John Ternus to Take Over in 2026](https://t.me/zaihuapd/41030) ⭐️ 8.0/10

Apple announced on April 20, 2026, that Tim Cook will step down as CEO and become executive chairman of the board, while hardware engineering senior vice president John Ternus will become CEO effective September 1, 2026. This marks the first CEO transition at Apple since Tim Cook took over from Steve Jobs in 2011, signaling a new era for the world's most valuable company and its product strategy, especially as Apple pushes deeper into AI and hardware innovation. John Ternus, who joined Apple in 2001 and became senior vice president of hardware engineering in 2021, will join the board on September 1, 2026, while current chairman Arthur Levinson will become lead independent director; Cook will remain CEO through the summer to ensure a smooth transition.

telegram · zaihuapd · Apr 23, 13:46

**Background**: Tim Cook became Apple's CEO in August 2011 after Steve Jobs resigned due to health issues, and under his leadership Apple's revenue and market capitalization grew dramatically. The role of executive chairman is a new position created for Cook, allowing him to remain involved in strategic oversight while Ternus handles day-to-day operations.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/John_Ternus">John Ternus - Wikipedia</a></li>
<li><a href="https://www.apple.com/leadership/john-ternus/">Apple Leadership - John Ternus - Apple</a></li>
<li><a href="https://www.cnbc.com/2026/04/20/apple-names-john-ternus-ceo-replacing-tim-cook-who-becomes-chairman.html">Apple taps John Ternus as CEO to replace Tim Cook, who will become chairman</a></li>

</ul>
</details>

**Tags**: `#Apple`, `#leadership change`, `#CEO transition`, `#tech industry`, `#corporate news`

---

<a id="item-15"></a>
## [EU Pressures Google to Open Android to Rival AI Assistants](https://www.bloomberg.com/news/articles/2026-04-23/google-faces-eu-pressure-to-open-up-android-to-gemini-rivals) ⭐️ 8.0/10

The European Union is pressuring Google to grant rival AI assistants like ChatGPT and Claude the same system-level access on Android as Google's own Gemini assistant. The requirements are still in draft form and may be delayed. This move could fundamentally reshape competition in the mobile AI assistant market by forcing Google to open up Android's deepest system integrations. If enacted, it would give users more choice but also raise significant security and privacy concerns for the platform. The EU's demands focus on granting rival assistants access to sensitive system features and data streams that Gemini currently enjoys exclusively. Google has expressed concerns that such openness could compromise user security and privacy on Android devices.

telegram · zaihuapd · Apr 23, 15:31

**Background**: Android is the world's most widely used mobile operating system, and Google's Gemini AI assistant has deep system-level integration that third-party assistants lack. The EU's Digital Markets Act (DMA) has previously forced Google to offer users choices for browsers and search engines, and this new push extends that logic to AI assistants. System-level access includes capabilities like reading screen content, controlling apps, and accessing sensitive data streams, which are critical for AI assistants to function effectively.

<details><summary>References</summary>
<ul>
<li><a href="https://truthonthemarket.com/2026/04/14/opening-pandoras-interface-ai-assistants-and-the-dma/">Opening Pandora’s Interface: AI Assistants and... - Truth on the Market</a></li>
<li><a href="https://developer.android.com/ai/gemini-nano">Gemini Nano | AI | Android Developers</a></li>
<li><a href="https://support.google.com/gemini/answer/16938321?hl=en">Manage or delete the Gemini app on your Android device</a></li>

</ul>
</details>

**Tags**: `#EU regulation`, `#Android`, `#AI assistants`, `#Google`, `#antitrust`

---

<a id="item-16"></a>
## [MIT Builds Math Bridge Between Classical and Quantum Physics](https://www.newsy-today.com/new-study-bridges-the-worlds-of-classical-and-quantum-physics-mit-news/) ⭐️ 8.0/10

MIT researchers introduced density calculations into the classical Hamilton-Jacobi equation, producing results identical to the Schrödinger equation for quantum phenomena. This breakthrough offers a simpler mathematical framework for quantum behavior, potentially improving quantum bit predictions and aiding the unification of quantum mechanics with general relativity. The method successfully explains the double-slit experiment and quantum tunneling, and the team believes it could enhance predictions of qubit behavior.

telegram · zaihuapd · Apr 23, 16:30

**Background**: The Hamilton-Jacobi equation is a classical mechanics formulation equivalent to Newton's laws, while the Schrödinger equation is the central equation of quantum mechanics. This work shows that by adding a density term to the classical equation, one can exactly reproduce quantum mechanical results.

<details><summary>References</summary>
<ul>
<li><a href="https://news.mit.edu/2026/new-study-bridges-classical-and-quantum-physics-0421">New study bridges the worlds of classical and quantum physics</a></li>
<li><a href="https://en.wikipedia.org/wiki/Hamilton–Jacobi_equation">Hamilton – Jacobi equation - Wikipedia</a></li>
<li><a href="https://quantumzeitgeist.com/quantum-motion-classical-calculate-using/">Researchers Calculate Quantum Motion Using Classical “Least ...</a></li>

</ul>
</details>

**Tags**: `#quantum physics`, `#mathematical physics`, `#MIT research`, `#quantum computing`, `#theoretical physics`

---

<a id="item-17"></a>
## [Intel Q2 Outlook Beats Estimates, Stock Surges 20%](https://www.bloomberg.com/news/articles/2026-04-23/intel-gives-strong-outlook-in-sign-of-payoff-from-ai-spending) ⭐️ 8.0/10

Intel reported Q1 revenue of $13.6 billion and adjusted EPS of $0.29, far exceeding the expected $0.01, and guided Q2 revenue between $13.8 billion and $14.8 billion, beating market expectations. The strong outlook, driven by AI inference demand and CPU recovery, sent Intel's stock up about 20% in after-hours trading. This earnings beat and strategic pivot to foundry services, with Tesla as a key customer for its 14A process, signal a potential turnaround for Intel and a major shift in the semiconductor landscape. If successful, Intel could challenge TSMC's dominance in advanced chip manufacturing by 2030. Intel's foundry business generated $5.4 billion in revenue in Q1, and the company has secured Tesla as the first customer for its 14A process node. Despite a net loss of $3.7 billion in Q1, CEO Chen Liwu is improving the balance sheet through restructuring and external partnerships.

telegram · zaihuapd · Apr 24, 00:20

**Background**: Intel, traditionally a leader in designing and manufacturing its own chips, is pivoting to become a foundry—a company that manufactures chips designed by others. This shift, known as the IDM 2.0 strategy, aims to compete with TSMC and Samsung in the advanced chip manufacturing market. The 14A process is Intel's upcoming advanced manufacturing node, expected to deliver significant performance and efficiency gains.

<details><summary>References</summary>
<ul>
<li><a href="https://www.eet-china.com/mp/a489739.html">马斯克：Terafab将采用英特尔14A制程-电子工程专辑</a></li>
<li><a href="https://news.mydrivers.com/1/1117/1117937.htm">马斯克：全球最大晶圆工厂定了！将采用Intel 14A工艺制造芯片</a></li>
<li><a href="https://www.trendforce.cn/industry-news/semiconductors/20260421-4545.html">英特尔代工业务势头回升 2026年设备订单量同比大增超50%-集邦咨询</a></li>

</ul>
</details>

**Tags**: `#Intel`, `#semiconductors`, `#AI`, `#foundry`, `#earnings`

---

<a id="item-18"></a>
## [LiteParse PDF Text Extraction Runs in Browser](https://simonwillison.net/2026/Apr/23/liteparse-for-the-web/#atom-everything) ⭐️ 7.0/10

Simon Willison has built a browser-based version of LiteParse, a Node.js CLI tool for PDF text extraction, allowing users to parse PDFs entirely in their browser without sending data to any server. This makes powerful PDF text extraction accessible to anyone with a web browser, enhancing privacy and ease of use for developers and users who need to extract text from PDFs without relying on cloud services or AI models. LiteParse uses spatial text parsing heuristics and optionally Tesseract OCR for image-based PDFs, and the browser version leverages PDF.js and Tesseract.js to run entirely client-side.

rss · Simon Willison · Apr 23, 21:54

**Background**: LiteParse is an open-source PDF parsing tool from LlamaIndex that extracts text while preserving document layout using heuristics rather than AI. It was originally a Node.js CLI tool, but Simon Willison adapted it for the browser by using the same underlying libraries (PDF.js and Tesseract.js) that work in both environments.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/run-llama/liteparse">GitHub - run-llama/liteparse: A fast, helpful, and open-source document parser</a></li>
<li><a href="https://simonwillison.net/2026/Apr/23/liteparse-for-the-web/">Extract PDF text in your browser with LiteParse for the web</a></li>
<li><a href="https://www.llamaindex.ai/blog/liteparse-local-document-parsing-for-ai-agents">LiteParse: Local Document Parsing for AI Agents - LlamaIndex</a></li>

</ul>
</details>

**Tags**: `#PDF parsing`, `#browser`, `#LiteParse`, `#spatial text parsing`, `#web development`

---

<a id="item-19"></a>
## [ByteDance Releases Seed3D 2.0 for Production-Ready 3D Generation](https://paipancon.com/fc2daily/detail/FC2-PPV-1700423) ⭐️ 7.0/10

ByteDance's Seed team officially launched Seed3D 2.0 on April 23, 2026, a next-generation 3D generation model that achieves state-of-the-art (SOTA) performance in both geometry and texture quality. In human evaluations for texture generation, Seed3D 2.0 achieved a preference rate of over 69% compared to mainstream models. This marks a significant step toward production-ready AI 3D content generation, addressing industry pain points such as edge softening and material realism. The model's compatibility with physics simulation engines like NVIDIA Isaac Sim and standard formats like URDF opens up new possibilities for robotics simulation, gaming, XR, and e-commerce workflows. Seed3D 2.0 extends its capabilities to component-level generation and scene composition, allowing users to decompose 3D content into parts and then complete shapes. The model outputs assets with full joint information in standard formats like URDF, making them directly usable in physics simulation environments.

telegram · zaihuapd · Apr 23, 08:15

**Background**: 3D generation models aim to create 3D assets from inputs like images or text, but earlier models often produced results with visible flaws such as blurry edges or unrealistic materials, limiting their use to demonstrations. URDF (Unified Robot Description Format) is an XML format used in robotics to describe robot kinematics, dynamics, and geometry, commonly used with ROS tools and simulators like Gazebo. NVIDIA Isaac Sim is a robotics simulation platform that enables physics-based simulation and robot learning.

<details><summary>References</summary>
<ul>
<li><a href="https://news.aibase.com/news/27393">ByteDance Launches Seed3D 2.0: Geometry and Texture Dual SOTA ...</a></li>
<li><a href="https://seed3d2.com/">Seed3D 2.0 - AI Image to 3D Model Generator</a></li>
<li><a href="https://en.wikipedia.org/wiki/URDF">URDF - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#3D generation`, `#ByteDance`, `#AI`, `#computer graphics`, `#physics simulation`

---

<a id="item-20"></a>
## [SFC and PwC Reach HK$1 Billion Settlement for Evergrande Fraud](https://apps.sfc.hk/edistributionWeb/gateway/TC/news-and-announcements/news/doc?refNo=26PR62) ⭐️ 7.0/10

Hong Kong's Securities and Futures Commission (SFC) announced a settlement with PwC Hong Kong, under which PwC will set aside HK$1 billion to compensate eligible minority shareholders of China Evergrande Group for financial fraud involving inflated revenues of 564.1 billion RMB over the 2019 and 2020 fiscal years. This is the first time in Hong Kong that an auditor of a collapsed company has agreed to compensate shareholders, setting a significant precedent for auditor accountability and investor protection in the region. The settlement underscores the growing regulatory scrutiny on audit quality and financial reporting integrity in Hong Kong's capital markets. The SFC investigation found that Evergrande inflated revenues by 564.1 billion RMB over two years, turning reported profits into substantial losses. PwC agreed to the settlement without admitting legal liability, and the SFC will take no further action against the firm.

telegram · zaihuapd · Apr 23, 12:07

**Background**: China Evergrande Group, once one of China's largest property developers, collapsed under massive debt in 2021. In 2024, Chinese regulators fined Evergrande 4.175 billion RMB for financial fraud, including inflating revenues by 564.1 billion RMB in 2019 and 2020. PwC served as Evergrande's auditor during those years and was accused of serious professional failures, including lack of independence and professional skepticism.

<details><summary>References</summary>
<ul>
<li><a href="https://news.qq.com/rain/a/20260423A063RP00?adChannelId=news_news_top">香港证监会：因恒大虚假财务报表问题，普华永道向股东赔偿10亿港元</a></li>
<li><a href="https://www.thepaper.cn/newsDetail_forward_33037031">香港证监会、会财局同日出手 普华永道同意预留10亿港元赔偿恒大股东_...</a></li>
<li><a href="https://www.nbd.com.cn/articles/2026-04-23/4354731.html">香港证监会与普华永道就恒大股东赔偿达成协议 赔偿达10亿港元</a></li>

</ul>
</details>

**Tags**: `#financial regulation`, `#auditing`, `#corporate fraud`, `#Hong Kong`, `#investor protection`

---

<a id="item-21"></a>
## [UK NCSC Officially Endorses Passkeys as Top Authentication Method](https://www.techradar.com/pro/security/uk-security-agency-officially-declares-passkeys-superior-to-passwords-passkeys-should-be-the-first-choice-for-authentication) ⭐️ 7.0/10

The UK National Cyber Security Centre (NCSC) has officially declared that passkeys are superior to traditional passwords and two-factor authentication, recommending them as the first-choice login method for digital services. This marks the end of NCSC's previous wait-and-see stance, as industry advancements over the past 12 months have resolved key implementation challenges. This official endorsement from a major government cybersecurity agency signals a significant shift in authentication guidance, potentially accelerating global adoption of passkeys across industries. It directly impacts how organizations and consumers approach online security, reducing reliance on passwords and improving protection against phishing and credential theft. Over 50% of active Google users in the UK have already registered for passkeys, and major platforms like eBay and PayPal have fully adapted to support them. Passkeys use asymmetric cryptography with a public-private key pair stored on the device, verified via biometrics (e.g., Face ID, Touch ID) or device PIN, eliminating the need for users to remember complex passwords.

telegram · zaihuapd · Apr 23, 14:47

**Background**: Passkeys are a passwordless authentication method based on public-key cryptography, where a private key stays on the user's device and a public key is stored on the server. Unlike passwords, passkeys are resistant to phishing, credential stuffing, and other common attacks because the private key never leaves the device and is unlocked only by biometric or PIN verification. The NCSC is the UK's leading authority on cybersecurity, providing guidance to protect citizens and organizations from cyber threats.

<details><summary>References</summary>
<ul>
<li><a href="https://developers.google.com/identity/passkeys?hl=zh-cn">通 行 密 钥 | Passkeys | Google for Developers</a></li>
<li><a href="https://www.corbado.com/zh/faq/passkeys-通行密钥">通 行 密 钥 （ Passkeys ）是什么？ 免 密 码登录与生物识别的安全指南</a></li>
<li><a href="https://blog.csdn.net/shaoshaoh/article/details/139117916">通 行 秘 钥 Passkeys 从入门到实现-CSDN博客</a></li>

</ul>
</details>

**Tags**: `#cybersecurity`, `#authentication`, `#passkeys`, `#NCSC`, `#identity`

---

<a id="item-22"></a>
## [UK Biobank Tightens Access After Data Illegally Listed for Sale](https://www.ukbiobank.ac.uk/news/a-message-to-our-participants-uk-biobank-data-security-update/) ⭐️ 7.0/10

Researchers from three academic institutions illegally listed de-identified UK Biobank participant data for sale on Alibaba's e-commerce platform, violating contractual agreements. In response, UK Biobank has suspended all research platform access, is implementing strict file export limits and daily monitoring, and is developing the world's first automated cloud-based data leakage prevention system, expected to launch by the end of 2026. This incident highlights critical vulnerabilities in research data governance and cross-border data transfer risks, especially for sensitive health and genetic data from 500,000 participants. The breach could undermine public trust in biomedical research and may set a precedent for stricter global data security standards in large-scale biobanks. The listings were removed before any transaction occurred, and the involved institutions and individuals have had their access permanently revoked. The new automated system will detect and prevent de-identified data from being removed from the cloud research platform, addressing re-identification risks that persist even with de-identified data.

telegram · zaihuapd · Apr 24, 00:58

**Background**: UK Biobank is a long-term prospective biobank study in the UK that houses de-identified biological samples and health-related data from half a million participants, making it one of the world's largest and most widely used genetic epidemiological datasets. De-identification removes direct identifiers but does not eliminate re-identification risk, especially when data is combined with other sources. Data loss prevention (DLP) software detects and prevents unauthorized transmission of sensitive data, and cloud-based DLP solutions are increasingly adopted as research platforms move to the cloud.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/UK_Biobank">UK Biobank - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Data_loss_prevention_software">Data loss prevention software - Wikipedia</a></li>
<li><a href="https://www.iri.com/support/data-education-center/what-is-re-identification-risk">What is Re-Identification Risk? | Data Education Center - IRI</a></li>

</ul>
</details>

**Tags**: `#data security`, `#biobank`, `#research ethics`, `#data governance`, `#health data`

---