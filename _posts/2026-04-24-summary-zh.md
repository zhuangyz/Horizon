---
layout: default
title: "Horizon Summary: 2026-04-24 (ZH)"
date: 2026-04-24
lang: zh
---

> From 29 items, 22 important content pieces were selected

---

1. [OpenAI 发布 GPT-5.5，新一代前沿编程模型](#item-1) ⭐️ 9.0/10
2. [Bitwarden CLI 在供应链攻击中被攻陷](#item-2) ⭐️ 9.0/10
3. [vLLM v0.20.0：CUDA 13、PyTorch 2.11、FA4、TurboQuant](#item-3) ⭐️ 8.0/10
4. [Anthropic 披露导致 Claude 健忘的漏洞](#item-4) ⭐️ 8.0/10
5. [Tailscale 联合创始人提出更简单的云方案](#item-5) ⭐️ 8.0/10
6. [Palantir 员工质疑自身道德角色](#item-6) ⭐️ 8.0/10
7. [通过 Codex 后门 API 访问 GPT-5.5](#item-7) ⭐️ 8.0/10
8. [吹风机操控巴黎天气传感器，Polymarket 获利 3.4 万美元](#item-8) ⭐️ 8.0/10
9. [Google Cloud 默认缺陷致用户产生 1.8 万美元账单](#item-9) ⭐️ 8.0/10
10. [DeepSeek 开源 TileKernels 算子库，支持 NVIDIA Blackwell](#item-10) ⭐️ 8.0/10
11. [腾讯开源混元 Hy3 Preview 模型](#item-11) ⭐️ 8.0/10
12. [台积电因成本过高推迟高数值孔径 EUV 至 2029 年](#item-12) ⭐️ 8.0/10
13. [中国三大运营商遭遇大范围国际网络故障](#item-13) ⭐️ 8.0/10
14. [苹果 CEO 库克将卸任，特努斯 2026 年接棒](#item-14) ⭐️ 8.0/10
15. [欧盟施压谷歌向竞争对手开放安卓 AI 助手权限](#item-15) ⭐️ 8.0/10
16. [MIT 搭建经典与量子物理的数学桥梁](#item-16) ⭐️ 8.0/10
17. [英特尔二季度营收展望超预期，股价盘后暴涨约 20%](#item-17) ⭐️ 8.0/10
18. [LiteParse PDF 文本提取在浏览器中运行](#item-18) ⭐️ 7.0/10
19. [字节跳动发布 Seed3D 2.0，实现生产级 3D 生成](#item-19) ⭐️ 7.0/10
20. [香港证监会与普华永道就恒大造假达成 10 亿港元和解](#item-20) ⭐️ 7.0/10
21. [英国 NCSC 正式将通行密钥列为首选身份验证方式](#item-21) ⭐️ 7.0/10
22. [英国生物样本库数据遭非法售卖，官方紧急收紧访问权限](#item-22) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [OpenAI 发布 GPT-5.5，新一代前沿编程模型](https://openai.com/index/introducing-gpt-5-5/) ⭐️ 9.0/10

OpenAI 宣布推出 GPT-5.5，这是一款新的前沿编程模型，将逐步向 Pro 和企业级账户开放，随后再覆盖 Plus 用户。该模型可通过 ChatGPT 和 Codex 使用，但尚未提供 API 访问。 GPT-5.5 代表了 AI 辅助编程领域的重大进步，在 CyberGym 基准测试中获得了 82% 的分数，使其成为进攻性和防御性网络安全任务中极具能力的工具。其发布引发了社区关于开发者对此类模型依赖性的广泛讨论，凸显了 AI 在编程中日益增长的重要性。 该模型的推出是逐步进行的，持续数小时以确保服务稳定，目前尚未通过 API 提供访问，但一些用户报告称通过 Codex API 的后门方式使用了该模型。NVIDIA 的一位工程师将失去 GPT-5.5 的访问权限比作截肢，凸显了该模型被认为的不可或缺性。

hackernews · rd · Apr 23, 18:01

**背景**: GPT-5.5 是一个专注于编程任务的前沿 AI 模型，基于 OpenAI 之前的 GPT 系列构建。前沿模型是目前可用的最先进的 AI 系统，常用于软件开发、网络安全等领域的复杂问题解决。逐步推出策略是重大发布中的常见做法，旨在管理服务器负载并确保可靠性。

**社区讨论**: 社区评论中既有兴奋也有担忧：一些用户称赞 GPT-5.5 的性能及其相比 Anthropic 的 Mythos 等竞品的开放性，而另一些用户则对开发者过度依赖此类工具表示不安。此外，还有关于缺乏官方 API 访问以及使用非官方后门的讨论。

**标签**: `#AI`, `#OpenAI`, `#GPT-5.5`, `#machine learning`, `#coding tools`

---

<a id="item-2"></a>
## [Bitwarden CLI 在供应链攻击中被攻陷](https://socket.dev/blog/bitwarden-cli-compromised) ⭐️ 9.0/10

Bitwarden CLI 版本 2026.4.0 在持续进行的 Checkmarx 供应链攻击活动中被攻陷，攻击者通过一个恶意的 npm 包窃取加密货币钱包数据和开发者凭据。 此事件凸显了 npm 生态系统的关键风险，一个广泛使用的密码管理器 CLI 工具被劫持以窃取敏感数据，可能影响数千名开发者和组织。 该攻击利用了 Bitwarden 构建流水线中被攻陷的 GitHub Action，恶意包 @bitwarden/cli@2026.4.0 被发布到 npm，其中包含一个自我传播的蠕虫，将凭据窃取到公开的 GitHub 仓库。

hackernews · tosh · Apr 23, 14:17

**背景**: 供应链攻击通过攻陷受信任的工具或依赖项来针对软件开发流水线。在此案例中，攻击者投毒了 Bitwarden CLI npm 包（开发者用于以编程方式管理密码），恶意代码被分发给更新或安装受影响版本的用户。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://thehackernews.com/2026/04/bitwarden-cli-compromised-in-ongoing.html">Bitwarden CLI Compromised in Ongoing Checkmarx Supply Chain ...</a></li>
<li><a href="https://tech.yahoo.com/cybersecurity/articles/bitwarden-cli-supply-chain-attack-142710104.html">Bitwarden CLI Supply Chain Attack Puts Crypto Wallet Keys at Risk</a></li>
<li><a href="https://www.ox.security/blog/shai-hulud-bitwarden-cli-supply-chain-attack/">Bitwarden CLI Compromised: Inside the Shai-Hulud Supply Chain Attack</a></li>

</ul>
</details>

**社区讨论**: 社区成员讨论了缓解策略，例如在 npm 中设置最小发布年龄（如 7 天）和固定依赖版本，一些人指出 Rust 替代方案（rbw）可以减小依赖树规模。其他人则担心 CLI 在 tmux 等终端复用器中暴露敏感数据。

**标签**: `#supply chain security`, `#npm`, `#Bitwarden`, `#supply chain attack`, `#dependency management`

---

<a id="item-3"></a>
## [vLLM v0.20.0：CUDA 13、PyTorch 2.11、FA4、TurboQuant](https://github.com/vllm-project/vllm/releases/tag/v0.20.0) ⭐️ 8.0/10

vLLM v0.20.0 由 257 位贡献者提交了 546 次提交，将默认 CUDA 轮升级至 CUDA 13.0，基于 PyTorch 2.11 发布，并增加了对 HuggingFace Transformers v5 的兼容性。同时，它默认启用 FlashAttention 4 作为 MLA 预填充后端，并引入了 TurboQuant 2 位 KV 缓存压缩后端，实现 4 倍容量。 此次发布显著提升了大型语言模型的推理性能和内存效率，尤其是在现代 Hopper 和 Blackwell GPU 上。TurboQuant 2 位 KV 缓存压缩可将内存使用量减少 4 倍，从而支持更大的上下文窗口或降低生产部署的硬件要求。 FlashAttention 4 被重新启用为默认的 MLA 预填充后端，支持 head-dim 512 和 SM90+ GPU 上的分页 KV。TurboQuant 是一个新的注意力后端，可将 KV 缓存压缩至 2 位，该版本还包括在线量化前端和 vLLM IR 的初始框架，为未来的内核开发奠定基础。

github · khluu · Apr 23, 21:02

**背景**: vLLM 是一个高吞吐量、内存高效的开源大型语言模型推理引擎，广泛应用于生产环境。多头潜在注意力（MLA）被 DeepSeek V3 等模型采用，相比标准 MHA 可将 KV 缓存内存减少 4-8 倍。FlashAttention 是一系列快速且内存高效的注意力算法，而 TurboQuant 是 Google 提出的一种压缩方法，可在最小化精度损失的同时大幅减小模型尺寸。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://langcopilot.com/posts/2025-09-13-multi-head-latent-attention-mla-explained">MLA Attention : 4 -8x Less Memory Than MHA (DeepSeek...)</a></li>
<li><a href="https://research.google/blog/turboquant-redefining-ai-efficiency-with-extreme-compression/">TurboQuant: Redefining AI efficiency with extreme compression</a></li>

</ul>
</details>

**标签**: `#vLLM`, `#LLM inference`, `#CUDA`, `#FlashAttention`, `#KV cache`

---

<a id="item-4"></a>
## [Anthropic 披露导致 Claude 健忘的漏洞](https://www.anthropic.com/engineering/april-23-postmortem) ⭐️ 8.0/10

Anthropic 披露了 Claude Code 中的一个漏洞，该漏洞导致 Claude 在每次对话轮次中清除思考上下文（而非仅在闲置会话后清除一次），使其显得健忘和重复，影响了 3 月 26 日至 4 月 10 日期间的 Sonnet 4.6 和 Opus 4.6 用户。 该漏洞直接导致用户体验连续两周下降，凸显了 AI 系统的脆弱性以及 AI 运营透明性的重要性。该事件还引发了社区关于可靠性和与 OpenAI 竞争的讨论。 该漏洞于 3 月 26 日引入，当时 Anthropic 发布了一项更改，旨在清除闲置超过一小时的会话中的旧思考内容以降低延迟，但编码错误导致每次对话轮次都进行清除而非仅一次。修复于 4 月 10 日部署，该问题影响了 Sonnet 4.6 和 Opus 4.6 模型。

hackernews · mfiguiere · Apr 23, 17:48

**背景**: Claude Code 是 Anthropic 的 AI 编码助手，它使用扩展思考功能来在长时间会话中保持上下文。该漏洞出现在 Claude Code 的上下文管理、Anthropic API 和扩展思考功能的交叉点，并且在部署前通过了多轮人工和自动化审查。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.anthropic.com/engineering/april-23-postmortem">An update on recent Claude Code quality reports \ Anthropic</a></li>
<li><a href="https://github.com/anthropics/claude-code/issues/8677">[BUG] /context fails on first try with thinking anabled ...</a></li>
<li><a href="https://dev.to/letanure/claude-code-part-10-common-issues-and-quick-fixes-186g">Claude Code: Part 10 - Common Issues and Quick Fixes</a></li>

</ul>
</details>

**社区讨论**: 社区反应不一：一些用户赞赏 Anthropic 的透明事后分析，而另一些用户则对漏洞修复延迟两周表示不满。多位评论者指出，该事件凸显了 AI 系统需要更好的透明性和测试，部分用户还将 Claude 的表现与 OpenAI 的产品进行了不利比较。

**标签**: `#AI`, `#Claude`, `#bug`, `#transparency`, `#Anthropic`

---

<a id="item-5"></a>
## [Tailscale 联合创始人提出更简单的云方案](https://crawshaw.io/blog/building-a-cloud) ⭐️ 8.0/10

Tailscale 联合创始人 David Crawshaw 发表了一篇博文，阐述了他对新云平台的愿景，该平台优先考虑简单性和性能，而非现有云和 Kubernetes 的复杂性。 来自一位备受尊敬的基础设施领导者的批评挑战了云复杂性的现状，可能影响开发者和公司对部署应用的思考方式。强烈的社区反响（983 分，486 条评论）表明对 Kubernetes 等当前工具的广泛不满。 Crawshaw 认为让 Kubernetes 变好本质上是不可能的，称其为“在猪上涂口红”，并批评传统云默认每个 VM 只有 3000 IOPS，而笔记本电脑能提供 500k。他提议的平台 exe.dev 使用 HTTP 代理处理入站连接，且没有公共 IPv4，一些评论者认为这很晦涩。

hackernews · bumbledraven · Apr 23, 04:44

**背景**: Kubernetes 是一个流行的容器编排系统，以其强大的功能而闻名，但也因其陡峭的学习曲线和操作复杂性而著称。Tailscale 是一家提供简单、零配置 VPN 服务的公司，其联合创始人的观点在基础设施社区中具有分量。这篇博文反映了一种日益增长的情绪，即许多云工具已经变得过于复杂，反而适得其反。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Tailscale">Tailscale - Wikipedia</a></li>
<li><a href="https://encore.cloud/resources/kubernetes-complexity">Why Kubernetes Is So Complicated (And What to Use Instead)</a></li>
<li><a href="https://dev.to/rocktimmanta/why-does-kubernetes-feel-so-complicated-1l14">Why Does Kubernetes Feel So Complicated? - DEV Community</a></li>

</ul>
</details>

**社区讨论**: 评论者大多同意对 Kubernetes 复杂性的批评，有人称其“说得太好了”，另一个人指出事故往往是由 Kubernetes 本身引起的。然而，一些人对 Crawshaw 自己的平台 exe.dev 表示怀疑，指出其自身的晦涩抽象和限制，例如没有公共 IPv4。

**标签**: `#cloud computing`, `#kubernetes`, `#PaaS`, `#infrastructure`, `#tailscale`

---

<a id="item-6"></a>
## [Palantir 员工质疑自身道德角色](https://www.wired.com/story/palantir-employees-are-starting-to-wonder-if-theyre-the-bad-guys/) ⭐️ 8.0/10

《连线》杂志报道称，在政治争议和内部异议中，Palantir 员工越来越对为美国国防承包商工作产生道德质疑。 这场辩论凸显了科技行业内部在国防承包和监控问题上日益增长的道德紧张关系，可能影响员工留任、招聘以及公众对 Palantir 等公司的看法。 文章包含内部消息，员工对公开讨论道德问题损害美国以外销售表示沮丧，而另一些人则认为这个问题影响每个人个人。

hackernews · pavel_lishin · Apr 23, 17:30

**背景**: Palantir 是一家美国软件公司，以其数据分析平台闻名，这些平台被政府机构（包括国防和情报部门）使用。其工作常涉及监控和反恐，引发关于隐私和人权的道德担忧。

**社区讨论**: 评论者指出，Palantir 员工应认识到自己为国防承包商工作，有人引用前员工关于公司演变的采访。一位评论者推荐阅读《Careless People》，以了解科技工作者如何合理化自己的角色。

**标签**: `#ethics`, `#defense-contracting`, `#palantir`, `#tech-culture`, `#surveillance`

---

<a id="item-7"></a>
## [通过 Codex 后门 API 访问 GPT-5.5](https://simonwillison.net/2026/Apr/23/gpt-5-5/#atom-everything) ⭐️ 8.0/10

OpenAI 发布了 GPT-5.5，该模型已在 Codex 中可用，并正在向付费 ChatGPT 订阅用户推送，但尚未通过标准 API 提供。Simon Willison 创建了一个名为 llm-openai-via-codex 的插件，利用半官方的 Codex 后端 API，通过现有的 ChatGPT 订阅来运行针对 GPT-5.5 的提示。 这种变通方法使开发者无需等待官方 API 即可通过 API 对 GPT-5.5 进行基准测试和使用，凸显了 AI 提供商与第三方工具之间持续的紧张关系。它还展示了如何将基于订阅的模型访问重新用于编程用途，可能影响未来的 API 政策。 该插件逆向工程了 OpenAI 开源 Codex CLI 仓库中的身份验证机制，以访问/backend-api/codex/responses 端点。Willison 使用此设置运行了他的“骑自行车的鹈鹕”基准测试，该测试评估模型生成骑自行车鹈鹕 SVG 的能力。

rss · Simon Willison · Apr 23, 19:59

**背景**: GPT-5.5 是 OpenAI 于 2026 年 4 月 23 日发布的最新语言模型，可在 AI 编码代理 Codex 中使用，并向付费 ChatGPT 订阅用户开放。“骑自行车的鹈鹕”基准测试是一种流行的非正式测试，要求 LLM 生成一只骑自行车的鹈鹕的 SVG，以评估其代码生成和空间推理能力。此处使用的 Codex API 端点是半官方的，因为 OpenAI 已公开支持 OpenClaw 和 Pi 等第三方工具使用它，但它并非标准 API。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://simonwillison.net/2026/Apr/23/gpt-5-5/">A pelican for GPT-5.5 via the semi-official Codex backdoor API</a></li>
<li><a href="https://grokipedia.com/page/Pelican_on_a_bicycle_AI_benchmark">Pelican on a bicycle (AI benchmark)</a></li>
<li><a href="https://github.com/openai/codex/blob/main/codex-rs/responses-api-proxy/README.md">codex/codex-rs/responses-api-proxy/README.md at main - GitHub</a></li>

</ul>
</details>

**标签**: `#GPT-5.5`, `#OpenAI`, `#API`, `#AI models`, `#benchmarking`

---

<a id="item-8"></a>
## [吹风机操控巴黎天气传感器，Polymarket 获利 3.4 万美元](https://fibo-crypto.fr/en/blog/polymarket-weather-sensor-manipulation-paris-meteo-france-2026/) ⭐️ 8.0/10

2026 年 4 月 6 日和 15 日，有人使用吹风机人为加热巴黎戴高乐机场的温度传感器，导致 Polymarket 预测市场根据虚假读数结算，获利超过 3.4 万美元。 这一事件凸显了依赖现实世界数据预言机的去中心化预测市场存在关键漏洞，物理传感器操纵可被用于牟利，对预言机安全和市场诚信提出了迫切问题。 4 月 6 日，传感器读数在数分钟内从接近 18°C 升至超过 21°C；4 月 15 日，22°C 区间的概率在 30 分钟内从 0.1%飙升至 95%。Polymarket 此后将数据源切换至巴黎勒布尔热机场，但未撤销已完成的结算结果。

telegram · zaihuapd · Apr 23, 04:36

**背景**: Polymarket 是一个去中心化预测市场平台，用户对现实世界结果下注，市场结算通常依赖天气传感器等数据预言机。UMA 乐观预言机通常用于解决争议，但在此次事件中，传感器数据本身遭到了物理篡改。法国气象局在实地检查中发现篡改痕迹后，已向航空运输宪兵队提出刑事控告。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.aol.com/articles/police-investigate-claims-hair-dryer-150607773.html">Police investigate after claims ‘ hair dryer used to manipulate weather ...</a></li>
<li><a href="https://finance.yahoo.com/markets/crypto/articles/trader-manipulates-city-weather-sensor-165804921.html">Trader manipulates city weather sensor to win $34K</a></li>
<li><a href="https://help.polymarket.com/en/articles/13364518-how-are-prediction-markets-resolved">How Are Prediction Markets Resolved? - Polymarket Help Center</a></li>

</ul>
</details>

**社区讨论**: Telegram 和加密论坛上的社区讨论对攻击的简单性表示震惊，一些人呼吁采用更强大的预言机设计，例如使用多个独立数据源。其他人则争论 Polymarket 是否应撤销被操纵的交易，据报道 Vitalik Buterin 就预测市场如何更好地应对此类预言机操纵风险发表了看法。

**标签**: `#prediction markets`, `#oracle manipulation`, `#weather sensors`, `#Polymarket`, `#security`

---

<a id="item-9"></a>
## [Google Cloud 默认缺陷致用户产生 1.8 万美元账单](https://www.tomshardware.com/tech-industry/artificial-intelligence/google-cloud-customer-wakes-up-to-usd18-000-bill-despite-usd7-budget-thanks-to-forgotten-public-api-key-attacker-put-in-60-000-requests-and-blasted-through-usd1-400-spending-cap) ⭐️ 8.0/10

一名 Google Cloud 用户（澳大利亚 AI 顾问 Jesse Davies）尽管设置了 7 美元预算，却因攻击者利用容器环境变量中明文存储的泄露 API 密钥发起 6 万次请求并绕过消费上限，收到了 1.8 万美元的账单。 此事件凸显了 Google Cloud 默认配置中的系统性安全风险——预算上限可被静默覆盖，信用额度会自动上调，可能使众多用户面临巨额意外费用。 攻击者通过公开 URL 获取了 API 密钥，而 Google Cloud 在触发阈值时会自动上调信用额度且不通知用户，从而加剧了损失。Truffle Security 指出，Gemini API 密钥格式单一且安全设置默认关闭，导致此类攻击频发。

telegram · zaihuapd · Apr 23, 05:21

**背景**: Google Cloud 的预算提醒和上限并非硬性限制，而是可被忽略或覆盖的通知。API 密钥（尤其是以明文存储在环境变量中的密钥）若未妥善保护，极易泄露。Gemini API 密钥格式统一，使得攻击者更容易识别和利用暴露的密钥。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://docs.cloud.google.com/billing/docs/how-to/budgets">Create, edit, or delete budgets and budget alerts | Cloud Billing | Google Cloud Documentation</a></li>
<li><a href="https://trufflesecurity.com/">Truffle Security Co.</a></li>
<li><a href="https://ai.google.dev/gemini-api/docs/api-key">Using Gemini API keys | Google AI for Developers</a></li>

</ul>
</details>

**标签**: `#Google Cloud`, `#security`, `#API key`, `#cloud billing`, `#misconfiguration`

---

<a id="item-10"></a>
## [DeepSeek 开源 TileKernels 算子库，支持 NVIDIA Blackwell](https://github.com/deepseek-ai/TileKernels) ⭐️ 8.0/10

DeepSeek 开源了基于 TileLang 的高性能 GPU 算子库 TileKernels，专为大语言模型（LLM）的训练和推理进行了深度优化。该库支持 NVIDIA 最新的 SM100（Blackwell）架构，运行环境要求 CUDA 13.1 及以上版本。 此次开源为 AI 社区提供了一个接近硬件极限性能的高效 GPU 算子库，能够显著加速在最新 NVIDIA Blackwell GPU 上的 LLM 工作负载。它降低了开发者在训练和推理中实现顶级性能的门槛，尤其适用于 MoE 路由和 FP8/FP4 量化等先进技术。 TileKernels 涵盖了 MoE 路由、FP8/FP4 量化及多种融合算子，并已在 DeepSeek 内部环境投入使用。该库的设计目标是接近支持硬件的计算强度与内存带宽的理论极限。

telegram · zaihuapd · Apr 23, 09:36

**背景**: TileLang 是一种领域特定语言，旨在简化高性能 GPU 和 CPU 算子的开发。NVIDIA Blackwell 架构（SM100）是 Hopper 的继任者，拥有 2080 亿个晶体管，采用定制 TSMC 4NP 工艺制造，旨在以前所未有的性能和效率驱动 AI 工厂。MoE（混合专家）路由和 FP8/FP4 量化是现代 LLM 中用于提升模型容量和减少内存占用的关键技术。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/tile-ai/tilelang">GitHub - tile-ai/tilelang: Domain-specific language designed to streamline the development of high-performance GPU/CPU/Accelerators kernels</a></li>
<li><a href="https://en.wikipedia.org/wiki/Blackwell_(microarchitecture)">Blackwell (microarchitecture) - Wikipedia</a></li>
<li><a href="https://resources.nvidia.com/en-us-blackwell-architecture">NVIDIA Blackwell Architecture Technical Overview</a></li>

</ul>
</details>

**标签**: `#DeepSeek`, `#GPU算子库`, `#LLM`, `#NVIDIA Blackwell`, `#开源`

---

<a id="item-11"></a>
## [腾讯开源混元 Hy3 Preview 模型](https://mp.weixin.qq.com/s/5_nUI2mDchlwoedinFUMeA) ⭐️ 8.0/10

腾讯正式发布并开源混元 Hy3 preview 语言模型，这是一个总参数量达 295B、激活参数 21B 的混合专家模型（MoE），支持 256K 上下文长度。该模型已在 GitHub、HuggingFace 及腾讯云上开源，并已集成到元宝、腾讯文档、QQ 等内部产品中。 此次发布意义重大，因为它为开源社区提供了一个来自中国科技巨头、具有竞争力的大规模 MoE 模型，增强了复杂推理和智能体任务的能力。推理性能的深度优化，包括 CodeBuddy 等产品首 token 延迟降低 54%，使其在实际应用中非常实用。 Hy3 preview 模型是腾讯架构重建后的首个 MoE 模型，总参数 295B，但每次推理仅激活 21B 参数，从而实现高效计算。腾讯云还配套推出了 API 及定制化 Token Plan，个人版定价最低 28 元/月。

telegram · zaihuapd · Apr 23, 10:07

**背景**: 混合专家模型（MoE）是一种机器学习技术，它使用多个专门的子网络（专家）来处理输入的不同部分，并通过门控机制选择激活哪些专家。这使得模型可以拥有非常大的总参数量，同时保持每次推理的计算成本较低，因为只使用了部分参数。总参数（295B）与激活参数（21B）之间的差异是 MoE 模型的一个关键特征，使其能够在不成比例增加推理成本的情况下进行扩展。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Mixture_of_experts">Mixture of experts - Wikipedia</a></li>
<li><a href="https://huggingface.co/blog/moe">Mixture of Experts Explained - Hugging Face</a></li>
<li><a href="https://pandaily.com/beyond-the-model-race-how-tencent-is-building-its-global-ai-moat">Beyond the Model Race: How Tencent Is Building Its Global AI ...</a></li>

</ul>
</details>

**标签**: `#AI/ML`, `#Large Language Model`, `#Open Source`, `#MoE`, `#Tencent`

---

<a id="item-12"></a>
## [台积电因成本过高推迟高数值孔径 EUV 至 2029 年](https://money.udn.com/money/story/5599/9458925?from=edn_newestlist_rank) ⭐️ 8.0/10

台积电在北美技术论坛上宣布，至少在 2029 年前不会将 ASML 的高数值孔径 EUV 光刻机用于量产，原因是单台设备售价超过 3.5 亿欧元，成本过高。公司还披露了在亚利桑那州建立 CoWoS 和 3D-IC 封装产能的计划，目标是在 2029 年前完成。 这一战略决策表明，台积电认为现有 EUV 设备仍能为即将推出的 A13 制程提供足够性能，可能延缓整个行业向下一代光刻技术的过渡。同时，这也凸显了先进封装作为成本更低的替代方案的重要性日益提升，台积电的美国扩产计划正试图解决供应链瓶颈问题。 ASML 的高数值孔径 EUV Twinscan EXE 光刻机单台售价约 3.5 亿欧元，大规模部署成本过高。台积电亚利桑那州首座晶圆厂的良率已接近台湾工厂，第二座晶圆厂计划于明年量产。

telegram · zaihuapd · Apr 23, 11:22

**背景**: 高数值孔径 EUV 光刻是 ASML 的下一代极紫外光技术，通过使用更大数值孔径的镜头来制造更精细的芯片特征。CoWoS（晶圆上芯片封装）和 3D-IC 是先进封装技术，通过垂直堆叠多个芯片或将其集成在中间层上，在不依赖最先进光刻的情况下提升性能并降低功耗。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.ithome.com/0/752/684.htm">ASML 高数值孔径 High NA EUV 光刻机实现“初次曝光”，助英特尔开启工艺进化 - IT之家</a></li>
<li><a href="https://www.slkormicro.com/indining-china/581256.html">ASML High-NA EUV光刻机</a></li>
<li><a href="https://en.wikipedia.org/wiki/3D_IC">3D IC</a></li>

</ul>
</details>

**标签**: `#semiconductor`, `#TSMC`, `#ASML`, `#EUV lithography`, `#manufacturing`

---

<a id="item-13"></a>
## [中国三大运营商遭遇大范围国际网络故障](https://t.me/zaihuapd/41029) ⭐️ 8.0/10

中国三大电信运营商——中国电信、中国联通和中国移动——正遭遇大范围国际网络中断，通往香港、日本和美国的路由出现严重丢包和连接中断。 此次故障影响了中国最大几家运营商面向消费者的国际连接和企业级国际连接，可能对数百万用户的跨境通信、云服务和全球互联网流量造成干扰。 受影响的路由包括中国电信的 CN2 和中国联通的 9929 等高级线路，以及 163 和 4837 等标准线路；中国移动的移动数据流量通往海外方向也出现严重丢包，尤其是北京移动用户。

telegram · zaihuapd · Apr 23, 12:45

**背景**: 中国三大电信运营商各自管理着不同的国际骨干网络：中国电信使用 163 骨干网和高级 CN2（全球互联网接入）网络，中国联通运营 AS4837 骨干网和性能更高的 AS9929（CUVIP）网络，中国移动则使用 CMI 骨干网。这些网络承载着中国消费者和企业的所有跨境互联网流量。当前故障同时影响了标准线路和高级线路，表明这是一个广泛的基础设施问题，而非局部故障。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.keepnight.com/archives/1781/">cn2 gia 、cn2 gt 、163、AS9929、AS4837线路区别 - keepnight</a></li>
<li><a href="https://www.nodeseek.com/post-137012-3">有无懂哥科普线路4837、CMI、cn2、GIA、GT、cmin2、9929、cmi知识</a></li>
<li><a href="https://www.hncloud.com/news/3311.html">一文带您了解什么是AS9929线路、AS4837线路、CUVIP、CIA线路-华纳云</a></li>

</ul>
</details>

**标签**: `#network outage`, `#China telecom`, `#internet infrastructure`, `#routing issues`, `#ISP`

---

<a id="item-14"></a>
## [苹果 CEO 库克将卸任，特努斯 2026 年接棒](https://t.me/zaihuapd/41030) ⭐️ 8.0/10

苹果于 2026 年 4 月 20 日宣布，蒂姆·库克将卸任 CEO 并出任董事会执行董事长，硬件工程高级副总裁约翰·特努斯将于 2026 年 9 月 1 日起担任新任 CEO。 这是自 2011 年库克从乔布斯手中接任以来苹果首次 CEO 交接，标志着这家全球市值最高公司及其产品战略进入新时代，尤其是在苹果深入布局 AI 和硬件创新的背景下。 约翰·特努斯于 2001 年加入苹果，2021 年升任硬件工程高级副总裁，他将于 2026 年 9 月 1 日加入董事会，现任董事长亚瑟·莱文森将转任首席独立董事；库克将在整个夏季继续担任 CEO 以确保平稳过渡。

telegram · zaihuapd · Apr 23, 13:46

**背景**: 蒂姆·库克于 2011 年 8 月在史蒂夫·乔布斯因健康原因辞职后成为苹果 CEO，在他的领导下苹果的营收和市值大幅增长。执行董事长是为库克新设立的职位，使他能继续参与战略监督，而特努斯负责日常运营。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/John_Ternus">John Ternus - Wikipedia</a></li>
<li><a href="https://www.apple.com/leadership/john-ternus/">Apple Leadership - John Ternus - Apple</a></li>
<li><a href="https://www.cnbc.com/2026/04/20/apple-names-john-ternus-ceo-replacing-tim-cook-who-becomes-chairman.html">Apple taps John Ternus as CEO to replace Tim Cook, who will become chairman</a></li>

</ul>
</details>

**标签**: `#Apple`, `#leadership change`, `#CEO transition`, `#tech industry`, `#corporate news`

---

<a id="item-15"></a>
## [欧盟施压谷歌向竞争对手开放安卓 AI 助手权限](https://www.bloomberg.com/news/articles/2026-04-23/google-faces-eu-pressure-to-open-up-android-to-gemini-rivals) ⭐️ 8.0/10

欧盟正施压谷歌，要求其让 ChatGPT、Claude 等竞争对手的 AI 助手在安卓系统上获得与谷歌自家 Gemini 助手相同的系统级权限。相关要求仍处于草案阶段，发布时间可能推迟。 此举可能从根本上重塑移动 AI 助手市场的竞争格局，迫使谷歌开放安卓最底层的系统集成。如果实施，用户将有更多选择，但也将给平台带来重大的安全和隐私担忧。 欧盟的要求重点在于让竞争对手的助手获得 Gemini 目前独占的敏感系统功能和数据流访问权限。谷歌担心这种开放可能会损害安卓设备上的用户安全和隐私。

telegram · zaihuapd · Apr 23, 15:31

**背景**: 安卓是全球使用最广泛的移动操作系统，谷歌的 Gemini AI 助手拥有第三方助手所缺乏的深度系统级集成。欧盟的《数字市场法案》(DMA)此前已迫使谷歌为用户提供浏览器和搜索引擎的选择，这一新举措将同样的逻辑延伸到了 AI 助手。系统级访问包括读取屏幕内容、控制应用以及访问敏感数据流等能力，这些对于 AI 助手有效运行至关重要。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://truthonthemarket.com/2026/04/14/opening-pandoras-interface-ai-assistants-and-the-dma/">Opening Pandora’s Interface: AI Assistants and... - Truth on the Market</a></li>
<li><a href="https://developer.android.com/ai/gemini-nano">Gemini Nano | AI | Android Developers</a></li>
<li><a href="https://support.google.com/gemini/answer/16938321?hl=en">Manage or delete the Gemini app on your Android device</a></li>

</ul>
</details>

**标签**: `#EU regulation`, `#Android`, `#AI assistants`, `#Google`, `#antitrust`

---

<a id="item-16"></a>
## [MIT 搭建经典与量子物理的数学桥梁](https://www.newsy-today.com/new-study-bridges-the-worlds-of-classical-and-quantum-physics-mit-news/) ⭐️ 8.0/10

MIT 研究人员在经典 Hamilton-Jacobi 方程中引入密度计算，得到了与薛定谔方程完全一致的量子现象结果。 这一突破为量子行为提供了更简洁的数学框架，有望改进量子比特预测，并助力量子力学与广义相对论的统一。 该方法成功解释了双缝实验和量子隧穿效应，团队认为它有望增强对量子比特行为的预测。

telegram · zaihuapd · Apr 23, 16:30

**背景**: Hamilton-Jacobi 方程是经典力学的一种表述形式，与牛顿定律等价；而薛定谔方程是量子力学的核心方程。这项工作表明，通过在经典方程中加入密度项，可以精确重现量子力学结果。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://news.mit.edu/2026/new-study-bridges-classical-and-quantum-physics-0421">New study bridges the worlds of classical and quantum physics</a></li>
<li><a href="https://en.wikipedia.org/wiki/Hamilton–Jacobi_equation">Hamilton – Jacobi equation - Wikipedia</a></li>
<li><a href="https://quantumzeitgeist.com/quantum-motion-classical-calculate-using/">Researchers Calculate Quantum Motion Using Classical “Least ...</a></li>

</ul>
</details>

**标签**: `#quantum physics`, `#mathematical physics`, `#MIT research`, `#quantum computing`, `#theoretical physics`

---

<a id="item-17"></a>
## [英特尔二季度营收展望超预期，股价盘后暴涨约 20%](https://www.bloomberg.com/news/articles/2026-04-23/intel-gives-strong-outlook-in-sign-of-payoff-from-ai-spending) ⭐️ 8.0/10

英特尔公布第一季度营收 136 亿美元，调整后每股收益 0.29 美元，远超预期的 0.01 美元，并预计第二季度营收在 138 亿至 148 亿美元之间，超出市场预期。受 AI 推理需求增长和 CPU 业务复苏推动，这一强劲展望带动英特尔股价盘后大涨约 20%。 此次财报超预期以及向晶圆代工的战略转型，加上特斯拉成为其 14A 制程的关键客户，标志着英特尔可能迎来转折，并预示着半导体行业格局的重大变化。如果成功，英特尔有望在 2030 年前挑战台积电在先进芯片制造领域的领先地位。 英特尔代工业务第一季度营收为 54 亿美元，并已锁定特斯拉为其 14A 制程的首个客户。尽管第一季度净亏损扩大至 37 亿美元，但首席执行官陈立武正通过重组计划和外部合作改善资产负债表。

telegram · zaihuapd · Apr 24, 00:20

**背景**: 英特尔传统上是自行设计并制造芯片的领导者，目前正转型为晶圆代工厂——即为其他公司设计的芯片提供制造服务。这一被称为 IDM 2.0 的战略转变，旨在与台积电和三星在先进芯片制造市场竞争。14A 制程是英特尔即将推出的先进制造节点，预计将带来显著的性能和能效提升。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.eet-china.com/mp/a489739.html">马斯克：Terafab将采用英特尔14A制程-电子工程专辑</a></li>
<li><a href="https://news.mydrivers.com/1/1117/1117937.htm">马斯克：全球最大晶圆工厂定了！将采用Intel 14A工艺制造芯片</a></li>
<li><a href="https://www.trendforce.cn/industry-news/semiconductors/20260421-4545.html">英特尔代工业务势头回升 2026年设备订单量同比大增超50%-集邦咨询</a></li>

</ul>
</details>

**标签**: `#Intel`, `#semiconductors`, `#AI`, `#foundry`, `#earnings`

---

<a id="item-18"></a>
## [LiteParse PDF 文本提取在浏览器中运行](https://simonwillison.net/2026/Apr/23/liteparse-for-the-web/#atom-everything) ⭐️ 7.0/10

Simon Willison 构建了 LiteParse 的浏览器版本，LiteParse 原本是一个用于 PDF 文本提取的 Node.js CLI 工具，现在用户可以在浏览器中完全解析 PDF，无需将数据发送到任何服务器。 这使得强大的 PDF 文本提取功能对任何拥有浏览器的人可用，增强了隐私性和易用性，适合需要从 PDF 中提取文本而不依赖云服务或 AI 模型的开发者和用户。 LiteParse 使用空间文本解析启发式算法，并可选择使用 Tesseract OCR 处理基于图像的 PDF，浏览器版本利用 PDF.js 和 Tesseract.js 完全在客户端运行。

rss · Simon Willison · Apr 23, 21:54

**背景**: LiteParse 是 LlamaIndex 开发的开源 PDF 解析工具，通过启发式算法而非 AI 提取文本并保留文档布局。它最初是 Node.js CLI 工具，但 Simon Willison 通过使用在两种环境中都适用的相同底层库（PDF.js 和 Tesseract.js）将其适配到浏览器中。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/run-llama/liteparse">GitHub - run-llama/liteparse: A fast, helpful, and open-source document parser</a></li>
<li><a href="https://simonwillison.net/2026/Apr/23/liteparse-for-the-web/">Extract PDF text in your browser with LiteParse for the web</a></li>
<li><a href="https://www.llamaindex.ai/blog/liteparse-local-document-parsing-for-ai-agents">LiteParse: Local Document Parsing for AI Agents - LlamaIndex</a></li>

</ul>
</details>

**标签**: `#PDF parsing`, `#browser`, `#LiteParse`, `#spatial text parsing`, `#web development`

---

<a id="item-19"></a>
## [字节跳动发布 Seed3D 2.0，实现生产级 3D 生成](https://paipancon.com/fc2daily/detail/FC2-PPV-1700423) ⭐️ 7.0/10

字节跳动 Seed 团队于 2026 年 4 月 23 日正式发布新一代 3D 生成大模型 Seed3D 2.0，在几何精度和材质质量两项核心指标上均达到行业最佳水平（SOTA）。在纹理生成的人类评测中，该模型相对主流模型的偏好率超过 69%。 这标志着 AI 3D 内容生成向生产可用迈出了关键一步，有效解决了边缘软化、材质真实感等行业痛点。该模型兼容 NVIDIA Isaac Sim 等物理仿真引擎和 URDF 等标准格式，为机器人仿真、游戏、XR 和电子商务工作流开辟了新可能。 Seed3D 2.0 将能力扩展到部件级生成和场景组合，可先拆分 3D 内容部件再补全形状。模型输出带完整关节信息、兼容 URDF 等标准格式的内容，可直接用于物理仿真环境。

telegram · zaihuapd · Apr 23, 08:15

**背景**: 3D 生成模型旨在从图像或文本等输入创建 3D 资产，但早期模型常产生边缘模糊或材质不真实等明显缺陷，仅适用于演示。URDF（统一机器人描述格式）是一种用于描述机器人运动学、动力学和几何形状的 XML 格式，常用于 ROS 工具和 Gazebo 等模拟器。NVIDIA Isaac Sim 是一个机器人仿真平台，支持基于物理的仿真和机器人学习。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://news.aibase.com/news/27393">ByteDance Launches Seed3D 2.0: Geometry and Texture Dual SOTA ...</a></li>
<li><a href="https://seed3d2.com/">Seed3D 2.0 - AI Image to 3D Model Generator</a></li>
<li><a href="https://en.wikipedia.org/wiki/URDF">URDF - Wikipedia</a></li>

</ul>
</details>

**标签**: `#3D generation`, `#ByteDance`, `#AI`, `#computer graphics`, `#physics simulation`

---

<a id="item-20"></a>
## [香港证监会与普华永道就恒大造假达成 10 亿港元和解](https://apps.sfc.hk/edistributionWeb/gateway/TC/news-and-announcements/news/doc?refNo=26PR62) ⭐️ 7.0/10

香港证监会宣布与普华永道香港达成和解协议，普华永道同意预留 10 亿港元，用于赔偿中国恒大集团合资格独立少数股东，因恒大在 2019 及 2020 财年虚增收入 5641 亿元人民币的财务造假行为。 这是香港首次有已倒闭公司的核数师同意向受损股东作出赔偿，为香港的审计问责制和投资者保护树立了重要先例。该和解凸显了监管机构对香港资本市场审计质量和财务报告诚信的日益严格审查。 香港证监会调查认定，恒大两年内虚增收入 5641 亿元人民币，使账面盈利实为巨额亏损。普华永道在不承认法律责任的前提下达成和解，香港证监会将不再对其采取进一步行动。

telegram · zaihuapd · Apr 23, 12:07

**背景**: 中国恒大集团曾是国内最大的房地产开发商之一，于 2021 年因巨额债务崩盘。2024 年，中国监管机构因恒大财务造假（包括 2019 年和 2020 年虚增收入 5641 亿元）对其处以 41.75 亿元罚款。普华永道在此期间担任恒大的审计师，被指控严重违反专业责任，包括丧失独立性和缺乏专业怀疑态度。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://news.qq.com/rain/a/20260423A063RP00?adChannelId=news_news_top">香港证监会：因恒大虚假财务报表问题，普华永道向股东赔偿10亿港元</a></li>
<li><a href="https://www.thepaper.cn/newsDetail_forward_33037031">香港证监会、会财局同日出手 普华永道同意预留10亿港元赔偿恒大股东_...</a></li>
<li><a href="https://www.nbd.com.cn/articles/2026-04-23/4354731.html">香港证监会与普华永道就恒大股东赔偿达成协议 赔偿达10亿港元</a></li>

</ul>
</details>

**标签**: `#financial regulation`, `#auditing`, `#corporate fraud`, `#Hong Kong`, `#investor protection`

---

<a id="item-21"></a>
## [英国 NCSC 正式将通行密钥列为首选身份验证方式](https://www.techradar.com/pro/security/uk-security-agency-officially-declares-passkeys-superior-to-passwords-passkeys-should-be-the-first-choice-for-authentication) ⭐️ 7.0/10

英国国家网络安全中心（NCSC）正式宣布通行密钥（Passkeys）优于传统密码和两步验证，并建议将其作为数字服务的首选登录方式。这标志着 NCSC 结束了此前的观望态度，因为过去 12 个月内的行业技术进步已解决了核心实施难题。 这一来自主要政府网络安全机构的官方认可标志着身份验证指导方针的重大转变，可能加速通行密钥在全球各行业的普及。它直接影响组织和个人对待在线安全的方式，减少对密码的依赖，并提升对钓鱼攻击和凭证窃取的防护能力。 英国超过 50%的 Google 活跃用户已注册使用通行密钥，eBay 和 PayPal 等主流平台也已完全适配。通行密钥采用非对称加密技术，使用存储在设备上的公钥-私钥对进行身份验证，并通过生物识别（如 Face ID、Touch ID）或设备 PIN 码验证，消除了用户记忆复杂密码的需要。

telegram · zaihuapd · Apr 23, 14:47

**背景**: 通行密钥是一种基于公钥加密的无密码身份验证方法，私钥存储在用户设备上，公钥存储在服务器上。与密码不同，通行密钥能够抵御钓鱼攻击、凭证填充等常见攻击，因为私钥永远不会离开设备，且仅通过生物识别或 PIN 码验证解锁。NCSC 是英国网络安全领域的最高权威机构，负责为保护公民和组织免受网络威胁提供指导。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://developers.google.com/identity/passkeys?hl=zh-cn">通 行 密 钥 | Passkeys | Google for Developers</a></li>
<li><a href="https://www.corbado.com/zh/faq/passkeys-通行密钥">通 行 密 钥 （ Passkeys ）是什么？ 免 密 码登录与生物识别的安全指南</a></li>
<li><a href="https://blog.csdn.net/shaoshaoh/article/details/139117916">通 行 秘 钥 Passkeys 从入门到实现-CSDN博客</a></li>

</ul>
</details>

**标签**: `#cybersecurity`, `#authentication`, `#passkeys`, `#NCSC`, `#identity`

---

<a id="item-22"></a>
## [英国生物样本库数据遭非法售卖，官方紧急收紧访问权限](https://www.ukbiobank.ac.uk/news/a-message-to-our-participants-uk-biobank-data-security-update/) ⭐️ 7.0/10

来自三家学术机构的研究人员违反合同协议，将脱敏后的英国生物样本库（UK Biobank）参与者数据在阿里巴巴旗下的电商平台挂牌出售。为此，UK Biobank 已暂停所有研究平台的访问权限，计划实施严格的文件导出限制与每日监控机制，并正在开发全球首个自动化云端数据泄露预防系统，预计于 2026 年底前上线。 此事件凸显了研究数据治理中的关键漏洞以及跨境数据传输风险，尤其是涉及 50 万名参与者的敏感健康与基因数据。此次违规可能削弱公众对生物医学研究的信任，并为全球大型生物样本库的数据安全标准树立更严格的先例。 涉事挂牌信息已在交易发生前被移除，相关机构及个人的访问权限已被永久吊销。新的自动化系统将检测并防止脱敏数据被带离云端研究平台，从而应对即使脱敏后仍存在的重识别风险。

telegram · zaihuapd · Apr 24, 00:58

**背景**: 英国生物样本库（UK Biobank）是英国一项长期前瞻性生物样本库研究，存储了 50 万名参与者的脱敏生物样本和健康相关数据，是全球最大、使用最广泛的遗传流行病学数据集之一。脱敏处理移除了直接标识符，但并未消除重识别风险，尤其是在数据与其他来源结合时。数据丢失预防（DLP）软件可检测并阻止敏感数据的未授权传输，随着研究平台迁移至云端，基于云的 DLP 解决方案正日益普及。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/UK_Biobank">UK Biobank - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Data_loss_prevention_software">Data loss prevention software - Wikipedia</a></li>
<li><a href="https://www.iri.com/support/data-education-center/what-is-re-identification-risk">What is Re-Identification Risk? | Data Education Center - IRI</a></li>

</ul>
</details>

**标签**: `#data security`, `#biobank`, `#research ethics`, `#data governance`, `#health data`

---