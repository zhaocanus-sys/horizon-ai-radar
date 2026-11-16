---
layout: default
title: "Horizon Summary: 2026-11-16 (EN)"
date: 2026-11-16
lang: en
---

> From 40 items, 27 important content pieces were selected

---

1. [MIT researchers use GPT-6 Astra to directly edit Qwen model weights, boosting math score from 7.9% to 48.1%](#item-1) ⭐️ 9.0/10
2. [Universal XSS in uBlock Origin via website-driven element picker](#item-2) ⭐️ 8.0/10
3. [Alibaba's Qwen Team Releases Qwen4-Max Flagship LLM](#item-3) ⭐️ 8.0/10
4. [Steve Blank Analyzes Nvidia's Strategic Threats as Customers Become Competitors](#item-4) ⭐️ 8.0/10
5. [MIT's 'How to Make Almost Anything' course sparks debate on breadth vs. depth](#item-5) ⭐️ 7.0/10
6. [Old Bitly Links Hijacked, Raising Concerns About URL Shortener Risks](#item-6) ⭐️ 7.0/10
7. [Tor Project releases emergency 0.4.9.17 security fix for ongoing DDoS attack](#item-7) ⭐️ 7.0/10
8. [Protomaps Makes Self-Hosting Map Tiles Cheap and Easy](#item-8) ⭐️ 7.0/10
9. [Internet Archive Preserves 30 Years of Salon Journalism](#item-9) ⭐️ 7.0/10
10. [MacBook Pro OLED PWM flicker issue raises usability concerns](#item-10) ⭐️ 7.0/10
11. [Crows make decisions twice as fast as humans, study finds](#item-11) ⭐️ 7.0/10
12. [Microsoft 365 outage linked to chlorine gas poisoning at German hotel](#item-12) ⭐️ 7.0/10
13. [Clice v1.0 Released: A Modern C++ Language Server](#item-13) ⭐️ 7.0/10
14. [Apple launches 200,000-person US health AI study with OpenEvidence](#item-14) ⭐️ 7.0/10
15. [South Korea in Uproar Over AI-Assisted Exam Cheating Before CSAT](#item-15) ⭐️ 7.0/10
16. [Handwriting, as a Font: Web Tool Turns Samples into Custom Fonts](#item-16) ⭐️ 6.0/10
17. [WebGL Flight Simulator with Seed-Generated Terrain Impresses Hacker News](#item-17) ⭐️ 6.0/10
18. [Turbo Pascal's Tiny Footprint Sparks Debate on Modern Software Bloat](#item-18) ⭐️ 6.0/10
19. [Coles investigates cybersecurity incident affecting internal staff systems](#item-19) ⭐️ 6.0/10
20. [datasette-maplibre 0.1a0: AI-built geospatial plugin for Datasette](#item-20) ⭐️ 6.0/10
21. [Datasette 1.0a43 adds streaming output renderers and security fixes](#item-21) ⭐️ 6.0/10
22. [Datasette 0.65.6 Backports Security Fix for Unauthorized Database Downloads](#item-22) ⭐️ 6.0/10
23. [Export-Banned Nvidia Chips Power China's Top AI Models](#item-23) ⭐️ 6.0/10
24. [Reddit Post Highlights Rise of APIs Built for AI Agents](#item-24) ⭐️ 6.0/10
25. [Developer launches LogicLens, a real-time AI fact-checker for political speech](#item-25) ⭐️ 6.0/10
26. [Stanford HAI's 'Jagged Edge' AI Boom: Uneven Gains](#item-26) ⭐️ 6.0/10
27. [LLM agents given self-written notes repeat losing moves in gamebook experiment](#item-27) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [MIT researchers use GPT-6 Astra to directly edit Qwen model weights, boosting math score from 7.9% to 48.1%](https://www.reddit.com/r/artificial/comments/1xx4kit/weightspace_programming_an_llm_edited_another/) ⭐️ 9.0/10

MIT researchers (Rikiya Takehi, Jayden Teoh, Alex Zhang, Omar Khattab) had OpenAI's GPT-6 Astra directly edit the weights of a small Qwen model, touching only 0.016% of parameters to remove a repetition habit, which raised its math score from 7.9% to 48.1%. Three related papers on this weight-space programming method were posted to arXiv on November 6 (e.g., arXiv:2611.09382). This suggests a potential paradigm shift: instead of retraining or fine-tuning, an LLM can perform 'surgery' on another model's weights to fix behavioral pathologies, which could make model debugging more like code debugging. If it generalizes, it could lead to practical tools for model maintenance and change how we think about where capabilities are locked behind fixable quirks. The gain came mostly from fixing a bad habit rather than adding math knowledge: before the edit, 93% of the model's math answers hit the length limit, and after the edit, 33.1% did. On a small Gemma model that rarely repeated itself, there was no established math gain, and independent reproduction of the headline results is still pending.

reddit · r/artificial · /u/winer666 · Nov 15, 19:37

**Background**: Weight-space programming is a technique where a general-purpose LLM reads and writes another neural network's weights directly, without gradient descent or training data, similar to patching source code. Qwen is a family of open-weight large language models developed by Alibaba Cloud, and MATH-500 is a benchmark of 500 competition-level math problems used to evaluate AI models. This approach contrasts with traditional fine-tuning, which adjusts weights via gradient-based optimization on a dataset.

<details><summary>References</summary>
<ul>
<li><a href="https://agora-intelligence.com/en/blog/weight-space-programming-llm-edits-model-weights-removes-defects-limits/">AI rewriting another AI's weights fixes flaws, adds little</a></li>
<li><a href="https://blog.authon.dev/qwen3-5-0-8b-weight-space-programming-math-500">GPT-6 Astra Edited Qwen3.5-0.8B's Weights . | Authon Blog</a></li>
<li><a href="https://grokipedia.com/page/MATH-500_benchmark">MATH-500 (benchmark)</a></li>

</ul>
</details>

**Discussion**: The Reddit discussion includes scrutiny: Matthew Honnibal argued the claim was overstated, while Simon Willison reproduced weight editing locally with Qwen 3.8 27B on his laptop. Commenters debate whether this is a practical tool for model maintenance, a narrow trick for pathological repetition, or the start of something bigger.

**Tags**: `#LLM`, `#weight-editing`, `#model-interpretability`, `#research`, `#MIT`

---

<a id="item-2"></a>
## [Universal XSS in uBlock Origin via website-driven element picker](https://iter.ca/post/ubo-uxss/) ⭐️ 8.0/10

A technical disclosure revealed a universal XSS (UXSS) vulnerability in uBlock Origin caused by the website-driven element picker, allowing malicious sites to execute scripts in the context of other origins. The issue was fixed in uBlock Origin 1.75.4 and uBO Lite 2026.1110.1816. uBlock Origin is one of the most widely used security extensions, so a UXSS flaw undermines the very protection users rely on and could expose sensitive data across sites. The finding also highlights broader risks in how extensions inject UI into page DOMs, prompting discussion about browser architecture and extension security models. The vulnerability stems from the element picker's UI being placed in the website's DOM, which a malicious page can manipulate to achieve cross-origin script execution. Users should ensure they are running uBlock Origin 1.75.4 or higher, or uBO Lite 2026.1110.1816 or higher, to be protected.

hackernews · zaik · Nov 16, 02:04 · [Discussion](https://news.ycombinator.com/item?id=50513160)

**Background**: Universal XSS (UXSS) is a class of vulnerability where a flaw in the browser or an extension allows script execution across origins, bypassing the same-origin policy. uBlock Origin's element picker is a tool that helps users create filters by selecting page elements, and its interface is typically injected into the page's DOM. Extensions often use content scripts and isolated worlds to separate their code from page scripts, but UI injection can create attack surface if not properly isolated.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/gorhill/uBlock/wiki/Element-picker">Element picker · gorhill/uBlock Wiki · GitHub</a></li>
<li><a href="https://splorix.com/glossary/universal-xss-uxss">Universal XSS (UXSS): Browser Bugs That Break Site Isolation ...</a></li>
<li><a href="https://www.appsecatlas.com/docs/specialized/browser-extension-security">Browser Extension Security Guide - AppSec Atlas</a></li>

</ul>
</details>

**Discussion**: Commenters expressed concern about extensions injecting interfaces into the website's DOM, noting that password managers could leak account information to sites. Some suggested moving the element picker UI to browser chrome, while others appreciated the author's disclosure that GPT wrote the proof-of-concept and shared version numbers for patched releases.

**Tags**: `#security`, `#xss`, `#browser-extensions`, `#uBlock-Origin`, `#vulnerability`

---

<a id="item-3"></a>
## [Alibaba's Qwen Team Releases Qwen4-Max Flagship LLM](https://qwen.ai/blog?id=qwen4-max) ⭐️ 8.0/10

Alibaba's Qwen team released Qwen4-Max, a new flagship multimodal LLM that supports text, image, and video input with a 1M-token context window and reasoning enabled by default. The release sparked discussion on Hacker News about its benchmark scores, pricing, and inference speed compared to competitors. Qwen4-Max represents Alibaba's latest push to compete with top-tier models from OpenAI and Anthropic, and its performance and pricing will influence developers choosing models for coding, agentic tasks, and multimodal applications. The community's focus on inference speed highlights that serving efficiency is becoming as important as raw benchmark scores. According to Artificial Analysis, Qwen4-Max scores 43 with an average cost of $3.27, while GPT-6.1 Sol (medium) scores 46 at $0.36, and community members note that Qwen models have historically been slower (e.g., 30 tokens per second vs. Opus's 80). The model is available via OpenRouter and QwenCloud, with a 984k-token context window reported by Artificial Analysis.

hackernews · ilreb · Nov 16, 02:14 · [Discussion](https://news.ycombinator.com/item?id=50513215)

**Background**: Qwen is Alibaba's family of large language models, and the 'Max' variant denotes the flagship, highest-capability version. Artificial Analysis is an independent platform that benchmarks LLMs on intelligence and cost, providing standardized comparisons. OpenRouter is a unified API gateway that lets developers access many models from different providers, which is why community members reference model variants like 'qwen3.8-max-prime' available there.

<details><summary>References</summary>
<ul>
<li><a href="https://artificialanalysis.ai/models/qwen4-max">Qwen 4 Max - Intelligence, Performance & Price... | Artificial Analysis</a></li>
<li><a href="https://openrouter.ai/qwen/qwen4-max">Qwen 4 Max - API Pricing & Providers | OpenRouter</a></li>
<li><a href="https://www.qwencloud.com/models/qwen4-max?region=ap-southeast-1">Qwen 4 - Max - QwenCloud</a></li>

</ul>
</details>

**Discussion**: Commenters highlighted a significant price-performance gap: Qwen4-Max scores 43 at $3.27 average cost, while GPT-6.1 Sol scores 46 at just $0.36, raising concerns about competitiveness. Others lamented slow inference speeds (30 tokens/s vs. Opus's 80) affecting agentic use cases, while some expressed hope for efficiency gains and upcoming smaller 'Flash' and 27B versions, and one user questioned whether open-weight models are lagging behind proprietary ones.

**Tags**: `#llm`, `#qwen`, `#ai-models`, `#benchmarks`, `#inference-performance`

---

<a id="item-4"></a>
## [Steve Blank Analyzes Nvidia's Strategic Threats as Customers Become Competitors](https://steveblank.com/2026/11/15/whats-next-for-nvidia/) ⭐️ 8.0/10

Steve Blank published a blog post analyzing the strategic threats facing Nvidia, particularly the risk of its largest customers becoming competitors. The post sparked a Hacker News discussion with 293 comments debating CUDA's declining relevance and potential margin collapse. This analysis matters because Nvidia's dominance in AI hardware is increasingly challenged by major customers like Google, Amazon, Microsoft, Meta, and OpenAI building custom chips. If CUDA's moat erodes, Nvidia's high margins could collapse, affecting the entire AI semiconductor ecosystem and investors. The discussion highlights that as the problem space stabilizes, big GPU buyers can work with companies like Broadcom to make custom chips and use AI agents to build their own abstraction layers and debug tools, accelerating CUDA's declining relevance. Nvidia's net profit margin is currently around 63.66% (TTM), well above the industry average of 27.16%, making it vulnerable to margin compression.

hackernews · zdw · Nov 15, 23:55 · [Discussion](https://news.ycombinator.com/item?id=50512235)

**Background**: CUDA is Nvidia's proprietary parallel computing platform and API, created in 2004 and released in 2007, which lets software use Nvidia GPUs for general-purpose processing and has been a key lock-in for AI and scientific computing. Steve Blank is a well-known startup authority, author of 'The Four Steps to the Epiphany' and 'The Startup Owner's Manual,' and creator of the Customer Development methodology. The debate echoes historical cases like Apple's iPod, which cannibalized its own products to avoid being disrupted by competitors.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/CUDA">CUDA - Wikipedia</a></li>
<li><a href="https://tech-insider.org/nvidia-customers-rivals-custom-silicon-race-2026/">Nvidia Customers Become Rivals: Custom Chip Race [2026]</a></li>
<li><a href="https://www.investing.com/equities/nvidia-corp-ratios">Nvidia (NVDA) Financial Ratios</a></li>

</ul>
</details>

**Discussion**: Commenters largely agree that Nvidia's biggest threat is customers becoming competitors, with one noting that CUDA is becoming less relevant at a rate 'about to go parabolic' and that margins will collapse. Others draw parallels to Steve Jobs' willingness to cannibalize Apple's own successful products, while some discuss Steve Blank's influential startup books.

**Tags**: `#nvidia`, `#semiconductors`, `#business-strategy`, `#ai-hardware`, `#cuda`

---

<a id="item-5"></a>
## [MIT's 'How to Make Almost Anything' course sparks debate on breadth vs. depth](https://pub.cba.mit.edu/863.26/site/) ⭐️ 7.0/10

A Hacker News discussion about MIT's 'How to Make Almost Anything' course (MAS.863) debated its broad but shallow approach, with commenters weighing the value of overview knowledge against deep specialization. The discussion highlights a tension in technical education between exposing students to a wide range of fabrication tools and techniques versus training them to deep expertise, which affects how future makers and engineers are prepared for real-world problem-solving. Commenters noted the course's intense pace and huge syllabus, with some arguing that projects like making a PC board are not overly complex with the right tools, while others pointed out gaps in higher education for understanding at-scale industrial processes from prototype to product.

hackernews · o4c · Nov 16, 05:50 · [Discussion](https://news.ycombinator.com/item?id=50514470)

**Background**: MAS.863 'How to Make (almost) Anything' is a famous course taught by Neil Gershenfeld at MIT's Center for Bits and Atoms, providing hands-on introduction to digital fabrication tools like CAD/CAM, 3D printing, and NC machining. The course is tied to the global Fab Lab network, which extends MIT's digital fabrication research to local workshops worldwide.

<details><summary>References</summary>
<ul>
<li><a href="https://ani-liu.com/how-to-make-almost-anything-1">how to make almost anything — Ani Liu</a></li>
<li><a href="https://en.wikipedia.org/wiki/Fab_lab">Fab lab - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Neil_Gershenfeld">Neil Gershenfeld - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Commenters were divided: some defended the course's broad overview as valuable for future problem-solving, while others criticized its insane pace and superficial coverage. Others highlighted the gap in higher education for industrial-scale processes and shared resources like a free precision machine design course.

**Tags**: `#education`, `#maker-culture`, `#hardware`, `#MIT`, `#curriculum`

---

<a id="item-6"></a>
## [Old Bitly Links Hijacked, Raising Concerns About URL Shortener Risks](https://ransomnews.com/burger-king-tweet-bitly-link-hijack-2026/) ⭐️ 7.0/10

A recent report highlights that old Bitly links are being hijacked, allowing attackers to redirect them to malicious or unintended destinations. The issue gained traction after a Burger King tweet with a Bitly link was reportedly hijacked in 2026, sparking a Hacker News discussion with 139 comments. This underscores the security and reliability risks of URL shorteners, especially when links are abandoned or the shortener service changes ownership. It affects anyone who has shared short links, as they may become permanently broken or redirect to harmful sites, impacting trust in web infrastructure. The hijacking exploits the fact that Bitly links can be reassigned if the original account is deactivated or the link expires, and Bitly's Trust and Safety team may not catch all cases. The incident involved a Burger King tweet, but the exact mechanism and scale of the hijacking remain unclear.

hackernews · hspeiser · Nov 15, 22:11 · [Discussion](https://news.ycombinator.com/item?id=50511395)

**Background**: Bitly is a popular URL shortening service that turns long URLs into short, shareable links and tracks click data. Link rot is the phenomenon where hyperlinks over time cease to point to their original target, often due to content removal or service changes. URL shorteners can exacerbate link rot because the short link depends on the shortener's continued operation and correct redirection.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Link_rot">Link rot - Wikipedia</a></li>
<li><a href="https://checkshorturl.com/blog/types-of-malware-shortened-links-avoid-online-dangers">Short URLs and Malware: What You Need to Know</a></li>
<li><a href="https://goo.by/blog/what-is-bitly-and-how-it-can-benefit-your-online-presence-and-marketing-strategy">What is Bitly ? Find out all you need to know about this URL ...</a></li>

</ul>
</details>

**Discussion**: Commenters expressed strong concerns about outsourced link shorteners, with one calling them 'an order of magnitude worse' due to accretion of URLs and potential for permanent breakage. Another shared an anecdote about a famous author's unregistered Bitly link being redirected, and others questioned the need for link shorteners or suggested a bureau to track abandoned URLs.

**Tags**: `#security`, `#url-shorteners`, `#link-rot`, `#web-infrastructure`, `#hackernews`

---

<a id="item-7"></a>
## [Tor Project releases emergency 0.4.9.17 security fix for ongoing DDoS attack](https://forum.torproject.org/t/security-release-0-4-9-17/22454) ⭐️ 7.0/10

The Tor Project released Tor 0.4.9.17 on November 13, 2026, as a rapid-response security update to defend against an ongoing distributed denial-of-service (DDoS) attack that is overwhelming network relays. The release includes several security fixes, with one particularly important fix addressing IPv6 handling in relay DoS defenses. This emergency update is critical for maintaining the stability and availability of the Tor anonymity network, which millions of users rely on for privacy and censorship circumvention. The ongoing DDoS attack has degraded performance for relay operators and users, and this fix aims to mitigate the impact while highlighting the cat-and-mouse nature of DoS defense. The most important fix in 0.4.9.17 is related to IPv6 handling in relay DoS defenses, which was being exploited during the attack. This release follows earlier DoS defense improvements, such as those in Tor 0.4.9.15 that introduced defenses against the BEGIN_DIR thunderstorm attack.

hackernews · aillia · Nov 16, 00:21 · [Discussion](https://news.ycombinator.com/item?id=50512441)

**Background**: Tor is a free overlay network that enables anonymous communication by directing internet traffic through a worldwide volunteer network of relays. A DDoS attack floods a network with excessive traffic to disrupt its normal functioning, and Tor has been a frequent target due to its role in privacy and censorship resistance. The Tor Project regularly releases updates to counter evolving attacks, including proof-of-work defenses and other mitigations.

<details><summary>References</summary>
<ul>
<li><a href="https://forum.torproject.org/t/security-release-0-4-9-17/22454">Security Release 0.4.9.17 - Tor Release Announcement - Tor ...</a></li>
<li><a href="https://cybersecuritynews.com/tor-ddos-attack/">Tor Releases Emergency Security Update as Ongoing DDoS Attack ...</a></li>
<li><a href="https://cyberpress.org/tor-project-emergency-security-update/">Tor Project Releases Emergency Security Update Amid Massive ...</a></li>

</ul>
</details>

**Discussion**: Community comments reflect a mix of operational experience and frustration: one relay operator described how the attack caused a 99% drop in download speed, while others complained about Tor's slowness and questioned whether it has improved over the years. Some users noted the cat-and-mouse nature of DoS defense and pointed out ironic issues, such as Tor's own website blocking Tor users with a 403 error.

**Tags**: `#Tor`, `#DDoS`, `#security`, `#privacy`, `#networking`

---

<a id="item-8"></a>
## [Protomaps Makes Self-Hosting Map Tiles Cheap and Easy](https://bruceroettgers.eu/blog/protomaps/) ⭐️ 7.0/10

A blog post explains how Protomaps, an open-source project, enables developers to self-host map tiles cheaply and easily by packaging map data into a single PMTiles file that can be served from commodity cloud storage without a dedicated tile server. This matters because it drastically reduces the cost and complexity of running custom maps, offering an alternative to commercial providers like Mapbox or Google Maps, and giving developers more control over privacy and access. PMTiles uses HTTP range requests to fetch only the needed tiles from a single archive, enabling serverless, zero-maintenance map applications; however, very large tiles (>128MB) and some raster formats may still have compatibility issues.

hackernews · bcye · Nov 15, 19:26 · [Discussion](https://news.ycombinator.com/item?id=50509837)

**Background**: Traditional web maps rely on tile servers that divide the map into small images or vector data for each zoom level. Self-hosting these tiles typically requires setting up and maintaining a tile server, which can be costly and complex. Protomaps simplifies this by storing all tiles in a single PMTiles archive that can be hosted on static storage like Amazon S3, and clients fetch tiles on demand using HTTP range requests.

<details><summary>References</summary>
<ul>
<li><a href="https://protomaps.com/">Protomaps - The open source map in a file</a></li>
<li><a href="https://docs.protomaps.com/pmtiles/">PMTiles Concepts | Protomaps Docs</a></li>
<li><a href="https://openfreemap.org/">OpenFreeMap</a></li>

</ul>
</details>

**Discussion**: Commenters highlighted alternatives like OpenFreeMap and VersaTiles, shared real-world cost savings (e.g., Cartes.app switched from MapTiler to Protomaps to avoid 150€/month bills), and discussed practical tips such as using PMTiles viewers and customizing map styles.

**Tags**: `#maps`, `#self-hosting`, `#protomaps`, `#open-source`, `#geospatial`

---

<a id="item-9"></a>
## [Internet Archive Preserves 30 Years of Salon Journalism](https://blog.archive.org/2026/11/12/preserving-30-years-of-salon-journalism/) ⭐️ 7.0/10

The Internet Archive announced on November 12, 2026, that it is preserving 30 years of journalism from Salon, the pioneering digital magazine that shut down earlier in November 2026 after 31 years due to financial reasons. This preservation effort ensures that Salon's extensive archive of reporting, commentary, and cultural criticism remains accessible to researchers, historians, and the public, highlighting the Internet Archive's role as a safeguard against the loss of born-digital journalism as online publications continue to close. The preservation covers Salon's entire 30-year output, and the announcement has drawn attention to practical challenges such as bulk-downloading from the Wayback Machine and the risk of bitrot in long-term digital archives.

hackernews · CharlesW · Nov 15, 23:00 · [Discussion](https://news.ycombinator.com/item?id=50511806)

**Background**: Salon was founded in 1995 as one of the first online-only magazines, known for its progressive commentary and early online communities like TableTalk. The Internet Archive, a nonprofit digital library, operates the Wayback Machine, which has archived hundreds of billions of web pages since 1996. Digital preservation ensures that content from defunct websites remains available even after the original domains go offline.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Internet_Archive">Internet Archive - Wikipedia</a></li>
<li><a href="https://www.nytimes.com/2026/11/05/business/media/salon-online-magazine-shutters.html">Salon , a Pioneer of Digital Journalism , Shuts Down - The New York...</a></li>
<li><a href="https://web.archive.org/?ref=gobigger">Wayback Machine</a></li>

</ul>
</details>

**Discussion**: Commenters praised the Internet Archive's mission, with some noting irony in preserving a publication they disliked, while others criticized Salon for failing to preserve its own communities like TableTalk. Several users questioned why Salon's domains must go offline and shared memories of features like Salon Personals, and one commenter asked about tools for bulk-downloading entire site snapshots from the Wayback Machine.

**Tags**: `#digital-preservation`, `#internet-archive`, `#journalism`, `#wayback-machine`, `#web-archiving`

---

<a id="item-10"></a>
## [MacBook Pro OLED PWM flicker issue raises usability concerns](https://macanorak.com/the-macbook-pros-oled-pwm-problem-when-a-better-display-becomes-worse-to-use/) ⭐️ 7.0/10

An article on MacAnorak examines the MacBook Pro's OLED display PWM flicker problem, arguing that a technically superior display can be worse for users sensitive to flicker. The piece highlights that the new MacBook Pro OLED screen uses PWM dimming at a relatively low frequency, causing discomfort for some users. This issue affects a significant minority of users who experience eye strain, headaches, and other symptoms from PWM flicker, potentially making the otherwise excellent display unusable for them. It also raises questions about Apple's choice of display technology and whether usability should trump technical specifications. The MacBook Pro's OLED display reportedly uses PWM at around 240 Hz, which is lower than the 14,880 Hz PWM found in the Mini-LED MacBook Pro, and some users are highly sensitive to such low-frequency flicker. Community analysis suggests the tandem OLED may effectively double the frequency to 480 Hz or 960 Hz under certain conditions, but the exact behavior remains debated.

hackernews · MacAnorak · Nov 15, 13:15 · [Discussion](https://news.ycombinator.com/item?id=50506719)

**Background**: PWM (pulse-width modulation) is a common method for dimming displays, where the backlight or pixels are rapidly switched on and off to control brightness. While most people don't perceive this flicker, a subset of users experience symptoms like eye strain, headaches, and nausea, especially at lower frequencies. OLED displays often use PWM because controlling brightness via voltage can shift colors, making PWM a simpler solution.

<details><summary>References</summary>
<ul>
<li><a href="https://www.oled-info.com/pulse-width-modulation-pwm-oled-displays">Pulse-width modulation (PWM) in OLED displays - OLED-Info What is PWM dimming, and what are the alternatives? PWM Screen Flicker Test | Monitor Pulse-Width Modulation ... OLED Eye Strain and PWM Flicker: How to Test and Reduce ... MacBook Pro OLED Eye Strain & PWM Flicker: 7 Moves - AH Eye care: prevent PWM and or temporal dithering - GitHub</a></li>
<li><a href="https://www.appleheadlines.com/macbook-pro-oled-eye-strain-pwm-flicker/">MacBook Pro OLED Eye Strain & PWM Flicker: 7 Moves - AH</a></li>
<li><a href="https://appleinsider.com/articles/26/11/10/if-youre-getting-dizzy-using-proled-macbook-pro-you-are-not-alone">Pulse width modulation on MacBook Pro with PROLED - AppleInsider</a></li>

</ul>
</details>

**Discussion**: Commenters shared personal experiences with flicker sensitivity, with some noting that other display factors like CRI and motion blur also cause discomfort. One commenter questioned the 240 Hz claim, suggesting the tandem OLED might effectively run at 480 Hz or 960 Hz out of phase, while another expressed shock that Apple would release a display with such low PWM frequency and cited research on flicker perception.

**Tags**: `#OLED`, `#PWM`, `#display technology`, `#health`, `#hardware`

---

<a id="item-11"></a>
## [Crows make decisions twice as fast as humans, study finds](https://www.nytimes.com/2026/11/15/science/birdbrain-crows-birds-research-decision.html) ⭐️ 7.0/10

Researchers at the University of Tübingen discovered that crows can make visual decisions in about 235 milliseconds, roughly twice as fast as rhesus monkeys or humans performing similar tasks. The birds were allowed three seconds but consistently answered in under one second. This finding challenges the assumption that mammalian brain architecture is necessary for complex cognition and suggests that intelligence can evolve through different neural designs. It has implications for understanding convergent evolution and may inspire new approaches in artificial intelligence and neuroscience. The crows' ultrafast decision speed may partly reflect the high temporal precision of the avian visual system, potentially shaped by selection for rapid sensory-motor processing. Unlike mammals, birds lack a layered cerebral cortex but achieve comparable cognitive flexibility through a different neural organization.

hackernews · gumby · Nov 15, 17:53 · [Discussion](https://news.ycombinator.com/item?id=50509023)

**Background**: Crows and other corvids are known for remarkable cognitive abilities, such as tool use and problem-solving, despite having brains structurally very different from mammals. Mammals have a layered cerebral cortex, which is considered the highest integration center in the mammalian brain, but birds lack this structure. Instead, corvids evolved a different neural architecture that supports complex cognition, making them a key example of convergent evolution of intelligence.

<details><summary>References</summary>
<ul>
<li><a href="https://www.nytimes.com/2026/11/15/science/birdbrain-crows-birds-research-decision.html">‘Birdbrain’ Is a Misnomer. Crows Make Decisions Faster Than We Can</a></li>
<li><a href="https://www.science.org/doi/10.1126/science.aed6459">Ultrarapid decision-making in an avian brain | Science</a></li>
<li><a href="https://www.sciencedaily.com/releases/2026/11/261111005850.htm">Crows can make decisions twice as fast as humans, scientists ...</a></li>

</ul>
</details>

**Discussion**: Commenters highlighted that intelligence has evolved independently at least three times (mammals, corvids, octopuses), with corvids having a different neuron design and brain architecture. Some suggested that smaller brains allow faster connections, while others noted that birds' high-speed flight demands rapid decision-making. The discussion also touched on birds' magnetic sensing and decentralized body clocks.

**Tags**: `#neuroscience`, `#animal cognition`, `#evolution`, `#decision-making`, `#hackernews`

---

<a id="item-12"></a>
## [Microsoft 365 outage linked to chlorine gas poisoning at German hotel](https://www1.wdr.de/nrw/rheinland/rhein-erft-kreis/technischer-defekt-chlor-phantasialand-100.html) ⭐️ 7.0/10

A Microsoft 365 outage disrupted email alerts from a hotel's chlorine dosing system, contributing to a malfunction that caused 15 guests to suffer chlorine gas poisoning. The incident occurred at a hotel in the Rhein-Erft district of Germany, with 13 guests initially complaining of airway irritation and two more later, and four taken to hospital. This incident highlights the dangers of relying on cloud services for safety-critical communications and the need for fail-safe designs in automated systems. It serves as a real-world example of cascading failures, prompting discussions on accountability and system resilience. The dosing system had a defect causing excessive chlorine dosing, and the monitoring system's email alerts failed due to the Microsoft 365 outage. The incident resulted in 13 guests with airway irritation, 2 more later, and 4 hospitalizations, with one medium injury.

hackernews · DeepLogin · Nov 15, 18:36 · [Discussion](https://news.ycombinator.com/item?id=50509411)

**Background**: Microsoft 365 is a cloud-based productivity suite that includes email and collaboration tools. Safety-critical systems, such as chlorine dosing in hotels, require robust fail-safe mechanisms to prevent accidents when components fail. This incident illustrates how a cloud outage can cascade into physical harm when systems lack redundancy.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/2026_Microsoft_outage">2026 Microsoft outage - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Safety-critical_system">Safety - critical system - Wikipedia</a></li>
<li><a href="https://www.linkedin.com/pulse/cloud-dependent-ot-authentication-someone-elses-single-kaan-8ntkf">Cloud - dependent OT authentication is someone else's single point of...</a></li>

</ul>
</details>

**Discussion**: Commenters largely blamed the hotel for poor system design, emphasizing that safety-critical systems should not depend on cloud services for alerts. Some noted the need for redundant sensors and human oversight, while others pointed out that the German article was less dramatic than the headline suggested.

**Tags**: `#system-reliability`, `#cloud-outage`, `#safety-critical-systems`, `#incident-analysis`, `#infrastructure`

---

<a id="item-13"></a>
## [Clice v1.0 Released: A Modern C++ Language Server](https://ykiko.me/en/articles/2105384023094834022/) ⭐️ 7.0/10

Clice, a C++ language server built from scratch on LLVM/Clang with selected components ported from clangd, has reached version 1.0. The release is accompanied by a technical article and active community discussion comparing it to clangd. Clice aims to solve long-standing problems in C++ tooling through redesigned architecture, asynchronous task scheduling, and intelligent caching, potentially offering a faster and more memory-efficient alternative to clangd. This matters for C++ developers who rely on language servers for code completion, navigation, and refactoring in their editors. Clice is written from scratch on LLVM/Clang and ports selected components from clangd, but redesigns key architectural decisions. It claims lower memory footprint and faster response times through excellent asynchronous task scheduling and intelligent caching.

hackernews · molenzwiebel · Nov 15, 17:22 · [Discussion](https://news.ycombinator.com/item?id=50508715)

**Background**: A C++ language server provides IDE features like code completion, go-to-definition, and find-all-references to editors via the Language Server Protocol (LSP). clangd is the standard language server based on the Clang compiler and part of the LLVM project, but it is known for slow indexing on large codebases. Clice is a new implementation that aims to address these performance issues.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/clice-io/clice">GitHub - clice-io/clice: A next-generation C++ language ...</a></li>
<li><a href="https://clangd.llvm.org/">What is clangd ?</a></li>
<li><a href="https://microsoft.github.io/language-server-protocol/">Official page for Language Server Protocol</a></li>

</ul>
</details>

**Discussion**: Commenters expressed interest in Clice but raised concerns about indexing performance, with one noting that clangd is orders of magnitude slower than non-clang-based indexers. Others discussed the author's reflective tone and the appeal of the term "modern C++", while some questioned why Clice would show clangd crashing without fixing it.

**Tags**: `#C++`, `#language-server`, `#clangd`, `#developer-tools`, `#static-analysis`

---

<a id="item-14"></a>
## [Apple launches 200,000-person US health AI study with OpenEvidence](https://www.reddit.com/r/artificial/comments/1xxigdv/apple_opens_a_us_study_of_health_ai_that_can/) ⭐️ 7.0/10

Apple announced a US health AI study that can enroll up to 200,000 participants aged 21 or older, using a research app built with OpenEvidence that delivers answers linked to clinical sources. Participation in sharing HealthKit data or survey responses is optional, and Apple says study data will not be used for AI training. This is one of the largest consumer-facing health AI studies to date, and it could shape how the industry measures trust in AI-generated clinical answers, especially whether users can detect citations that only partially support a polished response. The results may influence regulatory expectations and product design for clinical AI tools that rely on evidence citations. The study targets US adults 21 and older, and the OpenEvidence-built app provides answers with links to clinical sources rather than unsourced summaries. A key open question raised is whether participants can spot answers that stretch what their cited sources actually say, since a trust rating alone would not capture that distinction.

reddit · r/artificial · /u/andrewaltair · Nov 16, 06:40

**Background**: OpenEvidence is an AI medical information platform that synthesizes medical literature from sources such as NEJM and JAMA to give clinicians evidence-based answers with citations. HealthKit is Apple's framework for storing and sharing health and fitness data from iPhone and Apple Watch, with user permission and privacy controls. Citation faithfulness—whether each claim is actually supported by its cited source—has become a central metric for evaluating clinical AI systems.

<details><summary>References</summary>
<ul>
<li><a href="https://www.toolmage.com/en/tool/openevidence/">OpenEvidence : AI Medical Assistant for Clinical Decision... - ToolMage</a></li>
<li><a href="https://developer.apple.com/documentation/healthkit">HealthKit | Apple Developer Documentation</a></li>
<li><a href="https://cliniatlas.com/methodology/">How CliniAtlas is Evaluated — Citation Faithfulness , Recall...</a></li>

</ul>
</details>

**Discussion**: The discussion focuses on whether users can detect a polished answer that overstates its cited source, noting that an answer can feel helpful even when a citation supports only part of it. Commenters suggest that a simple trust rating would miss this nuance and ask whether the more informative measure is how often people check cited sources or whether they change their minds after seeing what the source actually says.

**Tags**: `#health-ai`, `#apple`, `#ai-trust`, `#citations`, `#clinical-ai`

---

<a id="item-15"></a>
## [South Korea in Uproar Over AI-Assisted Exam Cheating Before CSAT](https://www.reddit.com/r/artificial/comments/1xxhk3a/south_korea_is_currently_in_an_uproar_over_exam/) ⭐️ 7.0/10

The top scorer on South Korea's 63rd Tax Accountant Exam admitted to using generative AI to cheat and turned himself in to police, just days before the 2026 College Scholastic Ability Test (CSAT). The confession has triggered national alarm, with calls to cancel or postpone the exam and even to confiscate all glasses from test-takers. The incident highlights how generative AI is undermining high-stakes standardized testing in South Korea, where exam results heavily determine university admissions and career prospects. It also raises concerns that similar AI-enabled cheating may be spreading globally, forcing education systems to rethink exam security and integrity. The cheating was uncovered after a perfect scorer on the LEET (Legal Education Eligibility Test) appeared on YouTube with suspicious testimony, prompting wider scrutiny. Authorities are now under pressure to implement detection measures such as behavioral monitoring and AI-content detectors, though no technical solution has been announced.

reddit · r/artificial · /u/Active-Pound1624 · Nov 16, 05:47

**Background**: The CSAT (College Scholastic Ability Test) is South Korea's nationwide university entrance exam, and its results are critical for admission to top universities. The LEET is a separate test used for law school admissions in South Korea. Generative AI tools like large language models can produce human-like text and answers, making them increasingly difficult to detect in exam settings.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Legal_Education_Eligibility_Test">Legal Education Eligibility Test - Wikipedia</a></li>
<li><a href="https://en.sedaily.com/society/2026/11/13/koreas-first-perfect-leet-scorer-to-solve-exam-live-amid">Korea's First Perfect LEET Scorer to Solve Exam Live Amid ...</a></li>
<li><a href="https://edulegit.com/blog/how-to-detect-prevent-ai-generated-cheating-exams/">How to Detect and Prevent AI-Generated Cheating in Exams</a></li>

</ul>
</details>

**Tags**: `#AI cheating`, `#education`, `#South Korea`, `#generative AI`, `#academic integrity`

---

<a id="item-16"></a>
## [Handwriting, as a Font: Web Tool Turns Samples into Custom Fonts](https://ductus.sorenblank.com/) ⭐️ 6.0/10

A new web tool called 'Handwriting, as a Font' (ductus.sorenblank.com) lets users write individual letters to generate a custom font from their handwriting. The tool gained attention on Hacker News, drawing 259 points and 47 comments praising its execution while suggesting improvements. This tool democratizes font creation, enabling anyone to easily make a personal handwriting font for use in documents or design projects. It reflects a growing trend of accessible creative tools that leverage web technologies to simplify traditionally complex tasks. The tool captures per-letter samples, which works well for print-style handwriting but does not model contextual cursive connections. It also lacks accented characters and a preview feature before sampling, limiting its use for non-English languages and deterring some users.

hackernews · coinfused · Nov 15, 19:42 · [Discussion](https://news.ycombinator.com/item?id=50509972)

**Background**: Creating a custom font typically requires professional design software and knowledge of font formats like OpenType or TrueType. Web-based tools like Calligraphr have simplified this by letting users upload handwriting samples and generate a font file. This new tool follows that approach but focuses on a streamlined, interactive experience.

<details><summary>References</summary>
<ul>
<li><a href="https://handwriting-ai.com/">Text to Handwriting Generator – Realistic Notes | Handwriting AI</a></li>
<li><a href="https://en.wikipedia.org/wiki/OpenType">OpenType - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Commenters praised the tool's execution and ease of use, with one noting it made capturing an initial version easy in one sitting. However, several users requested accented characters for non-English names, a preview before committing to sampling, and better modeling of cursive connections. Others enjoyed using it on mobile and planned to use the font for fun at work.

**Tags**: `#fonts`, `#handwriting`, `#web-tools`, `#typography`, `#side-project`

---

<a id="item-17"></a>
## [WebGL Flight Simulator with Seed-Generated Terrain Impresses Hacker News](https://baron.by.dai.studio/) ⭐️ 6.0/10

A WebGL-based flight simulator with seed-generated terrain was shared on Hacker News, receiving 134 points and 26 comments. The project, hosted at baron.by.dai.studio, was praised for its flight dynamics and sparked discussion about its AI-assisted development. This project demonstrates the growing capability of browser-based simulations using WebGL and procedural generation, and highlights how AI-assisted development tools are enabling developers to create polished interactive experiences more rapidly. The simulator features an expert mode with flight dynamics that experienced users found surprisingly good, though not on par with dedicated simulators like X-Plane. A community member noted that pressing Ctrl-S to slow the engine triggers the browser's save dialog, indicating a minor UX issue.

hackernews · ranger_danger · Nov 15, 20:20 · [Discussion](https://news.ycombinator.com/item?id=50510296)

**Background**: WebGL is a JavaScript API for rendering interactive 3D graphics in browsers without plug-ins, enabling GPU-accelerated experiences. Procedural terrain generation uses algorithms and seed values to create vast, repeatable worlds on demand, as seen in games like Minecraft. AI-assisted development involves using AI tools to help write code, which can speed up the creation of complex projects like this flight simulator.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/WebGL">WebGL</a></li>
<li><a href="https://generalistprogrammer.com/procedural-generation-games">Procedural Generation in Games: Algorithms & Examples (2026)</a></li>
<li><a href="https://grokipedia.com/page/ai_assisted_software_development">AI-assisted software development</a></li>

</ul>
</details>

**Discussion**: Commenters were impressed with the flight dynamics, especially in expert mode, though some noted it's not a full simulator. One user shared a similar AI-assisted paper plane simulator, while others suggested showing the AI graph used to generate the game to lower the entry barrier.

**Tags**: `#WebGL`, `#flight-simulator`, `#procedural-generation`, `#AI-assisted-development`, `#browser-games`

---

<a id="item-18"></a>
## [Turbo Pascal's Tiny Footprint Sparks Debate on Modern Software Bloat](https://prog21.dadgum.com/116.html) ⭐️ 6.0/10

A 2011 blog post by James Hague titled 'Things That Turbo Pascal Is Smaller Than' was revived on Hacker News, comparing the size of Turbo Pascal (a few hundred kilobytes) to modern software like individual web pages and images. The post sparked a discussion with 127 comments about why contemporary binaries and systems have grown so large. The discussion highlights the trade-offs between developer productivity and software efficiency, and questions whether the current level of software bloat is justified. It resonates with developers concerned about resource usage and system design in modern computing. Turbo Pascal, originally developed by Anders Hejlsberg at Borland, was known for its extremely fast compilation and small memory footprint, fitting on a single floppy disk. The blog post notes that Turbo Pascal is smaller than a single modern web page or a low-resolution image, underscoring the dramatic increase in software size over decades.

hackernews · ksec · Nov 15, 13:44 · [Discussion](https://news.ycombinator.com/item?id=50506894)

**Background**: Turbo Pascal was a popular Pascal compiler and IDE for CP/M and MS-DOS in the 1980s and 1990s, notable for its speed and efficiency. Software bloat refers to the tendency of software to become slower and require more resources with each version, often due to added features or layers of abstraction. The comparison serves as a nostalgic reminder of how lean software used to be and a critique of modern development practices.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Turbo_Pascal">Turbo Pascal</a></li>
<li><a href="https://en.wikipedia.org/wiki/Software_bloat">Software bloat</a></li>

</ul>
</details>

**Discussion**: Commenters debated the causes of bloat: mbfg argued that 80s/90s code was mostly single-user applications, while modern systems require robustness and third-party libraries, making bloat a rational choice. jll29 expressed disbelief that the 'touch' command's binary exceeds Turbo Pascal, calling it insane and attributing it to laziness and repeated boilerplate. pron noted that RAM in 1986 was 30,000x smaller, and Turbo Pascal was no less bloated relative to its environment than VS Code is today.

**Tags**: `#software-bloat`, `#turbo-pascal`, `#binary-size`, `#systems-design`, `#programming-history`

---

<a id="item-19"></a>
## [Coles investigates cybersecurity incident affecting internal staff systems](https://www.colesgroup.com.au/updates/) ⭐️ 6.0/10

Australian supermarket giant Coles has confirmed it is investigating a cybersecurity incident, disclosing to the ASX that a small number of customers were affected while stating that no customer, team, or supplier data was breached. The company has apologised to customers and recommended they update their credentials. This incident adds to a growing list of cyberattacks against major Australian organisations, including Optus, Medibank, and government agencies, raising questions about corporate accountability and the effectiveness of Australia's mandatory data breach notification regime. It highlights systemic concerns about cybersecurity maturity in the Australian retail sector. Coles has provided minimal technical detail about the nature of the breach, and it remains unclear which internal systems were compromised. Under Australia's Notifiable Data Breaches scheme, organisations with annual turnover above $3 million must notify affected individuals and the OAIC when a breach is likely to cause serious harm.

hackernews · sagunsh · Nov 16, 01:14 · [Discussion](https://news.ycombinator.com/item?id=50512824)

**Background**: Coles is one of Australia's largest supermarket chains, operating over 800 stores and employing more than 100,000 staff. The retail sector has become a prime target for cyberattacks due to its extensive customer data, complex supply chains, and increasingly digitised operations. Australia's Notifiable Data Breaches scheme, introduced in 2018, requires organisations to report eligible data breaches to the Office of the Australian Information Commissioner.

<details><summary>References</summary>
<ul>
<li><a href="https://www.abc.net.au/news/2026-11-16/coles-investigates-cybersecurity-breach-but-little-detail/107390824">Supermarket group Coles investigates cybersecurity incident ...</a></li>
<li><a href="https://www.theguardian.com/business/2026/nov/16/coles-cyber-attack-incident-data">Coles investigating ‘cybersecurity incident’ and apologises ...</a></li>
<li><a href="https://www.varonis.com/blog/australian-notifiable-data-breach-explained">Australian Notifiable Data Breach Scheme, Explained</a></li>

</ul>
</details>

**Discussion**: Commenters expressed deep scepticism about Australia's cybersecurity standards, with one noting that major breaches now occur roughly every six months across companies and government agencies. Others questioned corporate incentives for security investment, arguing that companies face no meaningful consequences for doing the bare minimum, while one commenter criticised the submission itself for lacking detail about what actually happened.

**Tags**: `#cybersecurity`, `#Australia`, `#corporate breach`, `#incident response`, `#retail`

---

<a id="item-20"></a>
## [datasette-maplibre 0.1a0: AI-built geospatial plugin for Datasette](https://simonwillison.net/2026/Nov/15/datasette-maplibre/) ⭐️ 6.0/10

Simon Willison released datasette-maplibre 0.1a0, a new Datasette plugin that integrates MapLibre GL and OpenFreeMap to display maps for data with latitude/longitude columns or GeoJSON shapes. Most of the plugin was generated from a single prompt to Claude Fable 5.2, which also produced a comprehensive demo that runs in Datasette Lite via Pyodide and WebAssembly. This is the first new Datasette geospatial plugin in a while, giving Datasette users a modern, WebGL-based mapping option that combines point clustering and GeoJSON rendering. It also serves as a notable demonstration of AI-assisted development, where a single well-crafted prompt produced a functional, feature-rich plugin. The plugin was built by instructing Claude to study the datasette-cluster-map and datasette-leaflet-geojson plugins plus an OpenFreeMap demo, then combine their features creatively. One standout feature is that it displays SVG previews of GeoJSON shapes and only loads WebGL previews when they scroll into view, and the demo works in Datasette Lite via Pyodide/WebAssembly.

rss · Simon Willison · Nov 15, 23:58

**Background**: Datasette is an open-source tool for exploring and publishing SQLite databases as web interfaces, and its plugin system extends functionality such as mapping. MapLibre GL JS is an open-source TypeScript/JavaScript library that renders interactive vector tile maps in the browser using GPU-accelerated WebGL. OpenFreeMap is a free vector map server operated by Zsolt Ero that serves OpenStreetMap vector tiles without API keys. Datasette Lite is a version of Datasette that runs entirely in the browser via Pyodide and WebAssembly.

<details><summary>References</summary>
<ul>
<li><a href="https://maplibre.org/maplibre-gl-js/docs/">Introduction - MapLibre GL JS</a></li>
<li><a href="https://openfreemap.org/">OpenFreeMap</a></li>
<li><a href="https://datasette.io/plugins">Datasette Plugins</a></li>

</ul>
</details>

**Tags**: `#datasette`, `#maplibre`, `#geospatial`, `#ai-assisted-development`, `#open-source`

---

<a id="item-21"></a>
## [Datasette 1.0a43 adds streaming output renderers and security fixes](https://simonwillison.net/2026/Nov/15/datasette/) ⭐️ 6.0/10

Datasette 1.0a43 introduces streaming support for output renderers, with built-in CSV and TSV exports now using the new Response.stream() method, and plugins can register to stream every row of a table. The release also includes a security fix for private stored queries that could expose their title and SQL, along with dozens of smaller improvements as the 1.0 milestone reaches 53% completion. Streaming output renderers allow Datasette to export large tables without loading all rows into memory, improving performance and scalability for data-heavy deployments. The security fix addresses a vulnerability that could expose private stored queries, which is important for users relying on Datasette for sensitive data access. The new Response.stream() method enables plugins to stream rows one at a time, and the row page JSON representation has been redesigned for 1.0 compatibility. Other additions include a <datasette-copy-button> Web Component, pretty-printing of JSON columns, a DatasetteModal.confirm() JavaScript utility, and CSS multi-page view transitions for smoother navigation.

rss · Simon Willison · Nov 15, 23:20

**Background**: Datasette is an open-source tool for exploring and publishing data, built by Simon Willison, that lets users query SQLite databases via a web interface and JSON API. The 1.0 milestone is a long-running effort to stabilize the API and plugin ecosystem before a stable release. Output renderers are plugins that format query results in different ways, such as CSV, TSV, or custom formats.

<details><summary>References</summary>
<ul>
<li><a href="https://simonwillison.net/2026/Nov/15/datasette/">Release: datasette 1.0a43 - simonwillison.net</a></li>
<li><a href="https://explainx.ai/blog/datasette-1-0a43-stored-query-advisory-streaming-2026">Datasette 1.0a43: Stored-Query Security Fix (Nov 2026 ...</a></li>
<li><a href="https://github.com/simonw/datasette/issues/1101">register_output_renderer () should support streaming data ...</a></li>

</ul>
</details>

**Tags**: `#datasette`, `#open-source`, `#release`, `#data-tools`, `#security`

---

<a id="item-22"></a>
## [Datasette 0.65.6 Backports Security Fix for Unauthorized Database Downloads](https://simonwillison.net/2026/Nov/15/datasette-2/) ⭐️ 6.0/10

Datasette 0.65.6 has been released, backporting a security fix from version 1.0a43 that prevents unauthorized database downloads when a database is registered with a custom route different from its name. This fix is important for Datasette users who rely on custom routes for access control, as it closes a vulnerability that could allow restricted actors to download entire databases via the /<route>.db endpoint. The vulnerability specifically affects databases registered using add_database(db, name=..., route=...) where the route differs from the name; the fix ensures that access permissions are enforced for the .db download endpoint regardless of the route used.

rss · Simon Willison · Nov 15, 23:18

**Background**: Datasette is an open-source tool for exploring and publishing data, often used to serve SQLite databases as web APIs. It includes a permissions system to control access to databases and tables, and the add_database method allows plugins to register additional databases with custom names and routes. A route is the URL path under which a database is served, and if it differs from the database name, access checks might be bypassed.

<details><summary>References</summary>
<ul>
<li><a href="https://docs.datasette.io/en/stable/sql_queries.html">Running SQL queries - Datasette documentation</a></li>
<li><a href="https://simonwillison.net/tags/datasette/">Simon Willison on datasette</a></li>

</ul>
</details>

**Tags**: `#datasette`, `#security`, `#release`, `#backport`, `#database`

---

<a id="item-23"></a>
## [Export-Banned Nvidia Chips Power China's Top AI Models](https://www.reddit.com/r/artificial/comments/1xx4t46/exportbanned_nvidia_chips_are_behind_chinas_most/) ⭐️ 6.0/10

New research from nonprofit Epoch AI, reported by TechCrunch on November 13, 2026, estimates that about two million advanced Nvidia chips entered China in 2024 and 2025 through schemes designed to hide their final destination, and that China's most powerful AI models were trained on these export-banned chips. This finding directly challenges the effectiveness of U.S. export controls, which aim to prevent Chinese AI labs from training on the most powerful chips; it could intensify calls for stricter controls on who uses chips, not just who owns them, and reshape the geopolitical debate over AI competition. Epoch AI's estimate of roughly two million advanced chips entering China via obfuscated supply chains suggests large-scale circumvention, and the report notes that China hawks have long argued for stronger controls on chip usage rather than just ownership or installation location.

reddit · r/artificial · /u/IndependentCoast3974 · Nov 15, 19:46

**Background**: Since October 2022, the U.S. has restricted exports of cutting-edge GPU chips, including Nvidia's, to China to curb its ability to train the most powerful AI models. Nvidia later designed compliant chips like the H20 for the Chinese market, but these were also banned in 2025, and the Trump administration has since lifted some restrictions. Export controls are a key tool in the U.S.-China AI competition, and reports of circumvention raise questions about their enforcement.

<details><summary>References</summary>
<ul>
<li><a href="https://techcrunch.com/2026/11/13/export-banned-nvidia-chips-are-behind-chinas-most-powerful-ai-models-uh-oh-jensen/">Export-banned Nvidia chips are behind China 's most powerful AI ...</a></li>
<li><a href="https://builtin.com/articles/trump-lifts-ai-chip-ban-china-nvidia">Trump Lifted the AI Chip Ban on China, Clearing Nvidia and ...</a></li>
<li><a href="https://www.wired.com/story/memory-restrictions-china-advanced-chips/">US to Introduce New Restrictions on China ’s Access to... | WIRED</a></li>

</ul>
</details>

**Tags**: `#Nvidia`, `#AI chips`, `#export controls`, `#China AI`, `#geopolitics`

---

<a id="item-24"></a>
## [Reddit Post Highlights Rise of APIs Built for AI Agents](https://www.reddit.com/r/artificial/comments/1xxj7q6/feels_like_every_tool_is_turning_into_an_api_for/) ⭐️ 6.0/10

A Reddit post on r/artificial observes that everyday tools like email, browsers, payments, memory, and search are increasingly exposed as APIs purpose-built for AI agents, and lists example services such as AgentMail, Browserbase, Mem0, and Composio for each building block. This trend lowers the barrier to building AI agents by providing ready-made building blocks, potentially accelerating agent adoption beyond demos and into production workflows, and affecting developers and businesses that integrate AI automation. The post lists specific services for each capability, such as AgentPhone for phone numbers, Daytona and E2B for cloud computers, Firecrawl for web content extraction, and ElevenLabs and Vapi for voice, but the author questions how many people actually use such setups outside of demos and notes that making the whole system reliable is another challenge.

reddit · r/artificial · /u/for-entire-phonly · Nov 16, 07:27

**Background**: AI agents are autonomous software programs that can perform tasks by calling tools and APIs. Traditionally, connecting an agent to services like email or payments required writing custom scripts and handling separate authentication and integrations. Recently, a growing ecosystem of agent-native services has emerged, offering standardized APIs that abstract away these complexities, as seen with platforms like Composio for app integrations and Mem0 for persistent memory.

<details><summary>References</summary>
<ul>
<li><a href="https://www.browserbase.com/">Browserbase</a></li>
<li><a href="https://mem0.ai/">Mem 0 - AI Memory Layer for your Agents & Apps | Persistent Context</a></li>
<li><a href="https://composio.dev/content/ai-agent-integration-platforms">Best AI agent integration platforms (2026): comparison for ...</a></li>

</ul>
</details>

**Tags**: `#ai-agents`, `#apis`, `#tooling`, `#developer-tools`, `#agent-infrastructure`

---

<a id="item-25"></a>
## [Developer launches LogicLens, a real-time AI fact-checker for political speech](https://www.reddit.com/r/artificial/comments/1xwmtff/built_a_factchecker_that_catches_politicians/) ⭐️ 6.0/10

A developer released LogicLens, a free Chrome extension (also available on iOS) that transcribes political speech in real time, identifies checkable claims, and uses web search to ground Claude's fact-check verdicts, aiming to avoid hallucinated sources. The project, which took two years to build, works on YouTube as well as news and social media sites. This project demonstrates a practical application of retrieval-augmented generation (RAG) to combat political misinformation in real time, potentially empowering voters and journalists to verify claims instantly. It also highlights the growing trend of using LLMs with web grounding to improve fact-checking accuracy and transparency. The system first transcribes speech to text, then extracts checkable claims, and finally retrieves web sources to base Claude's verdict on, which helps reduce hallucinated citations. The developer notes that the extension is free and works across platforms, but the demo video may be confusing without context about which statements are true or false.

reddit · r/artificial · /u/Ok_Measurement5015 · Nov 15, 04:56

**Background**: Fact-checking political speech manually is time-consuming and often lags behind real-time discourse. Retrieval-augmented generation (RAG) is a technique where a language model retrieves relevant documents from a knowledge base to ground its responses, reducing hallucinations and improving factual accuracy. Chrome extensions are small software programs that customize the browsing experience, and real-time speech transcription is increasingly feasible with browser-based APIs and cloud services.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/abs/2505.21072">[2505.21072] Faithfulness-Aware Uncertainty Quantification ... [2505.17762] Resolving Conflicting Evidence in Automated Fact ... A Comparative Analysis of Retrieval-Augmented Generation and ... Faithfulness-Aware Uncertainty Quantification for Fact ... TrumorGPT: Graph-Based Retrieval-Augmented Large Language ... Use of Retrieval-Augmented Large Language Model for COVID-19 ... The blueprint of a new fact-checking system: A methodology to ...</a></li>
<li><a href="https://arxiv.org/abs/2505.17762">[2505.17762] Resolving Conflicting Evidence in Automated Fact ... A Comparative Analysis of Retrieval-Augmented Generation and ... Faithfulness-Aware Uncertainty Quantification for Fact ... TrumorGPT: Graph-Based Retrieval-Augmented Large Language ... Use of Retrieval-Augmented Large Language Model for COVID-19 ... The blueprint of a new fact-checking system: A methodology to ...</a></li>
<li><a href="https://chromewebstore.google.com/detail/speech-translator/jodfjmaiakpnmeddgpeflpafebmlhppn">Speech Translator - Chrome Web Store</a></li>

</ul>
</details>

**Tags**: `#fact-checking`, `#LLM`, `#Chrome extension`, `#real-time transcription`, `#misinformation`

---

<a id="item-26"></a>
## [Stanford HAI's 'Jagged Edge' AI Boom: Uneven Gains](https://www.reddit.com/r/artificial/comments/1xxbzrh/the_jagged_edge_of_the_ai_boom_stanford_hai_on/) ⭐️ 6.0/10

A Reddit post on r/artificial highlights a new Stanford HAI piece titled 'The Jagged Edge of the AI Boom,' which argues that AI's benefits are real but highly uneven across tasks and industries, and asks readers to share where they've felt this unevenness most. This framing shifts the debate from whether AI is broadly good or bad to how its gains and pains are distributed, which matters for policymakers, workers, and companies deciding where to invest or how to manage transition risks. The Reddit post notes that the dividing line is not always skill or effort, and asks whether the unevenness is temporary (tools improve and smooth the edge) or structural (some work simply fits AI better), while also linking to a related subreddit for AI news.

reddit · r/artificial · /u/Dense_Primary629 · Nov 16, 00:58

**Background**: Stanford HAI (Institute for Human-Centered Artificial Intelligence) is a research institute at Stanford University that studies AI's human and societal impact. Its AI Index is a widely cited annual report tracking AI trends, and the 'jagged edge' piece draws on new findings showing uneven public sentiment and labor market outcomes as AI investment surpasses $1 trillion.

<details><summary>References</summary>
<ul>
<li><a href="https://hai.stanford.edu/news/the-jagged-edge-of-the-ai-boom">The Jagged Edge of the AI Boom - Stanford HAI</a></li>
<li><a href="https://hai.stanford.edu/ai-index">AI Index | Stanford HAI</a></li>
<li><a href="https://en.wikipedia.org/wiki/Stanford_HAI">Stanford HAI</a></li>

</ul>
</details>

**Tags**: `#AI`, `#Stanford HAI`, `#AI impact`, `#inequality`, `#discussion`

---

<a id="item-27"></a>
## [LLM agents given self-written notes repeat losing moves in gamebook experiment](https://www.reddit.com/r/artificial/comments/1xxe7ie/an_ais_notes_for_its_next_attempt_told_it_to/) ⭐️ 6.0/10

A developer let LLMs play the 1988 detective gamebook The Money Spider with retries, comparing agents that received their full failure history against agents that received only notes they wrote for themselves. In one case, a model correctly identified a missing clue but then wrote advice to 'take the balloon trip and land when weather worsens,' which its later attempts followed, and none of the note-based runs won. This counterintuitive finding challenges the common assumption that self-reflection and self-generated memory summaries reliably improve LLM agents, suggesting that compressed notes can entrench mistaken strategies rather than correct them. It has implications for agent memory design in multi-step tasks where delayed feedback makes it hard to attribute failure to a specific earlier decision. The experiment is an informal single-case gamebook test from a Reddit post with limited methodological rigor, and the losing advice was self-consistent with the model's own (incorrect) diagnosis, illustrating how self-written notes can encode a plausible but wrong causal story. The game's delayed feedback—the loss is only revealed about ten decisions after the balloon choice—makes credit assignment especially difficult for any memory mechanism.

reddit · r/artificial · /u/shoumikgoswami · Nov 16, 02:47

**Background**: The Money Spider is a 1988 detective gamebook in which readers make branching choices, and some early decisions only cause failure many steps later. LLM agents often use self-reflection—where the model reviews its past attempts and writes lessons for next time—as a lightweight, gradient-free way to improve, and prior work such as Reflexion popularized storing such reflections in memory. This experiment tests whether that self-written memory is as effective as simply keeping the full history of failures.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/pdf/2503.16416">Survey on Evaluation of LLM -based Agents</a></li>
<li><a href="https://evo.si5.pl/chapters/retroagent.html">Ch 16. RetroAgent: Self -Evolving via Retrospective Feedback...</a></li>
<li><a href="https://arxiv.org/abs/2510.06092">[2510.06092] Learning from Failures: Understanding LLM ... Where LLM Agents Fail and How They can Learn From Failures Where LLM Agents Fail and How They can Learn From Failures Where LLM Agents Fail And How They can Learn From Failures Learning from Failures: Understanding LLM Alignment through... Where LLM Agents Fail and How They Can Learn From Failures Intention-behavior consistency-based automated failure ...</a></li>

</ul>
</details>

**Tags**: `#LLM agents`, `#self-reflection`, `#agent memory`, `#reinforcement learning`, `#AI research`

---