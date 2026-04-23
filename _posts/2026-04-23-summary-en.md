---
layout: default
title: "Horizon Summary: 2026-04-23 (EN)"
date: 2026-04-23
lang: en
---

> From 26 items, 20 important content pieces were selected

---

1. [Qwen3.6-27B: A 27B Dense Model Outperforms 397B MoE in Coding](#item-1) ⭐️ 9.0/10
2. [Anthropic's Mythos AI model breached on release day](#item-2) ⭐️ 9.0/10
3. [Bitwarden CLI npm Package Hit by Checkmarx Supply Chain Attack](#item-3) ⭐️ 9.0/10
4. [Tailscale cofounder proposes simpler cloud from first principles](#item-4) ⭐️ 8.0/10
5. [Alberta Startup Sells No-Tech Tractors at Half Price](#item-5) ⭐️ 8.0/10
6. [Apple fixes bug that cops used to extract deleted chat messages from iPhones](#item-6) ⭐️ 8.0/10
7. [Citizen Lab Uncovers Two Telecom Surveillance Campaigns](#item-7) ⭐️ 8.0/10
8. [France confirms data breach at ANTS, 19 million citizens at risk](#item-8) ⭐️ 8.0/10
9. [Hairdryer Used to Manipulate Paris Weather Sensor for Polymarket Profit](#item-9) ⭐️ 8.0/10
10. [Google Cloud default security flaw leads to $18,000 bill](#item-10) ⭐️ 8.0/10
11. [ByteDance Releases Seed3D 2.0, Making 3D Generation Production-Ready](#item-11) ⭐️ 8.0/10
12. [DeepSeek Open-Sources TileKernels for NVIDIA Blackwell](#item-12) ⭐️ 8.0/10
13. [Tencent Open-Sources Hy3 Preview: 295B MoE Model](#item-13) ⭐️ 8.0/10
14. [SFC and PwC Reach HK$1 Billion Settlement for Evergrande Fraud](#item-14) ⭐️ 8.0/10
15. [China's Three Major Carriers Report International Network Outages](#item-15) ⭐️ 8.0/10
16. [Apple CEO Tim Cook to Step Down, John Ternus to Succeed in 2026](#item-16) ⭐️ 8.0/10
17. [UK NCSC Officially Endorses Passkeys as Preferred Authentication Method](#item-17) ⭐️ 8.0/10
18. [EU Pressures Google to Open Android to AI Rivals](#item-18) ⭐️ 8.0/10
19. [OpenAI's Chronicle for macOS Sparks Privacy and Security Concerns](#item-19) ⭐️ 7.0/10
20. [TSMC Delays ASML High-NA EUV Adoption Until 2029 Due to Cost](#item-20) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [Qwen3.6-27B: A 27B Dense Model Outperforms 397B MoE in Coding](https://simonwillison.net/2026/Apr/22/qwen36-27b/#atom-everything) ⭐️ 9.0/10

Alibaba's Qwen team released Qwen3.6-27B, a 27-billion-parameter dense open-weight model that surpasses the previous flagship Qwen3.5-397B-A17B (a 397B total / 17B active MoE model) on all major coding benchmarks. The model is only 55.6GB in size, compared to 807GB for its predecessor, and a quantized 16.8GB version can run locally on consumer hardware. This represents a massive efficiency leap, demonstrating that a well-trained dense model can match or exceed the coding performance of a much larger Mixture-of-Experts model, dramatically lowering the hardware requirements for state-of-the-art agentic coding. It enables developers to run a flagship-level coding assistant locally on a single GPU or even a high-end laptop, democratizing access to advanced AI coding tools. On internal benchmarks like QwenWebBench, Qwen3.6-27B scored 1487, a significant jump from 1068 for the previous model. The model is available on Hugging Face, and a GGUF quantized version (Q4_K_M) at 16.8GB can be run locally using llama.cpp, achieving around 25 tokens per second on a typical consumer machine.

rss · Simon Willison · Apr 22, 16:45

**Background**: Dense models use all their parameters for every inference, while Mixture-of-Experts (MoE) models activate only a subset of parameters per token, allowing larger total parameter counts with similar computational cost. GGUF quantization reduces model size and memory requirements by compressing weights with minimal quality loss, enabling large models to run on consumer hardware.

<details><summary>References</summary>
<ul>
<li><a href="https://www.marktechpost.com/2026/04/22/alibaba-qwen-team-releases-qwen3-6-27b-a-dense-open-weight-model-outperforming-397b-moe-on-agentic-coding-benchmarks/">Alibaba Qwen Team Releases Qwen3.6-27B: A Dense Open-Weight Model Outperforming 397B MoE on Agentic Coding Benchmarks - MarkTechPost</a></li>
<li><a href="https://simonwillison.net/2026/Apr/22/qwen36-27b/">Qwen3.6-27B: Flagship-Level Coding in a 27B Dense Model</a></li>
<li><a href="https://www.buildfastwithai.com/blogs/qwen3-6-27b-review-2026">Qwen3.6-27B: 27B Model Beats 397B on Coding (2026)</a></li>

</ul>
</details>

**Discussion**: The Hacker News discussion (referenced in the post) shows high engagement, with users sharing hands-on testing results and recipes for running the model locally. The overall sentiment is positive, with many impressed by the model's coding performance at such a small size, though some note that math reasoning may lag behind other models like Gemma 4.

**Tags**: `#AI/ML`, `#open-source`, `#coding`, `#model efficiency`, `#Qwen`

---

<a id="item-2"></a>
## [Anthropic's Mythos AI model breached on release day](https://www.bloomberg.com/news/articles/2026-04-21/anthropic-s-mythos-model-is-being-accessed-by-unauthorized-users) ⭐️ 9.0/10

Anthropic's highly restricted cybersecurity AI model Mythos, designed for zero-day vulnerability discovery, was accessed by a small Discord group on its release day and used undetected for nearly two weeks before Bloomberg reported the breach. This incident highlights the severe security risks of powerful AI models, as Mythos—capable of finding flaws in critical infrastructure software—was exploited by unauthorized users, potentially enabling malicious cyberattacks and undermining trust in AI governance. Mythos was initially shared only with select companies like Apple, Amazon, and Cisco under a closed beta called Project Glasswing, and Anthropic has since launched an investigation into the unauthorized access claim.

telegram · zaihuapd · Apr 23, 01:49

**Background**: Mythos is an advanced AI model developed by Anthropic that can automatically discover zero-day vulnerabilities—previously unknown software flaws—in systems like banks, power grids, and governments. Anthropic described it as too dangerous for public release, sharing it only with a few trusted partners and the UK government. The model's capabilities have alarmed global leaders and cybersecurity experts, as it could be used for both defensive and offensive purposes.

<details><summary>References</summary>
<ul>
<li><a href="https://www.bbc.com/news/articles/cy41zejp9pko">Anthropic investigating claim of unauthorised access to Mythos AI tool</a></li>
<li><a href="https://www.theguardian.com/technology/2026/apr/22/what-is-anthropic-mythos-ai-threat-global-cybersecurity">What is Mythos AI and why could it be a threat to global cybersecurity? | AI (artificial intelligence) | The Guardian</a></li>
<li><a href="https://www.nytimes.com/2026/04/22/technology/anthropics-mythos-ai.html">Anthropic’s New Mythos A.I. Model Sets Off Global Alarms - The New York Times</a></li>

</ul>
</details>

**Tags**: `#AI security`, `#cybersecurity`, `#Anthropic`, `#Mythos`, `#data breach`

---

<a id="item-3"></a>
## [Bitwarden CLI npm Package Hit by Checkmarx Supply Chain Attack](https://socket.dev/blog/bitwarden-cli-compromised) ⭐️ 9.0/10

Socket researchers discovered that the Bitwarden CLI npm package @bitwarden/cli@2026.4.0 was compromised in a supply chain attack, with malicious code injected into the bw1.js file via a tampered GitHub Action in Bitwarden's CI/CD pipeline. This attack targets a widely-used password manager CLI tool, potentially exposing credentials, crypto wallet keys, and developer secrets of thousands of users, and highlights the growing threat of supply chain attacks on popular open-source packages. The malware steals GitHub tokens, cloud service credentials, SSH keys, npm configurations, and crypto wallet data, then exfiltrates them by creating public GitHub repositories with specific topics; it also includes a self-destruct mechanism targeting Russian-language systems.

telegram · zaihuapd · Apr 23, 16:02

**Background**: Supply chain attacks occur when attackers compromise a trusted component in the software development pipeline, such as a CI/CD tool or third-party package, to distribute malware to downstream users. Bitwarden is a popular open-source password manager, and its CLI is widely used by developers for automation and credential management. The Checkmarx campaign has previously targeted other tools like Trivy and LiteLLM, indicating a broader, ongoing threat.

<details><summary>References</summary>
<ul>
<li><a href="https://thehackernews.com/2026/04/bitwarden-cli-compromised-in-ongoing.html">Bitwarden CLI Compromised in Ongoing Checkmarx Supply Chain Campaign</a></li>
<li><a href="https://thehackernews.com/2026/04/malicious-kics-docker-images-and-vs.html">Malicious KICS Docker Images and VS Code Extensions Hit Checkmarx Supply Chain</a></li>
<li><a href="https://tech.yahoo.com/cybersecurity/articles/bitwarden-cli-supply-chain-attack-142710104.html">Bitwarden CLI Supply Chain Attack Puts Crypto Wallet Keys at Risk</a></li>

</ul>
</details>

**Tags**: `#supply chain attack`, `#security`, `#Bitwarden`, `#npm`, `#credential theft`

---

<a id="item-4"></a>
## [Tailscale cofounder proposes simpler cloud from first principles](https://crawshaw.io/blog/building-a-cloud) ⭐️ 8.0/10

David Crawshaw, a cofounder of Tailscale, published a blog post arguing that modern cloud infrastructure is overly complex and expensive, and proposed building a simpler, more user-centric cloud from first principles. This critique from a respected industry figure challenges the status quo of cloud computing, especially the dominance of Kubernetes, and could influence how startups and engineers rethink infrastructure design and cost efficiency. Crawshaw argues that VMs are the wrong shape because they tie costs to CPU and memory rather than actual work done, and that making Kubernetes good is inherently impossible. The post has sparked strong community engagement with 755 points and 393 comments.

hackernews · bumbledraven · Apr 23, 04:44

**Background**: Tailscale is a company founded by former Google engineers that provides a mesh VPN service known for its simplicity and ease of use. The post reflects a growing frustration among developers with the complexity and cost of modern cloud stacks, particularly Kubernetes, which many feel adds unnecessary overhead for small to medium-scale deployments.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Tailscale">Tailscale - Wikipedia</a></li>
<li><a href="https://councils.forbes.com/profile/Avery-Pennarun-CEO-Founder-Tailscale/0031c5ae-0eef-4a54-8298-cacfd34ee08d">Avery Pennarun | CEO/Founder - Tailscale | Forbes Technology Council</a></li>

</ul>
</details>

**Discussion**: Commenters largely agreed with Crawshaw's critique, sharing personal experiences of Kubernetes incidents and the mismatch between VM pricing and actual work. Some expressed skepticism about whether a simpler cloud could remain profitable at scale, while others pointed to self-hosted alternatives like Firecracker as promising directions.

**Tags**: `#cloud computing`, `#kubernetes`, `#infrastructure`, `#devops`, `#startup`

---

<a id="item-5"></a>
## [Alberta Startup Sells No-Tech Tractors at Half Price](https://wheelfront.com/this-alberta-startup-sells-no-tech-tractors-for-half-price/) ⭐️ 8.0/10

An Alberta-based startup is offering simple, low-tech tractors at half the price of traditional high-tech models, targeting farmers frustrated with locked-down, expensive agricultural machinery. This reflects a growing backlash against over-engineered, software-locked equipment in agriculture, tapping into the right-to-repair movement and broader tech industry debates about simplicity and open ecosystems. The tractors lack modern digital features like GPS tracking, touchscreens, and software locks, making them easier and cheaper to repair by independent mechanics or farmers themselves.

hackernews · Kaibeezy · Apr 22, 16:29

**Background**: Major tractor manufacturers like John Deere have increasingly equipped their machines with proprietary software and digital locks, restricting farmers from repairing their own equipment and forcing them to use authorized dealers. This has sparked a long-running right-to-repair battle, with the U.S. Federal Trade Commission suing John Deere in 2025 over these practices. The startup's approach directly counters this trend by offering a simpler, more repairable alternative.

<details><summary>References</summary>
<ul>
<li><a href="https://www.bbc.com/news/business-64206913">US farmers win right to repair John Deere equipment</a></li>
<li><a href="https://www.npr.org/2025/01/15/nx-s1-5260895/john-deere-ftc-lawsuit-right-to-repair-tractors">FTC sues John Deere over farmers' right to repair tractors : NPR</a></li>
<li><a href="https://thecounter.org/right-to-repair-elizabeth-warren-john-deere/">As farmers fight for the right to repair their tractors , an antitrust...</a></li>

</ul>
</details>

**Discussion**: Community comments are overwhelmingly positive, with many expressing nostalgia for simpler, repairable machines and frustration with locked-down ecosystems. Some commenters wish for similar options in cars and EVs, while others note that such products were historically difficult to sell in the U.S. due to regulatory barriers.

**Tags**: `#agriculture`, `#startups`, `#technology backlash`, `#open ecosystems`, `#simplicity`

---

<a id="item-6"></a>
## [Apple fixes bug that cops used to extract deleted chat messages from iPhones](https://techcrunch.com/2026/04/22/apple-fixes-bug-that-cops-used-to-extract-deleted-chat-messages-from-iphones/) ⭐️ 8.0/10

Apple released an emergency update (iOS 26.4.2 and iPadOS 26.4.2) to fix CVE-2026-28950, a Notification Services bug that caused deleted alerts to remain stored on devices, allowing law enforcement to recover deleted chat messages from apps like Signal. This bug exposed a significant privacy risk for users who rely on ephemeral messaging apps, as deleted messages could be retrieved by forensic tools. The fix addresses a specific caching issue, but the broader problem of notification content being stored on-device remains a concern across platforms. The bug was tracked as CVE-2026-28950 and was fixed in iOS 26.4.2 and iPadOS 26.4.2, with patches also released for older supported versions. The issue arose because the operating system cached notification content in a local database even after the originating app was deleted, and the bug failed to clear those cached notifications upon app deletion.

hackernews · cdrnsf · Apr 22, 20:27

**Background**: Modern messaging apps like Signal use end-to-end encryption for messages, but push notifications often contain message previews that are decrypted and displayed by the operating system. These notification previews are stored in a local database on the device, which can be accessed by digital forensics tools even after the user deletes the original messages or the app itself. Apple and Google's push notification services act as intermediaries, meaning notification content passes through their servers and is subject to legal requests.

<details><summary>References</summary>
<ul>
<li><a href="https://www.bleepingcomputer.com/news/security/apple-fixes-ios-bug-that-retained-deleted-notification-data/">Apple fixes iOS bug that retained deleted notification data</a></li>
<li><a href="https://www.macobserver.com/news/fbi-finds-deleted-signal-messages-on-iphone-via-notification-storage-heres-how-to-protect-your-privacy/">FBI Finds Deleted Signal Messages on iPhone via Notification ...</a></li>
<li><a href="https://www.infosecurity-magazine.com/news/apple-ios-notification-bug-deleted/">Apple Fixes iOS Notification Bug Exposing Deleted Messages</a></li>

</ul>
</details>

**Discussion**: Commenters noted that the bug was only part of the problem; the main issue is that notification text is stored in a system database outside of the app's control. Users suggested enabling generic notifications (e.g., "You've received messages") in Signal settings to prevent message content from being cached, and pointed out that this is a good privacy practice in general.

**Tags**: `#security`, `#privacy`, `#iOS`, `#digital forensics`, `#notifications`

---

<a id="item-7"></a>
## [Citizen Lab Uncovers Two Telecom Surveillance Campaigns](https://techcrunch.com/2026/04/23/surveillance-vendors-caught-abusing-access-to-telcos-to-track-peoples-phone-locations-researchers-say/) ⭐️ 8.0/10

Citizen Lab researchers have uncovered two sophisticated surveillance campaigns in which vendors abused their access to telecommunications networks to track the phone locations of victims worldwide. This discovery highlights systemic vulnerabilities in telecom infrastructure that can be exploited for mass surveillance, posing serious threats to privacy and security for individuals and organizations globally. The campaigns involved two separate surveillance vendors, with clues pointing to an Israeli-based commercial geo-intelligence provider, though the specific vendor was not named. The abuse exploited weaknesses in core telecom protocols like SS7 to track locations in real time.

hackernews · mentalgear · Apr 23, 12:12

**Background**: Telecommunications networks rely on protocols like SS7 (Signaling System No. 7) to route calls and share location data between carriers. These protocols were designed decades ago with trust-based assumptions and lack modern security safeguards, making them vulnerable to abuse by actors with network access.

<details><summary>References</summary>
<ul>
<li><a href="https://techcrunch.com/2026/04/23/surveillance-vendors-caught-abusing-access-to-telcos-to-track-peoples-phone-locations-researchers-say/">Surveillance vendors caught abusing access to telcos to... | TechCrunch</a></li>
<li><a href="https://securityaffairs.com/46473/hacking/ss7-protocol-surveillance.html">Hackers spy on Congressman abusing the SS 7 protocol</a></li>
<li><a href="https://arstechnica.com/information-technology/2019/09/hackers-are-exploiting-a-platform-agnostic-flaw-to-track-mobile-phone-locations/">Hackers are exploiting a platform-agnostic flaw to track mobile phone ...</a></li>

</ul>
</details>

**Discussion**: Community comments express deep concern and frustration, with users sharing personal stories of stalkers exploiting telecom access and noting that surveillance tools are often misused for personal gain, such as in LOVEINT incidents. Some commenters also point out that such tracking is routine in certain countries like Russia, where data ends up on the black market.

**Tags**: `#surveillance`, `#telecom security`, `#privacy`, `#citizen lab`, `#security research`

---

<a id="item-8"></a>
## [France confirms data breach at ANTS, 19 million citizens at risk](https://techcrunch.com/2026/04/22/france-confirms-data-breach-at-government-agency-that-manages-citizens-ids/) ⭐️ 8.0/10

France's National Agency for Secure Documents (ANTS) confirmed a data breach detected on April 15, 2026, with hackers claiming to possess a database containing 19 million records of citizens' personal information. This breach exposes highly sensitive personal data of millions of French citizens, posing significant risks of identity theft, fraud, and privacy violations, and highlights vulnerabilities in government digital infrastructure. Stolen data includes names, birth dates, places of birth, addresses, and phone numbers; ANTS is investigating the attack and has begun notifying affected individuals, while the exact number of victims remains unconfirmed.

telegram · zaihuapd · Apr 23, 00:08

**Background**: ANTS (Agence nationale des titres sécurisés) is the French government agency responsible for issuing identity cards, passports, and other secure documents. Its online portal, ants.gouv.fr, allows citizens to apply for and renew these documents, making it a prime target for cyberattacks. The breach was first detected on April 15, 2026, and hackers later claimed the stolen data on forums.

<details><summary>References</summary>
<ul>
<li><a href="https://www.xinouzhou.com/wenzhang/145213-tu-fa-fa-guo-ants-ping-tai-zao-wang-luo-gong-ji-bu-fen-zheng-jian-shen-qing-ren-xin-xi-xie-lu">突发：法国ANTS平台遭网络攻击，部分证件申请人信息泄露</a></li>
<li><a href="https://www.investgo.cn/article/gb/gbdt/202604/843239.html">法国国家权证中心网站遭骇 大量个人数据泄露-“走出去”导航网</a></li>

</ul>
</details>

**Tags**: `#data breach`, `#cybersecurity`, `#privacy`, `#government`, `#France`

---

<a id="item-9"></a>
## [Hairdryer Used to Manipulate Paris Weather Sensor for Polymarket Profit](https://fibo-crypto.fr/en/blog/polymarket-weather-sensor-manipulation-paris-meteo-france-2026/) ⭐️ 8.0/10

A person allegedly used a hairdryer to heat a Météo-France temperature sensor at Paris Charles de Gaulle Airport on April 6 and 15, 2026, causing abnormal readings that triggered payouts of over $34,000 on Polymarket's Paris weather prediction markets. This incident highlights a novel attack vector where physical manipulation of IoT sensors can be exploited to profit from prediction markets, raising serious concerns about data integrity and security in decentralized forecasting platforms. On April 6, the sensor reading jumped from near 18°C to over 21°C within minutes, and on April 15, the probability of a 22°C reading surged from 0.1% to 95% in 30 minutes. Météo-France filed a criminal complaint with the Air Transport Gendarmerie and found tampering evidence during an on-site inspection.

telegram · zaihuapd · Apr 23, 04:36

**Background**: Polymarket is a decentralized prediction market platform where users trade on the outcomes of real-world events, with payouts determined by verified data sources. IoT sensors, like weather stations, collect and transmit data remotely, making them potential targets for physical manipulation if not properly secured.

<details><summary>References</summary>
<ul>
<li><a href="https://nftenex.com/paris-weather-sensor-polymarket-bet-hair-dryer-manipulation/">Paris Weather Sensor in $34K Polymarket Bet Manipulated by Hair ...</a></li>
<li><a href="https://news.google.com/stories/CAAqNggKIjBDQklTSGpvSmMzUnZjbmt0TXpZd1NoRUtEd2pZZ3VYN0VCRndRREhCc0U1VjBDZ0FQAQ?hl=en-KE&gl=KE&ceid=KE:en">Report: Hair dryer used to manipulate Paris weather sensor - Overview</a></li>

</ul>
</details>

**Tags**: `#prediction markets`, `#IoT security`, `#sensor manipulation`, `#Polymarket`, `#cybersecurity`

---

<a id="item-10"></a>
## [Google Cloud default security flaw leads to $18,000 bill](https://www.tomshardware.com/tech-industry/artificial-intelligence/google-cloud-customer-wakes-up-to-usd18-000-bill-despite-usd7-budget-thanks-to-forgotten-public-api-key-attacker-put-in-60-000-requests-and-blasted-through-usd1-400-spending-cap) ⭐️ 8.0/10

Australian AI consultant Jesse Davies received a $18,000 bill from Google Cloud despite setting a $7 budget, after an attacker used a leaked API key from a historical project to make 60,000 requests. Google Cloud's automatic credit limit increase without notification exacerbated the financial damage, though Google later waived the charges. This incident highlights systemic security risks in Google Cloud's default configuration, where API keys that were once public identifiers can now silently grant access to billable AI services like Gemini. It underscores the urgent need for cloud providers to adopt secure defaults and transparent billing controls to protect customers from unexpected financial ruin. Truffle Security identified that Gemini API keys have a uniform format and that Google's default security settings are disabled, making legacy public-facing keys vulnerable to privilege escalation. The attacker bypassed multiple security measures by calling a plaintext key stored in a container environment variable via a public URL.

telegram · zaihuapd · Apr 23, 05:21

**Background**: Google Cloud API keys were originally designed as public identifiers for tracking usage, not as secret credentials. However, with the introduction of Gemini AI, these same keys now grant access to billable AI endpoints, effectively turning them into secrets without warning developers. This insecure default posture (CWE-1188) and incorrect privilege assignment (CWE-269) mean that keys leaked in code repositories or public URLs can be exploited for unauthorized AI usage, leading to massive bills.

<details><summary>References</summary>
<ul>
<li><a href="https://trufflesecurity.com/blog/google-api-keys-werent-secrets-but-then-gemini-changed-the-rules">Google API Keys Weren't Secrets. But then Gemini Changed the ...</a></li>
<li><a href="https://cybersecuritynews.com/google-api-keys-gemini/">Google API Keys Expose Private Data Silently Through Gemini</a></li>
<li><a href="https://www.techradar.com/pro/security/usd15k-bill-destroyed-a-solo-developers-startup-how-hackers-are-using-leaked-google-api-keys-to-go-wild-with-gemini-ai-for-free">Google API keys give attackers unauthorized Gemini AI access</a></li>

</ul>
</details>

**Tags**: `#Google Cloud`, `#security`, `#cloud computing`, `#API keys`, `#financial risk`

---

<a id="item-11"></a>
## [ByteDance Releases Seed3D 2.0, Making 3D Generation Production-Ready](https://paipancon.com/fc2daily/detail/FC2-PPV-1700423) ⭐️ 8.0/10

ByteDance has released Seed3D 2.0, a next-generation 3D generation model that achieves state-of-the-art (SOTA) results in both geometry and texture quality, with human evaluation showing a preference rate over 69% compared to mainstream models. This advancement pushes 3D content generation from demo-level to production-ready, significantly lowering the barrier for creating high-quality 3D assets for games, simulations, and robotics, and it extends to component-level generation with physics simulation compatibility. Seed3D 2.0 supports component-level generation and scene composition, allowing users to split 3D content into parts and complete shapes, and it outputs assets with full joint information in standard formats like URDF, compatible with physics simulation engines such as NVIDIA Isaac Sim.

telegram · zaihuapd · Apr 23, 08:15

**Background**: Traditional 3D model generation often produces assets that look good in demos but fail in production due to poor geometry or unrealistic textures. URDF (Unified Robot Description Format) is an XML-based standard used in robotics to describe robot structures with links and joints, while Isaac Sim is NVIDIA's GPU-accelerated physics simulation platform for training and validating AI-based robots.

<details><summary>References</summary>
<ul>
<li><a href="https://wiki.ros.org/urdf/XML/model">XML Robot Description Format (URDF) - ROS Wiki</a></li>
<li><a href="https://docs.isaacsim.omniverse.nvidia.com/4.5.0/physics/simulation_fundamentals.html">Physics Simulation Fundamentals — Isaac Sim Documentation</a></li>
<li><a href="https://github.com/isaac-sim">NVIDIA Isaac Sim - GitHub</a></li>

</ul>
</details>

**Tags**: `#3D generation`, `#ByteDance`, `#AI`, `#computer graphics`, `#physics simulation`

---

<a id="item-12"></a>
## [DeepSeek Open-Sources TileKernels for NVIDIA Blackwell](https://github.com/deepseek-ai/TileKernels) ⭐️ 8.0/10

DeepSeek has open-sourced TileKernels, a high-performance GPU operator library based on TileLang, optimized for large language model (LLM) training and inference. The library supports NVIDIA's SM90 and the latest SM100 (Blackwell) architectures and requires CUDA 13.1 or later. This release provides the AI community with production-ready, near-hardware-limit operators for LLM workloads on the latest Blackwell GPUs, potentially accelerating training and inference performance. It also demonstrates DeepSeek's commitment to open-source AI infrastructure, benefiting developers and researchers building large-scale models. TileKernels covers MoE routing, FP8/FP4 quantization, and various fused operators, and has already been deployed in DeepSeek's internal environment. The library is built on TileLang, a domain-specific language for GPU kernel development that uses a tiling abstraction.

telegram · zaihuapd · Apr 23, 09:36

**Background**: GPU operator libraries like TileKernels provide low-level, optimized kernels for common deep learning operations, such as matrix multiplications and attention mechanisms. TileLang is a domain-specific language that simplifies writing high-performance GPU kernels by using a tiling abstraction, reducing code complexity. NVIDIA's Blackwell architecture (SM100) introduces new tensor core instructions that are 2x to 4x faster than the previous Hopper architecture, making optimized operators critical for leveraging its full potential.

<details><summary>References</summary>
<ul>
<li><a href="https://tilelang.com/">TileLang 0.1.8 documentation</a></li>
<li><a href="https://docs.nvidia.com/cutlass/4.3.3/media/docs/cpp/blackwell_functionality.html">Blackwell SM 100 GEMMs — NVIDIA CUTLASS Documentation</a></li>

</ul>
</details>

**Tags**: `#DeepSeek`, `#GPU算子库`, `#LLM`, `#NVIDIA Blackwell`, `#开源`

---

<a id="item-13"></a>
## [Tencent Open-Sources Hy3 Preview: 295B MoE Model](https://mp.weixin.qq.com/s/5_nUI2mDchlwoedinFUMeA) ⭐️ 8.0/10

Tencent has released and open-sourced the Hy3 preview, a 295-billion-parameter Mixture-of-Experts (MoE) language model with 21 billion active parameters and a 256K-token context window, optimized for complex reasoning and agent applications. This release marks a significant open-source contribution from a major Chinese tech company, providing a large-scale MoE model with strong reasoning capabilities that can compete with other leading open-source models, and its integration into Tencent's products like Yuanbao and QQ demonstrates practical enterprise deployment. The model achieves a 54% reduction in first-token latency for products like CodeBuddy due to deep co-optimization of model architecture and inference framework, and it is available on GitHub, HuggingFace, and via Tencent Cloud's API with personal plans starting at 28 RMB per month.

telegram · zaihuapd · Apr 23, 10:07

**Background**: Mixture-of-Experts (MoE) is an architecture that divides a model into multiple specialized sub-models (experts) and activates only a subset for each input, allowing large total parameter counts while keeping inference efficient. A 295B total parameter model with 21B active parameters means that despite its massive size, it runs at a speed comparable to a much smaller dense model, making it practical for deployment.

<details><summary>References</summary>
<ul>
<li><a href="https://www.geeksforgeeks.org/nlp/what-is-mixture-of-experts-moe/">What is Mixture of Experts (MoE)? - GeeksforGeeks</a></li>
<li><a href="https://newsletter.maartengrootendorst.com/p/a-visual-guide-to-mixture-of-experts">A Visual Guide to Mixture of Experts (MoE) Images Mixture of Experts Explained - Hugging Face Understanding Mixture of Experts (MoE): The Architecture ... What is mixture of experts? - IBM What Is Mixture of Experts (MoE)? How It Works (2026) MoE LLM Architecture: How It Works, Benefits And Key Models ...</a></li>
<li><a href="https://medium.com/@sharanharsoor/understanding-mixture-of-experts-moe-the-architecture-powering-next-generation-language-models-49c1d1d467c9">Understanding Mixture of Experts (MoE): The Architecture ...</a></li>

</ul>
</details>

**Tags**: `#large language model`, `#open source`, `#MoE`, `#Tencent`, `#AI`

---

<a id="item-14"></a>
## [SFC and PwC Reach HK$1 Billion Settlement for Evergrande Fraud](https://apps.sfc.hk/edistributionWeb/gateway/TC/news-and-announcements/news/doc?refNo=26PR62) ⭐️ 8.0/10

On April 23, 2026, Hong Kong's Securities and Futures Commission (SFC) announced a settlement with PwC Hong Kong, under which PwC will set aside HK$1 billion to compensate eligible minority shareholders of China Evergrande Group for its role in the company's financial fraud involving inflated revenues of 564.1 billion RMB over 2019 and 2020. This marks the first time in Hong Kong that an auditor of a collapsed company has directly compensated shareholders, setting a landmark precedent for auditor accountability and market integrity. It underscores the critical role of audit independence and could reshape regulatory expectations for auditors in major financial markets. The SFC found that PwC seriously breached professional duties, including loss of audit independence, lack of professional skepticism, and tacitly allowing management to manipulate audit samples. Under the settlement, PwC does not admit legal liability, and the SFC will take no further action against the firm.

telegram · zaihuapd · Apr 23, 12:07

**Background**: China Evergrande Group, once one of China's largest property developers, collapsed under massive debt after years of financial misconduct. In 2024, Chinese regulators fined Evergrande 41.75 billion RMB for inflating revenues by 564.1 billion RMB across 2019 and 2020, turning reported profits into substantial losses. PwC served as Evergrande's auditor during those years and was accused of failing to detect the fraud.

<details><summary>References</summary>
<ul>
<li><a href="https://xueqiu.com/3338215700/385417746">突发！香港证监会与普华永道就恒大财务造假达成赔偿协议，10亿港元赔...</a></li>
<li><a href="https://www.thepaper.cn/newsDetail_forward_33037031">香港证监会、会财局同日出手 普华永道同意预留10亿港元赔偿恒大股东_...</a></li>

</ul>
</details>

**Tags**: `#financial regulation`, `#audit failure`, `#corporate fraud`, `#market integrity`, `#regulatory tech`

---

<a id="item-15"></a>
## [China's Three Major Carriers Report International Network Outages](https://t.me/zaihuapd/41029) ⭐️ 8.0/10

Unconfirmed reports indicate that China Telecom, China Unicom, and China Mobile are experiencing widespread network disruptions on international routes, with significant packet loss and connection interruptions to Hong Kong, Japan, and the United States. This incident affects a broad user base relying on cross-border connectivity for work, education, and communication, and could have geopolitical implications if the disruptions are intentional. The simultaneous failure across all three carriers suggests a systemic issue rather than isolated faults. The disruptions affect both premium routes like China Telecom's CN2 and China Unicom's 9929, as well as standard routes such as 163 and 4837. Reports are concentrated among Beijing Mobile users, with fewer samples for US-bound routes.

telegram · zaihuapd · Apr 23, 12:45

**Background**: Chinese telecom carriers operate multiple tiers of international routing: premium routes like CN2 (China Telecom) and 9929 (China Unicom) offer higher priority and lower latency, while standard routes like 163 and 4837 handle general traffic. These routes are critical for cross-border data transmission, and disruptions can stem from undersea cable cuts, routing misconfigurations, or deliberate policy changes. The cause of this incident remains unknown.

<details><summary>References</summary>
<ul>
<li><a href="https://x.com/yeahwu404/status/2047301068175065487">风闻消息，部分地区受影响，受影响的可以底下留言，也别说谣言不谣言...</a></li>
<li><a href="https://www.deepflood.com/post-37587-1">风闻消息：中国联通、移动、电信运营商对海外方向均报告网络故障</a></li>
<li><a href="https://tbbbk.com/vps-route-guide-tcping-as9929-cn2-explained/">VPS 路由完全指南（2026）：Tcping 测速、AS9929、CN2 线路怎么看？</a></li>

</ul>
</details>

**Discussion**: Community comments on social media and forums largely confirm the outages, with users sharing localized experiences and traceroute results. Some speculate whether the disruptions are due to a technical fault or intentional policy changes, but no consensus has emerged.

**Tags**: `#network outage`, `#China telecom`, `#internet infrastructure`, `#routing`, `#geopolitics`

---

<a id="item-16"></a>
## [Apple CEO Tim Cook to Step Down, John Ternus to Succeed in 2026](https://t.me/zaihuapd/41030) ⭐️ 8.0/10

Apple has announced that CEO Tim Cook will step down on September 1, 2026, and will be succeeded by John Ternus, the company's senior vice president of hardware engineering. Cook will transition to the role of executive chairman of Apple's board of directors. This leadership change marks the first CEO transition at Apple since Tim Cook took over in 2011, and it signals a new era for the company's product strategy and corporate direction. John Ternus, a hardware engineering veteran, will now lead one of the world's most valuable technology companies. Ternus joined Apple in 2001, became vice president of hardware engineering in 2013, and has been responsible for the engineering of iPhone, iPad, Mac, Apple Watch, AirPods, and Apple Vision Pro. Current chairman Arthur Levinson will become lead independent director on September 1, 2026, and Ternus will join the board on the same day.

telegram · zaihuapd · Apr 23, 13:46

**Background**: Tim Cook has served as Apple's CEO since 2011, succeeding Steve Jobs, and has overseen massive growth in revenue, services, and product lines. John Ternus has been a key figure in Apple's hardware engineering for over two decades, leading the development of many of the company's most iconic products. The executive chairman role allows Cook to remain involved in long-term strategy and public affairs while handing daily operations to Ternus.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/John_Ternus">John Ternus - Wikipedia</a></li>
<li><a href="https://www.apple.com/leadership/john-ternus/">Apple Leadership - John Ternus - Apple</a></li>
<li><a href="https://www.apple.com/newsroom/2026/04/tim-cook-to-become-apple-executive-chairman-john-ternus-to-become-apple-ceo/">Tim Cook to become Apple Executive Chairman John Ternus to ...</a></li>

</ul>
</details>

**Tags**: `#Apple`, `#leadership change`, `#CEO transition`, `#tech industry`

---

<a id="item-17"></a>
## [UK NCSC Officially Endorses Passkeys as Preferred Authentication Method](https://www.techradar.com/pro/security/uk-security-agency-officially-declares-passkeys-superior-to-passwords-passkeys-should-be-the-first-choice-for-authentication) ⭐️ 8.0/10

The UK's National Cyber Security Centre (NCSC) has officially declared that passkeys are superior to traditional passwords and two-factor authentication, recommending them as the first-choice login method for digital services. This marks a shift from the NCSC's previous cautious stance due to implementation challenges. As the UK's national technical authority for cybersecurity, the NCSC's endorsement provides significant industry validation for passkeys, likely accelerating their adoption across both public and private sectors. This move could reshape authentication standards globally, reducing reliance on vulnerable passwords and improving overall cyber resilience. Over 50% of active Google users in the UK have already registered passkeys, and major platforms like eBay and PayPal have fully adapted to support them. The NCSC noted that technological advancements over the past 12 months have resolved core implementation challenges, making passkeys both more secure and easier to use than password-based systems.

telegram · zaihuapd · Apr 23, 14:47

**Background**: The NCSC is the UK's technical authority for cyber incidents, part of GCHQ, and was formed in 2016 to provide a unified national response to cyber threats. Passkeys are a passwordless authentication method that uses device-stored cryptographic keys and biometric verification (e.g., fingerprint or face recognition) instead of traditional passwords. They are designed to eliminate common security risks like phishing and credential theft.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/National_Cyber_Security_Centre_(United_Kingdom)">National Cyber Security Centre (United Kingdom) - Wikipedia</a></li>
<li><a href="https://ico.org.uk/for-organisations/the-guide-to-nis/the-role-of-the-national-cyber-security-centre-ncsc/">The role of the National Cyber Security Centre (NCSC) | ICO</a></li>
<li><a href="https://www.gov.uk/government/organisations/national-cyber-security-centre">National Cyber Security Centre - GOV.UK Top Stories Cyber Security - GCHQ Understanding the Role of the NCSC - ukcybersecurity.co.uk National Cyber Security Centre (United Kingdom) - Wikipedia UK Faces a Cyber ‘Perfect Storm’ - Infosecurity Magazine The role of the National Cyber Security Centre ( NCSC ) | ICO Cyber Security | GCHQ - GCHQ.GOV. UK Understanding the Role of the NCSC - ukcybersecurity.co. uk The role of the National Cyber Security Centre ( NCSC ) | ICO</a></li>

</ul>
</details>

**Tags**: `#cybersecurity`, `#authentication`, `#passkeys`, `#NCSC`, `#identity`

---

<a id="item-18"></a>
## [EU Pressures Google to Open Android to AI Rivals](https://www.bloomberg.com/news/articles/2026-04-23/google-faces-eu-pressure-to-open-up-android-to-gemini-rivals) ⭐️ 8.0/10

The European Union is drafting requirements that would force Google to give rival AI assistants like ChatGPT and Claude the same system-level permissions on Android as its own Gemini assistant. This could reshape competition in the AI assistant market by lowering barriers for rivals on the dominant Android platform, but Google warns it may compromise user security and privacy. The requirements are still in draft stage and their release could be delayed; Google has expressed concerns that such openness could negatively impact user security and privacy.

telegram · zaihuapd · Apr 23, 15:31

**Background**: The EU's Digital Markets Act (DMA) designates large platforms like Google as "gatekeepers" and imposes rules to ensure fair competition. Android is the world's most widely used mobile operating system, and Google's Gemini is the default AI assistant on many Android devices, giving it a significant advantage over third-party assistants.

<details><summary>References</summary>
<ul>
<li><a href="https://digital-markets-act.ec.europa.eu/index_en">Digital Markets Act</a></li>
<li><a href="https://www.android.com/intl/en_us/ai/gemini/">Try Gemini, your personal AI assistant | Android</a></li>

</ul>
</details>

**Tags**: `#EU regulation`, `#Android`, `#AI assistants`, `#Google`, `#antitrust`

---

<a id="item-19"></a>
## [OpenAI's Chronicle for macOS Sparks Privacy and Security Concerns](https://www.theregister.com/2026/04/22/openai_chronicle_no_privacy_screenshot/) ⭐️ 7.0/10

OpenAI has released an opt-in research preview feature called Chronicle for its macOS Codex app, which captures screenshots to provide context for AI agents. Security researchers have criticized it as a clone of Microsoft's Recall feature, citing risks such as unencrypted local storage of OCR text and vulnerability to prompt injection attacks. This feature raises significant privacy and security concerns that could undermine user trust in AI tools and slow adoption, especially in security-sensitive environments. The controversy echoes past backlash against Microsoft's Recall, highlighting ongoing tensions between AI convenience and data protection. Screenshot data is stored locally for only 6 hours, but OCR-extracted text 'memories' are saved locally in unencrypted form indefinitely and can be accessed by other programs on the device. Additionally, these memories may be re-sent to OpenAI servers in subsequent conversations, and the feature accelerates Codex's rate limit consumption, reducing its practicality in secure settings.

telegram · zaihuapd · Apr 23, 03:06

**Background**: Prompt injection is a type of cybersecurity attack that targets machine learning models through malicious prompts, potentially causing the AI to ignore its intended instructions. Microsoft's Recall feature, which also captures screenshots for AI context, faced similar privacy backlash in 2024. OpenAI's Chronicle operates similarly by storing OCR text locally, making it susceptible to such attacks and unauthorized access.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Prompt_injection_attack">Prompt injection attack</a></li>
<li><a href="https://en.wikipedia.org/wiki/Prompt_injection">Prompt injection - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#OpenAI`, `#privacy`, `#security`, `#AI`, `#macOS`

---

<a id="item-20"></a>
## [TSMC Delays ASML High-NA EUV Adoption Until 2029 Due to Cost](https://money.udn.com/money/story/5599/9458925?from=edn_newestlist_rank) ⭐️ 7.0/10

TSMC announced at its North America Technology Forum that it will not use ASML's high-NA EUV lithography machines for mass production until at least 2029, citing a unit price exceeding 350 million euros. This decision signals a major shift in semiconductor manufacturing roadmaps, as TSMC—the world's leading foundry—chooses to optimize existing EUV tools rather than adopt the next-generation lithography, potentially slowing the pace of Moore's Law scaling and impacting ASML's revenue expectations. TSMC also disclosed that its A13 process node is scheduled for production in 2029, and the company plans to establish CoWoS and 3D-IC packaging capacity in Arizona by that same year, with the first local fab already achieving yield rates close to those in Taiwan.

telegram · zaihuapd · Apr 23, 11:22

**Background**: High-NA EUV lithography is ASML's latest extreme ultraviolet machine, designed to print smaller transistors for advanced chips. CoWoS (Chip-on-Wafer-on-Substrate) is TSMC's advanced packaging technology that stacks chips vertically to improve performance and reduce power consumption, critical for AI and high-performance computing applications.

<details><summary>References</summary>
<ul>
<li><a href="https://zhuanlan.zhihu.com/p/1890075894934132607">半导体芯片封装“CoWoS工艺技术”的详解； - 知乎</a></li>
<li><a href="https://blog.csdn.net/u013669912/article/details/143434272">CoWoS 封装 | CoWoS-S / CoWoS-R / CoWoS-L-CSDN博客</a></li>
<li><a href="https://finance.sina.com.cn/cj/2026-02-27/doc-inhpfxrh6696864.shtml">台积电先进封装科普：CoWoS、CoPoS、CoWoP 到底是个啥？谁才是下一代...</a></li>

</ul>
</details>

**Tags**: `#semiconductor`, `#TSMC`, `#ASML`, `#EUV`, `#manufacturing`

---