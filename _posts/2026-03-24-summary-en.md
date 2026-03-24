---
layout: default
title: "Horizon Summary: 2026-03-24 (EN)"
date: 2026-03-24
lang: en
---

> From 24 items, 4 important content pieces were selected

---

1. [iPhone 17 Pro Demonstrated Running a 400B Parameter LLM](#item-1) ⭐️ 8.0/10
2. [Autoresearch: An LLM-powered system for automated code improvement and experimentation](#item-2) ⭐️ 7.0/10
3. [Tech Companies Tie Performance Reviews to Employee LLM Token Consumption](#item-3) ⭐️ 7.0/10
4. [OpenAI urges UK to include AI chatbots in Google search choice screen](#item-4) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [iPhone 17 Pro Demonstrated Running a 400B Parameter LLM](https://twitter.com/anemll/status/2035901335984611412) ⭐️ 8.0/10

A demonstration showed a 400 billion parameter large language model running on an iPhone 17 Pro. The community discussion clarified that the model uses a Mixture of Experts (MoE) architecture and involves quantization techniques to achieve this. This demonstration represents significant progress in on-device AI, pushing the boundaries of what's possible on mobile hardware. It signals a future where powerful AI assistants can operate entirely locally, enhancing privacy, reducing latency, and enabling new applications without constant cloud connectivity. The model is a Mixture of Experts (MoE) model, meaning its 400B parameter count is sparse; only a fraction of parameters are active per inference, making it more efficient. The demonstration also relies on quantization, a compression technique that reduces the numerical precision of model weights to shrink its memory footprint and computational requirements.

hackernews · anemll · Mar 23, 14:30

**Background**: Large Language Models (LLMs) are AI systems trained on vast amounts of text data, with their capability often scaling with the number of parameters. Running such models on mobile devices is challenging due to limited memory and processing power. The Mixture of Experts (MoE) architecture is a design where a model consists of many sub-networks ('experts'), and a routing network selects only a few relevant experts for each input, allowing for a large total parameter count with manageable computational cost per token. Quantization is a technique to compress neural networks by representing their weights with fewer bits (e.g., 4-bit integers instead of 16-bit floating-point numbers), significantly reducing model size and speeding up inference, often with minimal accuracy loss.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/abs/2507.11181">[2507.11181] Mixture of Experts in Large Language Models</a></li>
<li><a href="https://huggingface.co/blog/moe">Mixture of Experts Explained - Hugging Face</a></li>
<li><a href="https://blog.premai.io/llm-quantization-guide-gguf-vs-awq-vs-gptq-vs-bitsandbytes-compared-2026/">LLM Quantization Guide: GGUF vs AWQ vs GPTQ vs bitsandbytes ...</a></li>

</ul>
</details>

**Discussion**: Community sentiment was mixed, combining technical scrutiny with broader concerns. Technically, commenters pointed out that the headline is misleading without mentioning the MoE architecture and quantization, which are crucial for making the 400B model runnable on a phone; one user noted that such a model may behave more like a much smaller dense model. Other comments raised concerns about device overheating during sustained inference and broader societal impacts, such as increased phone addiction.

**Tags**: `#on-device-ai`, `#llm`, `#mobile-computing`, `#quantization`, `#apple`

---

<a id="item-2"></a>
## [Autoresearch: An LLM-powered system for automated code improvement and experimentation](https://ykumar.me/blog/eclip-autoresearch/) ⭐️ 7.0/10

A blog post detailed an automated research system that uses Large Language Models (LLMs) to iteratively improve code, run experiments, and evaluate results in a loop. The core of the system is a single system prompt (program.md) that instructs the agent to repeatedly improve a training script, execute training, run evaluations, and record outcomes. This demonstrates a practical application of LLM agents to automate and accelerate the research and development cycle, particularly in machine learning. It could significantly reduce the manual effort required for tasks like code refinement and hyperparameter exploration, potentially leading to faster discovery of optimal solutions. The system is described as acting like a hyperparameter optimization algorithm with basic reasoning baked in, favoring simplicity in its iterative loop. A key insight from the community is that using different LLM models across iterations can be beneficial, akin to getting a fresh perspective on the problem.

hackernews · ykumards · Mar 23, 18:40

**Background**: LLM agents are AI systems that use large language models as a core reasoning engine to plan and execute sequences of actions towards a goal, such as conducting research or writing code. Automated research frameworks aim to span major research phases like ideation, experimentation, and analysis. Hyperparameter optimization is the process of finding the best set of configuration parameters for a machine learning model, which is often a manual and time-consuming task.

<details><summary>References</summary>
<ul>
<li><a href="https://agentlaboratory.github.io/">Agent Laboratory: Using LLMs as Research Assistants</a></li>
<li><a href="https://deepwiki.com/karpathy/autoresearch">karpathy/autoresearch | DeepWiki</a></li>
<li><a href="https://arxiv.org/html/2312.04528v2">Using Large Language Models for Hyperparameter Optimization</a></li>

</ul>
</details>

**Discussion**: Community discussion highlights practical applications and raises questions about efficiency. Some users compare the system to established hyperparameter optimization techniques and question its novelty, while others share their own experiences using LLMs for prior art exploration or iterative code debugging. A recurring theme is the balance between the potential of automated exploration and the costs (computational and financial) associated with letting an agent try all LLM-suggested ideas.

**Tags**: `#LLM-agents`, `#automated-research`, `#machine-learning`, `#code-generation`, `#hyperparameter-optimization`

---

<a id="item-3"></a>
## [Tech Companies Tie Performance Reviews to Employee LLM Token Consumption](https://gizmodo.com/tech-employees-are-reportedly-being-evaluated-by-how-fast-they-burn-through-llm-tokens-2000736627) ⭐️ 7.0/10

According to a New York Times column, tech companies like Meta and OpenAI are reportedly creating internal leaderboards to compare employee usage of LLM tokens, with Meta and Shopify explicitly tying AI usage metrics to performance reviews. The report also states that one OpenAI engineer has consumed 210 billion tokens, and OpenAI President Greg Brockman noted that GPT-5.4 processed 5 trillion tokens daily just one week after launch. This practice represents a significant shift in workplace performance metrics, directly linking AI tool adoption to individual evaluation, which could accelerate enterprise AI integration but also risks promoting wasteful usage over meaningful productivity. It reflects the growing pressure on tech companies to demonstrate and quantify return on investment in AI, potentially setting a new industry standard for measuring employee contribution in the AI era. The reported metrics focus on raw token consumption volume, which is a measure of input/output size for LLMs but not necessarily of output quality or task efficiency. The scale mentioned is immense, with individual engineers consuming hundreds of billions of tokens and flagship models like GPT-5.4 handling trillions daily, highlighting the massive computational resources involved in modern AI workflows.

telegram · zaihuapd · Mar 23, 08:42

**Background**: Large Language Models (LLMs) like GPT-4, LLaMA, or Gemini process text by breaking it down into tokens, which are numerical representations of words or word parts. The number of tokens a model processes directly correlates with computational cost and is a fundamental unit for billing in AI API services (e.g., OpenAI's API). A context window defines the maximum number of tokens a model can consider at once, influencing its ability to handle long documents or conversations. Companies track token usage to manage costs and understand adoption, but using it as a performance metric is a novel and controversial application.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Large_language_model">Large language model - Wikipedia</a></li>
<li><a href="https://winder.ai/calculating-token-counts-llm-context-windows-practical-guide/">Calculating LLM Token Counts: A Practical Guide</a></li>
<li><a href="https://hackernoon.com/whos-used-one-trillion-plus-openai-tokens-salesforce-shopify-canva-hubspot-and-26-more-companies">Who's Used One Trillion Plus OpenAI Tokens? Salesforce ...</a></li>

</ul>
</details>

**Tags**: `#AI Adoption`, `#Workplace Culture`, `#Performance Metrics`, `#LLM Usage`, `#Tech Industry`

---

<a id="item-4"></a>
## [OpenAI urges UK to include AI chatbots in Google search choice screen](https://assets.publishing.service.gov.uk/media/69b970dcc06ba9576435ab5a/OpenAI.pdf) ⭐️ 7.0/10

On March 6, OpenAI formally submitted a recommendation to the UK's Competition and Markets Authority (CMA) that the eligibility criteria for Google's search choice screen should explicitly include AI chatbots with search capabilities. This would allow services like ChatGPT to be selectable as the default search service on Android devices and Chrome browsers. This move is a strategic attempt by OpenAI to secure prominent placement and user access for its conversational AI products within the heavily regulated digital market of the UK. If adopted, it could significantly reshape search competition by giving AI-first services equal footing with traditional search engines on major platforms, potentially accelerating the shift towards AI-powered information retrieval. OpenAI argues that services like ChatGPT, which perform information discovery through conversational or multimodal interfaces, are functionally similar to Google's own AI Overviews and AI Mode features. It also recommends using a transparent, dynamic popularity metric to determine which services appear on the choice screen and expanding the screen's reach to include voice, visual, and AI-assisted search entry points.

telegram · zaihuapd · Mar 23, 14:50

**Background**: The UK's Competition and Markets Authority (CMA) has designated Google as having Strategic Market Status (SMS) in general search services, granting the regulator powers to impose pro-competitive rules. A key remedy under consideration is a 'search choice screen' that would prompt users on Android and Chrome to select a default search engine from a list of options. Currently, this list is limited to traditional 'general search services,' and the CMA is consulting on whether to include newer, generative AI-powered search tools. Google has integrated AI directly into its search results with features like AI Overviews (summaries) and an experimental AI Mode for complex queries.

<details><summary>References</summary>
<ul>
<li><a href="https://assets.publishing.service.gov.uk/media/68c29c52d65a1a2a5172a9ab/_Summary_of_choice_architecture_roundtable.pdf">Summary of choice architecture roundtable - GOV.UK</a></li>
<li><a href="https://www.gov.uk/cma-cases/googles-general-search-and-search-advertising-services">Google's general search and search advertising services</a></li>
<li><a href="https://en.wikipedia.org/wiki/AI_Overviews">AI Overviews - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#AI Regulation`, `#Search Competition`, `#OpenAI`, `#UK CMA`, `#Market Access`

---