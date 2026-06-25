---
layout: default
title: "Horizon Summary: 2026-06-25 (EN)"
date: 2026-06-25
lang: en
---

> From 37 items, 27 important content pieces were selected

---

1. [OpenAI unveils first custom AI chip 'Jalapeno' with Broadcom](#item-1) ⭐️ 9.0/10
2. [Self-play RL agent reaches #1 on Generals.io](#item-2) ⭐️ 9.0/10
3. [Anthropic Accuses Alibaba of Stealing Claude AI Capabilities](#item-3) ⭐️ 8.0/10
4. [Cloudflare Launches Self-Managed OAuth Service](#item-4) ⭐️ 8.0/10
5. [Qualcomm Acquires AI Startup Modular](#item-5) ⭐️ 8.0/10
6. [Nub: A Bun-like all-in-one toolkit for Node.js](#item-6) ⭐️ 8.0/10
7. [LLM-Generated Job Apps Obscure Candidate Authenticity](#item-7) ⭐️ 8.0/10
8. [Why I Stopped Trusting AI Benchmarks and Built My Own Eval](#item-8) ⭐️ 8.0/10
9. [HDD-RoPE: High-Dimensional Dynamic Rotary Positional Embedding](#item-9) ⭐️ 8.0/10
10. [DeepSWE: A Contamination-Free Benchmark for AI Coding Agents](#item-10) ⭐️ 8.0/10
11. [Half-Life 2 Now Playable in a Browser via WebAssembly](#item-11) ⭐️ 7.0/10
12. [LuaJIT 3.0 Proposes C-Style Syntax Extensions](#item-12) ⭐️ 7.0/10
13. [Blogging Can Just Be Stating the Obvious](#item-13) ⭐️ 7.0/10
14. [Nvidia's 45°C Cooling Slashes Data Center Water Use](#item-14) ⭐️ 7.0/10
15. [Zombie Unicorns Haunt Silicon Valley](#item-15) ⭐️ 7.0/10
16. [RubyLLM: A Unified Ruby Framework for Major AI Providers](#item-16) ⭐️ 7.0/10
17. [PR Spam in Open Source Echoes Early 2000s Email Spam](#item-17) ⭐️ 7.0/10
18. [Xteink X4: Low-Cost Open E-Ink Reader](#item-18) ⭐️ 7.0/10
19. [Datasette 1.0a35 Adds Create/Alter Table JSON APIs](#item-19) ⭐️ 7.0/10
20. [Curated OCR Models Hub Launched on Papers with Code](#item-20) ⭐️ 7.0/10
21. [MuJoFil: GPU-Accelerated Simulator for Vision RL](#item-21) ⭐️ 7.0/10
22. [LLM Inference Pricing Comparison Reveals Caching Cost Surprises](#item-22) ⭐️ 7.0/10
23. [Are ML teams testing model security in production?](#item-23) ⭐️ 7.0/10
24. [Claude Code v2.1.187: Sandbox Credentials Blocking and Bug Fixes](#item-24) ⭐️ 6.0/10
25. [Google Adds Computer Use to Gemini 3.5 Flash](#item-25) ⭐️ 6.0/10
26. [Simon Willison Converts MDN Browser Compat Data to SQLite](#item-26) ⭐️ 6.0/10
27. [OPFS + Pyodide Test Harness for Persistent SQLite](#item-27) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [OpenAI unveils first custom AI chip 'Jalapeno' with Broadcom](https://techcrunch.com/2026/06/24/openai-unveils-its-first-custom-chip-built-by-broadcom/) ⭐️ 9.0/10

OpenAI has unveiled its first custom AI inference chip, named 'Jalapeno', developed in collaboration with Broadcom and manufactured by TSMC. The chip was designed from concept to production in just nine months, accelerated by OpenAI's own AI models. This marks a major strategic move by OpenAI to reduce reliance on NVIDIA GPUs and optimize inference performance for its own models. The custom chip could significantly lower costs and improve efficiency for running large language models at scale. Jalapeno is a massive reticle-sized ASIC designed for LLM inference, featuring a large compute chiplet and HBM memory to balance high throughput and low latency. OpenAI plans to begin using the chip for customer queries later this year.

hackernews · jamdesk · Jun 24, 17:47 · [Discussion](https://news.ycombinator.com/item?id=48663324)

**Background**: AI inference chips are specialized processors that execute trained AI models to make predictions on new data. Unlike NVIDIA's general-purpose GPUs, custom ASICs like Jalapeno are optimized for specific workloads, offering better performance per watt. Broadcom has extensive experience designing custom AI chips for companies like Google (TPUs).

<details><summary>References</summary>
<ul>
<li><a href="https://openai.com/index/openai-broadcom-jalapeno-inference-chip/">OpenAI and Broadcom unveil LLM-optimized inference chip | OpenAI</a></li>
<li><a href="https://www.tomshardware.com/tech-industry/artificial-intelligence/broadcom-and-openai-unveil-custom-built-jalapeno-inference-processor-openais-first-chip-is-a-massive-reticle-sized-asic-built-in-an-ultra-fast-nine-month-development-cycle">Broadcom and OpenAI unveil custom-built Jalapeño inference processor — OpenAI's first chip is a massive reticle-sized ASIC built in an ultra-fast nine-month development cycle | Tom's Hardware</a></li>
<li><a href="https://www.axios.com/2026/06/24/openai-jalapeno-ai-chip-broadcom-nvidia">OpenAI tests homegrown AI chips</a></li>

</ul>
</details>

**Discussion**: Community comments show mixed reactions: some question the claim of AI-accelerated design, calling it potentially meaningless marketing, while others highlight the technical achievement and note that TSMC is the manufacturer. There is also discussion about alternative approaches like burning models into silicon.

**Tags**: `#AI hardware`, `#OpenAI`, `#custom chip`, `#inference`, `#Broadcom`

---

<a id="item-2"></a>
## [Self-play RL agent reaches #1 on Generals.io](https://www.reddit.com/r/MachineLearning/comments/1uei2yg/i_made_a_superhuman_generalsio_agent_with/) ⭐️ 9.0/10

A self-play reinforcement learning agent using JAX and Vision Transformers achieved superhuman performance and ranked #1 on the Generals.io human 1v1 leaderboard. The author open-sourced the code, including a fast JAX simulator and the agent, along with a comprehensive guide. This work demonstrates that scaling with modern architectures like Vision Transformers and JAX acceleration can outperform hand-crafted features and prior algorithms in imperfect-information games. It provides an open-source blueprint for building competitive game AI, potentially advancing research in RL and game playing. The agent was initially trained with behavior cloning and RL fine-tuning, but later reimplemented entirely in JAX with a Vision Transformer to improve scalability. The open-source JAX simulator is useful as an imperfect-information RTS environment for other research.

reddit · r/MachineLearning · /u/shrekofspeed · Jun 24, 16:18

**Background**: Generals.io is a fast-paced multiplayer strategy game where players control armies to capture territory and defeat opponents. Self-play reinforcement learning involves an agent learning by playing against itself, which has been successful in games like AlphaGo. JAX is a high-performance numerical computing library that accelerates RL training, and Vision Transformers are a neural network architecture that processes image patches with attention mechanisms.

**Discussion**: The Reddit discussion was substantive, with users asking technical questions about the architecture and training details. The author engaged actively, explaining design choices and sharing insights about the challenges of scaling RL with JAX and ViTs.

**Tags**: `#reinforcement learning`, `#self-play`, `#JAX`, `#vision transformer`, `#game AI`

---

<a id="item-3"></a>
## [Anthropic Accuses Alibaba of Stealing Claude AI Capabilities](https://www.reuters.com/world/china/anthropic-says-alibaba-illicitly-extracted-claude-ai-model-capabilities-2026-06-24/) ⭐️ 8.0/10

Anthropic publicly accused Alibaba of illicitly extracting capabilities from its Claude AI model through model distillation techniques, marking a major escalation in AI intellectual property disputes between US and Chinese tech firms. This accusation highlights growing tensions over AI model theft and raises questions about the ethics of training data usage, as many AI companies themselves have faced copyright infringement lawsuits for using web-scraped data. Anthropic described sophisticated extraction campaigns where proxy networks managed over 20,000 accounts simultaneously, and noted that Chinese labs like MiniMax redirected traffic within 24 hours of new Claude model releases to capture updated capabilities.

hackernews · htrp · Jun 24, 19:48 · [Discussion](https://news.ycombinator.com/item?id=48664814)

**Background**: Model distillation is a technique where one AI model is used to train another by using its outputs as training data. While common for fine-tuning, it can be used to illicitly replicate proprietary models. Anthropic, like other AI labs, has faced legal scrutiny for training its models on copyrighted material from the internet.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Claude_(language_model)">Claude (AI) - Wikipedia</a></li>
<li><a href="https://nationalcioreview.com/articles-insights/extra-bytes/claude-ai-model-extraction-security-and-export-control-implications/">Claude AI Model Extraction: Security and Export Control Implications - The National CIO Review</a></li>
<li><a href="https://www.nightfall.ai/ai-security-101/model-theft">Model Theft: The Essential Guide | Nightfall AI Security 101</a></li>

</ul>
</details>

**Discussion**: Commenters widely criticized Anthropic for hypocrisy, noting that the company itself used pirated books from LibGen for training and was ruled against in court. Others pointed out that model distillation is a common industry practice, and that US companies have historically copied innovations from others.

**Tags**: `#AI`, `#model theft`, `#Anthropic`, `#Alibaba`, `#ethics`

---

<a id="item-4"></a>
## [Cloudflare Launches Self-Managed OAuth Service](https://blog.cloudflare.com/oauth-for-all/) ⭐️ 8.0/10

Cloudflare announced a self-managed OAuth service that allows developers to run their own OAuth servers with high performance and low resource usage. The service is built on a new open-source library, reportedly coded largely using Anthropic's Claude LLM. This simplifies OAuth implementation for developers, offering a scalable and performant alternative to existing solutions like Keycloak or Ory Hydra. It could reduce the complexity of building SaaS integrations and improve security by enabling scoped access directly. The service is self-managed, meaning developers host and control their own OAuth servers, and it integrates with Cloudflare's ecosystem. The library's code was generated with AI assistance, which has drawn both interest and scrutiny from the security community.

hackernews · terryds · Jun 25, 02:18 · [Discussion](https://news.ycombinator.com/item?id=48668033)

**Background**: OAuth is an open standard for token-based authentication and authorization, commonly used to grant third-party applications limited access to user data without exposing passwords. Self-managed OAuth allows organizations to run their own authorization servers rather than relying on third-party providers, giving them more control and customization.

<details><summary>References</summary>
<ul>
<li><a href="https://neilmadden.blog/2025/06/06/a-look-at-cloudflares-ai-coded-oauth-library/">A look at CloudFlare's AI-coded OAuth library - Neil Madden</a></li>
<li><a href="https://cloudflare-docs.cloudflare-docs.workers.dev/changelog/post/2026-06-03-public-oauth-clients/">Introducing self - managed OAuth clients · Changelog</a></li>

</ul>
</details>

**Discussion**: The community response is mixed: some praise the performance and innovation, while others express skepticism about Cloudflare's track record of supporting new products long-term. The author of Ory Hydra congratulated Cloudflare, and some users pointed out alternatives like Keycloak.

**Tags**: `#OAuth`, `#Cloudflare`, `#Identity Management`, `#Developer Tools`, `#Security`

---

<a id="item-5"></a>
## [Qualcomm Acquires AI Startup Modular](https://www.reuters.com/business/qualcomm-buy-ai-startup-modular-2026-06-24/) ⭐️ 8.0/10

Qualcomm announced its acquisition of Modular, the AI infrastructure startup behind the Mojo programming language, on June 24, 2026. The deal is reportedly valued at $4 billion. This acquisition signals Qualcomm's strategic push into AI compute, aiming to strengthen its position against competitors like Nvidia. By integrating Modular's technology, Qualcomm can offer a unified software layer for AI workloads across its hardware, potentially accelerating AI adoption in edge devices. Modular's Mojo language is designed for high-performance AI infrastructure and heterogeneous hardware, combining Python-like syntax with systems-level performance. Qualcomm plans to open-source the Mojo compiler later this year, as confirmed by Modular on Twitter.

hackernews · timmyd · Jun 24, 13:49 · [Discussion](https://news.ycombinator.com/item?id=48659798)

**Background**: Modular was founded in 2022 by Chris Lattner, the creator of LLVM and Swift, and Tim Davis. The company raised $250 million to challenge Nvidia's CUDA dominance by building a unified compute layer for AI that runs across different chips. Mojo is a proprietary programming language that aims to bridge the gap between ease of use and high performance for AI workloads.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Mojo_(programming_language)">Mojo (programming language ) - Wikipedia</a></li>
<li><a href="https://news.google.com/stories/CAAqNggKIjBDQklTSGpvSmMzUnZjbmt0TXpZd1NoRUtEd2pBb2Q3UkR4R1E4ZXJMVFdsYnN5Z0FQAQ?hl=en-GH&gl=GH&ceid=GH:en">Google News - Modular AI raises $250 million to challenge...</a></li>
<li><a href="https://startups.in/ai-machine-learning/modular">Modular - Valuation, Funding, Competitors & News | AI ... | startups .in</a></li>

</ul>
</details>

**Discussion**: Community sentiment is mixed: some express disappointment that Mojo may not achieve true cross-platform support, while others see the acquisition as a positive move for Qualcomm's AI ambitions. There is also hope that the open-sourcing of Mojo will benefit the broader ecosystem.

**Tags**: `#acquisition`, `#AI`, `#Qualcomm`, `#Mojo`, `#hardware`

---

<a id="item-6"></a>
## [Nub: A Bun-like all-in-one toolkit for Node.js](https://github.com/nubjs/nub) ⭐️ 8.0/10

Colin McDonnell, creator of Zod, released Nub, a Bun-like all-in-one toolkit for Node.js that adds TypeScript transpilation, module resolution, and polyfills via preload hooks, without replacing Node's runtime. Nub improves the Node.js developer experience by providing Bun-like features such as fast TypeScript transpilation and polyfills, while keeping compatibility with the existing Node.js ecosystem. It offers a practical upgrade for developers who want modern tooling without switching runtimes. Nub uses an oxc-powered transpiler packaged as a Node-API add-on, registers a module resolution hook, and injects polyfills for APIs like Worker and Temporal. It runs with stock node via a --require preload hook, making all additions purely additive.

hackernews · colinmcd · Jun 24, 14:14 · [Discussion](https://news.ycombinator.com/item?id=48660267)

**Background**: Node.js natively supports JavaScript but requires additional tools like ts-node or esbuild for TypeScript transpilation. Bun is an alternative runtime that includes a built-in transpiler and bundler, but switching runtimes can break compatibility. Nub bridges this gap by enhancing Node.js with Bun-like features via hooks, without changing the underlying runtime.

<details><summary>References</summary>
<ul>
<li><a href="https://nodejs.org/api/module.html">Modules : ` node : module ` API | Node . js v26.3.0 Documentation</a></li>
<li><a href="https://git-stars.org/repositories/topic/transpiler">Top transpiler Repositories - GitHub Projects for transpiler ... | Git Stars</a></li>
<li><a href="https://prepfast.in/topics/nodejs/module-resolution/">Module Resolution Algorithm — Node . js Interview Revision</a></li>

</ul>
</details>

**Discussion**: The community discussion is generally positive, with users praising the idea and noting the author's credibility (creator of Zod, former Bun employee). Some technical concerns were raised about WebSocket support and ESM handling, but a user reported successfully migrating their entire monorepo with zero issues.

**Tags**: `#Node.js`, `#TypeScript`, `#Developer Tools`, `#JavaScript`, `#Bun`

---

<a id="item-7"></a>
## [LLM-Generated Job Apps Obscure Candidate Authenticity](https://simonwillison.net/2026/Jun/24/tom-macwright/#atom-everything) ⭐️ 8.0/10

Tom MacWright observes that job applications increasingly appear to be co-written by LLMs, linking to LLM-generated portfolios and GitHub projects with purely AI-generated commit messages, making it impossible to assess candidates' true abilities. This trend undermines the hiring process by erasing candidates' individuality and authenticity, forcing employers to rely on generic, impersonal materials that reveal nothing about a person's actual skills or character. MacWright's blog post 'Accidental Anonymity' highlights that LLM-generated content creates a 'perfected, generic, impersonal' resume that tells nothing about the person except their tool usage.

rss · Simon Willison · Jun 24, 18:13

**Background**: Large Language Models (LLMs) like GPT-4 can generate human-like text, including resumes, cover letters, and code. Job seekers increasingly use these tools to automate application materials, but over-reliance can produce content that lacks personal voice and genuine experience.

**Tags**: `#AI`, `#careers`, `#hiring`, `#LLM`, `#authenticity`

---

<a id="item-8"></a>
## [Why I Stopped Trusting AI Benchmarks and Built My Own Eval](https://www.reddit.com/r/MachineLearning/comments/1uf53un/i_stopped_trusting_model_benchmarks_and_started/) ⭐️ 8.0/10

A practitioner describes losing faith in published AI benchmarks due to vendor-controlled tests (e.g., Kimi K2.7 Code's own benchmarks) and self-reported parameters (e.g., GLM-5.2), and built a custom eval set of 240 tasks from real production traffic to evaluate models on their own distribution. This highlights a critical flaw in relying on public benchmarks for model selection, as vendor-designed tests may not reflect real-world performance, and independent evaluations like DeepSWE are rare. The approach of using frozen, workload-specific eval sets could become a best practice for production deployments. The author routes all candidate models through GPTProto to hold provider variance constant, and found that the best model on their set often differs from public leaderboards, with smaller performance gaps and one model having a dangerous failure mode on edge cases.

reddit · r/MachineLearning · /u/Additional-Engine402 · Jun 25, 09:22

**Background**: AI model benchmarks are widely used to compare model capabilities, but many are created by vendors themselves (e.g., Kimi Code Bench) or rely on self-reported parameters, leading to potential bias. Independent benchmarks like DeepSWE aim to provide unbiased comparisons but are less common. The Artificial Analysis Intelligence Index is a third-party suite but still uses self-reported model parameters.

<details><summary>References</summary>
<ul>
<li><a href="https://www.reddit.com/r/LLMDevs/comments/1u46zm2/kimi_k27_code_is_less_interesting_as_a_new_coder/">Kimi K2.7 Code is less interesting as a new coder model and ... - Reddit</a></li>
<li><a href="https://artificialanalysis.ai/">AI Model & API Providers Analysis | Artificial Analysis</a></li>
<li><a href="https://deepswe.datacurve.ai/">DeepSWE measures frontier coding agents on original, long-horizon...</a></li>

</ul>
</details>

**Discussion**: The Reddit discussion likely includes agreement on the need for custom evals, skepticism about vendor benchmarks, and debate on the trade-offs between standardized benchmarks and workload-specific testing. Some may argue that public benchmarks still serve as useful filters despite their flaws.

**Tags**: `#AI benchmarks`, `#model evaluation`, `#machine learning`, `#coding benchmarks`, `#vendor bias`

---

<a id="item-9"></a>
## [HDD-RoPE: High-Dimensional Dynamic Rotary Positional Embedding](https://www.reddit.com/r/MachineLearning/comments/1uelcm9/high_dimensional_dynamic_rotary_positional/) ⭐️ 8.0/10

The author introduces HDD-RoPE, a novel positional embedding that uses cumulative matrix products to create high-dimensional, data-dependent rotations, and shows it achieves faster convergence than xPos on the TinyStories dataset. This work challenges the standard RoPE assumption of 2D rotations per token pair, potentially enabling transformers to learn richer positional structures like paragraphs or sentences, which could improve performance on long-range dependency tasks. HDD-RoPE splits queries and keys into chunks of arbitrary size (e.g., 4) and applies rotations along multiple axes (e.g., 6 for chunk size 4), with rotation amounts learned dynamically from layer activations. The open-source repository provides full math and replication code.

reddit · r/MachineLearning · /u/mikayahlevi · Jun 24, 18:16

**Background**: Rotary Position Embedding (RoPE) encodes token positions by rotating pairs of query/key elements at fixed rates, enabling relative position awareness. xPos is an extension that improves extrapolation. HDD-RoPE generalizes RoPE to higher-dimensional rotations that are data-dependent.

<details><summary>References</summary>
<ul>
<li><a href="https://www.reddit.com/r/MachineLearning/comments/1uelcm9/high_dimensional_dynamic_rotary_positional/">High Dimensional, Dynamic Rotary Positional Embedding [P] - Reddit</a></li>
<li><a href="https://kaggle.curtischong.me/techniques/xpos-positional-encoding">xpos positional encoding</a></li>

</ul>
</details>

**Discussion**: The Reddit discussion includes technical questions about the mathematical formulation and comparisons with other positional embeddings. The author actively responds, clarifying details about the cumulative matrix product and training hyperparameters.

**Tags**: `#positional embedding`, `#transformer`, `#deep learning`, `#NLP`, `#RoPE`

---

<a id="item-10"></a>
## [DeepSWE: A Contamination-Free Benchmark for AI Coding Agents](https://www.reddit.com/r/MachineLearning/comments/1ue0hlp/deepswe_new_benchmark_looking_at_how_well_todays/) ⭐️ 8.0/10

DeepSWE is a new open-source benchmark that evaluates frontier AI coding agents using tasks written from scratch across 91 repositories and 5 languages, ensuring no contamination from pretraining data. This benchmark addresses critical flaws in existing benchmarks like SWE-bench, such as data contamination and lack of diversity, providing a more realistic measure of how well AI agents handle real-world software engineering tasks. DeepSWE tasks require 5.5x more code and ~2x more output tokens than SWE-bench Pro, yet prompts are about half the length; verifiers are hand-written to test behavior rather than implementation details.

reddit · r/MachineLearning · /u/we_are_mammals · Jun 24, 02:03

**Background**: Existing benchmarks for AI coding agents, such as SWE-bench, often suffer from data contamination because tasks are adapted from existing commits or pull requests that models may have seen during pretraining. This leads to inflated performance scores that do not reflect true generalization. DeepSWE avoids this by creating entirely new tasks, and also increases diversity by spanning multiple repositories and programming languages.

<details><summary>References</summary>
<ul>
<li><a href="https://deepswe.datacurve.ai/">DeepSWE measures frontier coding agents on original, long-horizon...</a></li>
<li><a href="https://deepswe.net/">DeepSWE Benchmark : GPT vs Claude for Agentic Coding</a></li>
<li><a href="https://deepswe.lol/">DeepSWE — Long-Horizon Software Engineering Benchmark</a></li>

</ul>
</details>

**Discussion**: The Reddit discussion highlights the benchmark's novelty in addressing contamination, with users debating the trade-offs between task complexity and evaluation cost. Some express skepticism about whether hand-written verifiers scale, while others praise the focus on real-world complexity.

**Tags**: `#benchmark`, `#AI coding agents`, `#software engineering`, `#machine learning`, `#evaluation`

---

<a id="item-11"></a>
## [Half-Life 2 Now Playable in a Browser via WebAssembly](https://hl2.slqnt.dev/) ⭐️ 7.0/10

Half-Life 2 has been ported to run directly in a web browser using WebAssembly, allowing players to experience the full game without any downloads or plugins. This demonstrates the growing capability of WebAssembly to handle complex, resource-intensive applications like AAA games, potentially opening the door for more legacy games to become accessible on the web. The port is based on the original game binaries and uses WebGL for rendering, though some shaders (e.g., character eyes) are missing, resulting in less accurate visuals compared to the native version.

hackernews · panza · Jun 25, 06:00 · [Discussion](https://news.ycombinator.com/item?id=48669534)

**Background**: WebAssembly (WASM) is a low-level binary format that runs in modern browsers at near-native speed, enabling applications like games to be ported from native code. Previous examples include Quake 3 and Unreal Tournament in the browser.

<details><summary>References</summary>
<ul>
<li><a href="https://news.ycombinator.com/item?id=48669534">Half - Life 2 in a Browser | Hacker News</a></li>

</ul>
</details>

**Discussion**: Commenters expressed excitement about the technical achievement, with some noting that it allows macOS users to play the game despite Valve dropping 32-bit support. Others raised legal concerns about redistribution of copyrighted assets.

**Tags**: `#webassembly`, `#gaming`, `#porting`, `#browser`, `#retro`

---

<a id="item-12"></a>
## [LuaJIT 3.0 Proposes C-Style Syntax Extensions](https://github.com/LuaJIT/LuaJIT/issues/1475) ⭐️ 7.0/10

LuaJIT 3.0 proposes syntax extensions including C-style operators (e.g., &&, ||) and compound assignments (e.g., +=, -=), as detailed in GitHub issue #1475. This proposal sparks debate on Lua's language identity and backward compatibility, potentially affecting the Lua ecosystem and users who rely on LuaJIT for performance. The proposal includes compound assignment operators and alternative syntax for logical operators, but critics argue it adds complexity without solving real problems. LuaJIT currently targets Lua 5.1, and these changes would deviate from standard Lua.

hackernews · phreddypharkus · Jun 25, 00:41 · [Discussion](https://news.ycombinator.com/item?id=48667336)

**Background**: LuaJIT is a just-in-time compiler for Lua, known for its high performance. Lua itself is a lightweight scripting language used in games and embedded systems. The proposal aims to modernize syntax but risks fragmenting the already diverse Lua ecosystem, which includes variants like Luau.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/LuaJIT">LuaJIT</a></li>
<li><a href="https://en.wikipedia.org/wiki/Compound-assignment_operators">Compound-assignment operators</a></li>

</ul>
</details>

**Discussion**: Community comments are mixed: some welcome compound assignments but oppose C-style logical operators, arguing they make Lua lose its identity. Others point out that LuaJIT is catching up to Lua 5.3 features, but the piecemeal approach is confusing.

**Tags**: `#LuaJIT`, `#syntax`, `#programming languages`, `#compiler`

---

<a id="item-13"></a>
## [Blogging Can Just Be Stating the Obvious](https://blog.jim-nielsen.com/2026/blogging-stating-the-obvious/) ⭐️ 7.0/10

Jim Nielsen reflects on the value of blogging by stating what seems obvious to oneself but not to others, and the community validates this insight with strong engagement. This article challenges the pressure to produce novel content, encouraging more people to share their knowledge and perspectives, which can foster a richer and more inclusive blogging ecosystem. The post scored 7.0/10 with 245 points and 87 comments, indicating high community resonance. The author emphasizes the 'curse of knowledge' and the importance of consistency in blogging.

hackernews · Curiositry · Jun 24, 23:46 · [Discussion](https://news.ycombinator.com/item?id=48666927)

**Background**: Blogging often faces the pressure to be groundbreaking, but the 'curse of knowledge' makes experts forget what beginners don't know. This post argues that stating the obvious can be valuable for those who haven't encountered that idea before.

**Discussion**: Commenters largely agree, sharing personal experiences: one mathematician notes losing enthusiasm for proving basic theorems, while another highlights that there's always a new cohort unaware of known ideas. The sentiment is supportive, with many appreciating the reminder to share obvious insights.

**Tags**: `#blogging`, `#writing`, `#knowledge sharing`, `#community`

---

<a id="item-14"></a>
## [Nvidia's 45°C Cooling Slashes Data Center Water Use](https://blogs.nvidia.com/blog/liquid-cooling-ai-factories/) ⭐️ 7.0/10

Nvidia announced a closed-loop liquid cooling design for AI data centers that uses coolant at up to 45°C, enabling near-zero on-site water consumption by eliminating chillers and cooling towers. This innovation addresses the massive water consumption of AI data centers—conventional systems can use 2.6 million gallons per megawatt annually—and aligns with growing environmental regulations and sustainability goals. The system uses direct-to-chip liquid cooling with coolant at up to 45°C (113°F), warmer than a hot tub, and relies on ambient air in suitable climates to dissipate heat without water evaporation.

hackernews · nitin_flanker · Jun 24, 14:10 · [Discussion](https://news.ycombinator.com/item?id=48660178)

**Background**: Data centers consume enormous amounts of water for cooling, with Water Usage Effectiveness (WUE) measuring efficiency. Traditional cooling towers evaporate water to remove heat, while liquid cooling typically uses lower-temperature coolants and still requires chillers. Nvidia's approach raises the coolant temperature to a point where air cooling alone can handle heat rejection in many geographies, drastically cutting water use.

<details><summary>References</summary>
<ul>
<li><a href="https://www.guru3d.com/story/nvidia-unveils-liquid-cooling-design-for-ai-data-centers/">NVIDIA Unveils 45 ° C Liquid Cooling Design for AI Data Centers</a></li>
<li><a href="https://www.businesstoday.in/technology/news/story/nvidia-says-its-new-liquid-cooling-system-can-reduce-water-and-energy-use-for-ai-data-centre-538735-2026-06-23">NVIDIA says its new liquid cooling system can... - BusinessToday</a></li>
<li><a href="https://schemaninja.com/nvidia-says-its-hotter-than-a-hot-tub/">Nvidia Says Its "Hotter Than a Hot Tub" Cooling Can Cut AI Data ...</a></li>

</ul>
</details>

**Discussion**: Commenters noted that the design's effectiveness depends on geography—requiring reliably cool outdoor air—and raised concerns about dumping waste heat into the environment. Some suggested district heating as a synergy, while others questioned why the temperature is only 45°C and whether higher temperatures could enable even simpler air cooling.

**Tags**: `#data centers`, `#cooling`, `#Nvidia`, `#energy efficiency`, `#water conservation`

---

<a id="item-15"></a>
## [Zombie Unicorns Haunt Silicon Valley](https://www.economist.com/business/2026/06/21/zombie-unicorns-are-haunting-silicon-valley) ⭐️ 7.0/10

The Economist reports that many once-highly-valued startups, dubbed 'zombie unicorns,' are struggling as rising interest rates expose overinflated venture capital valuations. This trend signals a potential correction in the startup ecosystem, affecting investors, employees, and the broader tech industry by forcing unsustainable companies to downsize or shut down. Zombie unicorns are firms once valued at over $1 billion but now struggle to justify that valuation due to lack of profitability and higher interest rates. Examples like Cameo, valued at $1 billion by SoftBank, illustrate the disconnect between VC valuations and actual business performance.

hackernews · andsoitis · Jun 25, 02:16 · [Discussion](https://news.ycombinator.com/item?id=48668020)

**Background**: A 'unicorn' is a private startup valued at over $1 billion, often based on growth potential rather than current profits. Venture capitalists use methods like the VC Method, which discounts future exit values, to justify high valuations. When interest rates rise, the cost of capital increases, making it harder for unprofitable startups to raise additional funding, turning them into 'zombies'—companies that can only survive by cutting costs.

<details><summary>References</summary>
<ul>
<li><a href="https://www.economist.com/business/2026/06/21/zombie-unicorns-are-haunting-silicon-valley">Zombie unicorns are haunting Silicon Valley</a></li>
<li><a href="https://www.wallstreetprep.com/knowledge/vc-valuation-6-steps-to-valuing-early-stage-firms-excel-template/">Venture Capital Valuation | VC Method Template + Example</a></li>

</ul>
</details>

**Discussion**: Commenters debate the validity of VC valuations, with one comparing them to gambling payouts and noting that valuations are based on low-confidence growth predictions. Another points out that profitable companies like Cameo can survive, but investors may not see expected returns. A third observes that many startups raised mega rounds before rate hikes and now tread water by cutting headcount.

**Tags**: `#venture capital`, `#startups`, `#economics`, `#Silicon Valley`

---

<a id="item-16"></a>
## [RubyLLM: A Unified Ruby Framework for Major AI Providers](https://rubyllm.com/) ⭐️ 7.0/10

RubyLLM is a Ruby framework that provides a unified API for major AI providers including OpenAI, Anthropic, and local Ollama models, allowing developers to build AI-powered applications with a single, elegant interface. This framework simplifies AI integration for Ruby developers, reducing boilerplate and enabling rapid prototyping, similar to how Rails revolutionized web development. It has gained strong community traction with 392 points and 68 comments on Hacker News. RubyLLM supports multiple AI providers through a consistent API, but community reports indicate cache issues with some providers like xAI, and maintenance concerns due to slow PR responses and merged 'vibe coded' pull requests.

hackernews · doener · Jun 24, 14:41 · [Discussion](https://news.ycombinator.com/item?id=48660711)

**Background**: RubyLLM is an open-source gem that abstracts away the differences between AI provider APIs, offering a Rails-like developer experience. It aims to be the go-to framework for adding AI capabilities to Ruby applications, competing with similar unified APIs like FastRouter and LiteRouter.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/crmne/ruby_llm">GitHub - crmne/ ruby _ llm : One delightful Ruby framework for every...</a></li>
<li><a href="https://rubyllm.com/">RubyLLM | One beautiful Ruby framework for all major AI providers.</a></li>
<li><a href="https://medium.com/airtribe/rubyllm-and-the-return-of-rails-superpower-notes-from-euruko-2025-b72eeeb6b185">RubyLLM and the Return of Rails’ Superpower — Notes... | Medium</a></li>

</ul>
</details>

**Discussion**: Community sentiment is largely positive, with users praising the API design and ease of use. However, some express frustration with cache reliability and maintainer responsiveness, noting that PRs are sometimes ignored or overwritten by 'vibe coded' changes. There is excitement for the upcoming 2.0 release.

**Tags**: `#Ruby`, `#AI`, `#LLM`, `#framework`, `#API`

---

<a id="item-17"></a>
## [PR Spam in Open Source Echoes Early 2000s Email Spam](https://www.greptile.com/blog/prs-on-openclaw) ⭐️ 7.0/10

A new article draws a direct parallel between modern pull request spam in open-source projects and the email spam epidemic of the early 2000s, arguing that similar filtering and reputation-based solutions are needed. This analogy highlights a growing problem that threatens the sustainability of open-source maintenance, as maintainers are overwhelmed by low-quality, automated PRs. Addressing PR spam is critical to preserving the health and productivity of open-source communities. GitHub recently added configurable PR limits for maintainers, and community projects like PR Captcha and Fossier are experimenting with reputation-based filtering. The article notes that unlike email spam, PR spam targets individual repositories rather than IP addresses, making reputation systems more complex.

hackernews · dakshgupta · Jun 24, 14:32 · [Discussion](https://news.ycombinator.com/item?id=48660579)

**Background**: In the early 2000s, email spam was rampant, leading to the development of filtering techniques like Bayesian filters and sender reputation systems. Today, open-source projects face a similar deluge of spam pull requests, often generated by automated tools or AI, which waste maintainer time and degrade project quality.

<details><summary>References</summary>
<ul>
<li><a href="https://dev.to/ryan_m_823cbee9f96a9dee29/pr-spam-the-modern-echo-of-early-2000s-email-spam-l1h">PR Spam : The Modern Echo of Early 2000s Email... - DEV Community</a></li>
<li><a href="https://github.com/PThorpe92/fossier">GitHub - PThorpe92/fossier: Vouch-compatible PR - spam reduction...</a></li>
<li><a href="https://socket.dev/blog/express-js-spam-prs-commoditization-of-open-source">Express.js Spam PRs Incident Highlights the Commoditization ..</a></li>

</ul>
</details>

**Discussion**: Commenters largely agree with the analogy, with some noting that email spam was solved by organizational reputation, which is harder to apply to individual PRs. Others shared tools like PR Captcha and GitHub's new PR limits as potential solutions, while one user lamented that many projects now ignore contributions due to spam overload.

**Tags**: `#open-source`, `#spam`, `#maintainer-tools`, `#community`

---

<a id="item-18"></a>
## [Xteink X4: Low-Cost Open E-Ink Reader](https://blog.omgmog.net/post/xteink-x4-e-ink-reader/) ⭐️ 7.0/10

The Xteink X4 is a low-cost, open e-ink reader that uses a microcontroller and offers WiFi-based book transfer via an HTTP server, praised for its simplicity but criticized for lacking a frontlight and poor sunlight readability. This device demonstrates that a microcontroller is sufficient for an e-reader, challenging proprietary ecosystems like Kindle and Kobo by offering an open, hackable alternative at a fraction of the cost. The X4 lacks a frontlight, making it hard to read in direct sunlight, and its screen uses older e-ink technology with lower contrast. An upcoming X4 S model is expected to add a frontlight and run Android.

hackernews · felixdoerp · Jun 24, 16:35 · [Discussion](https://news.ycombinator.com/item?id=48662381)

**Background**: E-ink displays use microcapsules filled with charged particles to create text, requiring no power to maintain an image but needing light to read. Traditional e-readers like Kindle and Kobo use frontlights for illumination, while the X4 relies on ambient light.

<details><summary>References</summary>
<ul>
<li><a href="https://mashable.com/roundup/best-e-readers-2026-tested">The 9 best e-readers of 2026: I compare Kindle, Kobo, and iPad</a></li>
<li><a href="https://www.reddit.com/r/eink/comments/132cu7s/how_exactly_does_epaper_work/">How exactly does e-paper work? : r/eink - Reddit</a></li>

</ul>
</details>

**Discussion**: Community members appreciate the X4's simplicity and WiFi transfer, with some using custom firmware like CrossPoint. However, many criticize the lack of a frontlight and poor sunlight readability, and some express hope for the upcoming X4 S model with a frontlight and Android.

**Tags**: `#e-ink`, `#e-reader`, `#hardware`, `#open-source`, `#microcontroller`

---

<a id="item-19"></a>
## [Datasette 1.0a35 Adds Create/Alter Table JSON APIs](https://simonwillison.net/2026/Jun/23/datasette/#atom-everything) ⭐️ 7.0/10

Datasette 1.0a35 introduces new JSON APIs for creating and altering tables, allowing schema management directly through the interface. It also includes stable template context documentation for custom templates. This release transforms Datasette from a read-only exploration tool into a full-fledged data management platform, enabling users to modify database schemas without external tools. It significantly expands Datasette's utility for data scientists and developers working with SQLite databases. The create table API supports defining columns, primary keys, custom types, NOT NULL constraints, defaults, expression defaults, and single-column foreign keys. The alter table API allows adding, renaming, reordering, dropping columns, changing types, defaults, constraints, primary keys, foreign keys, and renaming the table, plus a drop table button.

rss · Simon Willison · Jun 23, 21:34

**Background**: Datasette is an open-source tool for exploring and publishing SQLite databases. Previously, schema changes required external SQLite clients or manual SQL commands. This alpha release adds write APIs that make Datasette a more interactive data management tool.

<details><summary>References</summary>
<ul>
<li><a href="https://docs.datasette.io/en/latest/json_api.html?highlight=pagination">JSON API - Datasette documentation</a></li>
<li><a href="https://simonwillison.net/2022/Nov/9/designing-a-write-api-for-datasette/">Designing a write API for Datasette - Simon Willison's Weblog</a></li>
<li><a href="https://simonwillison.net/2026/jun/23/datasette/">Release: datasette 1.0a35 | Simon Willison’s Weblog</a></li>

</ul>
</details>

**Tags**: `#datasette`, `#release`, `#data tools`, `#JSON API`

---

<a id="item-20"></a>
## [Curated OCR Models Hub Launched on Papers with Code](https://www.reddit.com/r/MachineLearning/comments/1ueiam6/find_the_best_opensource_ocr_models_in_one_place/) ⭐️ 7.0/10

A curated page on Papers with Code now lists top open-source OCR models and benchmarks, including Baidu's Unlimited OCR (3B parameters with R-SWA) and Mistral's OCR 4 API. This centralizes fragmented OCR resources, helping developers easily find and compare models for document digitization, which is critical for AI agent workflows like agentic RAG. Top recommended benchmarks are OlmOCRBench (by Ai2) and OmniDocBench (by Shanghai AI Lab); top models include Chandra OCR 2 (open-source) and Mistral OCR v4 (API).

reddit · r/MachineLearning · /u/NielsRogge · Jun 24, 16:26

**Background**: OCR (Optical Character Recognition) converts scanned documents and PDFs into machine-readable text. Recent open-source releases from Baidu and Mistral have increased interest in using OCR for AI agent data ingestion, especially for converting messy PDFs into structured Markdown for retrieval-augmented generation (RAG).

<details><summary>References</summary>
<ul>
<li><a href="https://www.emergentmind.com/topics/reference-sliding-window-attention-r-swa">Reference Sliding Window Attention ( R - SWA )</a></li>
<li><a href="https://en.wikipedia.org/wiki/DeepSeek">DeepSeek</a></li>

</ul>
</details>

**Tags**: `#OCR`, `#Open-Source`, `#AI Models`, `#Document Digitization`, `#Benchmarks`

---

<a id="item-21"></a>
## [MuJoFil: GPU-Accelerated Simulator for Vision RL](https://www.reddit.com/r/MachineLearning/comments/1uemrch/mujoco_derived_simulator_for_high_fidelity_vision/) ⭐️ 7.0/10

A new open-source simulator called MuJoFil combines NVIDIA's Newton physics engine with Google's Filament render engine to enable GPU-accelerated, high-fidelity vision-based reinforcement learning training. This addresses a key limitation of MuJoCo for vision-based RL by providing GPU-native parallel simulation and high-quality rendering, making it more accessible than proprietary solutions like NVIDIA Isaac. MuJoFil supports PBR textures and can import environments in GLB, OpenUSD, and other formats from online sources like Sketchfab. It is available as two PyPI packages: mujofil (CPU) and mujofil-warp (GPU with CUDA).

reddit · r/MachineLearning · /u/MT1699 · Jun 24, 19:07

**Background**: MuJoCo is a popular physics simulator for robotics, but its CPU-based design limits parallelization for vision-based RL. MJX accelerates MuJoCo on GPU but lacks a rendering engine for visual tasks. NVIDIA Isaac offers high-fidelity simulation but requires powerful GPUs and a license. MuJoFil aims to fill this gap by combining GPU-native physics (Newton) with a modern renderer (Filament) in an open-source package.

<details><summary>References</summary>
<ul>
<li><a href="https://developer.nvidia.com/newton-physics">Newton Physics Engine | NVIDIA Developer</a></li>
<li><a href="https://github.com/google/filament">google / filament : Filament is a real-time physically based rendering ...</a></li>
<li><a href="https://mujoco.readthedocs.io/en/3.9.0/mjx.html">MuJoCo XLA ( MJX ) - MuJoCo Documentation</a></li>

</ul>
</details>

**Tags**: `#reinforcement learning`, `#simulation`, `#GPU`, `#MuJoCo`, `#open-source`

---

<a id="item-22"></a>
## [LLM Inference Pricing Comparison Reveals Caching Cost Surprises](https://www.reddit.com/r/MachineLearning/comments/1ueavxn/i_compiled_llm_inference_pricing_across_7/) ⭐️ 7.0/10

A Reddit user compiled and compared LLM inference pricing across 7 providers including OpenRouter, DeepSeek, Together AI, Fireworks, and Groq, highlighting dramatic differences in cached input costs that can make cache hits tens of times cheaper than misses. This matters because for developers building agents, RAG pipelines, or multi-turn conversations, caching policy can be more important than headline token price, directly impacting production cost optimization. The spreadsheet tracks input/output token pricing, context windows, cached input pricing, and provider-specific differences, but does not include latency, throughput, or quantization details. The same model can vary multiple times in cost across providers.

reddit · r/MachineLearning · /u/Technomadlyf · Jun 24, 11:28

**Background**: LLM inference pricing typically charges per token for input and output. Caching allows providers to reuse previously computed key-value pairs for repeated prefixes, offering discounts (often 50–90% off) on cached tokens. This is especially relevant for applications with large system prompts or reusable context, where cache hit rates significantly affect total cost.

<details><summary>References</summary>
<ul>
<li><a href="https://introl.com/blog/prompt-caching-infrastructure-llm-cost-latency-reduction-guide-2025">Prompt Caching Infrastructure | Introl Blog</a></li>
<li><a href="https://machinelearningmastery.com/the-complete-guide-to-inference-caching-in-llms/">The Complete Guide to Inference Caching in LLMs</a></li>
<li><a href="https://solana.garden/guides/llm-prompt-caching-explained/">LLM Prompt Caching Explained: Prefix Reuse, Cost... | Solana Garden</a></li>

</ul>
</details>

**Discussion**: The Reddit discussion was substantive, with users validating the importance of caching costs and sharing additional metrics like throughput and cold-start times that are hard to compare. Some noted that provider documentation on caching is often unclear.

**Tags**: `#LLM`, `#pricing`, `#caching`, `#inference`, `#cost optimization`

---

<a id="item-23"></a>
## [Are ML teams testing model security in production?](https://www.reddit.com/r/MachineLearning/comments/1uddtws/are_model_security_risks_extraction_poisoning/) ⭐️ 7.0/10

A Reddit post questions whether machine learning teams are actually testing model security risks like extraction and poisoning in production, noting that security review for models lags behind traditional software. This highlights a critical gap in ML deployment practices, as adversarial attacks can lead to data leakage, model theft, or compromised predictions, affecting trust and safety in AI systems. The post specifically mentions model extraction (where an attacker reconstructs a model via queries) and model poisoning (where malicious data corrupts training) as under-tested risks.

reddit · r/MachineLearning · /u/Xorphian · Jun 23, 10:52

**Background**: Model extraction attacks allow adversaries to steal a model's functionality by querying it, while model poisoning attacks inject harmful data into training to alter behavior. Adversarial testing systematically evaluates models against such malicious inputs, but many teams skip it before deployment.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Adversarial_machine_learning">Adversarial machine learning - Wikipedia</a></li>
<li><a href="https://developers.google.com/machine-learning/guides/adv-testing">Adversarial Testing for Generative AI | Machine Learning</a></li>
<li><a href="https://www.csoonline.com/article/570555/how-data-poisoning-attacks-corrupt-machine-learning-models.html">What is data poisoning ? Attacks thatcorrupt machine learning models</a></li>

</ul>
</details>

**Tags**: `#ML Security`, `#Adversarial Testing`, `#Model Deployment`, `#Production Risks`

---

<a id="item-24"></a>
## [Claude Code v2.1.187: Sandbox Credentials Blocking and Bug Fixes](https://github.com/anthropics/claude-code/releases/tag/v2.1.187) ⭐️ 6.0/10

Anthropic released Claude Code v2.1.187, introducing a sandbox.credentials setting to block sandboxed commands from reading credential files and secret environment variables, along with org-configured model restrictions, mouse click support for select menus, and 21 bug fixes. This release addresses a critical security vulnerability (SOCKS5 null-byte flaw) that could expose AWS credentials, GitHub tokens, and source code, making it essential for organizations using Claude Code in development environments. The org model restrictions also give enterprises more control over which AI models their teams can use. The sandbox.credentials setting blocks access to common credential files and secret environment variables, and the fix for remote MCP tool calls now aborts after 5 minutes of no response instead of blocking indefinitely. Additionally, the update fixes Korean/CJK text mojibake in terminals and improves subagent depth tracking.

github · ashwin-ant · Jun 23, 21:03

**Background**: Claude Code is an agentic coding tool from Anthropic that runs with elevated permissions on developer machines, enabling it to execute commands and access files. The sandbox feature is designed to isolate untrusted commands, but a SOCKS5 null-byte flaw in versions 2.0.24–2.1.89 allowed sandboxed commands to bypass restrictions and steal credentials. This release closes that vulnerability and adds enterprise model controls.

<details><summary>References</summary>
<ul>
<li><a href="https://howtoclaude.dev/claude-code-2-1-187-ships-critical-sandbox-credential-protections-and-enterprise-model-controls/">Claude Code 2.1.187 Ships Critical Sandbox Credential Protections...</a></li>
<li><a href="https://pasqualepillitteri.it/en/news/3035/claude-code-sandbox-bypass-socks5-credentials">Claude Code Sandbox Bypass: SOCKS5 Exposed Credentials for...</a></li>
<li><a href="https://aiweekly.co/alerts/claude-code-socks5-flaw-enables-full-sandbox-data-theft">Claude Code SOCKS5 flaw enables full sandbox data theft | AI Weekly</a></li>

</ul>
</details>

**Tags**: `#claude-code`, `#release`, `#security`, `#bug-fix`

---

<a id="item-25"></a>
## [Google Adds Computer Use to Gemini 3.5 Flash](https://blog.google/innovation-and-ai/models-and-research/gemini-models/introducing-computer-use-gemini-3-5-flash/) ⭐️ 6.0/10

Google has integrated computer use capabilities directly into Gemini 3.5 Flash, allowing the model to interact with graphical user interfaces by interpreting screenshots and executing actions. This feature was previously only available as a standalone model. This advancement enables AI agents to automate complex desktop tasks, potentially disrupting traditional robotic process automation (RPA) tools. However, user reports of frequent errors and limitations raise concerns about reliability for production use. The computer use feature is now a built-in tool in Gemini 3.5 Flash, delivering Google's best performance for agentic computer use tasks. Community comments reveal issues such as the model giving up on simple data extraction tasks and executing unintended git commands.

hackernews · swolpers · Jun 24, 17:21 · [Discussion](https://news.ycombinator.com/item?id=48662999)

**Background**: Large language models (LLMs) like Gemini are trained on vast text data to generate human-like responses. Computer use extends this by enabling the model to visually interpret screen content and perform actions, mimicking human interaction with software. This capability is key for building autonomous AI agents that can automate workflows.

<details><summary>References</summary>
<ul>
<li><a href="https://blog.google/innovation-and-ai/models-and-research/gemini-models/introducing-computer-use-gemini-3-5-flash/">Introducing computer use in Gemini 3 . 5 Flash</a></li>
<li><a href="https://deepmind.google/models/gemini/flash/">Gemini 3 . 5 Flash — Google DeepMind</a></li>
<li><a href="https://9to5google.com/2026/06/24/gemini-chrome-select-screen/">Gemini in Chrome adds ‘Select from screen’ tool</a></li>

</ul>
</details>

**Discussion**: User feedback is mixed: some report the model giving up on simple tasks or making destructive errors like running `git reset --hard` unexpectedly. Others express frustration over missing features like MCP support and question the reliability compared to competitors. Overall sentiment leans skeptical about practical usefulness.

**Tags**: `#AI`, `#Gemini`, `#LLM`, `#Google`, `#computer use`

---

<a id="item-26"></a>
## [Simon Willison Converts MDN Browser Compat Data to SQLite](https://simonwillison.net/2026/Jun/24/browser-compat-db/#atom-everything) ⭐️ 6.0/10

Simon Willison created a SQLite database from MDN's browser compatibility data using AI-generated scripts and hosted it on GitHub with open CORS headers, enabling direct querying via Datasette Lite. This project makes MDN's comprehensive browser compatibility data easily queryable offline or programmatically, benefiting developers who need to check feature support across browsers without relying on MDN's web interface. The ~66MB SQLite database is built by a Claude Code-generated script using sqlite-utils, and a GitHub Actions workflow pushes it to an orphan branch for CDN hosting with open CORS headers.

rss · Simon Willison · Jun 24, 23:59

**Background**: MDN (Mozilla Developer Network) maintains a comprehensive browser compatibility data repository (mdn/browser-compat-data) used by web developers to check which browser versions support specific web features. SQLite is a lightweight, file-based database engine. CORS headers allow web applications to access resources from different origins, enabling tools like Datasette Lite to load the database directly in the browser.

<details><summary>References</summary>
<ul>
<li><a href="https://developer.mozilla.org/en-US/blog/introducing-mdn-mcp-server/">Introducing the MDN MCP server - MDN Web Docs</a></li>
<li><a href="https://github.com/mdn/mcp">MDN's prototype MCP server - GitHub</a></li>
<li><a href="https://sqlite-utils.datasette.io/">sqlite - utils</a></li>

</ul>
</details>

**Tags**: `#browser-compat`, `#sqlite`, `#mdn`, `#developer-tools`, `#data-engineering`

---

<a id="item-27"></a>
## [OPFS + Pyodide Test Harness for Persistent SQLite](https://simonwillison.net/2026/Jun/23/opfs-pyodide/#atom-everything) ⭐️ 6.0/10

Simon Willison released a test harness that combines the Origin Private File System (OPFS) with Pyodide to enable persistent SQLite database storage directly in the browser. This experiment could allow Datasette Lite and other browser-based Python applications to read and write persistent SQLite files on the user's local file system, significantly expanding their offline and data-editing capabilities. The test harness is a playground UI built with Claude Code for web, designed to test OPFS support across different browsers. OPFS is part of the File System API and provides a private storage area per origin.

rss · Simon Willison · Jun 23, 18:58

**Background**: Pyodide is a port of CPython to WebAssembly, enabling Python to run in the browser. Datasette Lite uses Pyodide to run the full Datasette application client-side. OPFS allows web applications to store data persistently in a sandboxed file system, but browser support has been inconsistent.

<details><summary>References</summary>
<ul>
<li><a href="https://pyodide.org/">Pyodide</a></li>
<li><a href="https://github.com/simonw/datasette-lite">GitHub - simonw/ datasette - lite : Datasette running in your browser...</a></li>

</ul>
</details>

**Tags**: `#pyodide`, `#webassembly`, `#sqlite`, `#browsers`, `#datasette-lite`

---