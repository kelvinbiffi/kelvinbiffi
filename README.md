# Kelvin Biffi

### I design and build the interface for AI products, and the layer underneath that keeps them honest.

**UX, UI and AI** · React · Next.js · TypeScript · Design Systems · Accessibility · **MCP** · AI Agents · LLM Evaluation
15+ years shipping production software · Remote, Brazil (UTC-3) · [kelvinbiffi.com](https://kelvinbiffi.com)

> AI made me faster. It did not make me necessary. Fifteen years of engineering did that, and it is why I can tell a model where to look instead of watching it guess.

I wrote the books on **MCP**, **Context Engineering** and **AI Agents in Python**. Then I shipped all three to production, which is a very different experience.

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=flat-square&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/kelvinbiffi/)
[![Email](https://img.shields.io/badge/Email-EA4335?style=flat-square&logo=gmail&logoColor=white)](mailto:kelvinbiffi.developer@gmail.com)
[![Website](https://img.shields.io/badge/kelvinbiffi.com-111?style=flat-square&logo=googlechrome&logoColor=white)](https://kelvinbiffi.com)
[![YellowKode](https://img.shields.io/badge/YellowKode%20Academy-FFD700?style=flat-square&logoColor=black)](https://yellowkode.com)

---

## The part most teams underbuild

An agent does not fail loudly.

It returns something plausible. The logs look clean. Three weeks later someone finds a corrupted record.

So I stopped trusting model output and started validating it like user input: **schema-constrained, value-checked, with guardrails that can refuse to answer**, evaluation loops, and cost tracked per conversation instead of per call.

That layer is half of what I do. The other half is the interface on top of it, and it is the half almost everyone underbuilds.

Chat is the easy part. The hard part is every screen after it: the approval card for an action that cannot be undone, the refusal state where the model said no and that is the correct answer, the tool call you can inspect, the citation that ties a claim back to its source, the cost meter, the diff someone has to review before a record changes. Those screens decide whether a person trusts the system enough to use it. A model’s answer is worthless until someone can act on it.

---

## Products I built and run

| Product | What it is |
|---|---|
| **[Linkezera](https://linkezera.com)** | Link-in-bio SaaS. **3,700+ users** across LATAM. Built end to end. |
| **[Mentezinha](https://mentezinha.app)** | Child-safe conversational AI on Google Vertex AI. Built it for my son's homeschooling, now other families use it. With children as the users there is no acceptable failure rate, so the guardrail is a validation layer that can refuse to answer, not a line in a prompt. |
| **[StartAtende](https://startatende.com)** | AI-powered customer support on WhatsApp. Intent routing and cost control per conversation. |
| **[ViralRecast](https://viralrecast.com)** | Finds what is going viral on TikTok, Reels and YouTube, explains why a post worked and cuts the vertical clips. Web app **and an MCP server with OAuth 2.1** so it runs inside Claude and ChatGPT. Postgres with pgvector for post similarity, and an atomic credit wallet that refunds failed media jobs. |
| **[Renderster](https://renderster.com)** | Video rendering as a service, and the media engine behind ViralRecast. Visual editor or JSON in, finished video out. **Go** API and workers on a Redis queue with retries, backoff and dead-letter, FFmpeg underneath, output on Cloudflare R2. |
| **[Couryo](https://couryo.com)** | Transactional email API built for Brazil, in beta and already sending for my other products. **TypeScript end to end**: Hono with zod-openapi, BullMQ workers on Redis, Postgres with Drizzle. Delivery runs on **AWS SES v2** with a tenant per customer and BYODKIM. Every send takes an **Idempotency-Key**, so a retried request never becomes a second email. SMTP relay, an **MCP server with OAuth**, official SDKs for Node, Python and PHP, and 679 tests on the API. |
| **[SunoBoard](https://sunoboard.com)** | AI music studio. I built it to score the games I want to make, then gave it an **MCP server** so an agent can compose, check generation status and pull finished tracks without a human in the loop. |
| **[MentalKare](https://mentalkare.org)** | Accessible mental health platform, multilingual. |
| **[YellowKode Academy](https://yellowkode.com)** | Courses and technical books for developers. I teach the foundation that makes AI actually work. |

## Games: the dream that started it all

Around 2010 I asked my dad to pay for a game development course. His answer: "no way". I picked software engineering instead, and on the first day the professor asked who wanted to make games. I was the only one who raised a hand, and he said: *"then you're in the wrong course"*. Later another professor switched off my PC mid-game: *"in my class you only play what you build yourself"*. So I built one. **Das Buch**, a Gladiatus-style RPG, three months and more than 7,000 lines written by hand, in Delphi.

Unity3D product experiences and a long web career came after. Now I am back to the original dream as the founder of **[K3 Games Studio](https://github.com/K3-Games-Studio)**, with AI agents as part of the team. Games are also why I built SunoBoard in the first place. **[Read the full story →](https://k3gamesstudio.com/historia/?lang=en)**

**On Google Play**

| Game | |
|---|---|
| **[Lantern Logic](https://play.google.com/store/apps/details?id=com.k3games.lanternlogic)** | Daily logic puzzle of lighthouses and lanterns. |
| **[Stitch Logic](https://play.google.com/store/apps/details?id=com.k3games.stitchlogic)** | Cross-stitch nonograms with journeys and patterns. |
| **[Countryside Cove](https://play.google.com/store/apps/details?id=com.k3games.countrysidecove)** | Cozy countryside life: farm, fish and meet the neighbors. |

Plus **[free daily puzzles](https://k3gamesstudio.com/puzzles/)** in the browser (open source: [k3-puzzles](https://github.com/K3-Games-Studio/k3-puzzles)).

**On itch.io**

<p>
<a href="https://k3-games-studio.itch.io/bubble-blaster"><img src="https://img.itch.zone/aW1nLzMwMzU0NTk3LnBuZw==/315x250%23c/HkSmxi.png" width="180" alt="Bubble Blaster"></a>
<a href="https://k3-games-studio.itch.io/kaiju-siege"><img src="https://img.itch.zone/aW1nLzI4NDA4ODQyLmpwZw==/315x250%23c/KoyatI.jpg" width="180" alt="Kaiju Siege"></a>
<a href="https://k3-games-studio.itch.io/dino-breakout"><img src="https://img.itch.zone/aW1nLzI4MzA2NDEwLnBuZw==/315x250%23c/voGJhr.png" width="180" alt="Dino Breakout"></a>
<a href="https://k3-games-studio.itch.io/hollow-fields"><img src="https://img.itch.zone/aW1nLzI4MjgxNzA5LnBuZw==/315x250%23c/YAGu9s.png" width="180" alt="Hollow Fields"></a>
<a href="https://k3-games-studio.itch.io/gate-of-the-dead"><img src="https://img.itch.zone/aW1nLzI4NTkzNDIyLnBuZw==/315x250%23c/omhBg5.png" width="180" alt="Gate of the Dead"></a>
</p>

| Game | Genre | |
|---|---|---|
| **[Bubble Blaster](https://k3-games-studio.itch.io/bubble-blaster)** | Puzzle, arcade | Aim, shoot, match three. Chain reactions drop whole clusters in slow motion across 24 handcrafted levels in 3 neon worlds, each with its own pixel art creatures and an original synthwave soundtrack. |
| **[Kaiju Siege](https://k3-games-studio.itch.io/kaiju-siege)** | Strategy | The kaijus rose from the deep. Deploy five combat mechs, call orbital strikes and hold the city across four living biomes with day and night cycle and weather. Campaign with four bosses, plus an endless mode. |
| **[Dino Breakout](https://k3-games-studio.itch.io/dino-breakout)** | Action, arcade | The fences failed at midnight and the dinosaurs own the streets. Lead the Rescue Rangers through the city and get the civilians out. |
| **[Hollow Fields](https://k3-games-studio.itch.io/hollow-fields)** | Action, horror | The world did not end in fire, it rotted. You are Death's last servant, harvesting thousands of souls with auto-weapons, a manual reap sweep and a dash. |
| **[Gate of the Dead](https://k3-games-studio.itch.io/gate-of-the-dead)** | Shooter, arcade | Arcade shooter. |

## Shipped for other people

- Subscription, billing and lifecycle flows on **Stripe**, used by thousands of paying members at **Firstleaf** (US wine subscription)
- An enterprise login and registration gateway with **Keycloak and MFA** serving **millions of users** at Lojas Renner
- Frontend systems for **DIFC**, the Dubai International Financial Centre, and for **605 Media Analytics**
- A **Vue.js landing page builder** at Pmweb that cut development effort by **70%**, moving page creation out of the engineering queue and into the client's hands
- **Near Companion** at Hire With Near: a Chrome extension over an LLM pipeline with Recall.ai, Supabase, HubSpot, Cloudflare R2 and n8n. A bot joins the intake call as a silent participant and writes the structured job description live, during the call. I owned the whole interface, and every model output was schema-validated before it touched a CRM

---

## Stack

**Surface**
![React](https://img.shields.io/badge/React-20232A?style=flat-square&logo=react)
![Next.js](https://img.shields.io/badge/Next.js-000?style=flat-square&logo=nextdotjs)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)
![Tailwind](https://img.shields.io/badge/Tailwind-06B6D4?style=flat-square&logo=tailwindcss&logoColor=white)

**AI in production**
![Claude](https://img.shields.io/badge/Claude%20API-D97757?style=flat-square&logo=anthropic&logoColor=white)
![OpenAI](https://img.shields.io/badge/OpenAI-412991?style=flat-square&logo=openai&logoColor=white)
![Vertex AI](https://img.shields.io/badge/Vertex%20AI-4285F4?style=flat-square&logo=googlecloud&logoColor=white)
![MCP](https://img.shields.io/badge/MCP-000?style=flat-square)
![n8n](https://img.shields.io/badge/n8n-EA4B71?style=flat-square&logo=n8n&logoColor=white)

**Underneath**
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![Node.js](https://img.shields.io/badge/Node.js-339933?style=flat-square&logo=nodedotjs&logoColor=white)
![Go](https://img.shields.io/badge/Go-00ADD8?style=flat-square&logo=go&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white)
![GraphQL](https://img.shields.io/badge/GraphQL-E10098?style=flat-square&logo=graphql&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)

Agents with tool calling · MCP servers and clients · RAG and contextual retrieval · evaluation loops · guardrails · schema-constrained output · cost control · FFmpeg · WhisperX

**How I work:** Claude Code daily, with a written context file in every repo so the agent inherits the project's decisions instead of rediscovering them every session.

---

## Here on GitHub

Client work lives in private repos. What is open is everything I build under **[YellowKode](https://github.com/YellowKode-Academy)** and **[Wunka](https://github.com/Wunka-Tech)**, both mine, plus the tooling here.

### Couryo SDKs

The official clients for [Couryo](https://couryo.com), open source under Wunka. Each one wraps the API, retries safely with an idempotency key, and plugs into the mail layer the framework already has, so switching providers is a config change and not a rewrite.

- **[couryo-node](https://github.com/Wunka-Tech/couryo-node)** - TypeScript SDK. On npm as [`@couryo/node`](https://www.npmjs.com/package/@couryo/node).
- **[couryo-python](https://github.com/Wunka-Tech/couryo-python)** - Python SDK with a **Django email backend**. On PyPI as [`couryo`](https://pypi.org/project/couryo/).
- **[couryo-php](https://github.com/Wunka-Tech/couryo-php)** - PHP SDK with a **Laravel mail transport**. On Packagist as [`couryo/couryo-php`](https://packagist.org/packages/couryo/couryo-php).
- **[couryo-email-templates](https://github.com/Wunka-Tech/couryo-email-templates)** - Brazilian transactional email templates for React Email (Pix, boleto, password reset). Works with any provider. On npm as [`@couryo/email-templates`](https://www.npmjs.com/package/@couryo/email-templates).

### Agents, MCP and local AI

- **[ollos-mcp](https://github.com/kelvinbiffi/ollos-mcp)** - eyes and ears for agents. Whisper transcription, speaker segmentation, perceptual-hash keyframing and OCR, all running locally in Node through ONNX Runtime. No Python, no cloud, no API key, so the file never leaves the machine. Same core ships as an MCP server, a CLI and a Node library. The part I care about is that it reports confidence per block and per segment and filters the lines Whisper invents over silence, because a transcript that does not say where it is unsure is worse than one that is visibly wrong. On npm as [`ollos-mcp`](https://www.npmjs.com/package/ollos-mcp).
- **[suno-mcp](https://github.com/YellowKode-Academy/suno-mcp)** - MCP server that lets Claude, Cursor and any MCP client generate music with Suno from a plain sentence. It owns the whole generation flow, polling and retrieval, so the assistant never sits blocked on the API. On npm as [`@yellowkode/suno-mcp`](https://www.npmjs.com/package/@yellowkode/suno-mcp), with [`suno-mcp-core`](https://github.com/YellowKode-Academy/suno-mcp-core) holding the typed handlers and tool schemas so a new transport never means rewriting the tools.
- **[yk-agent](https://github.com/YellowKode-Academy/yk-agent)** - autonomous agent that runs entirely on your machine. Browses, extracts and executes with **no API key and no account**, with a retrieval knowledge base built in. The interesting constraint is privacy: nothing leaves the laptop, which changes what you are allowed to do at every step.
- **[yk-chat](https://github.com/YellowKode-Academy/yk-chat)** - local AI chat with the same knowledge base, for people who want to use a model without handing over their data.
- **[squadron](https://github.com/YellowKode-Academy/squadron)** - an opinionated skeleton for a project run by one person and a team of agents. Ten agents, five skills, and documentation the agents actually obey. Not a framework, a starting point you adapt.

### Design systems and teaching

- **[Guide-Book](https://github.com/kelvinbiffi/Guide-Book)** - design system and style guide generator that reads your CSS, SCSS, LESS or Stylus and produces the categories, elements and modules of your design system. On npm as [`guide-book-generator`](https://www.npmjs.com/package/guide-book-generator).
- **[javascript-book](https://github.com/kelvinbiffi/javascript-book)** - every code example from *JavaScript: Básico ao Avançado*.
- **Book source, all public:** [MCP na Prática com Python](https://github.com/YellowKode-Academy/mcp-na-pratica), [Agentes de IA com Python](https://github.com/YellowKode-Academy/agentes-ia-python) and [Multiagente com Python](https://github.com/YellowKode-Academy/multiagente-ia-python). I wrote the books, then shipped the same patterns to production, which is a very different experience.
- **[Bubble-Shooter](https://github.com/kelvinbiffi/Bubble-Shooter)** and **[GUI_Unity3D_Style_Guide_Base](https://github.com/kelvinbiffi/GUI_Unity3D_Style_Guide_Base)** - a JS game and a Unity3D GUI style guide. Games are the reason I built SunoBoard (the published ones are [above](#games-i-ship-on-the-side)), and a design system is a design system whether it renders in a browser or in Unity.
- **[Criando e aplicando um Style Guide do zero](https://github.com/kelvinbiffi/Criando-e-aplicando-um-Style-Guide-do-zero)** - full source for my design systems course.

---

## I write

Almost thirty published books. Four of them are the exact stack I work in.

**AI engineering**

| Book | |
|---|---|
| **MCP na Prática com Python** | [Amazon](https://www.amazon.com.br/dp/B0GX32HTH8) |
| **Context Engineering: O Guia Definitivo para LLMs** | [Amazon](https://www.amazon.com.br/dp/B0H1PTSJP7) |
| **Agentes de IA com Python** | [Amazon](https://www.amazon.com.br/dp/B0H2RZ1VBM) |
| **Spec Driven Development na Prática** | [Amazon](https://www.amazon.com.br/dp/B0H2RP3V54) |

<details>
<summary><b>Everything else I have written</b> (languages, fundamentals, and a cosmic horror series)</summary>

**Dev na Prática series**

- [JavaScript na Prática](https://www.amazon.com.br/dp/B0GZGG6Q77)
- [Go na Prática](https://www.amazon.com.br/dp/B0H3WTFPCW)
- [TDD na Prática com Python](https://www.amazon.com.br/dp/B0H2JRFTFT)
- [TypeScript na Prática](https://www.amazon.com.br/dp/B0GX6W5ZCV)
- [SQL na Prática com PostgreSQL](https://www.amazon.com.br/dp/B0H6688KL4)

**Technical, standalone**

- [JavaScript: Básico ao Avançado](https://www.amazon.com.br/dp/B0BS9VQTJW)
- [Lógica de Programação na Prática](https://www.amazon.com.br/dp/B0H3KVBPB2)
- [Guia do Programador Moderno](https://www.amazon.com.br/dp/B0H637DJGL)
- [Algoritmo para Leigos](https://www.amazon.com.br/dp/B0DG32258Z)

**Fiction: Arquivo Morto, a cosmic horror series**

- [O Andar que Não Existe](https://www.amazon.com.br/dp/B0H2ZBL27B) · [A Geometria do Arquiteto](https://www.amazon.com.br/dp/B0H2ZG8Z4V) · [O Corredor Sem Fim](https://www.amazon.com.br/dp/B0GXNQMJ43) · [A Escada do Consolação](https://www.amazon.com.br/dp/B0H3NN3QSB) · [O Arquivo Submerso](https://www.amazon.com.br/dp/B0H2W7C1NX) · [A Janela Fechada de Dentro](https://www.amazon.com.br/dp/B0H4F3D35M) · [O Jardim Sem Saída](https://www.amazon.com.br/dp/B0H581853P)

**Other**

- [Método IAPA: Um Ciclo Constante de Crescimento Pessoal e Profissional](https://www.amazon.com.br/dp/B0DWMGVK5L)
- [As 5 Leis Universais do Dinheiro](https://www.amazon.com.br/dp/B0DTJHX4S6)
- [Construindo o Futuro: Os Benefícios do LEGO para Desenvolvimento Infantil](https://www.amazon.com.br/dp/B0DK6MRTDY)
- [O Menino Dentro da Cartola de Retalhos](https://www.amazon.com.br/dp/B0CW1CSD1N)
- [O Tamanduá Mensageiro do Rei](https://loja.uiclap.com/titulo/ua67047/)
- [Economópolis](https://economopolis.com.br/)

[→ All books on Amazon](https://www.amazon.com.br/s?i=digital-text&rh=p_27%3AKelvin%2BBaumhardt%2BBiffi&s=relevancerank&text=Kelvin+Baumhardt+Biffi)

</details>

---

Remote, Brazil (UTC-3), so most of a US or European day is my day too.

**kelvinbiffi.developer@gmail.com** · [LinkedIn](https://www.linkedin.com/in/kelvinbiffi/) · [kelvinbiffi.com](https://kelvinbiffi.com)
