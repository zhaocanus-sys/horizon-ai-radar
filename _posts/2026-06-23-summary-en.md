---
layout: default
title: "Horizon Summary: 2026-06-23 (EN)"
date: 2026-06-23
lang: en
---

> From 34 items, 25 important content pieces were selected

---

1. [Valve Launches Steam Machine with Randomized Reservation System](#item-1) ⭐️ 9.0/10
2. [3B Model VibeThinker Beats Opus 4.5 on Reasoning](#item-2) ⭐️ 8.0/10
3. [In Praise of Memcached: Simplicity Over Redis Bloat](#item-3) ⭐️ 8.0/10
4. [OpenAI Releases GPT-5.5-Cyber Amid Access Controversy](#item-4) ⭐️ 8.0/10
5. [Prompt Injection as Role Confusion](#item-5) ⭐️ 8.0/10
6. [Porting Moebius 0.2B Inpainting Model to Browser with WebGPU](#item-6) ⭐️ 8.0/10
7. [browser-search: Free open-source tools for AI web browsing](#item-7) ⭐️ 8.0/10
8. [Prior Context Alters LLM Responses via Hidden States](#item-8) ⭐️ 8.0/10
9. [HTTP QUERY Method Proposed for Read Requests with Body](#item-9) ⭐️ 7.0/10
10. [Crypto in 2026: Scams, Fraud, and Stablecoin Utility](#item-10) ⭐️ 7.0/10
11. [GLM-5.2 Local Inference Guide with Quantized MoE](#item-11) ⭐️ 7.0/10
12. [Oak: A Git Alternative Built for AI Agents](#item-12) ⭐️ 7.0/10
13. [Canada plans nuclear renaissance with up to 10 reactors by 2040](#item-13) ⭐️ 7.0/10
14. [sqlite-utils 4.0rc1 adds migrations and nested transactions](#item-14) ⭐️ 7.0/10
15. [Cloudflare Launches Temporary Accounts for Workers](#item-15) ⭐️ 7.0/10
16. [Google Invests $75M in A24 for AI Filmmaking Tools](#item-16) ⭐️ 7.0/10
17. [Canada secretly spent millions on Palantir AI surveillance](#item-17) ⭐️ 7.0/10
18. [AI Cost Paradox: Spending More Despite Automation](#item-18) ⭐️ 7.0/10
19. [Investment Lawyer Explains AI Deepfake Scams](#item-19) ⭐️ 7.0/10
20. [Developer Spends Month Optimizing AI Agent Without Defining Goals](#item-20) ⭐️ 7.0/10
21. [Claude Code v2.1.186: MCP Auth CLI and Bug Fixes](#item-21) ⭐️ 6.0/10
22. [Blog Post Compares AI Models, Community Debates](#item-22) ⭐️ 6.0/10
23. [Autodesk invests $350M in AI workforce training](#item-23) ⭐️ 6.0/10
24. [Are AI Benchmarks Valid for Passive Users?](#item-24) ⭐️ 6.0/10
25. [Kimi K2.6 vs Claude: Which Coding Agent Is Better?](#item-25) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [Valve Launches Steam Machine with Randomized Reservation System](https://store.steampowered.com/news/group/45479024/view/685257114654870245) ⭐️ 9.0/10

Valve launched the Steam Machine on June 29, 2026, a new gaming PC priced at $1,049, with a randomized reservation system to combat bots and scalpers. The sign-up window runs until June 25, after which a one-time randomization determines the order of reservations. This launch represents a paradigm shift in PC gaming hardware, emphasizing openness and user freedom by allowing users to install any apps or operating systems. The randomized reservation system could set a new standard for fair product launches in the gaming industry. The Steam Machine is optimized for gaming but remains an open PC, with Valve stating users can install other operating systems. Accounts must have made at least one purchase on Steam before April 27, 2026, and be in good standing to reserve one unit per account.

hackernews · theschwa · Jun 22, 17:09 · [Discussion](https://news.ycombinator.com/item?id=48632884)

**Background**: Valve previously attempted a Steam Machine initiative in 2015 with third-party hardware, which failed to gain traction. The new Steam Machine is a first-party device, similar to the Steam Deck, designed to bring PC gaming to the living room with a console-like experience while maintaining PC openness.

<details><summary>References</summary>
<ul>
<li><a href="https://www.pcgamer.com/hardware/gaming-pcs/steam-machine-reservations/">Sign up for a Steam Machine before June 25: Valve running one-time randomized queue due to limited availability and to 'limit resellers' | PC Gamer</a></li>
<li><a href="https://arstechnica.com/gaming/2026/06/valves-steam-machine-ships-june-29-for-1049-but-you-probably-wont-be-able-to-buy-one-yet/">Valve's Steam Machine ships June 29 for $1,049, but you probably won't be able to buy one yet - Ars Technica</a></li>
<li><a href="https://www.theverge.com/games/952191/valve-steam-machine-reservation-preorder-process">Here’s how you can reserve a Steam Machine | The Verge</a></li>

</ul>
</details>

**Discussion**: Community comments are largely positive, with users praising the randomized reservation system as fair and the open nature of the hardware. Some users note the high price and express curiosity about specs, while others appreciate Valve's anti-scalper measures and the authentic marketing video.

**Tags**: `#gaming`, `#hardware`, `#valve`, `#steam`, `#pc`

---

<a id="item-2"></a>
## [3B Model VibeThinker Beats Opus 4.5 on Reasoning](https://arxiv.org/abs/2606.16140) ⭐️ 8.0/10

VibeThinker, a 3.1-billion-parameter model fine-tuned from Qwen2.5-Coder-3B using a combination of supervised fine-tuning (SFT) and group relative policy optimization (GRPO), achieves state-of-the-art reasoning scores of 94.3 on AIME 2026 and 80.2 on LiveCodeBench, outperforming much larger models like Opus 4.5. This demonstrates that efficient training techniques can overcome raw parameter count, potentially democratizing access to high-performance reasoning models and challenging the notion that only massive models can achieve frontier results. The model is released under an MIT license, fits in about 6.7 GB of VRAM, and runs on a single consumer GPU. However, its strong results are currently limited to Python programming tasks, and performance on other languages may be lower.

hackernews · timhigins · Jun 23, 02:01 · [Discussion](https://news.ycombinator.com/item?id=48639240)

**Background**: Supervised fine-tuning (SFT) adapts a pre-trained model to a specific task using labeled data, while group relative policy optimization (GRPO) is a reinforcement learning technique that improves reasoning without a separate critic model. VibeThinker combines both in a post-training paradigm called Spectrum-to-Signal, which also includes multi-domain RL and self-distillation.

<details><summary>References</summary>
<ul>
<li><a href="https://www.datacamp.com/blog/what-is-grpo-group-relative-policy-optimization">What is GRPO? Group Relative Policy Optimization Explained</a></li>
<li><a href="https://theplanettools.ai/blog/weibo-vibethinker-3b-open-weight-reasoning-benchmark-controversy-2026">VibeThinker-3B: A 3B Model vs the Benchmark Debate (2026)</a></li>
<li><a href="https://explainx.ai/blog/vibethinker-3b-small-model-frontier-reasoning-2026">VibeThinker-3B: Frontier Reasoning at 3B Parameters (2026 ...</a></li>

</ul>
</details>

**Discussion**: The community is excited about the small model's breakthrough but debates benchmark validity and practical applicability. Some question whether the benchmarks truly capture real-world developer workflows, while others note the Python-only limitation and suggest more domain-focused small language models are needed.

**Tags**: `#AI`, `#machine learning`, `#reasoning`, `#small models`, `#benchmarks`

---

<a id="item-3"></a>
## [In Praise of Memcached: Simplicity Over Redis Bloat](https://jchri.st/blog/in-praise-of-memcached/) ⭐️ 8.0/10

A blog post argues that memcached's simplicity and reliability make it a better choice for pure caching than Redis, which has grown feature-heavy and caused production failures. The article cites community experiences with Redis and Valkey outages due to memory policy issues and AOF write failures. This discussion highlights a growing tension in the caching ecosystem between feature-rich tools like Redis and focused, minimalistic ones like memcached. It matters for engineers designing systems that need predictable performance and minimal operational risk. Memcached guarantees O(1) time complexity for all operations, avoiding unpredictable stalls that can occur with Redis's single-threaded model when complex commands are executed. Redis's persistence (AOF) and memory policy misconfigurations have caused production outages, as noted in community comments.

hackernews · j03b · Jun 23, 01:15 · [Discussion](https://news.ycombinator.com/item?id=48638886)

**Background**: Memcached is a high-performance, distributed memory caching system designed for simplicity and speed, storing data only as key-value pairs. Redis, originally a cache, has evolved into a multi-model database with persistence, complex data structures, and scripting, which can introduce operational complexity. Valkey is a fork of Redis created after Redis changed its license, aiming to keep the project open source.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/valkey-io/valkey">GitHub - valkey-io/valkey: A flexible distributed key-value ...</a></li>
<li><a href="https://scalegrid.io/blog/redis-vs-memcached/">Redis Vs Memcached In 2025 - ScaleGrid</a></li>
<li><a href="https://redis.io/compare/memcached/">Memcached vs Redis: fast caching for devs</a></li>

</ul>
</details>

**Discussion**: Commenters share real-world production failures with Redis and Valkey, including memory exhaustion and AOF write errors, and note that memcached's O(1) guarantees prevent such stalls. Some advocate using memcached for caching and Redis only when persistent data structures are needed.

**Tags**: `#memcached`, `#Redis`, `#caching`, `#software engineering`, `#system design`

---

<a id="item-4"></a>
## [OpenAI Releases GPT-5.5-Cyber Amid Access Controversy](https://openai.com/index/daybreak-securing-the-world/) ⭐️ 8.0/10

OpenAI has released GPT-5.5-Cyber, a security-focused AI model, but is restricting access to a handpicked group of 'cyber defenders' while criticizing Anthropic for similar restrictions on its Mythos model. This release intensifies the debate over unequal access to advanced AI models and potential government favoritism, as OpenAI's model appears to face fewer restrictions than Anthropic's, despite both being highly capable cybersecurity tools. GPT-5.5-Cyber is reported to be on par with or slightly outperform Anthropic's Mythos 5 in cybersecurity benchmarks, yet it remains locked behind a velvet rope for approved users only, similar to the restrictions OpenAI previously criticized.

hackernews · AaronO · Jun 23, 01:36 · [Discussion](https://news.ycombinator.com/item?id=48639063)

**Background**: In June 2026, the U.S. Department of Commerce imposed export controls on Anthropic's latest models (Fable 5 and Mythos 5), forcing Anthropic to abruptly disable them for all users. OpenAI's GPT-5.5-Cyber, released shortly after, has not faced similar government restrictions, leading to accusations of favoritism given OpenAI's political connections.

<details><summary>References</summary>
<ul>
<li><a href="https://www.reddit.com/r/singularity/comments/1ucvx1g/an_updated_gpt55_cyber_outperforms_mythos_5_in/">an updated GPT-5.5 Cyber outperforms Mythos 5 in CyberGym : r/singularity - Reddit</a></li>
<li><a href="https://forums.theregister.com/forum/all/2026/05/01/openai_locks_gpt55cyber_behind_velvet/">OpenAI locks GPT-5.5-Cyber behind velvet rope despite slamming Anthropic for doing exactly that - The Register Forums</a></li>
<li><a href="https://www.csis.org/analysis/department-commerce-restricted-access-anthropics-latest-models-what-comes-next">The Department of Commerce Restricted Access to Anthropic’s ...</a></li>

</ul>
</details>

**Discussion**: Community comments express frustration over unequal access, with users noting that paying customers cannot use the best models for security audits. Some question whether OpenAI's political ties influenced the lack of restrictions, while others recommend trying the model themselves to evaluate its capabilities.

**Tags**: `#AI`, `#security`, `#OpenAI`, `#regulation`, `#GPT-5.5-Cyber`

---

<a id="item-5"></a>
## [Prompt Injection as Role Confusion](https://simonwillison.net/2026/Jun/22/prompt-injection-as-role-confusion/#atom-everything) ⭐️ 8.0/10

Research by Charles Ye, Jasmine Cui, and Dylan Hadfield-Menell reveals that large language models (LLMs) cannot reliably distinguish privileged text (e.g., system instructions) from user input based on role tags, and instead prioritize the style of the text over its content. This leads to effective jailbreaks, such as appending text that mimics the model's internal thinking style to bypass safety filters. This research confirms fundamental limitations of role-based defenses against prompt injection, a critical security issue for LLM-based applications. The findings imply that current defense strategies are insufficient and that achieving genuine role perception in LLMs is necessary to prevent ongoing security arms races. The researchers found that "destyling"—rewriting text to look less like the expected format of a role tag—reduced attack success from 61% to 10%, even though the content remained semantically identical. Models like gpt-oss-20b were shown to override their training when presented with text that stylistically matched internal thinking blocks.

rss · Simon Willison · Jun 22, 23:59

**Background**: Prompt injection is a security vulnerability where an attacker tricks an LLM into following malicious instructions hidden within user input, often by exploiting the model's inability to distinguish system prompts from user data. Role tags like <system>, <user>, and <assistant> are commonly used to separate different types of text in LLM interactions, but this research shows that models rely more on stylistic cues than on these tags. The term "prompt injection" was coined by Simon Willison in 2022, and it differs from jailbreaking, which directly bypasses safety filters.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Prompt_injection">Prompt injection - Wikipedia</a></li>
<li><a href="https://role-confusion.github.io/">Prompt Injection as Role Confusion</a></li>
<li><a href="https://arxiv.org/html/2603.12277">Prompt Injection as Role Confusion</a></li>

</ul>
</details>

**Discussion**: The Hacker News discussion (from which this article was sourced) likely includes comments expressing concern about the severity of the vulnerability and the inadequacy of current defenses. Some commenters may debate the feasibility of achieving genuine role perception in LLMs, while others might share practical mitigation strategies or related research.

**Tags**: `#prompt injection`, `#LLM security`, `#role confusion`, `#jailbreak`, `#AI safety`

---

<a id="item-6"></a>
## [Porting Moebius 0.2B Inpainting Model to Browser with WebGPU](https://simonwillison.net/2026/Jun/22/porting-moebius/#atom-everything) ⭐️ 8.0/10

Simon Willison successfully ported the Moebius 0.2B image inpainting model to run entirely in the browser using ONNX Runtime Web with WebGPU acceleration, and published a live demo at simonw.github.io/moebius-web/. This port makes a state-of-the-art inpainting model accessible to anyone without requiring a GPU or Python environment, lowering the barrier for creative and practical use cases. It also demonstrates the growing capability of WebGPU for running complex AI models directly in the browser. The model requires a ~1.3GB download and runs at 512x512 resolution; non-square images are letterboxed. Simon used Claude Code to assist with the porting process, leveraging ONNX Runtime Web on the WebGPU backend.

rss · Simon Willison · Jun 22, 23:43

**Background**: Image inpainting is the task of filling in missing or removed regions of an image with plausible content. Moebius is a lightweight 0.2B parameter model that claims performance comparable to 10B parameter models. WebGPU is a modern browser API that provides low-level access to GPU hardware, enabling efficient machine learning inference in the browser.

<details><summary>References</summary>
<ul>
<li><a href="https://simonwillison.net/2026/Jun/22/porting-moebius/">Porting the Moebius 0.2B image inpainting model to run in the ...</a></li>
<li><a href="https://arxiv.org/html/2606.19195v1">Moebius: 0.2B Lightweight Image Inpainting Framework with 10B ...</a></li>
<li><a href="https://developer.chrome.com/blog/webgpu-io2023">WebGPU: Unlocking modern GPU access in the browser | Blog | Chrome for Developers</a></li>

</ul>
</details>

**Discussion**: The Hacker News discussion was generally positive, with the author sharing the demo and code. Some users noted that while impressive for a 0.2B model, the inpainting quality does not fully match 10B models, especially on novel objects, and the 512x512 output limit reduces practical usefulness.

**Tags**: `#image inpainting`, `#WebGPU`, `#browser ML`, `#model porting`, `#Simon Willison`

---

<a id="item-7"></a>
## [browser-search: Free open-source tools for AI web browsing](https://www.reddit.com/r/artificial/comments/1udbuid/browsersearch_three_tools_zero_cost_and_your_ai/) ⭐️ 8.0/10

browser-search is a new open-source project that combines three tools—SearXNG, Camofox, and CloakBrowser—into a single skill, enabling AI agents to autonomously search and browse the web without any API costs or subscriptions. This project addresses a common pain point for AI agents like OpenCode and Claude Code: web browsing is often blocked by anti-bot systems or requires costly APIs. By providing a free, self-hosted solution, it lowers the barrier for developers to build agents with real-time web access. The skill uses automatic navigation escalation: if Camofox gets blocked, it switches to CloakBrowser. It also integrates Readability.js for clean article extraction, saving about 70% on tokens, and includes a Deep Research mode for thorough cross-verification.

reddit · r/artificial · /u/Ill-Tradition1362 · Jun 23, 09:00

**Background**: AI agents often need to browse the web to gather information, but many websites use anti-bot systems like Cloudflare, Akamai, or DataDome that block standard automation tools. SearXNG is a metasearch engine that aggregates results from multiple search engines without tracking users. Camofox and CloakBrowser are stealth browsers designed to evade bot detection by spoofing browser fingerprints at the engine level.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/searxng/searxng">GitHub - searxng/searxng: SearXNG is a free internet ...</a></li>
<li><a href="https://github.com/jo-inc/camofox-browser">jo-inc/camofox-browser: Stealth headless ...</a></li>
<li><a href="https://github.com/CloakHQ/CloakBrowser">CloakHQ/CloakBrowser: Stealth Chromium that passes ...</a></li>

</ul>
</details>

**Tags**: `#AI agents`, `#web scraping`, `#open source`, `#automation`, `#browsing`

---

<a id="item-8"></a>
## [Prior Context Alters LLM Responses via Hidden States](https://www.reddit.com/r/artificial/comments/1ud98oz/what_a_model_reads_beforehand_changes_how_it/) ⭐️ 8.0/10

A new study shows that reading a long, structured text before a task can measurably shift a language model's hidden states, leading to different answers on unrelated topics. The effect was first observed in Claude and then mechanistically confirmed in Gemma-3-12B using open-weight models. This finding reveals a subtle but systematic vulnerability in LLM behavior that is not a jailbreak but can still alter responses on sensitive topics. It highlights the need for deeper mechanistic interpretability to understand and control how prior context influences model outputs. The behavioral pattern was first observed in GPT and Claude, but the mechanistic investigation used open-weight models like Gemma-3-12B to inspect hidden states. The study found that after processing a structured text, the model's pre-output hidden states in late layers occupy a measurably different region compared to a neutral control text.

reddit · r/artificial · /u/Historical-Cod-2537 · Jun 23, 06:24

**Background**: Mechanistic interpretability aims to reverse-engineer neural networks by understanding internal components like hidden states and attention circuits. Hidden states are internal representations that encode information as the model processes input; they can be analyzed to see what the model 'knows' before generating output. This study uses that approach to show that prior context can shift these states in a way that affects subsequent answers.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Mechanistic_interpretability">Mechanistic interpretability - Wikipedia</a></li>
<li><a href="https://medium.com/@thekzgroupllc/the-blueprint-of-mechanistic-interpretability-58e56e476768">The Blueprint of Mechanistic Interpretability | by Zaina Haider | Medium</a></li>
<li><a href="https://threatmodel.co/blog/llm_jailbreaking_explained_attacks_risks_defenses">LLM Jailbreaking Explained: Attack Methods, Real Risks, and ...</a></li>

</ul>
</details>

**Discussion**: The Reddit discussion is technically substantive, with users praising the reproducible code and clear methodology. Some commenters debate whether this is truly distinct from jailbreaking, while others suggest it could be used for safety testing or adversarial robustness research.

**Tags**: `#mechanistic interpretability`, `#LLM safety`, `#hidden states`, `#jailbreak`, `#AI alignment`

---

<a id="item-9"></a>
## [HTTP QUERY Method Proposed for Read Requests with Body](https://kreya.app/blog/new-http-query-method-explained/) ⭐️ 7.0/10

A new HTTP method called QUERY has been proposed in an IETF draft to allow safe and idempotent read requests with a request body, addressing the long-standing issue of using GET with a body. This provides a standardized alternative to the hack of sending a body with GET, improving interoperability and enabling proper caching and retries for complex queries, especially in API design. The QUERY method is defined as safe and idempotent, similar to GET, but explicitly allows a request body. It is intended for use cases like GraphQL queries or search endpoints where the query parameters are too large for a URL.

hackernews · CommonGuy · Jun 23, 06:05 · [Discussion](https://news.ycombinator.com/item?id=48640974)

**Background**: HTTP GET requests are not supposed to carry a body according to the HTTP specification, yet many APIs need to send complex queries that exceed URL length limits. Using POST for such queries breaks idempotency and caching. The QUERY method fills this gap by providing a safe, idempotent method that can carry a body.

<details><summary>References</summary>
<ul>
<li><a href="https://httpwg.org/http-extensions/draft-ietf-httpbis-safe-method-w-body.html">The HTTP QUERY Method</a></li>
<li><a href="https://datatracker.ietf.org/doc/draft-ietf-httpbis-safe-method-w-body/">draft-ietf-httpbis-safe-method-w-body-14 - The HTTP QUERY Method</a></li>
<li><a href="https://www.baeldung.com/cs/http-get-with-body">Why an HTTP Get Request Shouldn’t Have a Body | Baeldung on Computer Science</a></li>

</ul>
</details>

**Discussion**: The community discussion highlights both support and concerns. Some argue that QUERY is essentially GET with a body and that legacy proxies may not support it, potentially causing issues. Others appreciate the formalization, noting that using GET with a body is a hack that should be avoided.

**Tags**: `#HTTP`, `#Web Standards`, `#Protocol Design`, `#API Design`

---

<a id="item-10"></a>
## [Crypto in 2026: Scams, Fraud, and Stablecoin Utility](https://www.stephendiehl.com/posts/bad_place_2026/) ⭐️ 7.0/10

A critical analysis published in 2026 argues that the crypto industry is dominated by scams, fraud, and gambling, with stablecoins being the only practical use case, primarily in developing countries. This critique challenges the narrative of crypto as a transformative technology, highlighting systemic issues that undermine trust and adoption, and reinforces the need for regulation and real-world utility. The author notes that even legitimate exchanges like Coinbase allow unregistered securities trading, and that fraud at the exchange level remains rampant post-FTX. Stablecoins like USDT and USDC are praised for enabling access to stable currency in developing economies.

hackernews · ibobev · Jun 23, 10:04 · [Discussion](https://news.ycombinator.com/item?id=48642699)

**Background**: Cryptocurrencies were designed to enable decentralized, peer-to-peer transactions without intermediaries. However, the industry has been plagued by scams, exchange collapses, and regulatory issues. Stablecoins are a type of cryptocurrency pegged to a stable asset like the US dollar, offering price stability. They have gained traction in emerging markets for cross-border payments and wealth preservation.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Stablecoin">Stablecoin - Wikipedia</a></li>
<li><a href="https://www.bitget.com/news/detail/12560604206939">Stablecoins are Popular in Developing Countries for Payments and Transfers | Bitget News</a></li>
<li><a href="https://business.cornell.edu/article/2025/04/stablecoins-importance-in-emerging-markets/">Stablecoins: Importance in Emerging Markets and Recommended Regulatory Framework | Cornell SC Johnson</a></li>

</ul>
</details>

**Discussion**: Commenters largely agree with the critique, with one noting that 'pure' decentralization is impractical and that stablecoins are the only real use case. Another highlights ongoing fraud at exchanges, while a third points out that Bitcoin has real utility in the dark web drug market.

**Tags**: `#cryptocurrency`, `#blockchain`, `#scams`, `#stablecoins`, `#decentralization`

---

<a id="item-11"></a>
## [GLM-5.2 Local Inference Guide with Quantized MoE](https://unsloth.ai/docs/models/glm-5.2) ⭐️ 7.0/10

Unsloth published a guide for running GLM-5.2 locally using quantized Mixture-of-Experts (MoE) offloading, requiring 256GB RAM and 24GB VRAM. The model achieves about 6 tokens per second on a budget build with 512GB RAM and two RTX 3090 GPUs. This guide lowers the barrier for running a large open-source MoE model locally, enabling AI practitioners to experiment with state-of-the-art models without relying on cloud APIs. It also highlights the growing feasibility of local inference for large models as quantization and hardware improve. The model requires 256GB of system RAM for MoE offloading and 24GB of VRAM for the GPU. Using llama.cpp with the -cmoe flag, a setup with 512GB DDR4 RAM and two RTX 3090s achieves ~6 tok/s, while faster RAM and more CPU cores can boost speed to ~11 tok/s.

hackernews · TechTechTech · Jun 22, 21:21 · [Discussion](https://news.ycombinator.com/item?id=48636377)

**Background**: GLM-5.2 is a large open-source language model that uses a Mixture-of-Experts (MoE) architecture, meaning only a subset of parameters are activated per token, enabling high performance with lower computational cost. Quantization reduces model precision (e.g., from 16-bit to 4-bit) to shrink memory footprint, allowing the model to run on consumer hardware. MoE offloading further distributes expert weights between GPU VRAM and system RAM to fit within limited GPU memory.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/abs/2504.02658">[2504.02658] MiLo: Efficient Quantized MoE Inference with ...</a></li>

</ul>
</details>

**Discussion**: Community members shared practical hardware experiences: one user runs the model at ~6 tok/s with 512GB RAM and two 3090s, noting that faster RAM and more CPU cores improve speed. Another user with 192GB RAM and a single 3090 found it almost sufficient but noted the 256GB RAM requirement. Some expressed optimism about the trend toward local inference, while others cautioned that prompt processing speeds remain much slower than GPU-only setups.

**Tags**: `#AI/ML`, `#open-source`, `#local inference`, `#quantization`, `#hardware`

---

<a id="item-12"></a>
## [Oak: A Git Alternative Built for AI Agents](https://oak.space/oak/oak) ⭐️ 7.0/10

Oak is a new version control system designed for AI agents, featuring virtual mounts that allow agents to work on repositories without downloading the full copy, enabling parallel tasking and faster snapshots. As AI agents become more involved in software development, traditional VCS like Git become a bottleneck due to full clones and serial workflows; Oak addresses this by reducing repo size and enabling parallel operations, potentially accelerating agent-driven development. Oak claims snapshots are up to 95% faster than Git and eliminates the need for commit messages. It is still early-stage, lacking Windows support, CI, issues, and comments, but the Oak repository itself has been bootstrapped on Oak for several months without Git backup.

hackernews · zdgeier · Jun 22, 15:37 · [Discussion](https://news.ycombinator.com/item?id=48631726)

**Background**: Version control systems (VCS) track changes to files over time, enabling collaboration and rollback. Git is the dominant VCS, but its design assumes human users who clone entire repositories and work sequentially. AI agents, however, often need to work on many tasks in parallel across large repos, where full clones waste time and storage. Virtual mounts, similar to Microsoft's VFS for Git, allow on-demand file access without downloading everything.

<details><summary>References</summary>
<ul>
<li><a href="https://oak.space/">Version control at the speed of agents · oak</a></li>
<li><a href="https://github.com/microsoft/VFSForGit">GitHub - microsoft/VFSForGit: Virtual File System for Git ... The Lore Version Control System - Lore Developer Documentation DAEMON Tools Lite - Download DAEMON Tools Lite: The most personal application for disc ... Top ISO Mounter Tools for Windows and Mac Comparison Review Comparison of version-control software - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Commenters raised concerns about AI agents' familiarity with Git due to training data, questioning whether a new VCS is justified. Some praised the lazy mount concept, comparing it to Google's internal system and Microsoft's VFS for Git, while others noted the lack of compatibility with the Git ecosystem as a significant hurdle.

**Tags**: `#version control`, `#AI agents`, `#git alternative`, `#developer tools`

---

<a id="item-13"></a>
## [Canada plans nuclear renaissance with up to 10 reactors by 2040](https://www.cbc.ca/news/politics/federal-nuclear-strategy-9.7244509) ⭐️ 7.0/10

Canada announced a federal strategy to build up to 10 new nuclear reactors by 2040, including two large-scale reactors starting construction by 2035 and at least one reactor outside Ontario by 2035. This marks a significant policy shift toward nuclear energy, leveraging Canada's large uranium reserves and CANDU technology, and could provide reliable baseload power to complement renewables, impacting energy security and climate goals. The strategy calls for construction start on two new large-scale reactors by 2035, five more planned or under development by 2040, and at least one reactor under construction outside Ontario by 2035. The Darlington New Nuclear Project is already underway.

hackernews · geox · Jun 22, 19:06 · [Discussion](https://news.ycombinator.com/item?id=48634585)

**Background**: CANDU (Canada Deuterium Uranium) is a pressurized heavy-water reactor design developed in Canada, known for using natural uranium as fuel and offering high safety and efficiency. Canada has one of the world's largest uranium reserves and extensive experience with CANDU reactors, including refurbishments at Darlington. The strategy aims to meet growing electricity demand and support net-zero emissions goals.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/CANDU_reactor">CANDU reactor - Wikipedia</a></li>
<li><a href="https://www.atkinsrealis.com/en/projects/candu-technology">CANDU technology: helping Ontario achieve Net Zero</a></li>
<li><a href="https://natural-resources.canada.ca/energy-sources/nuclear-energy-uranium/canadian-nuclear-energy-technology">The Canadian Nuclear Energy Technology - Natural Resources Canada</a></li>

</ul>
</details>

**Discussion**: Commenters generally support the plan, citing Canada's uranium reserves and CANDU expertise, but express skepticism about the timeline, noting that construction start by 2035 is too far away. Some highlight the Darlington project as a positive sign, while others reflect on the shift in public opinion toward nuclear energy.

**Tags**: `#nuclear energy`, `#Canada`, `#energy policy`, `#CANDU`, `#infrastructure`

---

<a id="item-14"></a>
## [sqlite-utils 4.0rc1 adds migrations and nested transactions](https://simonwillison.net/2026/Jun/21/sqlite-utils-40rc1/#atom-everything) ⭐️ 7.0/10

The first release candidate for sqlite-utils 4.0 introduces built-in database migrations and nested transaction support via db.atomic(). These features simplify database schema management and safe concurrent writes for Python developers using SQLite, making sqlite-utils a more complete tool for application development. The migration system is a port of the proven sqlite-migrate package and does not support reverse migrations. Nested transactions use SQLite savepoints under the hood.

rss · Simon Willison · Jun 21, 23:35

**Background**: sqlite-utils is a Python library and CLI tool that provides high-level operations on SQLite databases. It is widely used in the Datasette ecosystem and by Python developers for data analysis and prototyping.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/simonw/sqlite-migrate">simonw/sqlite-migrate - GitHub</a></li>
<li><a href="https://sqlite-utils.datasette.io/en/latest/migrations.html">Database migrations - sqlite-utils</a></li>
<li><a href="https://simonwillison.net/2026/Jun/21/sqlite-utils-40rc1/">sqlite-utils 4.0rc1 adds migrations and nested transactions - Simon Willison's Weblog</a></li>

</ul>
</details>

**Tags**: `#sqlite`, `#python`, `#database`, `#release`, `#migrations`

---

<a id="item-15"></a>
## [Cloudflare Launches Temporary Accounts for Workers](https://simonwillison.net/2026/Jun/21/temporary-cloudflare-accounts/#atom-everything) ⭐️ 7.0/10

Cloudflare introduced temporary, ephemeral accounts that allow developers to deploy Workers projects without registration, with deployments staying live for 60 minutes. The feature is accessible via the wrangler CLI command `npx wrangler deploy --temporary`. This feature significantly lowers the barrier for rapid prototyping and testing, especially for AI agents and developers who need quick, disposable deployments. It also demonstrates a broader trend toward ephemeral environments in serverless computing. The temporary deployment URL includes a claim page that allows users to take ownership of the project if they want it to persist beyond 60 minutes. The feature is marketed for AI agents but is useful for all developers.

rss · Simon Willison · Jun 21, 22:01

**Background**: Cloudflare Workers is a serverless computing platform that runs code on Cloudflare's global edge network. Wrangler is the official CLI for building, testing, and deploying Workers projects. Ephemeral environments are short-lived, isolated deployments created on demand for specific tasks.

<details><summary>References</summary>
<ul>
<li><a href="https://developers.cloudflare.com/workers/wrangler/">Wrangler · Cloudflare Workers docs</a></li>
<li><a href="https://developers.cloudflare.com/workers/">Overview · Cloudflare Workers docs</a></li>

</ul>
</details>

**Discussion**: The Hacker News discussion (referenced in the article) likely highlights the convenience for rapid prototyping and the AI agent use case, though no specific comments are provided here.

**Tags**: `#cloudflare`, `#serverless`, `#deployment`, `#developer tools`, `#AI agents`

---

<a id="item-16"></a>
## [Google Invests $75M in A24 for AI Filmmaking Tools](https://www.reddit.com/r/artificial/comments/1ud44pc/google_invests_75_million_in_a24_to_develop/) ⭐️ 7.0/10

Google has invested $75 million in independent film studio A24 to develop AI-powered filmmaking tools, marking a significant push into AI-driven content creation. This investment signals a major industry shift toward AI-assisted filmmaking, potentially lowering production costs and democratizing high-quality video creation for independent creators. A24 is known for critically acclaimed films like 'Everything Everywhere All at Once' and 'Moonlight', and the partnership aims to integrate Google's AI technologies such as Gemini into the filmmaking workflow.

reddit · r/artificial · /u/ControlCAD · Jun 23, 02:04

**Background**: AI filmmaking tools are increasingly used for tasks like scriptwriting, storyboarding, visual effects, and editing. Google's investment in A24, a prestigious independent studio, suggests a focus on high-quality, artistically driven AI applications rather than mass-produced content.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/A24">A24 - Wikipedia</a></li>
<li><a href="https://interestingengineering.com/ai-robotics/ai-tools-filmmaking-movies">How to make a film using AI tools in 2026</a></li>

</ul>
</details>

**Tags**: `#AI`, `#Filmmaking`, `#Google`, `#Investment`, `#Creative AI`

---

<a id="item-17"></a>
## [Canada secretly spent millions on Palantir AI surveillance](https://www.reddit.com/r/artificial/comments/1ucilr4/canadian_government_spent_tens_of_millions_on/) ⭐️ 7.0/10

The Canadian government secretly spent tens of millions of dollars on a contract with Palantir Canada for AI-powered surveillance services, with documents revealing the contract was worth $30 million more than initially disclosed. This raises significant privacy and ethical concerns about government use of AI surveillance technology, especially given Palantir's controversial history of enabling mass surveillance and targeting individuals. The contract was with an elite military unit, and the government made over a dozen amendments to hide the true cost. Palantir's technology aggregates massive amounts of data to create AI-driven profiles for enforcement decisions.

reddit · r/artificial · /u/Goldenmentis · Jun 22, 11:59

**Background**: Palantir is a US-based data analytics company known for its work with intelligence and defense agencies, often criticized for expanding government surveillance using AI and facial recognition. The Canadian contract was first reported by the Investigative Journalism Foundation via its Open By Default database.

<details><summary>References</summary>
<ul>
<li><a href="https://theijf.org/brief/canadian-palantir-contract-amendments-obd">Canadian government spent tens of millions on secret Palantir contract</a></li>
<li><a href="https://www.thestar.com/politics/federal/documents-reveal-that-palantir-contract-was-worth-30m-more-than-government-disclosed/article_360cfa78-7ada-4b82-a06d-3e0287eb4c8d.html">Documents reveal that Palantir contract was worth $30M more than government disclosed</a></li>
<li><a href="https://en.wikipedia.org/wiki/Palantir">Palantir - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Reddit users expressed outrage over the secrecy and cost, with many criticizing the government for lack of transparency and questioning the ethics of using Palantir for surveillance. Some debated whether the technology is necessary for national security.

**Tags**: `#Palantir`, `#government surveillance`, `#AI ethics`, `#privacy`, `#Canada`

---

<a id="item-18"></a>
## [AI Cost Paradox: Spending More Despite Automation](https://www.reddit.com/r/artificial/comments/1udc6in/the_ai_cost_paradox_why_are_some_companies/) ⭐️ 7.0/10

A Reddit analysis highlights that companies deploying AI are not reducing overall costs but instead shifting spending from human salaries to infrastructure, monitoring, and human oversight, leading to higher-than-expected bills. This paradox challenges the common narrative that AI will drastically cut labor costs, revealing that scaling AI requires significant investment in infrastructure and quality control, which may reshape enterprise budgeting and AI adoption strategies. The post notes that AI systems scale errors: one mistake can affect thousands of customers, necessitating human reviewers and AI engineers. This mirrors patterns seen with cloud infrastructure or ERP software, which are initially expensive but become indispensable.

reddit · r/artificial · /u/ExcellentBandicoot57 · Jun 23, 09:18

**Background**: AI deployment often involves a stack of AI model, monitoring, human review, integrations, and infrastructure. While AI excels at repetitive tasks, its errors can scale rapidly, requiring additional oversight. This is similar to Jevons Paradox, where efficiency gains increase total resource consumption.

<details><summary>References</summary>
<ul>
<li><a href="https://www.mindstudio.ai/blog/jevons-paradox-ai-human-work-demand">What Is Jevons Paradox in AI? Why Cheaper Intelligence Creates More Demand for Human Work | MindStudio</a></li>
<li><a href="https://www.cake.ai/blog/ai-infrastructure-costs">AI Infrastructure Costs: A Practical Guide</a></li>
<li><a href="https://docs.aws.amazon.com/sagemaker/latest/dg/a2i-use-augmented-ai-a2i-human-review-loops.html">Using Amazon Augmented AI for Human Review - Amazon SageMaker AI</a></li>

</ul>
</details>

**Discussion**: The Reddit discussion largely agrees with the analysis, with users sharing experiences of hiring AI evaluators and facing unexpected costs. Some argue that AI is more like a new infrastructure layer than a labor replacement, while others question whether long-term savings will materialize.

**Tags**: `#AI`, `#cost analysis`, `#deployment`, `#scaling`, `#infrastructure`

---

<a id="item-19"></a>
## [Investment Lawyer Explains AI Deepfake Scams](https://www.reddit.com/r/artificial/comments/1ucpgrh/investment_lawyer_breaking_down_how_ai_deepfakes/) ⭐️ 7.0/10

An investment lawyer has broken down how AI deepfakes are used in high-profile scams, detailing real-world cases and the legal challenges they pose. This analysis highlights the growing threat of AI-generated fraud, which can undermine trust in digital communications and cause significant financial losses for individuals and businesses. The lawyer explains that scammers use deepfakes to impersonate executives or loved ones, often combining video, audio, and text to create convincing scenarios. Legal remedies are still evolving, with existing laws like defamation and fraud being stretched to cover AI-generated content.

reddit · r/artificial · /u/MW2_Lobbies · Jun 22, 16:30

**Background**: Deepfakes are AI-generated media that can make people appear to say or do things they never did. They are created using deep learning techniques, such as generative adversarial networks (GANs). While initially used for entertainment, deepfakes are increasingly weaponized in scams, political disinformation, and identity theft.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Deepfake">Deepfake - Wikipedia</a></li>
<li><a href="https://www.americanbar.org/groups/senior_lawyers/resources/voice-of-experience/2025-june/what-deepfake-scams-teach-us-about-ai-and-fraud/">What Deepfake Scams Teach Us About AI and Fraud</a></li>
<li><a href="https://www.mcafee.com/learn/a-guide-to-deepfake-scams-and-ai-voice-spoofing/">A Guide to Deepfake Scams and AI Voice Spoofing | McAfee</a></li>

</ul>
</details>

**Tags**: `#AI`, `#deepfakes`, `#security`, `#scams`, `#law`

---

<a id="item-20"></a>
## [Developer Spends Month Optimizing AI Agent Without Defining Goals](https://www.reddit.com/r/artificial/comments/1udbnfe/i_spent_a_month_optimizing_my_ai_agent_then/) ⭐️ 7.0/10

A developer realized after a month of optimizing his AI agent that he had never defined what "optimized" meant, highlighting the lack of standardized evaluation metrics for AI agent specifications. This issue is significant because as AI agents become more common, the absence of clear, measurable goals and universal evaluation metrics can lead to wasted effort and unreliable performance, hindering the development of robust agentic systems. The developer's agent was designed to take notes, structure them, file them, and handle version control, but he found himself optimizing vague terms like "reliable" and "no drift" without baselines or meaningful scoring criteria.

reddit · r/artificial · /u/hikaze_369 · Jun 23, 08:48

**Background**: AI agents are autonomous systems that use large language models (LLMs) to plan and execute tasks. The AGENT.md format is an emerging open standard for providing instructions to coding agents, but there is no equivalent standard for evaluating the quality of an agent's specification or performance.

<details><summary>References</summary>
<ul>
<li><a href="https://deepwiki.com/openai/agents.md/5-agents.md-format-documentation">AGENTS.md Format Documentation | openai/agents.md | DeepWiki</a></li>
<li><a href="https://machinelearningmastery.com/agent-evaluation-how-to-test-and-measure-agentic-ai-performance/">Agent Evaluation: How to Test and Measure Agentic AI ...</a></li>
<li><a href="https://www.confident-ai.com/blog/definitive-ai-agent-evaluation-guide">AI Agent Evaluation: Metrics, Traces, Human Review, and ...</a></li>

</ul>
</details>

**Discussion**: The Reddit discussion likely resonated with many developers who have faced similar challenges in defining and measuring agent performance, with comments emphasizing the need for better evaluation frameworks and the pitfalls of optimizing without clear metrics.

**Tags**: `#AI agents`, `#optimization`, `#evaluation metrics`, `#software engineering`

---

<a id="item-21"></a>
## [Claude Code v2.1.186: MCP Auth CLI and Bug Fixes](https://github.com/anthropics/claude-code/releases/tag/v2.1.186) ⭐️ 6.0/10

Anthropic released Claude Code v2.1.186, adding `claude mcp login` and `claude mcp logout` commands for authenticating MCP servers from the CLI, along with status filtering in the `/workflows` view and numerous bug fixes. This update improves developer workflow by enabling MCP server authentication without opening the interactive menu, and fixes critical issues like streaming failures after sleep and subagent scroll bleeding, enhancing reliability for daily use. The new MCP auth commands support `--no-browser` for SSH sessions; `!` bash commands now automatically trigger a response from Claude, configurable via `respondToBashCommands`. The update also caps `CLAUDE_CODE_MAX_RETRIES` at 15 and changes background subagents to surface permission prompts in the main session.

github · ashwin-ant · Jun 22, 20:37

**Background**: Claude Code is Anthropic's CLI-based AI coding assistant. MCP (Model Context Protocol) servers provide external tools and data to the AI. Subagents are specialized AI assistants that handle specific tasks within a Claude Code session, helping manage context and delegate work.

<details><summary>References</summary>
<ul>
<li><a href="https://deepwiki.com/openai/codex/6.3-mcp-cli-commands">MCP CLI Commands | openai/codex | DeepWiki</a></li>
<li><a href="https://github.com/anthropics/claude-code/issues/24292">teammateMode: "tmux" does not create iTerm2 split panes ...</a></li>

</ul>
</details>

**Tags**: `#CLI`, `#MCP`, `#bug-fix`, `#developer-tools`

---

<a id="item-22"></a>
## [Blog Post Compares AI Models, Community Debates](https://swelljoe.com/post/will-it-mythos/) ⭐️ 6.0/10

A blog post titled 'Will It Mythos?' compares various AI model capabilities, including Anthropic's Fable and GPT-5.5 Pro, with community members sharing firsthand experiences and critiques. This discussion highlights ongoing concerns about AI model performance consistency and evaluation methodology, which are critical for developers and researchers relying on these models. The blog post uses a leaderboard with a $100 budget per model, and commenters note that GPT-5.5 Pro's top ranking is skewed because it only completed 2 out of 4 cases, yielding a 50% score.

hackernews · mindingnever · Jun 23, 04:15 · [Discussion](https://news.ycombinator.com/item?id=48640196)

**Background**: AI model comparisons often use benchmarks and leaderboards to evaluate performance, but methodology issues like incomplete tasks can skew results. The community discusses using Wilson score intervals for more accurate rankings.

**Discussion**: Commenters share mixed experiences: Tossrock finds Fable substantially more powerful, while airstrike notes that Opus models were lobotomized after updates. JumpCrisscross critiques the leaderboard methodology, suggesting Wilson score intervals.

**Tags**: `#AI`, `#machine learning`, `#model comparison`, `#Anthropic`

---

<a id="item-23"></a>
## [Autodesk invests $350M in AI workforce training](https://www.reddit.com/r/artificial/comments/1ucxiby/autodesk_commits_350m_to_help_prepare_students/) ⭐️ 6.0/10

Autodesk announced a $350 million commitment to prepare students, educators, job-seekers, and professionals for AI jobs in design and manufacturing. This significant investment signals a major push by a leading design software company to address the AI skills gap in industries that build the physical world, potentially influencing workforce development trends. The $350 million commitment will fund training programs, certifications, and learning resources, targeting roles that use AI for design, engineering, and manufacturing.

reddit · r/artificial · /u/LinkedInNews · Jun 22, 21:24

**Background**: Autodesk is a major provider of design software like AutoCAD and Fusion 360, used in architecture, engineering, and manufacturing. As AI transforms these fields, companies need workers skilled in AI-assisted design and production.

**Tags**: `#AI`, `#Education`, `#Autodesk`, `#Investment`

---

<a id="item-24"></a>
## [Are AI Benchmarks Valid for Passive Users?](https://www.reddit.com/r/artificial/comments/1ucvrir/did_we_only_ever_test_ai_when_the_user_was_ready/) ⭐️ 6.0/10

A Reddit post questions whether current AI benchmarks, which assume an active user preparing a query, are valid for real-time, ambient AI applications like voice agents, autonomous cars, and smart glasses where the user is not actively engaged. As AI moves into always-on, background roles, relying on benchmarks designed for deliberate user interactions may misrepresent real-world performance, potentially leading to safety and reliability issues in critical applications. The post specifically mentions voice agents taking calls, cars making real-time decisions, and devices like Ray-Ban Meta, Rokid, and XRAI Glass running AI in the background, highlighting that benchmarks were not built for these contexts.

reddit · r/artificial · /u/Trickyeahh · Jun 22, 20:19

**Background**: AI benchmarks like MMLU or Chatbot Arena typically evaluate models on static, user-initiated tasks. However, emerging ambient AI systems operate continuously, processing sensor data and making decisions without explicit user prompts, requiring different evaluation criteria.

<details><summary>References</summary>
<ul>
<li><a href="https://www.meta.com/ai-glasses/ray-ban-meta/">Ray-Ban Meta AI Glasses: New Styles & Colors | Meta Store</a></li>
<li><a href="https://global.rokid.com/products/rokid-glasses">49g Ultra-Light AR glasses with AI - Rokid</a></li>
<li><a href="https://xrai.glass/">XRAI Glass | Life. Subtitled</a></li>

</ul>
</details>

**Tags**: `#AI benchmarks`, `#real-time AI`, `#AI evaluation`, `#ambient AI`

---

<a id="item-25"></a>
## [Kimi K2.6 vs Claude: Which Coding Agent Is Better?](https://www.reddit.com/r/artificial/comments/1uddjsh/is_kimi_k26_agent_better_than_claude_codeclaude/) ⭐️ 6.0/10

A Reddit user asks whether Kimi K2.6 Agent outperforms Claude Code or Claude Co-work for coding tasks, sparking a comparison between two leading AI coding agents. This comparison highlights the growing competition in AI-assisted coding, where open-source models like Kimi K2.6 challenge proprietary tools like Claude, potentially lowering costs and increasing accessibility for developers. Kimi K2.6 is an open-source multimodal agentic model with long-horizon coding and agent swarm capabilities, while Claude Code and Claude Co-work are Anthropic's proprietary coding and knowledge-work agents.

reddit · r/artificial · /u/Confident-Rush8127 · Jun 23, 10:37

**Background**: AI coding agents are tools that can read codebases, edit files, and run commands autonomously. Kimi K2.6, released about a week ago, is positioned as a state-of-the-art open-source model for coding and agent tasks. Claude Code and Claude Co-work are Anthropic's offerings, with Claude Code focused on terminal/IDE coding and Claude Co-work on desktop knowledge work.

<details><summary>References</summary>
<ul>
<li><a href="https://www.kimi.com/en">Kimi AI with K2.6 | Better Coding, Smarter Agents</a></li>
<li><a href="https://www.kimi.com/ai-models/kimi-k2-6">Kimi K2.6 | Leading Open-Source Model in Coding & Agent</a></li>
<li><a href="https://ollama.com/library/kimi-k2.6">kimi-k2.6</a></li>
<li><a href="https://claude.com/product/claude-code">Claude Code by Anthropic | AI Coding Agent, Terminal, IDE</a></li>
<li><a href="https://www.anthropic.com/product/claude-cowork">Claude Cowork | Anthropic’s agentic AI for knowledge work \ Anthropic</a></li>

</ul>
</details>

**Tags**: `#AI agents`, `#coding assistants`, `#Claude`, `#Kimi`

---