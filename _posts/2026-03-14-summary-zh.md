---
layout: default
title: "Horizon Summary: 2026-03-14 (ZH)"
date: 2026-03-14
lang: zh
---

> From 19 items, 4 important content pieces were selected

---

1. [Anthropic 为 Claude Opus 和 Sonnet 4.6 全面开放 100 万上下文窗口，并取消长上下文溢价。](#item-1) ⭐️ 8.0/10
2. [Anthropic 发布 Claude Opus 4.6，支持 200K 上下文窗口和自适应思考模式。](#item-2) ⭐️ 8.0/10
3. [Instagram 将取消私信的端到端加密功能](#item-3) ⭐️ 8.0/10
4. [马斯克承认 xAI 架构失误拟推倒重构，12 名联合创始人仅剩 3 人](#item-4) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [Anthropic 为 Claude Opus 和 Sonnet 4.6 全面开放 100 万上下文窗口，并取消长上下文溢价。](https://claude.com/blog/1m-context-ga) ⭐️ 8.0/10

Anthropic 宣布为其 Claude Opus 4.6 和 Sonnet 4.6 模型全面开放 100 万 token 的上下文窗口。关键变化在于，标准定价现在适用于整个 100 万窗口，取消了之前的长上下文溢价，并且媒体处理限制已扩展至 600 张图像或 PDF 页面。 此举大幅降低了处理长文档、代码库或多步骤推理任务的开发者和企业的成本，使先进 AI 技术更易获得。这也给 OpenAI 和 Google Gemini 等仍对扩展上下文收费的竞争对手带来压力，可能重塑 AI 工具开发的经济格局。 取消溢价意味着一个 90 万 token 的请求现在与一个 9 千 token 的请求按相同的单价计费。社区提出的一个实际关切是，模型在超过 20 万 token 后是否仍能保持强大的连贯性，这对于分析整个代码库等任务至关重要。

hackernews · meetpateltech · Mar 13, 17:19

**背景**: 上下文窗口是指大语言模型（LLM）单次请求能够处理和记忆的 token（词块）数量。Claude Opus 4.6 是 Anthropic 能力最强但最昂贵的模型，而 Sonnet 4.6 则在速度和智能之间提供了更具成本效益的平衡。此前，包括 Anthropic 在测试阶段在内的许多 LLM 提供商，会对使用大上下文窗口的扩展部分收取溢价，这使得长上下文工作的成本很高。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://awesomeagents.ai/news/anthropic-1m-context-ga-opus-sonnet/">Claude's 1M Context Window Now GA - No Premium Pricing | Awesome Agents</a></li>
<li><a href="https://balajiraj.medium.com/claude-sonnet-4s-one-million-token-context-window-what-it-means-and-how-it-works-1003ef649de3">Claude Sonnet 4’s One-Million Token Context Window ... | Medium</a></li>
<li><a href="https://www.tensorlake.ai/blog-posts/claude-opus-4-6-vs-claude-sonnet-4-6">Claude Opus 4.6 vs. Claude Sonnet 4.6 - tensorlake.ai</a></li>

</ul>
</details>

**社区讨论**: 社区反应总体积极，用户们为取消令人头疼的“压缩”成本而欢呼，并强调了这对 Claude Code 用户的影响。讨论集中在实际影响上，例如订阅用户超过 20 万 token 是否仍需额外付费，以及与竞争对手定价模式的比较。一些用户也对将 Claude 重新作为长会话的主要工具表示兴奋。

**标签**: `#llm`, `#claude`, `#context-window`, `#pricing`, `#ai-tools`

---

<a id="item-2"></a>
## [Anthropic 发布 Claude Opus 4.6，支持 200K 上下文窗口和自适应思考模式。](https://t.me/zaihuapd/40251) ⭐️ 8.0/10

Anthropic 发布了新一代 Claude Opus 4.6 模型，该模型支持 200K token 的上下文窗口（测试版提供 100 万 token），并将最大输出 token 数提升至 128K，较前代翻倍。该模型引入了自适应思考模式，可根据问题复杂度动态调整思考深度，并新增了上下文压缩功能，当对话接近窗口限制时自动总结早期内容，从而实现近乎无限长度的对话。 此次发布标志着 AI 模型能力的一次重大飞跃，扩展的上下文窗口和输出长度使其能够处理更长、更复杂的文档和对话。自适应思考和上下文压缩功能是使 AI 交互更高效、更具成本效益、且无需人工干预即可处理现实世界长期任务的关键步骤。 自适应思考模式由提供商管理，当未明确设置思考级别时默认启用，允许模型根据请求的复杂性自行决定推理预算。100 万 token 的上下文窗口目前处于测试阶段，这表明该功能正在测试中，大多数用户的标准支持上限仍是 200K token。

telegram · zaihuapd · Mar 14, 01:19

**背景**: 大型语言模型（LLM）中的上下文窗口类似于其短期记忆，定义了它能在单个提示中处理的 token（文本片段）的最大数量。自适应思考是一种技术，模型根据感知到的任务难度自行决定何时以及进行多少扩展的内部推理，而不是采用固定的、用户指定的预算。上下文压缩指的是通过总结或有选择地保留信息来减少长对话或文档的 token 使用量或内存占用的技术，以克服模型固有的限制。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.mckinsey.com/featured-insights/mckinsey-explainers/what-is-a-context-window">What is a context window for Large Language Models? | McKinsey</a></li>
<li><a href="https://platform.claude.com/docs/en/build-with-claude/adaptive-thinking">Adaptive thinking - Claude API Docs</a></li>
<li><a href="https://agenta.ai/blog/top-6-techniques-to-manage-context-length-in-llms">Top techniques to Manage Context Lengths in LLMs - agenta.ai</a></li>

</ul>
</details>

**标签**: `#AI`, `#LLM`, `#Anthropic`, `#Claude`, `#Natural Language Processing`

---

<a id="item-3"></a>
## [Instagram 将取消私信的端到端加密功能](https://www.theverge.com/tech/894752/instagram-end-to-end-encryption) ⭐️ 8.0/10

Instagram 已更新其支持页面，确认其私信的端到端加密功能将在 2026 年 5 月 8 日后停止支持。Meta 表示做出此调整是因为 Instagram 私信端到端加密的实际使用人数“非常少”，并建议用户转向 WhatsApp 进行加密通信。 这一决定标志着 Meta 在隐私和安全策略上的重大转变，可能影响数十亿 Instagram 用户，降低了其私人对话的默认隐私级别。这表明 Meta 正将加密通信的努力整合到 WhatsApp 上，这可能影响用户在数据保护方面的平台选择和信任。 被移除的具体功能是 Instagram 私信中可选的端到端加密，而非整个消息服务。Meta 明确表示，寻求加密聊天的用户应使用 WhatsApp，后者多年来一直默认启用端到端加密，这凸显了其产品组合内的战略差异化。

telegram · zaihuapd · Mar 14, 04:47

**背景**: 端到端加密是一种安全方法，只有通信双方可以读取消息，防止包括服务提供商（如 Meta）在内的第三方获取解密对话所需的加密密钥。与默认启用端到端加密的 WhatsApp 不同，Instagram 的私信端到端加密是一个可选功能，而 Facebook Messenger 仅在“私密对话”模式下启用它。此举符合 Meta 在其不同消息应用间区分安全模式的历史模式。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://zh.wikipedia.org/wiki/端到端加密">端到端加密 - 维基百科，自由的百科全书</a></li>
<li><a href="https://www.sohu.com/a/291886178_413981">Facebook 打算让 WhatsApp 和 Instagram 消息互通，还要用上点对点加密_用户</a></li>

</ul>
</details>

**标签**: `#privacy`, `#encryption`, `#social-media`, `#meta`, `#security`

---

<a id="item-4"></a>
## [马斯克承认 xAI 架构失误拟推倒重构，12 名联合创始人仅剩 3 人](https://futurism.com/artificial-intelligence/elon-musk-screwed-up-xai-rebuilding) ⭐️ 7.0/10

埃隆·马斯克于 3 月 13 日表示，其人工智能初创公司 xAI 正在从底层进行重构，并承认该公司最初的构建方式并不正确。目前，xAI 的 12 名联合创始人中已有 9 人离职，仅剩 3 人留任，其中包括近期宣布离职的图像生成产品负责人张国栋。 这标志着由埃隆·马斯克支持的一家高调 AI 初创公司正面临重大的技术和组织动荡，可能延误其产品路线图并影响其竞争力。联合创始人的大规模流失，加上彻底的架构重建，引发了外界对公司战略方向和执行能力的严重质疑。 为应对人才流失，马斯克正与人才主管 Baris Akis 重新联系此前被拒绝的候选人，并从 AI 编程初创公司 Cursor 聘请了两名资深员工。此外，特斯拉已获准将其对 xAI 的投资转换为 SpaceX 的少量股权，而 SpaceX 预计将于今年晚些时候以约 1.25 万亿美元的估值上市。

telegram · zaihuapd · Mar 14, 02:21

**背景**: xAI 是埃隆·马斯克于 2023 年创立的人工智能公司，旨在构建“寻求真理”和具有最大好奇心的 AI 系统。该公司以其 Grok 大语言模型而闻名，该模型的架构和权重已于 2024 年 3 月开源。文中提及作为新员工来源的 Cursor，是一个 AI 辅助的集成开发环境（IDE），它是 Visual Studio Code 的一个分支，近期有报道称其估值正接近 500 亿美元。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://siliconangle.com/2024/03/17/elon-musks-xai-releases-grok-1-architecture-apple-advances-multimodal-ai-research/">Elon Musk's xAI releases Grok-1 architecture, while Apple advances multimodal AI research</a></li>
<li><a href="https://en.wikipedia.org/wiki/Cursor_(code_editor)">Cursor (code editor) - Wikipedia</a></li>
<li><a href="https://startupwired.com/2026/03/12/ai-coding-startup-cursor-nears-50b-valuation-in-new-funding/">AI Coding Startup Cursor Nears $50B Valuation in New Funding</a></li>

</ul>
</details>

**标签**: `#artificial-intelligence`, `#startups`, `#organizational-change`, `#elon-musk`, `#talent-acquisition`

---